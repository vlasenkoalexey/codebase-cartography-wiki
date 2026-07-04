---
title: Knowledge-graph schema and the defensive validation/repair pipeline
type: concept
provenance: mixed
concept: understand-anything-plugin-packages-core-src-schema.ts
concepts: [symbol-graph]
updated: 2026-07-04
status: fresh
---
# Knowledge-graph schema and the defensive validation/repair pipeline

<!-- connect:up:begin -->
> **Cross-repo concept:** part of [symbol-graph](../../../concepts/symbol-graph.md) across this wiki's repos.
<!-- connect:up:end -->
`schema.ts` is where Understand-Anything commits to *how it represents a codebase*: a single typed
**knowledge graph** of typed nodes (files, functions, classes, domains, articles…) joined by typed
edges. But the file is only half schema. The other half — and the larger half — is a four-tier
**repair pipeline** that takes untrusted JSON and coerces it into a graph that conforms to that
schema, logging every change instead of rejecting the whole document.

## Overview

Understand-Anything's code representation is a property graph, not a SCIP-style symbol index: nodes
carry a `type` from a fixed vocabulary, a summary, tags and a complexity band; edges carry a `type`
from a 35-value vocabulary and a `weight`. That shape is declared once, with Zod, in
[`KnowledgeGraphSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#KnowledgeGraphSchema)
and its parts ([`GraphNodeSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphNodeSchema),
[`GraphEdgeSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphEdgeSchema)).

The single design fact that explains the rest of the file: **this graph is produced by an LLM, not
by a deterministic indexer.** Where wikify-repo and graphify derive their graph from SCIP / static
analysis (so the nodes are ground truth and only need assembling), Understand-Anything's nodes and
edges are *generated text* that only approximately obeys the schema. So the schema ships paired with
[`validateGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#validateGraph) — a
tolerant pipeline that sanitizes, normalizes aliases, fills defaults, coerces types, and drops
individually-broken items rather than failing the whole graph, returning a repair log in
[`ValidationResult`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ValidationResult).

## Diagram

```mermaid
flowchart TD
    IN[unknown JSON] --> VG[validateGraph]
    VG --> SAN[sanitizeGraph: null→[], lowercase enums]
    SAN --> NORM[normalizeGraph: NODE/EDGE_TYPE_ALIASES]
    NORM --> AF[autoFixGraph: defaults, COMPLEXITY/DIRECTION_ALIASES, weight coercion+clamp]
    AF --> COL{collections are arrays?}
    COL -- no --> FATAL1[buildInvalidCollectionIssue → fatal]
    COL -- yes --> PM{ProjectMetaSchema.safeParse}
    PM -- fail --> FATAL2[fatal: missing project metadata]
    PM -- ok --> NODES[per-node GraphNodeSchema.safeParse<br/>drop broken]
    NODES --> HASNODES{any valid nodes?}
    HASNODES -- no --> FATAL3[fatal: no valid nodes]
    HASNODES -- yes --> EDGES[per-edge GraphEdgeSchema.safeParse<br/>+ referential integrity → drop]
    EDGES --> LT[LayerSchema / TourStepSchema<br/>drop broken, filter dangling nodeIds]
    LT --> OUT[ValidationResult: success, data, issues]
    FATAL1 --> ERR[ValidationResult: success=false, fatal, buildErrors]
    FATAL2 --> ERR
    FATAL3 --> ERR
```

## Design rationale (why it's built this way)

**The alias tables exist because the source is an LLM.** The comments say so verbatim:
[`NODE_TYPE_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#NODE_TYPE_ALIASES)
is documented as "Aliases that LLMs commonly generate instead of canonical node types," and
[`EDGE_TYPE_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#EDGE_TYPE_ALIASES),
[`COMPLEXITY_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#COMPLEXITY_ALIASES),
and [`DIRECTION_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#DIRECTION_ALIASES)
carry the same intent. `func`/`fn`/`method` collapse to `function`; `extends`→`inherits`;
`low`/`easy`→`simple`. These are not a general normalization layer — they are a curated list of the
mistakes a language model makes when asked to emit graph JSON. One inline comment even records a
*deliberate non-alias*: `implemented_by` is intentionally NOT mapped to `implements` because it would
invert edge direction, so the model is expected to use `implements` with swapped source/target.

**Graceful degradation over strict rejection.** A validator over trusted input would reject on the
first schema violation. Here the opposite: only four conditions are fatal (not an object, a
top-level collection that is present but not an array, missing project metadata, and zero surviving
nodes). Everything else is *repaired or dropped* and recorded. A single malformed node or a dangling
edge must not throw away an otherwise-useful 500-node graph.

**The `GraphIssue` level tri-state is the audit trail.**
[`GraphIssue.level`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphIssue.level)
is exactly `"auto-corrected" | "dropped" | "fatal"` — three tiers of intervention. `auto-corrected`
means the value was silently fixed (default filled, alias mapped, weight clamped); `dropped` means an
item failed validation and was removed; `fatal` means the whole graph is unusable. This lets the
dashboard surface a "we repaired N things, dropped M" banner rather than a binary pass/fail.

> [!inferred]
> Relative to the surveyed tools, this makes Understand-Anything's *grounding substrate* fundamentally
> different: wikify-repo/graphify ground claims in SCIP symbols (deterministic, verifiable back to
> source lines), whereas this schema grounds nothing about *correctness of meaning* — it only
> guarantees *structural well-formedness* of an LLM-authored graph. The node's `filePath`/`lineRange`
> are optional and unverified; the schema cannot tell a hallucinated edge from a real one, only a
> shaped edge from a malformed one.

**`.passthrough()` and the `kind` discriminator keep the graph extensible.** `GraphNodeSchema`,
`DomainMetaSchema` and `KnowledgeMetaSchema` are declared `.passthrough()` so unknown fields survive
validation, and node `type` spans code (`file`/`function`/`class`), infra (`service`/`resource`),
domain (`domain`/`flow`/`step`) and knowledge (`article`/`claim`/`source`) vocabularies. The same
graph shape represents a codebase *and* a knowledge base — a design choice that mirrors this wiki's
own two-source-type model.

## Entry points

- [`validateGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#validateGraph) —
  the single door in. Every graph read from disk or produced by the analyzer passes through here before
  it is trusted. It accepts `unknown` (not a typed graph) precisely because the caller cannot assume the
  input is well-formed.
- [`loadGraph`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#loadGraph)
  and [`loadDomainGraph`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#loadDomainGraph) —
  the production callers. Each reads `.understand-anything/*.json`, calls `validateGraph`, and (unless
  `validate: false`) throws `Invalid … graph: <fatal>` when
  [`success`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ValidationResult.success)
  is false, otherwise hands back the repaired
  [`data`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ValidationResult.data).
  This is where the `fatal` string becomes a user-facing error.

## Mechanism (step-by-step)

1. **Reject the non-object early, then treat input as a loose record.**
   [`validateGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#validateGraph)
   first checks `typeof data !== "object"`; if so it returns immediately with an empty
   [`issues`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ValidationResult.issues)
   list and a `fatal` of `"Invalid input: not an object"`. Otherwise it casts to a bag of unknown keys —
   nothing downstream assumes any field exists or has the right type.

2. **Sanitize shape-level noise (Tier 1).**
   [`sanitizeGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#sanitizeGraph)
   coerces `null`/missing `tour` and `layers` into `[]`, deletes `null`-valued optional node fields
   (`filePath`, `lineRange`, `languageNotes`) so Zod's `.optional()` sees "absent" rather than "null",
   and lowercases enum-like strings (`type`, `complexity`, edge `direction`). This runs *first* so the
   alias lookups that follow can assume lowercase keys. It produces no issues — it is silent cleanup.

3. **Map LLM aliases to canonical types (existing/pre-Tier).**
   [`normalizeGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#normalizeGraph)
   rewrites each node `type` through
   [`NODE_TYPE_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#NODE_TYPE_ALIASES)
   and each edge `type` through
   [`EDGE_TYPE_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#EDGE_TYPE_ALIASES).
   Note it does this silently (no `GraphIssue`), unlike the complexity/direction aliasing below — type
   aliasing is treated as pure vocabulary translation, not a correction worth reporting.

4. **Fill defaults, alias, and coerce values (Tier 2).**
   [`autoFixGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#autoFixGraph)
   is the heavy repairer. Per node: missing `type`→`"file"`, missing `complexity`→`"moderate"` (or
   aliased via [`COMPLEXITY_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#COMPLEXITY_ALIASES)),
   missing `tags`→`[]`, missing `summary`→the name. Per edge: missing `type`→`"depends_on"`, missing
   `direction`→`"forward"` (or aliased via
   [`DIRECTION_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#DIRECTION_ALIASES)),
   missing `weight`→`0.5`, a *string* weight `parseFloat`-coerced (falling back to `0.5` if `NaN`), and
   any out-of-range weight clamped to `[0,1]`. Every one of these appends an
   [`issues`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#autoFixGraph.typeLiteral28.issues)
   entry at level `auto-corrected` with a human-readable `message` and JSON `path`, so the repair is
   traceable. It returns both the fixed
   [`data`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#autoFixGraph.typeLiteral28.data)
   and the accumulated issues.

5. **Fail fast on structurally-impossible input (Tier 4).** Back in `validateGraph`, if any of
   `nodes`/`edges`/`layers`/`tour` is present but not an array,
   [`buildInvalidCollectionIssue`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#buildInvalidCollectionIssue)
   produces a `fatal` `GraphIssue` and the function returns — you cannot iterate a non-array collection.
   Then [`ProjectMetaSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ProjectMetaSchema)
   (name, languages, frameworks, description, analyzedAt, gitCommitHash — all required) is `safeParse`d;
   a miss is fatal because the graph has no identity without it.

6. **Validate items individually and drop the broken (Tier 3).** Each node is
   [`GraphNodeSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphNodeSchema)`.safeParse`d;
   failures become `dropped` issues instead of aborting. If *zero* nodes survive, that is fatal — an
   empty graph is not useful. Edges then pass
   [`GraphEdgeSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphEdgeSchema)
   **plus referential integrity**: an edge whose `source` or `target` is not in the surviving node-id set
   is dropped with an `invalid-reference` issue. This is the step that makes the graph internally
   consistent — no edge can point at a node that was itself dropped.

7. **Filter dangling references in layers and tour, then assemble the result.**
   [`LayerSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#LayerSchema) and
   [`TourStepSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#TourStepSchema)
   items are validated the same drop-broken way, and their `nodeIds` arrays are filtered down to ids that
   actually exist. `validateGraph` returns
   [`success`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ValidationResult.success)`: true`
   with the cleaned graph in
   [`data`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ValidationResult.data),
   the full [`issues`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ValidationResult.issues)
   log, and a legacy string[] from
   [`buildErrors`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#buildErrors).

## Key data structures

- **The graph shape** —
  [`KnowledgeGraphSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#KnowledgeGraphSchema)
  = `{ version, kind?, project, nodes[], edges[], layers[], tour[] }`. Nodes
  ([`GraphNodeSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphNodeSchema))
  are the units of comprehension; edges
  ([`GraphEdgeSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphEdgeSchema))
  carry a typed relation from `EdgeTypeSchema` and a `[0,1]` weight; `layers` and `tour` are *views*
  over node subsets (an architecture grouping and a guided walkthrough) rather than new entities.
- **The repair log** —
  [`GraphIssue`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphIssue) with
  its [`level`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphIssue.level),
  [`category`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphIssue.category),
  [`message`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphIssue.message),
  and optional JSON [`path`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#GraphIssue.path).
- **The result envelope** —
  [`ValidationResult`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ValidationResult):
  `success`, repaired `data`, the `issues` array, a `fatal` string, and a `@deprecated`
  [`errors`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ValidationResult.errors)
  string[] kept for backward compatibility (its docstring says "Use issues/fatal instead").
- **The alias vocabularies** — four `Record<string,string>` tables
  ([`NODE_TYPE_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#NODE_TYPE_ALIASES),
  [`EDGE_TYPE_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#EDGE_TYPE_ALIASES),
  [`COMPLEXITY_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#COMPLEXITY_ALIASES),
  [`DIRECTION_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#DIRECTION_ALIASES))
  that encode the domain knowledge of *how LLMs get the vocabulary wrong*.

## Dynamics (design intent)

The pipeline order is load-bearing and intentional: sanitize (lowercase, null-strip) must precede
alias mapping (which does case-sensitive key lookups), which precedes autofix (which fills defaults on
the now-canonical fields), which precedes per-item Zod validation (which assumes canonical enums). Run
out of order, alias lookups would miss and valid items would be dropped.

The test files exercise exactly this contract.
`schema.test.ts`
imports `validateGraph`, `sanitizeGraph`, `autoFixGraph` and the alias tables directly, asserting on
`success`, `data`, `issues`, `errors`, `fatal`, and issue `level`.
`domain-types.test.ts`
validates a graph built from `domain`/`flow`/`step` nodes with `domainMeta`, confirming the single
schema really does span the non-code vocabularies.
`normalize-graph.test.ts`
pairs node-id normalization with `validateGraph`, checking the two cooperate.

## Edge cases

- **Present-but-not-array collection** is fatal (Tier 4), whereas a *missing* collection is fine —
  `sanitizeGraph` already defaults `tour`/`layers` to `[]`. The distinction is enforced in
  [`validateGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#validateGraph).
- **String weights** like `"0.8"` are `parseFloat`-coerced in
  [`autoFixGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#autoFixGraph);
  an unparseable string falls back to `0.5`, and any number outside `[0,1]` is clamped — so
  `GraphEdgeSchema`'s `.min(0).max(1)` never actually rejects a weight, autofix guarantees it in range.
- **Dangling edges/layer-ids/tour-ids** are silently pruned against the surviving node set, so the
  returned graph is guaranteed internally consistent even if the LLM referenced ids it never defined.
- **All nodes invalid** is fatal even though individual node failures are only `dropped` — the empty
  graph is caught explicitly after the node loop in
  [`validateGraph`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#validateGraph).
- **The `errors` field is a trap for new code** — it is `@deprecated` on
  [`ValidationResult`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#ValidationResult);
  read `issues`/`fatal` instead.

## Open questions

- `KnowledgeGraphSchema` accepts an optional `kind: "codebase" | "knowledge"`, but nothing in this
  packet's subgraph branches on it during validation. Where (if anywhere) `kind` changes behavior lives
  outside `schema.ts` and is not resolvable from this packet.
- `normalizeGraph` maps type aliases *without* recording a `GraphIssue`, while complexity/direction
  aliasing in `autoFixGraph` *does* log one. Whether that asymmetry is deliberate or historical is not
  settled by the source.

## See also

- [core-src-types](understand-anything-plugin-packages-core-src-types.ts.md) — the hand-written
  TypeScript `KnowledgeGraph`/`GraphNode` types this Zod schema mirrors.
- [normalize-graph](understand-anything-plugin-packages-core-src-analyzer-normalize-graph.ts.md) —
  node-id normalization that runs alongside this schema's alias normalization.
- [graph-builder](understand-anything-plugin-packages-core-src-analyzer-graph-builder.ts.md) — assembles
  the graph that this schema then validates.
- [persistence-index](understand-anything-plugin-packages-core-src-persistence-index.ts.md) — `loadGraph`
  / `loadDomainGraph`, the callers that gate every disk read on `validateGraph`.
