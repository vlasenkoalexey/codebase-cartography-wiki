---
title: 'Module: website/src/lib/parser.worker.ts'
type: catalog
provenance: extracted
module: website/src/lib/parser.worker.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/lib/`parser.worker.ts`/
symbols:
  processNextBatch: processNextBatch().
  QUERIES: QUERIES.
  addNode: addNode.
  LangQueries.definitions: LangQueries#definitions.
  LangQueries.imports: LangQueries#imports.
  LangQueries.calls: LangQueries#calls.
  LangQueries.inherits: LangQueries#inherits.
  getOrCreateFolderChain: getOrCreateFolderChain().
  resolveSymbol: resolveSymbol().
  links: links.
  LangQueries.variables: LangQueries#variables.
  getLanguageForFile: getLanguageForFile().
  wasmLanguageCache: wasmLanguageCache.
  nodes: nodes.
  nodeSymbolIndex: nodeSymbolIndex.
  initParser: initParser().
  pendingFileQueue: pendingFileQueue.
  originalWarn: originalWarn.
  getCompiledQueries: getCompiledQueries().
  indexOptions: indexOptions.
  parser: parser.
  indexOptions.typeLiteral109.indexVariables: indexOptions.typeLiteral109:indexVariables.
  processedCount: processedCount.
  fileCalls: fileCalls.
  inheritances: inheritances.
  repoRootPrefix: repoRootPrefix.
  initPromise: initPromise.
  compiledQueryCache: compiledQueryCache.
  totalFiles: totalFiles.
  folderNodes: folderNodes.
  repoId: repoId.
  filePathToNodeId: filePathToNodeId.
  originalLog: originalLog.
  IGNORED_DIRS: IGNORED_DIRS.
  LangQueries: LangQueries#
  getLanguageQueryKey: getLanguageQueryKey().
  getNodeDisplayLabel: getNodeDisplayLabel().
  calculateComplexity: calculateComplexity().
  getPythonDocstring: getPythonDocstring().
  valForLabel: valForLabel().
  nodeIdSequence: nodeIdSequence.
  MAX_PARSEABLE_FILE_CHARS: MAX_PARSEABLE_FILE_CHARS.
  MAX_PARSEABLE_MINIFIED_FILE_CHARS: MAX_PARSEABLE_MINIFIED_FILE_CHARS.
  computeCommonPrefix: computeCommonPrefix().
---
# Module: [`website/src/lib/parser.worker.ts`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts)

## Classes
### `LangQueries`
- def: [`website/src/lib/parser.worker.ts:132`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L132)
- signature: `interface LangQueries`
- members:
  - `calls` — [`L138`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L138) — Captures
  - `definitions` — [`L134`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L134) — Captures
  - `imports` — [`L136`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L136) — Captures
  - `inherits` — [`L140`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L140) — Captures
  - `variables` — [`L142`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L142) — Captures
- used by: [`QUERIES`](parser.worker.ts.md#QUERIES)

## Functions
- `calculateComplexity(node: any)` — [`L528`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L528)
- `computeCommonPrefix(paths: string[])` — [`L618`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L618) — Compute the longest common directory prefix of all queued file paths.
- `getCompiledQueries(lang: any, queryKey: string)` — [`L574`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L574)
- `getLanguageForFile(path: string)` — [`L55`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L55)
- `getLanguageQueryKey(path: string)` — [`L491`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L491)
- `getNodeDisplayLabel(nodeType: string)` — [`L514`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L514)
- `getOrCreateFolderChain(filePath: string)` — [`L645`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L645) — Lazily create (or return cached) Folder nodes for the repo-relative segments only.
- `getPythonDocstring(node: any)` — [`L547`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L547)
- `initParser()` — [`L37`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L37)
- `processNextBatch()` — [`L750`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L750)
- `resolveSymbol(key: string, callerFile?: string)` — [`L739`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L739) — Resolve a symbol name to a single node ID, preferring candidates
- `valForLabel(label: string)` — [`L561`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L561)

## Module values
- `IGNORED_DIRS` — [`L25`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L25)
- `MAX_PARSEABLE_FILE_CHARS` — [`L610`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L610)
- `MAX_PARSEABLE_MINIFIED_FILE_CHARS` — [`L611`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L611)
- `QUERIES` — [`L144`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L144)
- `addNode` — [`L720`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L720)
- `compiledQueryCache` — [`L572`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L572)
- `fileCalls` — [`L604`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L604)
- `filePathToNodeId` — [`L602`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L602)
- `folderNodes` — [`L603`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L603)
- `indexOptions` — [`L609`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L609)
- `indexVariables` — [`L609`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L609)
- `inheritances` — [`L605`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L605)
- `initPromise` — [`L34`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L34)
- `links` — [`L600`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L600)
- `nodeIdSequence` — [`L606`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L606)
- `nodeSymbolIndex` — [`L601`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L601)
- `nodes` — [`L599`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L599)
- `originalLog` — [`L6`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L6)
- `originalWarn` — [`L7`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L7)
- `parser` — [`L33`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L33)
- `pendingFileQueue` — [`L595`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L595)
- `processedCount` — [`L597`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L597)
- `repoId` — [`L607`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L607)
- `repoRootPrefix` — [`L608`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L608)
- `totalFiles` — [`L596`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L596)
- `wasmLanguageCache` — [`L35`](../../../../../../../raw/code/codegraphcontext/website/src/lib/parser.worker.ts#L35)

