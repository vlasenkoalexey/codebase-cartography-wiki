---
title: Business-domain knowledge extraction
type: doc-concept
provenance: doc
source: docs/superpowers/specs/2026-04-01-business-domain-knowledge-design.md
updated: 2026-07-04
status: fresh
---
# Business-domain knowledge extraction

## Definition
File-level dependency edges have limited value — you can already see imports in
an IDE. `/understand-domain` instead extracts the *business logic* embedded in the
code as a three-level hierarchy: **domain** (e.g. "Order Management") → **flow**
(a process, e.g. "Create Order") → **step** (a single action, e.g. "Validate
input"), plus `cross_domain` interactions. It is rendered as a left-to-right flow
graph and stored in a separate `domain-graph.json` that reuses the same
`KnowledgeGraph` type system, with `implements` edges that drill from a step down
to the structural node that realizes it. This is the semantic-comprehension axis:
what the code *does*, not how it is wired.

## In understand-anything (grounded)
The domain types extend the shared schema (Approach C — separate file, shared
type). In `packages/core/src/types.ts`, the `domain`/`flow`/`step` members live in
the [`NodeType`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#NodeType)
union, `contains_flow`/`flow_step`/`cross_domain`/`implements` in
[`EdgeType`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#EdgeType),
and the payload is
[`GraphNode.domainMeta`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#GraphNode.domainMeta)
→ [`DomainMeta`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#DomainMeta)
([`entities`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#DomainMeta.entities),
[`businessRules`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#DomainMeta.businessRules),
[`crossDomainInteractions`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#DomainMeta.crossDomainInteractions),
[`entryPoint`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#DomainMeta.entryPoint),
[`entryType`](../catalog/understand-anything-plugin/packages/core/src/types.ts.md#DomainMeta.entryType)).
Validation and the spec's normalization aliases (e.g. `process`→`flow`) are
[`DomainMetaSchema`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#DomainMetaSchema),
[`NODE_TYPE_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#NODE_TYPE_ALIASES),
[`EDGE_TYPE_ALIASES`](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md#EDGE_TYPE_ALIASES).

The separate file is loaded/saved by
[`loadDomainGraph`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#loadDomainGraph)
/ [`saveDomainGraph`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#saveDomainGraph)
([`DOMAIN_GRAPH_FILE`](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md#DOMAIN_GRAPH_FILE)).
The preprocessing script (Python, bundled with the skill) builds the LLM's
context:
[`scan_file_tree`](../catalog/understand-anything-plugin/skills/understand-domain/extract-domain-context.md#scan_file_tree),
[`detect_entry_points`](../catalog/understand-anything-plugin/skills/understand-domain/extract-domain-context.md#detect_entry_points)
(route decorators, `app.get/post`, `main()`, event listeners), and
[`extract_file_signatures`](../catalog/understand-anything-plugin/skills/understand-domain/extract-domain-context.md#extract_file_signatures).
For large codebases, per-subdomain results merge via
[`merge_graphs`](../catalog/understand-anything-plugin/skills/understand/merge-subdomain-graphs.md#merge_graphs).

## Why it matters / when it applies
Two extraction paths converge on the same output: a **lightweight scan** (~10–20%
of a full `/understand`) when no graph exists, or a near-free **derive-from-graph**
path that reasons over the existing summaries and call edges. Error tolerance is
first-class — orphan steps attach to a synthetic flow, duplicate domains merge by
name, and unresolved `implements` edges are kept but marked so the dashboard just
drops the drill-down link. For the survey, this is the layer that maps code to
human processes — the payoff of a summarized graph over a raw call graph.

## Connections
- Code concepts: [core types](../concepts/understand-anything-plugin-packages-core-src-types.ts.md), [schema](../concepts/understand-anything-plugin-packages-core-src-schema.ts.md), [persistence](../concepts/understand-anything-plugin-packages-core-src-persistence-index.ts.md)
- Module catalogs: [types.ts](../catalog/understand-anything-plugin/packages/core/src/types.ts.md), [schema.ts](../catalog/understand-anything-plugin/packages/core/src/schema.ts.md), [persistence/index.ts](../catalog/understand-anything-plugin/packages/core/src/persistence/index.ts.md), [skills/understand-domain/extract-domain-context.py](../catalog/understand-anything-plugin/skills/understand-domain/extract-domain-context.md), [skills/understand/merge-subdomain-graphs.py](../catalog/understand-anything-plugin/skills/understand/merge-subdomain-graphs.md)
- Related doc-concepts: [knowledge-graph-schema](knowledge-graph-schema.md), [knowledge-base-analysis](knowledge-base-analysis.md), [multi-agent-pipeline](multi-agent-pipeline.md)

## Source
Extracted from `docs/superpowers/specs/2026-04-01-business-domain-knowledge-design.md`
(kept in place).
