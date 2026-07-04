---
title: 'Module: understand-anything-plugin/src/diff-analyzer.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/src/diff-analyzer.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/skill 2.8.2 src/`diff-analyzer.ts`/
symbols:
  buildDiffContext: buildDiffContext().
  formatDiffAnalysis: formatDiffAnalysis().
  DiffContext.affectedNodes: DiffContext#affectedNodes.
  DiffContext.changedNodes: DiffContext#changedNodes.
  DiffContext.unmappedFiles: DiffContext#unmappedFiles.
  DiffContext.affectedLayers: DiffContext#affectedLayers.
  DiffContext.impactedEdges: DiffContext#impactedEdges.
  DiffContext: DiffContext#
  DiffContext.projectName: DiffContext#projectName.
  DiffContext.changedFiles: DiffContext#changedFiles.
---
# Module: [`understand-anything-plugin/src/diff-analyzer.ts`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts)

## Classes
### `DiffContext`
- def: [`understand-anything-plugin/src/diff-analyzer.ts:8`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts#L8)
- signature: `interface DiffContext`
- members:
  - `affectedLayers` — [`L14`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts#L14)
  - `affectedNodes` — [`L12`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts#L12)
  - `changedFiles` — [`L10`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts#L10)
  - `changedNodes` — [`L11`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts#L11)
  - `impactedEdges` — [`L13`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts#L13)
  - `projectName` — [`L9`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts#L9)
  - `unmappedFiles` — [`L15`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts#L15)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-skill-2.8.2-src-index.ts), [`buildDiffContext`](diff-analyzer.ts.md#buildDiffContext), [`diff-analyzer.test.ts`](__tests__/diff-analyzer.test.ts.md#scip-typescript-npm-understand-anything-skill-2.8.2-src-__tests__-diff-analyzer.test.ts), [`formatDiffAnalysis`](diff-analyzer.ts.md#formatDiffAnalysis)

## Functions
- `buildDiffContext(graph: KnowledgeGraph, changedFiles: string[])` — [`L22`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts#L22) — Map a list of changed file paths to knowledge graph nodes and
- `formatDiffAnalysis(ctx: DiffContext)` — [`L93`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/diff-analyzer.ts#L93) — Format the diff analysis as structured markdown for LLM or human consumption.

