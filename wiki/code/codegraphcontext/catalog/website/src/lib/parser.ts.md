---
title: 'Module: website/src/lib/parser.ts'
type: catalog
provenance: extracted
module: website/src/lib/parser.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/lib/`parser.ts`/
symbols:
  parseFilesIntoGraph.options-typeLiteral9.maxEdges: parseFilesIntoGraph().(options)typeLiteral9:maxEdges.
  readDirectoryRecursive: readDirectoryRecursive().
  fetchGitlabRepoFiles: fetchGitlabRepoFiles().
  parseFilesIntoGraph: parseFilesIntoGraph().
  parseFilesIntoGraph.options-typeLiteral9.indexVariables: parseFilesIntoGraph().(options)typeLiteral9:indexVariables.
  parseFilesIntoGraph.options-typeLiteral9.maxNodes: parseFilesIntoGraph().(options)typeLiteral9:maxNodes.
  parseFilesIntoGraph.Promise.typeLiteral10.nodes: parseFilesIntoGraph().Promise:typeLiteral10:nodes.
  parseFilesIntoGraph.Promise.typeLiteral10.links: parseFilesIntoGraph().Promise:typeLiteral10:links.
  parseFilesIntoGraph.Promise.typeLiteral10.files: parseFilesIntoGraph().Promise:typeLiteral10:files.
  unzipFiles: unzipFiles().
  fetchGithubRepoFiles: fetchGithubRepoFiles().
---
# Module: [`website/src/lib/parser.ts`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts)

## Functions
- `fetchGithubRepoFiles(url: string, onProgress?: (msg: string) => void)` — [`L125`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L125)
- `fetchGitlabRepoFiles(url: string, onProgress?: (msg: string) => void)` — [`L83`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L83)
- `parseFilesIntoGraph(files: { path: string; content: string; }[], onProgressTracker?: (progressMsg: string, percentage: number, diagnosticLog?: string) => void, options?: { indexVariables?: boolean; maxNodes?: number; maxEdges?: number; })` — [`L7`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L7) — Parses files into a high-fidelity AST graph using a Web Worker.
- `readDirectoryRecursive(dirHandle: any, prefix?: string)` — [`L53`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L53)
- `unzipFiles(zipBuffer: ArrayBuffer)` — [`L70`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L70)

## Module values
- `files` — [`L15`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L15)
- `indexVariables` — [`L11`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L11)
- `links` — [`L15`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L15)
- `maxEdges` — [`L13`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L13)
- `maxNodes` — [`L12`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L12)
- `nodes` — [`L15`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.ts#L15)

