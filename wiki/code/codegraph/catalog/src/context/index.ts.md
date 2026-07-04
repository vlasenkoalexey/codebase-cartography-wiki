---
title: 'Module: src/context/index.ts'
type: catalog
provenance: extracted
module: src/context/index.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/context/`index.ts`/
symbols:
  ContextBuilder.findRelevantContext: ContextBuilder#findRelevantContext().
  ContextBuilder.buildContext: ContextBuilder#buildContext().
  ContextBuilder.extractCodeBlocks: ContextBuilder#extractCodeBlocks().
  ContextBuilder.resolveImportsToDefinitions: ContextBuilder#resolveImportsToDefinitions().
  ContextBuilder.extractNodeCode: ContextBuilder#extractNodeCode().
  DEFAULT_FIND_OPTIONS: DEFAULT_FIND_OPTIONS.
  ContextBuilder.buildCallPathsSection: ContextBuilder#buildCallPathsSection().
  DEFAULT_BUILD_OPTIONS: DEFAULT_BUILD_OPTIONS.
  ContextBuilder.generateSummary: ContextBuilder#generateSummary().
  ContextBuilder.queries: ContextBuilder#queries.
  ContextBuilder.-constructor: ContextBuilder#`<constructor>`().
  createContextBuilder: createContextBuilder().
  ContextBuilder.getEntryPoints: ContextBuilder#getEntryPoints().
  ContextBuilder.getRelatedFiles: ContextBuilder#getRelatedFiles().
  ContextBuilder.buildLowConfidenceNote: ContextBuilder#buildLowConfidenceNote().
  ContextBuilder.getCode: ContextBuilder#getCode().
  ContextBuilder.traverser: ContextBuilder#traverser.
  HIGH_VALUE_NODE_KINDS: HIGH_VALUE_NODE_KINDS.
  ContextBuilder: ContextBuilder#
  ContextBuilder.projectRoot: ContextBuilder#projectRoot.
  extractSymbolsFromQuery: extractSymbolsFromQuery().
---
# Module: [`src/context/index.ts`](../../../../../../raw/code/codegraph/src/context/index.ts)

## Classes
### `ContextBuilder`
- def: [`src/context/index.ts:187`](../../../../../../raw/code/codegraph/src/context/index.ts#L187)
- doc: Context Builder
- signature: `class ContextBuilder`
- members:
  - `<constructor>(projectRoot: string, queries: QueryBuilder, traverser: GraphTraverser)` — [`L192`](../../../../../../raw/code/codegraph/src/context/index.ts#L192) — Context Builder
  - `buildCallPathsSection(method)` — [`L320`](../../../../../../raw/code/codegraph/src/context/index.ts#L320) — Surface short call-paths among the symbols this context already found,
  - `buildContext(method)` — [`L216`](../../../../../../raw/code/codegraph/src/context/index.ts#L216) — Build context for a task
  - `buildLowConfidenceNote(method)` — [`L285`](../../../../../../raw/code/codegraph/src/context/index.ts#L285) — Honest handoff appended when retrieval confidence is low (the query matched
  - `extractCodeBlocks(method)` — [`L1205`](../../../../../../raw/code/codegraph/src/context/index.ts#L1205) — Extract code blocks for key nodes in the subgraph
  - `extractNodeCode(method)` — [`L1163`](../../../../../../raw/code/codegraph/src/context/index.ts#L1163) — Extract code from a node's source file — documented in [utils.ts](../../../concepts/utils.ts.md)
  - `findRelevantContext(method)` — [`L432`](../../../../../../raw/code/codegraph/src/context/index.ts#L432) — Find relevant subgraph for a query — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `generateSummary(method)` — [`L1282`](../../../../../../raw/code/codegraph/src/context/index.ts#L1282) — Generate a summary of the context
  - `getCode(method)` — [`L1151`](../../../../../../raw/code/codegraph/src/context/index.ts#L1151) — Get the source code for a node
  - `getEntryPoints(method)` — [`L1196`](../../../../../../raw/code/codegraph/src/context/index.ts#L1196) — Get entry points from a subgraph (the root nodes)
  - `getRelatedFiles(method)` — [`L1271`](../../../../../../raw/code/codegraph/src/context/index.ts#L1271) — Get unique files from a subgraph
  - `resolveImportsToDefinitions(method)` — [`L1309`](../../../../../../raw/code/codegraph/src/context/index.ts#L1309) — Resolve import/export nodes to their actual definitions
  - `projectRoot` — [`L188`](../../../../../../raw/code/codegraph/src/context/index.ts#L188)
  - `queries` — [`L189`](../../../../../../raw/code/codegraph/src/context/index.ts#L189)
  - `traverser` — [`L190`](../../../../../../raw/code/codegraph/src/context/index.ts#L190)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`startLine`](../types.ts.md#Node.startLine), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`source`](../types.ts.md#Edge.source), [`kind`](../types.ts.md#Edge.kind), [`endLine`](../types.ts.md#Node.endLine), [`node`](../types.ts.md#SearchResult.node), [`searchNodes`](../db/queries.ts.md#QueryBuilder.searchNodes), [`traverseBFS`](../graph/traversal.ts.md#GraphTraverser.traverseBFS), [`getNodeById`](../db/queries.ts.md#QueryBuilder.getNodeById), [`nodes`](../types.ts.md#Subgraph.nodes), [`formatContextAsJson`](formatter.ts.md#formatContextAsJson), [`score`](../types.ts.md#SearchResult.score), [`formatContextAsMarkdown`](formatter.ts.md#formatContextAsMarkdown), [`NodeKind`](../types.ts.md#NodeKind), [`getOutgoingEdges`](../db/queries.ts.md#QueryBuilder.getOutgoingEdges), [`signature`](../types.ts.md#Node.signature), [`QueryBuilder`](../db/queries.ts.md#QueryBuilder), [`metadata`](../types.ts.md#Edge.metadata), [`provenance`](../types.ts.md#Edge.provenance), [`logDebug`](../errors.ts.md#logDebug), [`findNodesByExactName`](../db/queries.ts.md#QueryBuilder.findNodesByExactName), [`getTypeHierarchy`](../graph/traversal.ts.md#GraphTraverser.getTypeHierarchy), [`SearchResult`](../types.ts.md#SearchResult), [`edges`](../types.ts.md#Subgraph.edges), [`Subgraph`](../types.ts.md#Subgraph), [`findNodesByNameSubstring`](../db/queries.ts.md#QueryBuilder.findNodesByNameSubstring), [`DEFAULT_FIND_OPTIONS`](index.ts.md#DEFAULT_FIND_OPTIONS), [`EdgeKind`](../types.ts.md#EdgeKind), [`DEFAULT_BUILD_OPTIONS`](index.ts.md#DEFAULT_BUILD_OPTIONS), [`roots`](../types.ts.md#Subgraph.roots), [`validatePathWithinRoot`](../utils.ts.md#validatePathWithinRoot), [`findEdgesBetweenNodes`](../db/queries.ts.md#QueryBuilder.findEdgesBetweenNodes)  (+43 more)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`buildContext`](../index.ts.md#CodeGraph.buildContext), [`createContextBuilder`](index.ts.md#createContextBuilder), [`findRelevantContext`](../index.ts.md#CodeGraph.findRelevantContext), [`contextBuilder`](../index.ts.md#CodeGraph.contextBuilder), [`getCode`](../index.ts.md#CodeGraph.getCode)

## Functions
- `createContextBuilder(projectRoot: string, queries: QueryBuilder, traverser: GraphTraverser)` — [`L1363`](../../../../../../raw/code/codegraph/src/context/index.ts#L1363) — Create a context builder
- `extractSymbolsFromQuery(query: string)` — [`L44`](../../../../../../raw/code/codegraph/src/context/index.ts#L44) — Extract likely symbol names from a natural language query

## Module values
- `DEFAULT_BUILD_OPTIONS` — [`L143`](../../../../../../raw/code/codegraph/src/context/index.ts#L143) — Default options for context building
- `DEFAULT_FIND_OPTIONS` — [`L167`](../../../../../../raw/code/codegraph/src/context/index.ts#L167) — Default options for finding relevant context
- `HIGH_VALUE_NODE_KINDS` — [`L159`](../../../../../../raw/code/codegraph/src/context/index.ts#L159) — Node kinds that provide high information value in context results.

