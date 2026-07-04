---
title: 'Module: understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/components/`FileExplorer.tsx`/
symbols:
  FileExplorer: FileExplorer().
  FileTreeRow.-entry-depth-expanded-toggleFolder-openFile-.typeLiteral67.openFile: "FileTreeRow().(`{\n\
    \  entry,\n  depth,\n  expanded,\n  toggleFolder,\n  openFile,\n}`)typeLiteral67:openFile."
  buildFileTree: buildFileTree().
  FileTreeRow: FileTreeRow().
  FileEntry.children: FileEntry#children.
  FileEntry: FileEntry#
  FileEntry.path: FileEntry#path.
  FileEntry.type: FileEntry#type.
  FileEntry.name: FileEntry#name.
  FileTreeRow.-entry-depth-expanded-toggleFolder-openFile-.typeLiteral67.entry: "FileTreeRow().(`{\n\
    \  entry,\n  depth,\n  expanded,\n  toggleFolder,\n  openFile,\n}`)typeLiteral67:entry."
  FileEntry.nodeId: FileEntry#nodeId.
  FileTreeRow.-entry-depth-expanded-toggleFolder-openFile-.typeLiteral67.depth: "FileTreeRow().(`{\n\
    \  entry,\n  depth,\n  expanded,\n  toggleFolder,\n  openFile,\n}`)typeLiteral67:depth."
  FileTreeRow.-entry-depth-expanded-toggleFolder-openFile-.typeLiteral67.expanded: "FileTreeRow().(`{\n\
    \  entry,\n  depth,\n  expanded,\n  toggleFolder,\n  openFile,\n}`)typeLiteral67:expanded."
  FileTreeRow.-entry-depth-expanded-toggleFolder-openFile-.typeLiteral67.toggleFolder: "FileTreeRow().(`{\n\
    \  entry,\n  depth,\n  expanded,\n  toggleFolder,\n  openFile,\n}`)typeLiteral67:toggleFolder."
  normalizeFilePath: normalizeFilePath().
  bestFileNode: bestFileNode().
---
# Module: [`understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx)

## Classes
### `FileEntry`
- def: [`understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx:6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L6) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
- signature: `interface FileEntry`
- members:
  - `children` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L10) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
  - `name` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L7) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
  - `nodeId` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L11) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
  - `path` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L8) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
  - `type` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L9) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
- used by: [`FileExplorer`](FileExplorer.tsx.md#FileExplorer), [`openFile`](FileExplorer.tsx.md#FileTreeRow.-entry-depth-expanded-toggleFolder-openFile-.typeLiteral67.openFile), [`buildFileTree`](FileExplorer.tsx.md#buildFileTree), [`entry`](FileExplorer.tsx.md#FileTreeRow.-entry-depth-expanded-toggleFolder-openFile-.typeLiteral67.entry)

## Functions
- `FileExplorer()` — [`L142`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L142) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
- `FileTreeRow({ entry, depth, expanded, toggleFolder, openFile, }: { entry: FileEntry; depth: number; expanded: Set<string>; toggleFolder: (path: string) => void; openFile: (nodeId: string) => void; })` — [`L84`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L84) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
- `bestFileNode(existing: any, candidate: GraphNode)` — [`L21`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L21) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
- `buildFileTree(nodes: GraphNode[])` — [`L27`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L27) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)
- `normalizeFilePath(filePath: string)` — [`L14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L14) — documented in [understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx](../../../../../../concepts/understand-anything-plugin-packages-dashboard-src-components-FileExplorer.tsx.md)

## Module values
- `depth` — [`L92`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L92)
- `entry` — [`L91`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L91)
- `expanded` — [`L93`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L93)
- `openFile` — [`L95`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L95)
- `toggleFolder` — [`L94`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/FileExplorer.tsx#L94)

