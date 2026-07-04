---
title: Value-reference edges — "change this constant, break its readers"
type: doc-concept
provenance: doc
source: docs/design/value-reference-edges.md
updated: 2026-07-04
status: fresh
---
# Value-reference edges — "change this constant, break its readers"

## Definition
A **value-reference edge** is a `references` edge (tagged `metadata: { valueRef: true }`)
drawn from a *reader symbol* to the **file-scope `const`/`var` it reads** — same-file only.
It exists to close an impact-analysis hole: static extraction edges *calls*, *imports*, and
*inheritance*, but never edged a constant, config object, or lookup table to the symbols that
merely **read** it. So changing a shared table looked like "nothing depends on this" — the
ReScript-PR false positive that motivated the work. Value-refs is the **data** half of a
broader idea — *a symbol used as a value, not called, still creates a dependency*; the
**function** half (a callback passed as an argument, a handler in a table) is
[function-ref capture](function-ref-capture.md).

## In codegraph (grounded)
The whole feature lives in the extractor, emitted as `references` edges (an
[`EdgeKind`](../catalog/src/types.ts.md#EdgeKind)) — no resolution pass, because same-file
resolution is unambiguous. Owning module:
[`src/extraction/tree-sitter.ts`](../catalog/src/extraction/tree-sitter.ts.md).

- [`captureValueRefScope`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.captureValueRefScope)
  runs from `createNode` on every node — it records **targets** (file/class/module-scope
  `const`/`var` with a "distinctive" name) and **reader scopes** (`function`/`method`/
  `const`/`var`).
- [`flushValueRefs`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.flushValueRefs)
  runs once at the end of `extract()`: prunes shadowed targets, then walks each reader's
  subtree for identifiers matching a target name and emits the deduped edges. The feature is
  **edges-only** — node count is identical on/off (a hard validation invariant).
- [`VALUE_REF_LANGS`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.VALUE_REF_LANGS)
  is the enabled-language set (TS/JS/tsx, Go, Python, Rust, Ruby, C, Java, C#, PHP, Scala,
  Kotlin, Swift, Dart, Pascal; Svelte/Vue/Astro inherit via their re-parsed `<script>`);
  [`valueRefsEnabled`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.valueRefsEnabled)
  is the `CODEGRAPH_VALUE_REFS !== '0'` default-on switch, and
  [`MAX_VALUE_REF_NODES`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.MAX_VALUE_REF_NODES)
  caps per-scope traversal.

**Two gates** decide what edges. *Target gate:* `kind ∈ {constant, variable}`, name length ≥3
containing an uppercase or `_` (dodges single-letter / all-lowercase shadowing), and a
`file:`/`class:`/`module:`/`struct:`/`enum:` scoped parent. *Reader gate:* `kind ∈ {function,
method, constant, variable}`. The class-scope side of the gate is why several languages needed
their constants re-kinded from `field` to `constant`
([`extractField`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.extractField)
for Java/C#/Scala/Kotlin) or extracted at all
([`extractVariable`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.extractVariable)'s
C branch, where file-scope consts weren't emitted as nodes before).

**Three precision guards**, in emission order:
1. [`isGeneratedFile`](../catalog/src/extraction/generated-detection.ts.md#isGeneratedFile) —
   skips *suffix-recognised* generated files (`.pb.ts`, `.min.js`, …); path-only, so it cannot
   catch content-minified bundles.
2. **Shadow prune** — drop a target when its declarator count *exceeds its file-scope node
   count*, i.e. the name is also bound in an inner/local scope. Declarators are counted at the
   syntax level (per-grammar node types), so this is the **per-language-sensitive** guard.
   Comparing against file-scope node count (not a flat `>1`) is what keeps legitimate
   **conditional module defs** (`try: X = a; except: X = b`) — the Python-forced refinement
   that is strictly more correct for every language.
3. **Distinctive-name + same-file** (the target gate above).

## Why it matters / when it applies
The win is **impact-radius correctness**, and *only* that. Value-ref edges flow straight into
`getImpactRadius` → `codegraph impact` and the impact trail in `codegraph_explore` /
`codegraph_node` with no graph-layer change. The measured effect is turning a blind radius into
a real one — a const 80–140 symbols read that reported "1 affected" now reports its true fan-out
(`LayoutStateKeys` 1→85 on vscode, `INDEX_NOT_FOUND` 4→165 on commons-lang). The design doc is
explicit that this does **not** reduce agent reads: across a 12-run A/B the agent answers impact
questions in one call and reaches for `search`/`callers`, not `impact`, so it often never
queries these edges — the value is blast-radius correctness for the impact API, not fewer turns.

**Known limits (intentional):** same-file only (cross-file value consumers would need
import/scope resolution — out of scope for every language, so cross-file-heavy languages like
PHP yield less, correctly); parameter-only shadowing is unguarded; reactive/computed reads with
no static identifier aren't covered.

## Per-language coverage approach
Adding a language is a repeatable runbook (the companion **playbook**), not a rewrite. Decide
first whether constants sit at file/module scope (fits the gate) or inside a class/type (the
"Ruby treatment" — may need the extractor to *emit* them and to emit them as `constant`, not
`field`); confirm the grammar's **declarator node type** for the shadow prune (Go was the worked
example of this step being load-bearing); confirm the **reader-scan node type** for a constant
*read* (PHP's is a `name` node — a zero-edge sweep is usually this); then sweep small/medium/large
public OSS repos, hunt false-positive clusters, and add a matrix row + test. False positives
concentrate in bundled/minified/generated files (intra-file shadowing); one-offs are recorded,
clusters are fixed with a guard. Fifteen languages are validated this way with node count stable
on/off and precision guards holding.

## Connections
- Code concepts:
  [extraction-tree-sitter.ts](../concepts/extraction-tree-sitter.ts.md) — the extractor that
  owns `captureValueRefScope`/`flushValueRefs`;
  [types.ts](../concepts/types.ts.md) — `NodeKind`/`EdgeKind` (`constant`/`variable` targets,
  the `references` edge).
- Module catalogs:
  [extraction/tree-sitter.ts](../catalog/src/extraction/tree-sitter.ts.md),
  [extraction/generated-detection.ts](../catalog/src/extraction/generated-detection.ts.md),
  [types.ts](../catalog/src/types.ts.md).
- Related doc-concepts:
  [function-ref-capture](function-ref-capture.md) — the function-as-value sibling (same
  "used as a value, not called → a `references` edge" mental model, different metadata key and
  a resolution pass);
  [dynamic-dispatch-coverage](dynamic-dispatch-coverage.md) — the other family of synthesized
  edges that make a flow connect end-to-end.

## Source
Extracted from `docs/design/value-reference-edges.md` (the design + the fifteen-language
validation matrix) and `docs/design/value-reference-edges-playbook.md` (the extend-to-a-new-language
runbook, guard rules, and per-language declarator table). Both kept in place.
