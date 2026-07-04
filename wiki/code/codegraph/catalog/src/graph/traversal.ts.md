---
title: 'Module: src/graph/traversal.ts'
type: catalog
provenance: extracted
module: src/graph/traversal.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/graph/`traversal.ts`/
symbols:
  GraphTraverser.traverseBFS: GraphTraverser#traverseBFS().
  GraphTraverser.dfsRecursive: GraphTraverser#dfsRecursive().
  GraphTraverser.getCallGraph: GraphTraverser#getCallGraph().
  GraphTraverser.queries: GraphTraverser#queries.
  GraphTraverser.getImpactRecursive: GraphTraverser#getImpactRecursive().
  GraphTraverser.traverseDFS: GraphTraverser#traverseDFS().
  GraphTraverser.getTypeHierarchy: GraphTraverser#getTypeHierarchy().
  GraphTraverser.getImpactRadius: GraphTraverser#getImpactRadius().
  GraphTraverser.getCallersRecursive: GraphTraverser#getCallersRecursive().
  GraphTraverser.getCalleesRecursive: GraphTraverser#getCalleesRecursive().
  GraphTraverser.getTypeAncestors: GraphTraverser#getTypeAncestors().
  GraphTraverser.getTypeDescendants: GraphTraverser#getTypeDescendants().
  GraphTraverser.findPath: GraphTraverser#findPath().
  DEFAULT_OPTIONS: DEFAULT_OPTIONS.
  GraphTraverser.getAncestors: GraphTraverser#getAncestors().
  GraphTraverser.findUsages: GraphTraverser#findUsages().
  GraphTraverser.getAdjacentEdges: GraphTraverser#getAdjacentEdges().
  GraphTraverser.getChildren: GraphTraverser#getChildren().
  GraphTraverser: GraphTraverser#
  GraphTraverser.getCallers: GraphTraverser#getCallers().
  GraphTraverser.getCallees: GraphTraverser#getCallees().
  GraphTraverser.-constructor: GraphTraverser#`<constructor>`().
  TraversalStep.node: TraversalStep#node.
  TraversalStep.edge: TraversalStep#edge.
  GraphTraverser.getCallers.Array.typeLiteral125.node: GraphTraverser#getCallers().Array:typeLiteral125:node.
  GraphTraverser.getCallersRecursive.result-Array.typeLiteral136.node: GraphTraverser#getCallersRecursive().(result)Array:typeLiteral136:node.
  GraphTraverser.getCallees.Array.typeLiteral155.node: GraphTraverser#getCallees().Array:typeLiteral155:node.
  GraphTraverser.getCalleesRecursive.result-Array.typeLiteral166.node: GraphTraverser#getCalleesRecursive().(result)Array:typeLiteral166:node.
  TraversalStep.depth: TraversalStep#depth.
  GraphTraverser.findUsages.Array.typeLiteral256.node: GraphTraverser#findUsages().Array:typeLiteral256:node.
  TraversalStep: TraversalStep#
  GraphTraverser.getCallers.Array.typeLiteral125.edge: GraphTraverser#getCallers().Array:typeLiteral125:edge.
  GraphTraverser.getCallersRecursive.result-Array.typeLiteral136.edge: GraphTraverser#getCallersRecursive().(result)Array:typeLiteral136:edge.
  GraphTraverser.getCallees.Array.typeLiteral155.edge: GraphTraverser#getCallees().Array:typeLiteral155:edge.
  GraphTraverser.getCalleesRecursive.result-Array.typeLiteral166.edge: GraphTraverser#getCalleesRecursive().(result)Array:typeLiteral166:edge.
  GraphTraverser.findUsages.Array.typeLiteral256.edge: GraphTraverser#findUsages().Array:typeLiteral256:edge.
---
# Module: [`src/graph/traversal.ts`](../../../../../../raw/code/codegraph/src/graph/traversal.ts)

## Classes
### `GraphTraverser`
- def: [`src/graph/traversal.ts:34`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L34)
- doc: Graph traverser for BFS and DFS traversal
- signature: `class GraphTraverser`
- members:
  - `<constructor>(queries: QueryBuilder)` — [`L37`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L37) — Graph traverser for BFS and DFS traversal
  - `dfsRecursive(method)` — [`L182`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L182) — Recursive DFS helper
  - `findPath(method)` — [`L617`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L617) — Find the shortest path between two nodes
  - `findUsages(method)` — [`L494`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L494) — Find all usages of a symbol
  - `getAdjacentEdges(method)` — [`L235`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L235) — Get adjacent edges based on direction
  - `getAncestors(method)` — [`L682`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L682) — Get the containment hierarchy for a node (ancestors)
  - `getCallGraph(method)` — [`L373`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L373) — Get the call graph for a function (both callers and callees)
  - `getCallees(method)` — [`L319`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L319) — Find all functions/methods called by a function
  - `getCalleesRecursive(method)` — [`L328`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L328)
  - `getCallers(method)` — [`L261`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L261) — Find all callers of a function/method
  - `getCallersRecursive(method)` — [`L270`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L270)
  - `getChildren(method)` — [`L720`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L720) — Get immediate children of a node
  - `getImpactRadius(method)` — [`L520`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L520) — Calculate the impact radius of a node
  - `getImpactRecursive(method)` — [`L543`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L543)
  - `getTypeAncestors(method)` — [`L438`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L438)
  - `getTypeDescendants(method)` — [`L463`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L463)
  - `getTypeHierarchy(method)` — [`L412`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L412) — Get the type hierarchy for a class/interface
  - `traverseBFS(method)` — [`L48`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L48) — Traverse the graph using breadth-first search — documented in [mcp-tools.ts](../../../concepts/mcp-tools.ts.md)
  - `traverseDFS(method)` — [`L154`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L154) — Traverse the graph using depth-first search
  - `edge` — [`L261`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L261)
  - `edge` — [`L274`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L274)
  - `edge` — [`L319`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L319)
  - `edge` — [`L332`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L332)
  - `edge` — [`L494`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L494)
  - `node` — [`L261`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L261)
  - `node` — [`L274`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L274)
  - `node` — [`L319`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L319)
  - `node` — [`L332`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L332)
  - `node` — [`L494`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L494)
  - `queries` — [`L35`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L35)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`Edge`](../types.ts.md#Edge), [`target`](../types.ts.md#Edge.target), [`source`](../types.ts.md#Edge.source), [`kind`](../types.ts.md#Edge.kind), [`getNodeById`](../db/queries.ts.md#QueryBuilder.getNodeById), [`nodes`](../types.ts.md#Subgraph.nodes), [`line`](../types.ts.md#Edge.line), [`getOutgoingEdges`](../db/queries.ts.md#QueryBuilder.getOutgoingEdges), [`QueryBuilder`](../db/queries.ts.md#QueryBuilder), [`getIncomingEdges`](../db/queries.ts.md#QueryBuilder.getIncomingEdges), [`getNodesByIds`](../db/queries.ts.md#QueryBuilder.getNodesByIds), [`edges`](../types.ts.md#Subgraph.edges), [`Subgraph`](../types.ts.md#Subgraph), [`EdgeKind`](../types.ts.md#EdgeKind), [`roots`](../types.ts.md#Subgraph.roots), [`DEFAULT_OPTIONS`](traversal.ts.md#DEFAULT_OPTIONS), [`nodeKinds`](../types.ts.md#TraversalOptions.nodeKinds), [`TraversalOptions`](../types.ts.md#TraversalOptions), [`column`](../types.ts.md#Edge.column), [`edgeKinds`](../types.ts.md#TraversalOptions.edgeKinds), [`node`](traversal.ts.md#TraversalStep.node), [`limit`](../types.ts.md#TraversalOptions.limit), [`edge`](traversal.ts.md#TraversalStep.edge), [`depth`](traversal.ts.md#TraversalStep.depth), [`direction`](../types.ts.md#TraversalOptions.direction), [`includeStart`](../types.ts.md#TraversalOptions.includeStart), [`maxDepth`](../types.ts.md#TraversalOptions.maxDepth), [`TraversalStep`](traversal.ts.md#TraversalStep)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`findRelevantContext`](../context/index.ts.md#ContextBuilder.findRelevantContext), [`index.ts`](../context/index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-context-index.ts), [`getContext`](queries.ts.md#GraphQueryManager.getContext), [`wireLayers`](../index.ts.md#CodeGraph.wireLayers), [`getNodeMetrics`](queries.ts.md#GraphQueryManager.getNodeMetrics), [`queries.ts`](queries.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-graph-queries.ts), [`getCallers`](../index.ts.md#CodeGraph.getCallers), [`getCallees`](../index.ts.md#CodeGraph.getCallees), [`traverser`](../index.ts.md#CodeGraph.traverser), [`<constructor>`](../context/index.ts.md#ContextBuilder.-constructor), [`findPath`](../index.ts.md#CodeGraph.findPath), [`createContextBuilder`](../context/index.ts.md#createContextBuilder), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-graph-index.ts), [`<constructor>`](queries.ts.md#GraphQueryManager.-constructor), [`getImpactRadius`](../index.ts.md#CodeGraph.getImpactRadius), [`traverse`](../index.ts.md#CodeGraph.traverse), [`getChildren`](../index.ts.md#CodeGraph.getChildren), [`findUsages`](../index.ts.md#CodeGraph.findUsages), [`getAncestors`](../index.ts.md#CodeGraph.getAncestors), [`getCallGraph`](../index.ts.md#CodeGraph.getCallGraph), [`getTypeHierarchy`](../index.ts.md#CodeGraph.getTypeHierarchy), [`traverser`](queries.ts.md#GraphQueryManager.traverser), [`traverser`](../context/index.ts.md#ContextBuilder.traverser), [`getTraverser`](queries.ts.md#GraphQueryManager.getTraverser)

### `TraversalStep`
- def: [`src/graph/traversal.ts:25`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L25)
- doc: Result of a single traversal step
- signature: `interface TraversalStep`
- members:
  - `depth` — [`L28`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L28)
  - `edge` — [`L27`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L27)
  - `node` — [`L26`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L26)
- uses (calls/refs, reference-scoped): [`Node`](../types.ts.md#Node), [`Edge`](../types.ts.md#Edge)
- used by: [`traverseBFS`](traversal.ts.md#GraphTraverser.traverseBFS)

## Module values
- `DEFAULT_OPTIONS` — [`L13`](../../../../../../raw/code/codegraph/src/graph/traversal.ts#L13) — Default traversal options

