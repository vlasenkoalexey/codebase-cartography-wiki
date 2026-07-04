---
title: 'Module: website/src/lib/html-exporter.ts'
type: catalog
provenance: extracted
module: website/src/lib/html-exporter.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/lib/`html-exporter.ts`/
symbols:
  packageInteractiveExport: packageInteractiveExport().
  generateClassicHTML: generateClassicHTML().
  generateFlowchartHTML: generateFlowchartHTML().
  GraphLink.source: GraphLink#source.
  GraphLink.target: GraphLink#target.
  GraphNode.id: GraphNode#id.
  SHARED_CSS: SHARED_CSS.
  fetchD3: fetchD3().
  GraphNode: GraphNode#
  GraphNode.name: GraphNode#name.
  GraphNode.type: GraphNode#type.
  GraphNode.file: GraphNode#file.
  GraphNode.val: GraphNode#val.
  GraphLink: GraphLink#
  GraphLink.type: GraphLink#type.
  GraphMetadata: GraphMetadata#
  GraphMetadata.repo: GraphMetadata#repo.
  GraphNode.properties: GraphNode#properties.
  GraphNode.color: GraphNode#color.
  GraphLink.id: GraphLink#id.
  GraphMetadata.branch: GraphMetadata#branch.
  GraphMetadata.commit: GraphMetadata#commit.
  GraphMetadata.version: GraphMetadata#version.
---
# Module: [`website/src/lib/html-exporter.ts`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts)

## Classes
### `GraphLink`
- def: [`website/src/lib/html-exporter.ts:19`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L19)
- signature: `interface GraphLink`
- members:
  - `id` — [`L20`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L20)
  - `source` — [`L21`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L21)
  - `target` — [`L22`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L22)
  - `type` — [`L23`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L23)
- used by: [`packageInteractiveExport`](html-exporter.ts.md#packageInteractiveExport)

### `GraphMetadata`
- def: [`website/src/lib/html-exporter.ts:26`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L26)
- signature: `interface GraphMetadata`
- members:
  - `branch` — [`L28`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L28)
  - `commit` — [`L29`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L29)
  - `repo` — [`L27`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L27)
  - `version` — [`L30`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L30)
- used by: [`packageInteractiveExport`](html-exporter.ts.md#packageInteractiveExport)

### `GraphNode`
- def: [`website/src/lib/html-exporter.ts:9`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L9)
- signature: `interface GraphNode`
- members:
  - `color` — [`L16`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L16)
  - `file` — [`L13`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L13)
  - `id` — [`L10`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L10)
  - `name` — [`L11`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L11)
  - `properties` — [`L15`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L15)
  - `type` — [`L12`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L12)
  - `val` — [`L14`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L14)
- used by: [`packageInteractiveExport`](html-exporter.ts.md#packageInteractiveExport)

## Functions
- `fetchD3()` — [`L3`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L3)
- `generateClassicHTML(dataJson: string, nodeColorsJson: string, edgeColorsJson: string, d3Bundle: string)` — [`L76`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L76) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `generateFlowchartHTML(dataJson: string, nodeColorsJson: string, edgeColorsJson: string, d3Bundle: string)` — [`L255`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L255) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `packageInteractiveExport(nodes: GraphNode[], links: GraphLink[], metadata: GraphMetadata, nodeColors: Record<string, string>, edgeColors: Record<string, string>, mode?: "classic" | "mermaid")` — [`L560`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L560) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)

## Module values
- `SHARED_CSS` — [`L35`](../../../../../../../raw/code/codegraphcontext/website/src/lib/html-exporter.ts#L35)

