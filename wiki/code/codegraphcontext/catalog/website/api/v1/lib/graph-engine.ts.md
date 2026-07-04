---
title: 'Module: website/api/v1/lib/graph-engine.ts'
type: catalog
provenance: extracted
module: website/api/v1/lib/graph-engine.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 api/v1/lib/`graph-engine.ts`/Graph
symbols:
  GraphEngine.loadFromZip: Engine#loadFromZip().
  GraphNode: Node#
  GraphEngine.findCallers: Engine#findCallers().
  GraphEngine.findCallees: Engine#findCallees().
  GraphEngine.getFileStructure: Engine#getFileStructure().
  GraphEngine.nodes: Engine#nodes.
  GraphEngine.findDefinitions: Engine#findDefinitions().
  GraphEngine.nameIndex: Engine#nameIndex.
  GraphEngine.outEdges: Engine#outEdges.
  GraphEngine.inEdges: Engine#inEdges.
  GraphEngine.search: Engine#search().
  GraphNode.id: Node#id.
  GraphEdge: Edge#
  GraphNode.name: Node#name.
  GraphNode.type: Node#type.
  GraphNode.file: Node#file.
  GraphNode.properties: Node#properties.
  GraphEdge.from: Edge#from.
  GraphEdge.to: Edge#to.
  GraphEdge.type: Edge#type.
  GraphEdge.properties: Edge#properties.
  GraphEngine.metadata: Engine#metadata.
  GraphEngine.getFileStructure.typeLiteral202.files: Engine#getFileStructure().typeLiteral202:files.
  GraphEngine.getFileStructure.typeLiteral202.structure: Engine#getFileStructure().typeLiteral202:structure.
  GraphEngine: Engine#
  GraphEngine.-constructor: Engine#`<constructor>`().
---
# Module: [`website/api/v1/lib/graph-engine.ts`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts)

## Classes
### `GraphEdge`
- def: [`website/api/v1/lib/graph-engine.ts:12`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L12)
- signature: `interface GraphEdge`
- members:
  - `from` — [`L13`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L13)
  - `properties` — [`L16`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L16)
  - `to` — [`L14`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L14)
  - `type` — [`L15`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L15)
- used by: [`loadFromZip`](graph-engine.ts.md#GraphEngine.loadFromZip), [`inEdges`](graph-engine.ts.md#GraphEngine.inEdges), [`outEdges`](graph-engine.ts.md#GraphEngine.outEdges)

### `GraphEngine`
- def: [`website/api/v1/lib/graph-engine.ts:19`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L19)
- signature: `class GraphEngine`
- members:
  - `<constructor>()` — [`L26`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L26)
  - `findCallees(method)` — [`L131`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L131)
  - `findCallers(method)` — [`L112`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L112)
  - `findDefinitions(method)` — [`L102`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L102)
  - `getFileStructure(method)` — [`L173`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L173)
  - `loadFromZip(method)` — [`L28`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L28)
  - `search(method)` — [`L150`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L150)
  - `files` — [`L173`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L173)
  - `inEdges` — [`L23`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L23)
  - `metadata` — [`L24`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L24)
  - `nameIndex` — [`L21`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L21)
  - `nodes` — [`L20`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L20)
  - `outEdges` — [`L22`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L22)
  - `structure` — [`L173`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L173)
- uses (calls/refs, reference-scoped): [`GraphNode`](graph-engine.ts.md#GraphNode), [`GraphEdge`](graph-engine.ts.md#GraphEdge), [`id`](graph-engine.ts.md#GraphNode.id), [`file`](graph-engine.ts.md#GraphNode.file), [`from`](graph-engine.ts.md#GraphEdge.from), [`name`](graph-engine.ts.md#GraphNode.name), [`properties`](graph-engine.ts.md#GraphEdge.properties), [`properties`](graph-engine.ts.md#GraphNode.properties), [`to`](graph-engine.ts.md#GraphEdge.to), [`type`](graph-engine.ts.md#GraphEdge.type), [`type`](graph-engine.ts.md#GraphNode.type)  (1 test-only)

### `GraphNode`
- def: [`website/api/v1/lib/graph-engine.ts:4`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L4)
- signature: `interface GraphNode`
- members:
  - `file` — [`L8`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L8)
  - `id` — [`L5`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L5)
  - `name` — [`L6`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L6)
  - `properties` — [`L9`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L9)
  - `type` — [`L7`](../../../../../../../../raw/code/codegraphcontext/website/api/v1/lib/graph-engine.ts#L7)
- used by: [`loadFromZip`](graph-engine.ts.md#GraphEngine.loadFromZip), [`findCallees`](graph-engine.ts.md#GraphEngine.findCallees), [`findCallers`](graph-engine.ts.md#GraphEngine.findCallers), [`getFileStructure`](graph-engine.ts.md#GraphEngine.getFileStructure), [`findDefinitions`](graph-engine.ts.md#GraphEngine.findDefinitions), [`nodes`](graph-engine.ts.md#GraphEngine.nodes), [`search`](graph-engine.ts.md#GraphEngine.search)

