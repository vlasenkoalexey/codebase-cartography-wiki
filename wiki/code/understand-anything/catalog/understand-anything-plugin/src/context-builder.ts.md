---
title: 'Module: understand-anything-plugin/src/context-builder.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/src/context-builder.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/skill 2.8.2 src/`context-builder.ts`/
symbols:
  buildChatContext: buildChatContext().
  formatContextForPrompt: formatContextForPrompt().
  ChatContext.relevantNodes: ChatContext#relevantNodes.
  ChatContext.relevantEdges: ChatContext#relevantEdges.
  ChatContext.relevantLayers: ChatContext#relevantLayers.
  ChatContext: ChatContext#
  ChatContext.projectName: ChatContext#projectName.
  ChatContext.projectDescription: ChatContext#projectDescription.
  ChatContext.languages: ChatContext#languages.
  ChatContext.frameworks: ChatContext#frameworks.
  ChatContext.query: ChatContext#query.
---
# Module: [`understand-anything-plugin/src/context-builder.ts`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts)

## Classes
### `ChatContext`
- def: [`understand-anything-plugin/src/context-builder.ts:9`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L9)
- signature: `interface ChatContext`
- members:
  - `frameworks` — [`L13`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L13)
  - `languages` — [`L12`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L12)
  - `projectDescription` — [`L11`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L11)
  - `projectName` — [`L10`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L10)
  - `query` — [`L17`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L17)
  - `relevantEdges` — [`L15`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L15)
  - `relevantLayers` — [`L16`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L16)
  - `relevantNodes` — [`L14`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L14)
- used by: [`buildChatContext`](context-builder.ts.md#buildChatContext), [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-skill-2.8.2-src-index.ts), [`context-builder.test.ts`](__tests__/context-builder.test.ts.md#scip-typescript-npm-understand-anything-skill-2.8.2-src-__tests__-context-builder.test.ts), [`formatContextForPrompt`](context-builder.ts.md#formatContextForPrompt)

## Functions
- `buildChatContext(graph: KnowledgeGraph, query: string, maxNodes?: number | undefined)` — [`L25`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L25) — Build a ChatContext by searching the knowledge graph for nodes relevant
- `formatContextForPrompt(context: ChatContext)` — [`L85`](../../../../../../raw/code/understand-anything/understand-anything-plugin/src/context-builder.ts#L85) — Format the ChatContext as a readable markdown string for LLM consumption.

