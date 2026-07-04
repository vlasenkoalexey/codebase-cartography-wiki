---
title: 'Module: src/graph/queries.ts'
type: catalog
provenance: extracted
module: src/graph/queries.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/graph/`queries.ts`/GraphQueryManager#
symbols:
  GraphQueryManager.getContext: getContext().
  GraphQueryManager.getNodeMetrics: getNodeMetrics().
  GraphQueryManager.getFilteredSubgraph: getFilteredSubgraph().
  GraphQueryManager.queries: queries.
  GraphQueryManager.findDeadCode: findDeadCode().
  GraphQueryManager.findByQualifiedName: findByQualifiedName().
  GraphQueryManager.-constructor: '`<constructor>`().'
  GraphQueryManager.findCircularDependencies: findCircularDependencies().
  GraphQueryManager.getExportedSymbols: getExportedSymbols().
  GraphQueryManager.traverser: traverser.
  GraphQueryManager.getModuleStructure: getModuleStructure().
  GraphQueryManager.getFileDependencies: getFileDependencies().
  GraphQueryManager.getFileDependents: getFileDependents().
  GraphQueryManager.getTraverser: getTraverser().
  GraphQueryManager: ''
  GraphQueryManager.getNodeMetrics.typeLiteral156.incomingEdgeCount: getNodeMetrics().typeLiteral156:incomingEdgeCount.
  GraphQueryManager.getNodeMetrics.typeLiteral156.outgoingEdgeCount: getNodeMetrics().typeLiteral156:outgoingEdgeCount.
  GraphQueryManager.getNodeMetrics.typeLiteral156.callCount: getNodeMetrics().typeLiteral156:callCount.
  GraphQueryManager.getNodeMetrics.typeLiteral156.callerCount: getNodeMetrics().typeLiteral156:callerCount.
  GraphQueryManager.getNodeMetrics.typeLiteral156.childCount: getNodeMetrics().typeLiteral156:childCount.
  GraphQueryManager.getNodeMetrics.typeLiteral156.depth: getNodeMetrics().typeLiteral156:depth.
---
# Module: [`src/graph/queries.ts`](../../../../../../raw/code/codegraph/src/graph/queries.ts)

## Classes
### `GraphQueryManager`
- def: [`src/graph/queries.ts:14`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L14)
- doc: Graph query manager for complex queries
- signature: `class GraphQueryManager`
- members:
  - `<constructor>(queries: QueryBuilder)` — [`L18`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L18) — Graph query manager for complex queries
  - `findByQualifiedName(method)` — [`L162`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L162) — Find symbols by qualified name pattern
  - `findCircularDependencies(method)` — [`L225`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L225) — Find circular dependencies in the graph
  - `findDeadCode(method)` — [`L304`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L304) — Find dead code (nodes with no incoming references)
  - `getContext(method)` — [`L32`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L32) — Get full context for a node
  - `getExportedSymbols(method)` — [`L151`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L151) — Get all symbols exported by a file
  - `getFileDependencies(method)` — [`L118`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L118) — Get dependencies of a file
  - `getFileDependents(method)` — [`L134`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L134) — Get dependents of a file
  - `getFilteredSubgraph(method)` — [`L337`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L337) — Get subgraph containing nodes matching a filter
  - `getModuleStructure(method)` — [`L203`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L203) — Get the module/package structure
  - `getNodeMetrics(method)` — [`L271`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L271) — Get complexity metrics for a node
  - `getTraverser(method)` — [`L391`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L391) — Access the underlying traverser for direct traversal operations
  - `callCount` — [`L274`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L274)
  - `callerCount` — [`L275`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L275)
  - `childCount` — [`L276`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L276)
  - `depth` — [`L277`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L277)
  - `incomingEdgeCount` — [`L272`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L272)
  - `outgoingEdgeCount` — [`L273`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L273)
  - `queries` — [`L15`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L15)
  - `traverser` — [`L16`](../../../../../../raw/code/codegraph/src/graph/queries.ts#L16)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`Edge`](../types.ts.md#Edge), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`source`](../types.ts.md#Edge.source), [`kind`](../types.ts.md#Edge.kind), [`getNodeById`](../db/queries.ts.md#QueryBuilder.getNodeById), [`nodes`](../types.ts.md#Subgraph.nodes), [`getOutgoingEdges`](../db/queries.ts.md#QueryBuilder.getOutgoingEdges), [`QueryBuilder`](../db/queries.ts.md#QueryBuilder), [`getIncomingEdges`](../db/queries.ts.md#QueryBuilder.getIncomingEdges), [`getNodesByKind`](../db/queries.ts.md#QueryBuilder.getNodesByKind), [`path`](../types.ts.md#FileRecord.path), [`edges`](../types.ts.md#Subgraph.edges), [`Subgraph`](../types.ts.md#Subgraph), [`isExported`](../types.ts.md#Node.isExported), [`getAllFiles`](../db/queries.ts.md#QueryBuilder.getAllFiles), [`EdgeKind`](../types.ts.md#EdgeKind), [`getNodesByFile`](../db/queries.ts.md#QueryBuilder.getNodesByFile), [`roots`](../types.ts.md#Subgraph.roots), [`getAncestors`](traversal.ts.md#GraphTraverser.getAncestors), [`getChildren`](traversal.ts.md#GraphTraverser.getChildren), [`GraphTraverser`](traversal.ts.md#GraphTraverser), [`getDependencyFilePaths`](../db/queries.ts.md#QueryBuilder.getDependencyFilePaths), [`getDependentFilePaths`](../db/queries.ts.md#QueryBuilder.getDependentFilePaths), [`<constructor>`](traversal.ts.md#GraphTraverser.-constructor), [`Context`](../types.ts.md#Context), [`ancestors`](../types.ts.md#Context.ancestors), [`children`](../types.ts.md#Context.children), [`focal`](../types.ts.md#Context.focal), [`imports`](../types.ts.md#Context.imports), [`types`](../types.ts.md#Context.types), [`incomingRefs`](../types.ts.md#Context.incomingRefs), [`outgoingRefs`](../types.ts.md#Context.outgoingRefs)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`wireLayers`](../index.ts.md#CodeGraph.wireLayers), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-graph-index.ts), [`findDeadCode`](../index.ts.md#CodeGraph.findDeadCode), [`graphManager`](../index.ts.md#CodeGraph.graphManager), [`getContext`](../index.ts.md#CodeGraph.getContext), [`getFileDependents`](../index.ts.md#CodeGraph.getFileDependents), [`findCircularDependencies`](../index.ts.md#CodeGraph.findCircularDependencies), [`getFileDependencies`](../index.ts.md#CodeGraph.getFileDependencies), [`getNodeMetrics`](../index.ts.md#CodeGraph.getNodeMetrics)

