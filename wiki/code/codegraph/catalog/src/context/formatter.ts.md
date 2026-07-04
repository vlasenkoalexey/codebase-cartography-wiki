---
title: 'Module: src/context/formatter.ts'
type: catalog
provenance: extracted
module: src/context/formatter.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/context/`formatter.ts`/
symbols:
  formatContextAsJson: formatContextAsJson().
  formatContextAsMarkdown: formatContextAsMarkdown().
  serializeNode: serializeNode().
  formatNodeTree: formatNodeTree().
  formatSubgraphTree: formatSubgraphTree().
  serializeEdge: serializeEdge().
  truncate: truncate().
  formatBytes: formatBytes().
---
# Module: [`src/context/formatter.ts`](../../../../../../raw/code/codegraph/src/context/formatter.ts)

## Functions
- `formatBytes(bytes: number)` — [`L282`](../../../../../../raw/code/codegraph/src/context/formatter.ts#L282) — Format bytes as human-readable string
- `formatContextAsJson(context: TaskContext)` — [`L97`](../../../../../../raw/code/codegraph/src/context/formatter.ts#L97) — Format context as JSON
- `formatContextAsMarkdown(context: TaskContext)` — [`L18`](../../../../../../raw/code/codegraph/src/context/formatter.ts#L18) — Format context as markdown
- `formatNodeTree(node: Node, subgraph: Subgraph, outgoing: Map<string, Edge[]>, printed: Set<string>, lines: string[], depth: number, prefix: string)` — [`L166`](../../../../../../raw/code/codegraph/src/context/formatter.ts#L166) — Format a single node and its relationships
- `formatSubgraphTree(subgraph: Subgraph, entryPoints: Node[])` — [`L124`](../../../../../../raw/code/codegraph/src/context/formatter.ts#L124) — Format a subgraph as an ASCII tree structure
- `serializeEdge(edge: Edge)` — [`L259`](../../../../../../raw/code/codegraph/src/context/formatter.ts#L259) — Serialize an edge for JSON output
- `serializeNode(node: Node)` — [`L237`](../../../../../../raw/code/codegraph/src/context/formatter.ts#L237) — Serialize a node for JSON output
- `truncate(str: string, maxLength: number)` — [`L272`](../../../../../../raw/code/codegraph/src/context/formatter.ts#L272) — Truncate a string with ellipsis

