---
title: 'Module: understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx
status: fresh
symbol_base: scip-typescript npm @understand-anything/dashboard 0.1.0 src/components/`CodeViewer.tsx`/
symbols:
  CodeViewer: CodeViewer().
  SourceState: SourceState#
  SourceFile: SourceFile#
  CodeViewerProps: CodeViewerProps#
  CodeViewerProps.accessToken: CodeViewerProps#accessToken.
  CodeViewerProps.presentation: CodeViewerProps#presentation.
  CodeViewerProps.onClose: CodeViewerProps#onClose.
  CodeViewerProps.onExpand: CodeViewerProps#onExpand.
  fileContentUrl: fileContentUrl().
  fallbackLanguage: fallbackLanguage().
  formatBytes: formatBytes().
  SourceFile.path: SourceFile#path.
  SourceFile.language: SourceFile#language.
  SourceFile.content: SourceFile#content.
  SourceFile.sizeBytes: SourceFile#sizeBytes.
  SourceFile.lineCount: SourceFile#lineCount.
---
# Module: [`understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx)

## Classes
### `CodeViewerProps`
- def: [`understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx:6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L6)
- signature: `interface CodeViewerProps`
- members:
  - `accessToken` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L7)
  - `onClose` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L9)
  - `onExpand` — [`L10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L10)
  - `presentation` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L8)
- used by: [`CodeViewer`](CodeViewer.tsx.md#CodeViewer)

### `SourceFile`
- def: [`understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx:13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L13)
- signature: `interface SourceFile`
- members:
  - `content` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L16)
  - `language` — [`L15`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L15)
  - `lineCount` — [`L18`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L18)
  - `path` — [`L14`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L14)
  - `sizeBytes` — [`L17`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L17)
- used by: [`CodeViewer`](CodeViewer.tsx.md#CodeViewer), [`SourceState`](CodeViewer.tsx.md#SourceState)

### `SourceState`
- def: [`understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx:21`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L21)
- signature: `type SourceState`
- uses (calls/refs, reference-scoped): [`SourceFile`](CodeViewer.tsx.md#SourceFile)
- used by: [`CodeViewer`](CodeViewer.tsx.md#CodeViewer)

## Functions
- `CodeViewer({ accessToken, presentation, onClose, onExpand, }: CodeViewerProps)` — [`L59`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L59)
- `fallbackLanguage(filePath: string | undefined)` — [`L31`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L31)
- `fileContentUrl(filePath: string, token: string)` — [`L26`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L26)
- `formatBytes(bytes: number)` — [`L53`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/dashboard/src/components/CodeViewer.tsx#L53)

