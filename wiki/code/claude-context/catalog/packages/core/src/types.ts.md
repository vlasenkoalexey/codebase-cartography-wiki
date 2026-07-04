---
title: 'Module: packages/core/src/types.ts'
type: catalog
provenance: extracted
module: packages/core/src/types.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/`types.ts`/Se
symbols:
  SemanticSearchResult: manticSearchResult#
  SemanticSearchResult.relativePath: manticSearchResult#relativePath.
  SemanticSearchResult.startLine: manticSearchResult#startLine.
  SemanticSearchResult.content: manticSearchResult#content.
  SemanticSearchResult.endLine: manticSearchResult#endLine.
  SearchQuery: archQuery#
  SearchQuery.term: archQuery#term.
  SearchQuery.limit: archQuery#limit.
  SearchQuery.includeContent: archQuery#includeContent.
  SemanticSearchResult.score: manticSearchResult#score.
  SemanticSearchResult.language: manticSearchResult#language.
---
# Module: [`packages/core/src/types.ts`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts)

## Classes
### `SearchQuery`
- def: [`packages/core/src/types.ts:1`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L1)
- signature: `interface SearchQuery`
- members:
  - `includeContent` — [`L3`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L3)
  - `limit` — [`L4`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L4)
  - `term` — [`L2`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L2)
- used by: [`execute`](../../vscode-extension/src/commands/searchCommand.ts.md#SearchCommand.execute), [`searchCommand.ts`](../../vscode-extension/src/commands/searchCommand.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-commands-searchCommand.ts)

### `SemanticSearchResult`
- def: [`packages/core/src/types.ts:7`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L7)
- signature: `interface SemanticSearchResult`
- members:
  - `content` — [`L8`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L8)
  - `endLine` — [`L11`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L11)
  - `language` — [`L12`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L12)
  - `relativePath` — [`L9`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L9)
  - `score` — [`L13`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L13)
  - `startLine` — [`L10`](../../../../../../../raw/code/claude-context/packages/core/src/types.ts#L10)
- used by: [`semanticSearch`](context.ts.md#Context.semanticSearch), [`context.ts`](context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`deduplicateResults`](context.ts.md#Context.deduplicateResults), [`searchCommand.ts`](../../vscode-extension/src/commands/searchCommand.ts.md#scip-typescript-npm-semanticcodesearch-0.1.11-src-commands-searchCommand.ts), [`executeForWebview`](../../vscode-extension/src/commands/searchCommand.ts.md#SearchCommand.executeForWebview), [`generateQuickPickItems`](../../vscode-extension/src/commands/searchCommand.ts.md#SearchCommand.generateQuickPickItems), [`openResult`](../../vscode-extension/src/commands/searchCommand.ts.md#SearchCommand.openResult)

