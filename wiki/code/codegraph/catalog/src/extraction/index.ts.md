---
title: 'Module: src/extraction/index.ts'
type: catalog
provenance: extracted
module: src/extraction/index.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`index.ts`/
symbols:
  ExtractionOrchestrator.indexAll: ExtractionOrchestrator#indexAll().
  ExtractionOrchestrator.storeExtractionResult: ExtractionOrchestrator#storeExtractionResult().
  ExtractionOrchestrator.sync: ExtractionOrchestrator#sync().
  ExtractionOrchestrator.indexFileWithContent: ExtractionOrchestrator#indexFileWithContent().
  ExtractionOrchestrator.getChangedFiles: ExtractionOrchestrator#getChangedFiles().
  ExtractionOrchestrator.buildDetectionContext: ExtractionOrchestrator#buildDetectionContext().
  collectGitStatus: collectGitStatus().
  ExtractionOrchestrator.indexFiles: ExtractionOrchestrator#indexFiles().
  discoverEmbeddedRepoRoots: discoverEmbeddedRepoRoots().
  scanDirectoryWalk: scanDirectoryWalk().
  ExtractionOrchestrator.indexFile: ExtractionOrchestrator#indexFile().
  collectGitFiles: collectGitFiles().
  getGitChangedFiles: getGitChangedFiles().
  ExtractionOrchestrator.rootDir: ExtractionOrchestrator#rootDir.
  findNestedGitRepos: findNestedGitRepos().
  ExtractionOrchestrator.queries: ExtractionOrchestrator#queries.
  ExtractionOrchestrator.ensureDetectedFrameworks: ExtractionOrchestrator#ensureDetectedFrameworks().
  IndexProgress.phase: IndexProgress#phase.
  IndexProgress.current: IndexProgress#current.
  IndexProgress.total: IndexProgress#total.
  buildScopeIgnore: buildScopeIgnore().
  ScopeIgnore.ignores: ScopeIgnore#ignores().
  findIgnoredEmbeddedRepos: findIgnoredEmbeddedRepos().
  getGitVisibleFiles: getGitVisibleFiles().
  scanDirectory: scanDirectory().
  scanDirectoryAsync: scanDirectoryAsync().
  buildDefaultIgnore: buildDefaultIgnore().
  defaultsOnlyIgnore: defaultsOnlyIgnore().
  ExtractionOrchestrator.-constructor: ExtractionOrchestrator#`<constructor>`().
  SyncResult.filesAdded: SyncResult#filesAdded.
  SyncResult.filesModified: SyncResult#filesModified.
  DEFAULT_IGNORE_PATTERNS: DEFAULT_IGNORE_PATTERNS.
  readGitignorePatterns: readGitignorePatterns().
  IndexProgress: IndexProgress#
  IndexResult: IndexResult#
  IndexResult.success: IndexResult#success.
  SyncResult.filesRemoved: SyncResult#filesRemoved.
  loadIncludeIgnoredMatcher: loadIncludeIgnoredMatcher().
  loadExcludeMatcher: loadExcludeMatcher().
  IndexResult.filesIndexed: IndexResult#filesIndexed.
  ScopeIgnore.-constructor-.embedded-Array.typeLiteral95.matcher: ScopeIgnore#`<constructor>`().(embedded)Array:typeLiteral95:matcher.
  ExtractionOrchestrator.detectedFrameworkNames: ExtractionOrchestrator#detectedFrameworkNames.
  gitlinkEmbeddedRepoSkipped: gitlinkEmbeddedRepoSkipped().
  SyncResult: SyncResult#
  hashContent: hashContent().
  MAX_FILE_SIZE: MAX_FILE_SIZE.
  classifyGitDir: classifyGitDir().
  listIgnoredDirs: listIgnoredDirs().
  ScopeIgnore.defaults: ScopeIgnore#defaults.
  IndexProgress.currentFile: IndexProgress#currentFile.
  SyncResult.durationMs: SyncResult#durationMs.
  ScopeIgnore: ScopeIgnore#
  ScopeIgnore.embedded: ScopeIgnore#embedded.
  GitChanges: GitChanges#
  GitChanges.modified: GitChanges#modified.
  GitChanges.added: GitChanges#added.
  GitChanges.deleted: GitChanges#deleted.
  IndexResult.errors: IndexResult#errors.
  FILE_IO_BATCH_SIZE: FILE_IO_BATCH_SIZE.
  SYNC_RECONCILE_YIELD_INTERVAL: SYNC_RECONCILE_YIELD_INTERVAL.
  SyncResult.changedFilePaths: SyncResult#changedFilePaths.
  isWholeCwdEntry: isWholeCwdEntry().
  ScopeIgnore.embedded.Array.typeLiteral94.root: ScopeIgnore#embedded.Array:typeLiteral94:root.
  ScopeIgnore.-constructor-.embedded-Array.typeLiteral95.root: ScopeIgnore#`<constructor>`().(embedded)Array:typeLiteral95:root.
  ExtractionOrchestrator: ExtractionOrchestrator#
  ExtractionOrchestrator.getChangedFiles.typeLiteral962.added: ExtractionOrchestrator#getChangedFiles().typeLiteral962:added.
  ExtractionOrchestrator.getChangedFiles.typeLiteral962.modified: ExtractionOrchestrator#getChangedFiles().typeLiteral962:modified.
  ExtractionOrchestrator.getChangedFiles.typeLiteral962.removed: ExtractionOrchestrator#getChangedFiles().typeLiteral962:removed.
  PARSE_TIMEOUT_MS: PARSE_TIMEOUT_MS.
  WORKER_RECYCLE_INTERVAL: WORKER_RECYCLE_INTERVAL.
  IndexResult.nodesCreated: IndexResult#nodesCreated.
  IndexResult.edgesCreated: IndexResult#edgesCreated.
  SyncResult.filesChecked: SyncResult#filesChecked.
  SyncResult.nodesUpdated: SyncResult#nodesUpdated.
  DEFAULT_IGNORE_DIRS: DEFAULT_IGNORE_DIRS.
  ANDROID_RES_TYPES: ANDROID_RES_TYPES.
  isValidUtf8: isValidUtf8().
  EMBEDDED_REPO_SEARCH_DEPTH: EMBEDDED_REPO_SEARCH_DEPTH.
  EMBEDDED_REPO_SEARCH_ENTRIES: EMBEDDED_REPO_SEARCH_ENTRIES.
  ScopeIgnore.embedded.Array.typeLiteral94.matcher: ScopeIgnore#embedded.Array:typeLiteral94:matcher.
  ScopeIgnore.-constructor: ScopeIgnore#`<constructor>`().
  IndexResult.filesSkipped: IndexResult#filesSkipped.
  IndexResult.filesErrored: IndexResult#filesErrored.
  IndexResult.durationMs: IndexResult#durationMs.
---
# Module: [`src/extraction/index.ts`](../../../../../../raw/code/codegraph/src/extraction/index.ts)

## Classes
### `ExtractionOrchestrator`
- def: [`src/extraction/index.ts:1115`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1115)
- doc: Extraction orchestrator
- signature: `class ExtractionOrchestrator`
- members:
  - `<constructor>(rootDir: string, queries: QueryBuilder)` — [`L1126`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1126) — Extraction orchestrator
  - `buildDetectionContext(method)` — [`L1137`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1137) — Build a filesystem-backed ResolutionContext sufficient for framework — documented in [utils.ts](../../../concepts/utils.ts.md)
  - `ensureDetectedFrameworks(method)` — [`L1192`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1192) — Detect frameworks on demand using the current scanned files (or a fresh
  - `getChangedFiles(method)` — [`L2080`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L2080) — Get files that have changed since last index.
  - `indexAll(method)` — [`L1203`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1203) — Index all files in the project — documented in [extraction-index.ts](../../../concepts/extraction-index.ts.md)
  - `indexFile(method)` — [`L1705`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1705) — Index a single file — documented in [utils.ts](../../../concepts/utils.ts.md)
  - `indexFileWithContent(method)` — [`L1749`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1749) — Index a single file with pre-read content and stats. — documented in [extraction-index.ts](../../../concepts/extraction-index.ts.md)
  - `indexFiles(method)` — [`L1658`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1658) — Index specific files
  - `storeExtractionResult(method)` — [`L1814`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1814) — Store extraction result in database — documented in [extraction-index.ts](../../../concepts/extraction-index.ts.md)
  - `sync(method)` — [`L1938`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1938) — Sync the index with the current file state. — documented in [extraction-index.ts](../../../concepts/extraction-index.ts.md)
  - `added` — [`L2080`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L2080)
  - `detectedFrameworkNames` — [`L1124`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1124) — Names of frameworks detected for this project, populated by indexAll().
  - `modified` — [`L2080`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L2080)
  - `queries` — [`L1117`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1117)
  - `removed` — [`L2080`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L2080)
  - `rootDir` — [`L1116`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L1116)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`ResolutionContext`](../resolution/types.ts.md#ResolutionContext), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`target`](../types.ts.md#Edge.target), [`source`](../types.ts.md#Edge.source), [`kind`](../types.ts.md#Edge.kind), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`extractFromSource`](tree-sitter.ts.md#extractFromSource), [`Language`](../types.ts.md#Language), [`readFile`](../resolution/types.ts.md#ResolutionContext.readFile), [`getNodesByName`](../resolution/types.ts.md#ResolutionContext.getNodesByName), [`getNodesInFile`](../resolution/types.ts.md#ResolutionContext.getNodesInFile), [`line`](../types.ts.md#Edge.line), [`getAllFiles`](../resolution/types.ts.md#ResolutionContext.getAllFiles), [`<constructor>`](parse-pool.ts.md#ParseWorkerPool.-constructor), [`QueryBuilder`](../db/queries.ts.md#QueryBuilder), [`metadata`](../types.ts.md#Edge.metadata), [`provenance`](../types.ts.md#Edge.provenance), [`ExtractionResult`](../types.ts.md#ExtractionResult), [`fileExists`](../resolution/types.ts.md#ResolutionContext.fileExists), [`logDebug`](../errors.ts.md#logDebug), [`nodes`](../types.ts.md#ExtractionResult.nodes), [`upsertFile`](../db/queries.ts.md#QueryBuilder.upsertFile), [`errors`](../types.ts.md#ExtractionResult.errors), [`name`](../resolution/types.ts.md#FrameworkResolver.name), [`path`](../types.ts.md#FileRecord.path), [`detectLanguage`](grammars.ts.md#detectLanguage), [`severity`](../types.ts.md#ExtractionError.severity), [`message`](../types.ts.md#ExtractionError.message), [`loadGrammarsForLanguages`](grammars.ts.md#loadGrammarsForLanguages), [`requestParse`](parse-pool.ts.md#ParseWorkerPool.requestParse), [`edges`](../types.ts.md#ExtractionResult.edges), [`insertEdges`](../db/queries.ts.md#QueryBuilder.insertEdges), [`getAllFiles`](../db/queries.ts.md#QueryBuilder.getAllFiles), [`unresolvedReferences`](../types.ts.md#ExtractionResult.unresolvedReferences), [`getFileByPath`](../db/queries.ts.md#QueryBuilder.getFileByPath)  (+65 more)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`indexAll`](../index.ts.md#CodeGraph.indexAll), [`sync`](../index.ts.md#CodeGraph.sync), [`wireLayers`](../index.ts.md#CodeGraph.wireLayers), [`indexFiles`](../index.ts.md#CodeGraph.indexFiles), [`orchestrator`](../index.ts.md#CodeGraph.orchestrator), [`getChangedFiles`](../index.ts.md#CodeGraph.getChangedFiles)

### `GitChanges`
- def: [`src/extraction/index.ts:813`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L813)
- doc: Result of git-based change detection.
- signature: `interface GitChanges`
- members:
  - `added` — [`L815`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L815)
  - `deleted` — [`L816`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L816)
  - `modified` — [`L814`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L814)
- used by: [`getChangedFiles`](index.ts.md#ExtractionOrchestrator.getChangedFiles), [`collectGitStatus`](index.ts.md#collectGitStatus), [`getGitChangedFiles`](index.ts.md#getGitChangedFiles)

### `IndexProgress`
- def: [`src/extraction/index.ts:71`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L71)
- doc: Progress callback for indexing operations
- signature: `interface IndexProgress`
- members:
  - `current` — [`L73`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L73)
  - `currentFile` — [`L75`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L75)
  - `phase` — [`L72`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L72)
  - `total` — [`L74`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L74)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`indexAll`](index.ts.md#ExtractionOrchestrator.indexAll), [`indexAll`](../index.ts.md#CodeGraph.indexAll), [`sync`](../index.ts.md#CodeGraph.sync), [`sync`](index.ts.md#ExtractionOrchestrator.sync), [`onProgress`](../index.ts.md#IndexOptions.onProgress), [`InitOptions`](../index.ts.md#InitOptions)

### `IndexResult`
- def: [`src/extraction/index.ts:81`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L81)
- doc: Result of an indexing operation
- signature: `interface IndexResult`
- members:
  - `durationMs` — [`L89`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L89)
  - `edgesCreated` — [`L87`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L87)
  - `errors` — [`L88`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L88)
  - `filesErrored` — [`L85`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L85)
  - `filesIndexed` — [`L83`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L83)
  - `filesSkipped` — [`L84`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L84)
  - `nodesCreated` — [`L86`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L86)
  - `success` — [`L82`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L82)
- uses (calls/refs, reference-scoped): [`ExtractionError`](../types.ts.md#ExtractionError)
- used by: [`main`](../bin/codegraph.ts.md#main), [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`indexAll`](index.ts.md#ExtractionOrchestrator.indexAll), [`indexAll`](../index.ts.md#CodeGraph.indexAll), [`indexFiles`](index.ts.md#ExtractionOrchestrator.indexFiles), [`indexFiles`](../index.ts.md#CodeGraph.indexFiles)

### `ScopeIgnore`
- def: [`src/extraction/index.ts:460`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L460)
- doc: Workspace-scope ignore matcher. Ordinary paths get the root's matcher
- signature: `class ScopeIgnore`
- members:
  - `<constructor>(rootMatcher: Ignore, embedded: { root: string; matcher: Ignore; }[], exclude?: any)` — [`L463`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L463) — Workspace-scope ignore matcher. Ordinary paths get the root's matcher
  - `ignores(method)` — [`L477`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L477) — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
  - `defaults` — [`L462`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L462)
  - `embedded` — [`L461`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L461)
  - `matcher` — [`L461`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L461)
  - `matcher` — [`L465`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L465)
  - `root` — [`L461`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L461)
  - `root` — [`L465`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L465)
- uses (calls/refs, reference-scoped): [`defaultsOnlyIgnore`](index.ts.md#defaultsOnlyIgnore)
- used by: [`watcher.ts`](../sync/watcher.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-sync-watcher.ts), [`handleChange`](../sync/watcher.ts.md#FileWatcher.handleChange), [`buildScopeIgnore`](index.ts.md#buildScopeIgnore), [`shouldIgnoreDir`](../sync/watcher.ts.md#FileWatcher.shouldIgnoreDir), [`getGitVisibleFiles`](index.ts.md#getGitVisibleFiles), [`ignoreMatcher`](../sync/watcher.ts.md#FileWatcher.ignoreMatcher)

### `SyncResult`
- def: [`src/extraction/index.ts:95`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L95)
- doc: Result of a sync operation
- signature: `interface SyncResult`
- members:
  - `changedFilePaths` — [`L102`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L102)
  - `durationMs` — [`L101`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L101)
  - `filesAdded` — [`L97`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L97)
  - `filesChecked` — [`L96`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L96)
  - `filesModified` — [`L98`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L98)
  - `filesRemoved` — [`L99`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L99)
  - `nodesUpdated` — [`L100`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L100)
- used by: [`main`](../bin/codegraph.ts.md#main), [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`sync`](../index.ts.md#CodeGraph.sync), [`sync`](index.ts.md#ExtractionOrchestrator.sync), [`watch`](../index.ts.md#CodeGraph.watch), [`catchUpSync`](../mcp/engine.ts.md#MCPEngine.catchUpSync)

## Functions
- `buildDefaultIgnore(rootDir: string)` — [`L281`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L281) — An `ignore` matcher seeded with the built-in defaults, merged with the project's — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
- `buildScopeIgnore(rootDir: string, embeddedRoots?: Iterable<string> | undefined)` — [`L505`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L505) — Build the workspace-scope matcher. When the caller already knows the — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
- `classifyGitDir(absDir: string)` — [`L380`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L380) — Classify a directory's `.git` entry for embedded-repo discovery.
- `collectGitFiles(repoDir: string, prefix: string, files: Set<string>, embeddedRoots?: Set<string> | undefined, includeIgnored?: any)` — [`L661`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L661) — Collect git-visible files (tracked + untracked, .gitignore-respected) from the — documented in [utils.ts](../../../concepts/utils.ts.md)
- `collectGitStatus(repoDir: string, prefix: string, out: GitChanges, overrides?: Record<string, "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | ... 28 more ... | "unknown"> | undefined, includeIgnored?: any, exclude?: any)` — [`L846`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L846) — documented in [utils.ts](../../../concepts/utils.ts.md)
- `defaultsOnlyIgnore()` — [`L293`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L293) — Defaults-only ignore matcher (no root `.gitignore` merged). Used wherever the
- `discoverEmbeddedRepoRoots(rootDir: string)` — [`L557`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L557) — Standalone discovery of every embedded repo root under `rootDir` (relative, — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
- `findIgnoredEmbeddedRepos(repoDir: string, includeIgnored: any, prefix: string)` — [`L630`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L630) — Discover embedded repos hidden by `repoDir`'s OWN gitignore rules: for each — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
- `findNestedGitRepos(absDir: string, relPrefix: string)` — [`L410`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L410) — Find git repositories nested under `absDir` (inclusive), shallow bounded BFS. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
- `getGitChangedFiles(rootDir: string)` — [`L833`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L833) — Use `git status` to detect changed files instead of scanning every file.
- `getGitVisibleFiles(rootDir: string)` — [`L766`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L766) — Get all files visible to git (tracked + untracked but not ignored).
- `gitlinkEmbeddedRepoSkipped(relDir: string, prefix: string, defaults: Ignore, repoIgnore: Ignore, includeIgnored: any)` — [`L535`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L535) — Whether an embedded repo found as a tracked gitlink (mode 160000, #1031/#1033) — documented in [utils.ts](../../../concepts/utils.ts.md)
- `hashContent(content: string)` — [`L108`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L108) — Calculate SHA256 hash of file contents
- `isValidUtf8(buf: Buffer)` — [`L203`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L203) — True if `buf` decodes as strict UTF-8 (no invalid byte sequences).
- `isWholeCwdEntry(entry: string)` — [`L336`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L336) — `git ls-files --directory` collapses a wholly-untracked/ignored directory into
- `listIgnoredDirs(repoDir: string)` — [`L347`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L347) — List the gitignored DIRECTORIES of a repo (collapsed, trailing-slash form),
- `loadExcludeMatcher(rootDir: string)` — [`L320`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L320) — Matcher for the project's `codegraph.json` `exclude` patterns — paths to keep
- `loadIncludeIgnoredMatcher(rootDir: string)` — [`L306`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L306) — Matcher for the project's `codegraph.json` `includeIgnored` patterns — the
- `readGitignorePatterns(giPath: string)` — [`L229`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L229) — Read a `.gitignore` and return patterns safe to hand to the `ignore` matcher —
- `scanDirectory(rootDir: string, onProgress?: ((current: number, file: string) => void) | undefined)` — [`L928`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L928) — Recursively scan a directory for source files.
- `scanDirectoryAsync(rootDir: string, onProgress?: ((current: number, file: string) => void) | undefined)` — [`L958`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L958) — Async variant of scanDirectory that yields to the event loop periodically,
- `scanDirectoryWalk(rootDir: string, onProgress?: ((current: number, file: string) => void) | undefined)` — [`L989`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L989) — Filesystem walk fallback for non-git projects. — documented in [utils.ts](../../../concepts/utils.ts.md)

## Module values
- `ANDROID_RES_TYPES` — [`L187`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L187) — Android resource directory types. A `res/` tree holds ONLY non-code resources —
- `DEFAULT_IGNORE_DIRS` — [`L133`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L133) — Directory names that are dependency, build, cache, or tooling output across the
- `DEFAULT_IGNORE_PATTERNS` — [`L193`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L193) — Gitignore-style patterns for the `ignore` matcher: the dirs above plus a few globs.
- `EMBEDDED_REPO_SEARCH_DEPTH` — [`L361`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L361) — Max directory depth searched below an ignored dir for nested `.git` roots.
- `EMBEDDED_REPO_SEARCH_ENTRIES` — [`L363`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L363) — Max directories examined per search — a huge ignored data dir must never stall a scan/sync.
- `FILE_IO_BATCH_SIZE` — [`L36`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L36) — Number of files to read in parallel during indexing.
- `MAX_FILE_SIZE` — [`L117`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L117) — Skip files larger than this (bytes). Generated bundles, minified JS, and
- `PARSE_TIMEOUT_MS` — [`L57`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L57) — Maximum time (ms) to wait for a single file to parse in the worker thread.
- `SYNC_RECONCILE_YIELD_INTERVAL` — [`L48`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L48) — How many files the `sync()` reconcile processes between cooperative yields to
- `WORKER_RECYCLE_INTERVAL` — [`L66`](../../../../../../raw/code/codegraph/src/extraction/index.ts#L66) — Number of files to parse before recycling the worker thread.

