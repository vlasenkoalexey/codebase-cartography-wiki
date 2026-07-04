---
title: 'Module: website/src/components/PRReviewer.tsx'
type: catalog
provenance: extracted
module: website/src/components/PRReviewer.tsx
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/components/`PRReviewer.tsx`/
symbols:
  PRReviewer: PRReviewer().
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
  PRReviewer.-data-rawData-onClose-.typeLiteral289.data: 'PRReviewer().(`{ data: rawData,
    onClose }`)typeLiteral289:data.'
  PRReviewer.-data-rawData-onClose-.typeLiteral289.onClose: 'PRReviewer().(`{ data:
    rawData, onClose }`)typeLiteral289:onClose.'
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
# Module: [`website/src/components/PRReviewer.tsx`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx)

## Classes
### `CityPlatform`
- def: [`website/src/components/PRReviewer.tsx:116`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L116) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- signature: `interface CityPlatform`
- members:
  - `depth` — [`L118`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L118)
  - `h` — [`L117`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L117)
  - `name` — [`L118`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L118)
  - `path` — [`L118`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L118)
  - `w` — [`L117`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L117)
  - `x` — [`L117`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L117)
  - `z` — [`L117`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L117)
- used by: [`PRReviewer`](PRReviewer.tsx.md#PRReviewer), [`platformTop`](PRReviewer.tsx.md#layoutCityIslands.positions-Map.typeLiteral64.platformTop)

### `TreeNode`
- def: [`website/src/components/PRReviewer.tsx:194`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L194) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- signature: `interface TreeNode`
- members:
  - `children` — [`L198`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L198) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `isDir` — [`L197`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L197) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `name` — [`L195`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L195) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `path` — [`L196`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L196) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- used by: [`platformTop`](PRReviewer.tsx.md#layoutCityIslands.positions-Map.typeLiteral64.platformTop), [`searchQuery`](PRReviewer.tsx.md#TreeItem.-node-depth-selectedFile-onFileClick-searchQuery-.typeLiteral182.searchQuery), [`countTreeLeaves`](PRReviewer.tsx.md#countTreeLeaves), [`buildTree`](PRReviewer.tsx.md#buildTree), [`node`](PRReviewer.tsx.md#TreeItem.-node-depth-selectedFile-onFileClick-searchQuery-.typeLiteral182.node), [`layoutCityIslands`](PRReviewer.tsx.md#layoutCityIslands)

### `VisualizationMode`
- def: [`website/src/components/PRReviewer.tsx:95`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L95)
- signature: `type VisualizationMode`
- used by: [`PRReviewer`](PRReviewer.tsx.md#PRReviewer), [`VISUALIZATION_MODES`](PRReviewer.tsx.md#VISUALIZATION_MODES)

## Functions
- `PRReviewer({ data: rawData, onClose }: { data: any; onClose: () => void; })` — [`L357`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L357) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `TreeItem({ node, depth, selectedFile, onFileClick, searchQuery, }: { node: TreeNode; depth: number; selectedFile: string; onFileClick: (path: string) => void; searchQuery: string; })` — [`L238`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L238) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `buildTree(files: string[])` — [`L201`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L201) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `clamp(value: number, min: number, max: number)` — [`L340`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L340)
- `countTreeLeaves(node: TreeNode, nodesByFile: Map<string, any[]>)` — [`L121`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L121) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `getGraphAwareNodeScale(totalNodes: number)` — [`L350`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L350) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `getNodeDisplayName(node: any)` — [`L344`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L344) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `layoutCityIslands(items: TreeNode[], rect: { x: number; z: number; w: number; h: number; }, nodesByFile: Map<string, any[]>, positions: Map<number, { x: number; z: number; platformTop: number; }>, platforms: CityPlatform[], depth?: number)` — [`L130`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L130) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)

## Module values
- `CITY_ARC_SEGMENTS` — [`L191`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L191) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `CITY_HEIGHTS` — [`L185`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L185)
- `DEFAULT_EDGE_COLORS` — [`L84`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L84)
- `DEFAULT_NODE_COLORS` — [`L63`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L63) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `DEFAULT_SIDEBAR_W` — [`L338`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L338)
- `EMOJI_MAP` — [`L108`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L108) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `MAX_SIDEBAR_W` — [`L337`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L337)
- `MIN_SIDEBAR_W` — [`L336`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L336)
- `PALETTE` — [`L24`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L24)
- `PLATFORM_LAYER_H` — [`L127`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L127)
- `PLATFORM_PAD` — [`L128`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L128) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `VISUALIZATION_MODES` — [`L97`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L97) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `data` — [`L357`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L357)
- `depth` — [`L246`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L246)
- `h` — [`L132`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L132)
- `node` — [`L245`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L245)
- `onClose` — [`L357`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L357)
- `onFileClick` — [`L248`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L248)
- `platformTop` — [`L134`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L134) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `searchQuery` — [`L249`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L249)
- `selectedFile` — [`L247`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L247)
- `w` — [`L132`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L132)
- `x` — [`L132`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L132)
- `x` — [`L134`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L134)
- `z` — [`L132`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L132)
- `z` — [`L134`](../../../../../../../raw/code/codegraphcontext/website/src/components/PRReviewer.tsx#L134)

