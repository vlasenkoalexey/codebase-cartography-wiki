---
title: 'Module: website/src/components/CodeGraphViewer.tsx'
type: catalog
provenance: extracted
module: website/src/components/CodeGraphViewer.tsx
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/components/`CodeGraphViewer.tsx`/
symbols:
  CodeGraphViewer: CodeGraphViewer().
  layoutCityIslands.positions-Map.typeLiteral64.platformTop: layoutCityIslands().(positions)Map:typeLiteral64:platformTop.
  TreeItem.-node-depth-selectedFile-onFileClick-searchQuery-.typeLiteral182.searchQuery: "TreeItem().(`{\n\
    \  node,\n  depth,\n  selectedFile,\n  onFileClick,\n  searchQuery,\n}`)typeLiteral182:searchQuery."
  countTreeLeaves: countTreeLeaves().
  TreeItem: TreeItem().
  buildTree: buildTree().
  TreeNode: TreeNode#
  TreeNode.children: TreeNode#children.
  TreeNode.name: TreeNode#name.
  TreeNode.isDir: TreeNode#isDir.
  TreeNode.path: TreeNode#path.
  VISUALIZATION_MODES: VISUALIZATION_MODES.
  TreeItem.-node-depth-selectedFile-onFileClick-searchQuery-.typeLiteral182.node: "TreeItem().(`{\n\
    \  node,\n  depth,\n  selectedFile,\n  onFileClick,\n  searchQuery,\n}`)typeLiteral182:node."
  layoutCityIslands: layoutCityIslands().
  DEFAULT_NODE_COLORS: DEFAULT_NODE_COLORS.
  EMOJI_MAP: EMOJI_MAP.
  PLATFORM_PAD: PLATFORM_PAD.
  getNodeDisplayName: getNodeDisplayName().
  getGraphAwareNodeScale: getGraphAwareNodeScale().
  CityPlatform: CityPlatform#
  layoutCityIslands.rect-typeLiteral63.w: layoutCityIslands().(rect)typeLiteral63:w.
  layoutCityIslands.rect-typeLiteral63.h: layoutCityIslands().(rect)typeLiteral63:h.
  CITY_ARC_SEGMENTS: CITY_ARC_SEGMENTS.
  TreeItem.-node-depth-selectedFile-onFileClick-searchQuery-.typeLiteral182.depth: "TreeItem().(`{\n\
    \  node,\n  depth,\n  selectedFile,\n  onFileClick,\n  searchQuery,\n}`)typeLiteral182:depth."
  TreeItem.-node-depth-selectedFile-onFileClick-searchQuery-.typeLiteral182.selectedFile: "TreeItem().(`{\n\
    \  node,\n  depth,\n  selectedFile,\n  onFileClick,\n  searchQuery,\n}`)typeLiteral182:selectedFile."
  TreeItem.-node-depth-selectedFile-onFileClick-searchQuery-.typeLiteral182.onFileClick: "TreeItem().(`{\n\
    \  node,\n  depth,\n  selectedFile,\n  onFileClick,\n  searchQuery,\n}`)typeLiteral182:onFileClick."
  PALETTE: PALETTE.
  DEFAULT_EDGE_COLORS: DEFAULT_EDGE_COLORS.
  VisualizationMode: VisualizationMode#
  PLATFORM_LAYER_H: PLATFORM_LAYER_H.
  layoutCityIslands.rect-typeLiteral63.x: layoutCityIslands().(rect)typeLiteral63:x.
  layoutCityIslands.rect-typeLiteral63.z: layoutCityIslands().(rect)typeLiteral63:z.
  CITY_HEIGHTS: CITY_HEIGHTS.
  DEFAULT_SIDEBAR_W: DEFAULT_SIDEBAR_W.
  clamp: clamp().
  CodeGraphViewer.-data-rawData-onClose-.typeLiteral289.data: 'CodeGraphViewer().(`{
    data: rawData, onClose }`)typeLiteral289:data.'
  CodeGraphViewer.-data-rawData-onClose-.typeLiteral289.onClose: 'CodeGraphViewer().(`{
    data: rawData, onClose }`)typeLiteral289:onClose.'
  CityPlatform.x: CityPlatform#x.
  CityPlatform.z: CityPlatform#z.
  CityPlatform.w: CityPlatform#w.
  CityPlatform.h: CityPlatform#h.
  CityPlatform.depth: CityPlatform#depth.
  CityPlatform.name: CityPlatform#name.
  CityPlatform.path: CityPlatform#path.
  MIN_SIDEBAR_W: MIN_SIDEBAR_W.
  MAX_SIDEBAR_W: MAX_SIDEBAR_W.
  layoutCityIslands.positions-Map.typeLiteral64.x: layoutCityIslands().(positions)Map:typeLiteral64:x.
  layoutCityIslands.positions-Map.typeLiteral64.z: layoutCityIslands().(positions)Map:typeLiteral64:z.
---
# Module: [`website/src/components/CodeGraphViewer.tsx`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx)

## Classes
### `CityPlatform`
- def: [`website/src/components/CodeGraphViewer.tsx:126`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L126) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- signature: `interface CityPlatform`
- members:
  - `depth` — [`L128`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L128)
  - `h` — [`L127`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L127)
  - `name` — [`L128`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L128)
  - `path` — [`L128`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L128)
  - `w` — [`L127`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L127)
  - `x` — [`L127`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L127)
  - `z` — [`L127`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L127)
- used by: [`CodeGraphViewer`](CodeGraphViewer.tsx.md#CodeGraphViewer), [`platformTop`](CodeGraphViewer.tsx.md#layoutCityIslands.positions-Map.typeLiteral64.platformTop)

### `TreeNode`
- def: [`website/src/components/CodeGraphViewer.tsx:204`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L204) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- signature: `interface TreeNode`
- members:
  - `children` — [`L208`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L208) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
  - `isDir` — [`L207`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L207) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
  - `name` — [`L205`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L205) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
  - `path` — [`L206`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L206) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- used by: [`platformTop`](CodeGraphViewer.tsx.md#layoutCityIslands.positions-Map.typeLiteral64.platformTop), [`searchQuery`](CodeGraphViewer.tsx.md#TreeItem.-node-depth-selectedFile-onFileClick-searchQuery-.typeLiteral182.searchQuery), [`countTreeLeaves`](CodeGraphViewer.tsx.md#countTreeLeaves), [`buildTree`](CodeGraphViewer.tsx.md#buildTree), [`node`](CodeGraphViewer.tsx.md#TreeItem.-node-depth-selectedFile-onFileClick-searchQuery-.typeLiteral182.node), [`layoutCityIslands`](CodeGraphViewer.tsx.md#layoutCityIslands)

### `VisualizationMode`
- def: [`website/src/components/CodeGraphViewer.tsx:105`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L105)
- signature: `type VisualizationMode`
- used by: [`CodeGraphViewer`](CodeGraphViewer.tsx.md#CodeGraphViewer), [`VISUALIZATION_MODES`](CodeGraphViewer.tsx.md#VISUALIZATION_MODES)

## Functions
- `CodeGraphViewer({ data: rawData, onClose }: { data: any; onClose: () => void; })` — [`L367`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L367) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `TreeItem({ node, depth, selectedFile, onFileClick, searchQuery, }: { node: TreeNode; depth: number; selectedFile: string; onFileClick: (path: string) => void; searchQuery: string; })` — [`L248`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L248) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `buildTree(files: string[])` — [`L211`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L211) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `clamp(value: number, min: number, max: number)` — [`L350`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L350)
- `countTreeLeaves(node: TreeNode, nodesByFile: Map<string, any[]>)` — [`L131`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L131) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `getGraphAwareNodeScale(totalNodes: number)` — [`L360`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L360) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `getNodeDisplayName(node: any)` — [`L354`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L354) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `layoutCityIslands(items: TreeNode[], rect: { x: number; z: number; w: number; h: number; }, nodesByFile: Map<string, any[]>, positions: Map<number, { x: number; z: number; platformTop: number; }>, platforms: CityPlatform[], depth?: number)` — [`L140`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L140) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)

## Module values
- `CITY_ARC_SEGMENTS` — [`L201`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L201)
- `CITY_HEIGHTS` — [`L195`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L195) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `DEFAULT_EDGE_COLORS` — [`L94`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L94)
- `DEFAULT_NODE_COLORS` — [`L73`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L73) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `DEFAULT_SIDEBAR_W` — [`L348`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L348)
- `EMOJI_MAP` — [`L118`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L118) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `MAX_SIDEBAR_W` — [`L347`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L347)
- `MIN_SIDEBAR_W` — [`L346`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L346)
- `PALETTE` — [`L34`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L34)
- `PLATFORM_LAYER_H` — [`L137`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L137)
- `PLATFORM_PAD` — [`L138`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L138) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `VISUALIZATION_MODES` — [`L107`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L107) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `data` — [`L367`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L367) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `depth` — [`L256`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L256)
- `h` — [`L142`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L142) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `node` — [`L255`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L255)
- `onClose` — [`L367`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L367)
- `onFileClick` — [`L258`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L258)
- `platformTop` — [`L144`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L144) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `searchQuery` — [`L259`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L259)
- `selectedFile` — [`L257`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L257)
- `w` — [`L142`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L142) — documented in [website-src-components-CodeGraphViewer.tsx](../../../../concepts/website-src-components-CodeGraphViewer.tsx.md)
- `x` — [`L142`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L142)
- `x` — [`L144`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L144)
- `z` — [`L142`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L142)
- `z` — [`L144`](../../../../../../../raw/code/codegraphcontext/website/src/components/CodeGraphViewer.tsx#L144)

