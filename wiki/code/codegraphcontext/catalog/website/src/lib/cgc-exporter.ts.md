---
title: 'Module: website/src/lib/cgc-exporter.ts'
type: catalog
provenance: extracted
module: website/src/lib/cgc-exporter.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/lib/`cgc-exporter.ts`/
symbols:
  packageCgcBundle: packageCgcBundle().
  publishCgcBundle: publishCgcBundle().
  downloadBlob: downloadBlob().
  GraphLink.source: GraphLink#source.
  GraphLink.target: GraphLink#target.
  GraphNode.id: GraphNode#id.
  GraphNode.type: GraphNode#type.
  publishCgcBundle.Promise.typeLiteral71.success: publishCgcBundle().Promise:typeLiteral71:success.
  publishCgcBundle.Promise.typeLiteral71.message: publishCgcBundle().Promise:typeLiteral71:message.
  GraphNode: GraphNode#
  GraphNode.name: GraphNode#name.
  GraphNode.file: GraphNode#file.
  GraphNode.val: GraphNode#val.
  GraphNode.properties: GraphNode#properties.
  GraphLink: GraphLink#
  GraphLink.type: GraphLink#type.
  GraphLink.id: GraphLink#id.
  publishCgcBundle.Promise.typeLiteral71.entry: publishCgcBundle().Promise:typeLiteral71:entry.
---
# Module: [`website/src/lib/cgc-exporter.ts`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts)

## Classes
### `GraphLink`
- def: [`website/src/lib/cgc-exporter.ts:15`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L15)
- signature: `interface GraphLink`
- members:
  - `id` — [`L16`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L16)
  - `source` — [`L17`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L17)
  - `target` — [`L18`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L18)
  - `type` — [`L19`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L19)
- used by: [`packageCgcBundle`](cgc-exporter.ts.md#packageCgcBundle)

### `GraphNode`
- def: [`website/src/lib/cgc-exporter.ts:6`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L6)
- signature: `interface GraphNode`
- members:
  - `file` — [`L10`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L10)
  - `id` — [`L7`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L7)
  - `name` — [`L8`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L8)
  - `properties` — [`L12`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L12)
  - `type` — [`L9`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L9)
  - `val` — [`L11`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L11)
- used by: [`packageCgcBundle`](cgc-exporter.ts.md#packageCgcBundle)

## Functions
- `downloadBlob(blob: Blob, filename: string)` — [`L106`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L106) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `packageCgcBundle(repoName: string, nodes: GraphNode[], links: GraphLink[], version?: string, extraMetadata?: Record<string, any>)` — [`L22`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L22) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `publishCgcBundle(blob: Blob, repoName: string, version: string)` — [`L117`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L117) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)

## Module values
- `entry` — [`L121`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L121)
- `message` — [`L121`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L121)
- `success` — [`L121`](../../../../../../../raw/code/codegraphcontext/website/src/lib/cgc-exporter.ts#L121)

