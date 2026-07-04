---
title: 'Module: understand-anything-plugin/src/explain-builder.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/src/explain-builder.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/skill 2.8.2 src/`explain-builder.ts`/
symbols:
  buildExplainContext: buildExplainContext().
  formatExplainPrompt: formatExplainPrompt().
  ExplainContext.targetNode: ExplainContext#targetNode.
  ExplainContext.childNodes: ExplainContext#childNodes.
  ExplainContext.connectedNodes: ExplainContext#connectedNodes.
  ExplainContext.layer: ExplainContext#layer.
  ExplainContext: ExplainContext#
  ExplainContext.projectName: ExplainContext#projectName.
  ExplainContext.path: ExplainContext#path.
  ExplainContext.relevantEdges: ExplainContext#relevantEdges.
---
# Module: [`understand-anything-plugin/src/explain-builder.ts`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts)

## Classes
### `ExplainContext`
- def: [`understand-anything-plugin/src/explain-builder.ts:8`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts#L8)
- signature: `interface ExplainContext`
- members:
  - `childNodes` — [`L12`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts#L12)
  - `connectedNodes` — [`L13`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts#L13)
  - `layer` — [`L15`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts#L15)
  - `path` — [`L10`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts#L10)
  - `projectName` — [`L9`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts#L9)
  - `relevantEdges` — [`L14`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts#L14)
  - `targetNode` — [`L11`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts#L11)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-skill-2.8.2-src-index.ts), [`buildExplainContext`](explain-builder.ts.md#buildExplainContext), [`formatExplainPrompt`](explain-builder.ts.md#formatExplainPrompt), [`explain-builder.test.ts`](__tests__/explain-builder.test.ts.md#scip-typescript-npm-understand-anything-skill-2.8.2-src-__tests__-explain-builder.test.ts)

## Functions
- `buildExplainContext(graph: KnowledgeGraph, path: string)` — [`L22`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts#L22) — Build a context for explaining a specific file or function.
- `formatExplainPrompt(ctx: ExplainContext)` — [`L108`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/explain-builder.ts#L108) — Format the explain context as a structured prompt for LLM consumption.

