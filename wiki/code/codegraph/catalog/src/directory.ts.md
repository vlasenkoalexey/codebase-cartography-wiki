---
title: 'Module: src/directory.ts'
type: catalog
provenance: extracted
module: src/directory.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/`directory.ts`/
symbols:
  isInitialized: isInitialized().
  getCodeGraphDir: getCodeGraphDir().
  planFrontload: planFrontload().
  findNearestCodeGraphRoot: findNearestCodeGraphRoot().
  validateDirectory: validateDirectory().
  findIndexedSubprojectRoots: findIndexedSubprojectRoots().
  hasStructuralKeyword: hasStructuralKeyword().
  codeGraphDirName: codeGraphDirName().
  isCodeGraphDataDir: isCodeGraphDataDir().
  FrontloadPlan.exploreRoot: FrontloadPlan#exploreRoot.
  FrontloadPlan.nudgeProjects: FrontloadPlan#nudgeProjects.
  STRUCTURAL_WORDS_RE: STRUCTURAL_WORDS_RE.
  createDirectory: createDirectory().
  FrontloadPlan.viaSubScan: FrontloadPlan#viaSubScan.
  ensureGitignore: ensureGitignore().
  STRUCTURAL_STEMS_RE: STRUCTURAL_STEMS_RE.
  extractCodeTokens: extractCodeTokens().
  DEFAULT_CODEGRAPH_DIR: DEFAULT_CODEGRAPH_DIR.
  NOT_WORD_AFTER: NOT_WORD_AFTER.
  isStructuralPrompt: isStructuralPrompt().
  validateDirectory.typeLiteral198.valid: validateDirectory().typeLiteral198:valid.
  validateDirectory.typeLiteral198.errors: validateDirectory().typeLiteral198:errors.
  removeDirectory: removeDirectory().
  CODEGRAPH_DIR: CODEGRAPH_DIR.
  looksLikeProjectRoot: looksLikeProjectRoot().
  STRUCTURAL_STEMS: STRUCTURAL_STEMS.
  isStaleDefaultGitignore: isStaleDefaultGitignore().
  unsafeIndexRootReason: unsafeIndexRootReason().
  listDirectoryContents: listDirectoryContents().
  getDirectorySize: getDirectorySize().
  ensureSubdirectory: ensureSubdirectory().
  warnedBadDirName: warnedBadDirName.
  NOT_WORD_BEFORE: NOT_WORD_BEFORE.
  FrontloadPlan: FrontloadPlan#
  SUBPROJECT_SCAN_SKIP: SUBPROJECT_SCAN_SKIP.
  WORKSPACE_ROOT_MANIFESTS: WORKSPACE_ROOT_MANIFESTS.
  escapeRegExp: escapeRegExp().
  findIndexedSubprojectRoots.opts-typeLiteral50.maxDepth: findIndexedSubprojectRoots().(opts)typeLiteral50:maxDepth.
  findIndexedSubprojectRoots.opts-typeLiteral50.max: findIndexedSubprojectRoots().(opts)typeLiteral50:max.
  STRUCTURAL_WORDS: STRUCTURAL_WORDS.
  STRUCTURAL_UNSEGMENTED: STRUCTURAL_UNSEGMENTED.
  DOC_DATA_EXT: DOC_DATA_EXT.
  GITIGNORE_CONTENT: GITIGNORE_CONTENT.
  GITIGNORE_MARKER: GITIGNORE_MARKER.
---
# Module: [`src/directory.ts`](../../../../../raw/code/codegraph/src/directory.ts)

## Classes
### `FrontloadPlan`
- def: [`src/directory.ts:515`](../../../../../raw/code/codegraph/src/directory.ts#L515) — documented in [directory.ts](../../concepts/directory.ts.md)
- doc: What the front-load hook should do for a prompt issued from a directory.
- signature: `interface FrontloadPlan`
- members:
  - `exploreRoot` — [`L519`](../../../../../raw/code/codegraph/src/directory.ts#L519) — Open + explore this project and inject its source as context. `null` when — documented in [directory.ts](../../concepts/directory.ts.md)
  - `nudgeProjects` — [`L523`](../../../../../raw/code/codegraph/src/directory.ts#L523) — Indexed sub-projects to surface in a "pass `projectPath`" nudge: the rest — documented in [directory.ts](../../concepts/directory.ts.md)
  - `viaSubScan` — [`L527`](../../../../../raw/code/codegraph/src/directory.ts#L527) — True when the plan came from scanning DOWN into sub-projects (cwd itself — documented in [directory.ts](../../concepts/directory.ts.md)
- used by: [`main`](bin/codegraph.ts.md#main), [`planFrontload`](directory.ts.md#planFrontload)

## Functions
- `codeGraphDirName()` — [`L35`](../../../../../raw/code/codegraph/src/directory.ts#L35) — Resolve the per-project data directory name, honoring the `CODEGRAPH_DIR` — documented in [directory.ts](../../concepts/directory.ts.md)
- `createDirectory(projectRoot: string)` — [`L644`](../../../../../raw/code/codegraph/src/directory.ts#L644) — Create the .codegraph directory structure — documented in [directory.ts](../../concepts/directory.ts.md)
- `ensureGitignore(gitignorePath: string)` — [`L623`](../../../../../raw/code/codegraph/src/directory.ts#L623) — Write `.codegraph/.gitignore` if it's absent, or upgrade a stale
- `ensureSubdirectory(projectRoot: string, subdirName: string)` — [`L764`](../../../../../raw/code/codegraph/src/directory.ts#L764) — Ensure a subdirectory exists within .codegraph
- `escapeRegExp(s: string)` — [`L200`](../../../../../raw/code/codegraph/src/directory.ts#L200) — documented in [directory.ts](../../concepts/directory.ts.md)
- `extractCodeTokens(prompt: string)` — [`L479`](../../../../../raw/code/codegraph/src/directory.ts#L479) — Identifier-shaped tokens in `prompt` — camelCase / PascalCase-with-inner-cap,
- `findIndexedSubprojectRoots(root: string, opts?: { maxDepth?: number | undefined; max?: number | undefined; })` — [`L212`](../../../../../raw/code/codegraph/src/directory.ts#L212) — Indexed sub-project roots beneath `root` (bounded breadth-first scan). For — documented in [directory.ts](../../concepts/directory.ts.md)
- `findNearestCodeGraphRoot(startPath: string)` — [`L158`](../../../../../raw/code/codegraph/src/directory.ts#L158) — documented in [directory.ts](../../concepts/directory.ts.md)
- `getCodeGraphDir(projectRoot: string)` — [`L85`](../../../../../raw/code/codegraph/src/directory.ts#L85) — Get the .codegraph directory path for a project — documented in [directory.ts](../../concepts/directory.ts.md)
- `getDirectorySize(projectRoot: string)` — [`L728`](../../../../../raw/code/codegraph/src/directory.ts#L728) — Get the total size of the .codegraph directory in bytes
- `hasStructuralKeyword(prompt: string)` — [`L458`](../../../../../raw/code/codegraph/src/directory.ts#L458) — Does `prompt` contain an explicit structural keyword? A keyword is a strong,
- `isCodeGraphDataDir(name: string)` — [`L74`](../../../../../raw/code/codegraph/src/directory.ts#L74) — Is `name` (a single path segment) a CodeGraph data directory? Matches the
- `isInitialized(projectRoot: string)` — [`L93`](../../../../../raw/code/codegraph/src/directory.ts#L93) — Check if a project has been initialized with CodeGraph — documented in [directory.ts](../../concepts/directory.ts.md)
- `isStaleDefaultGitignore(content: string)` — [`L613`](../../../../../raw/code/codegraph/src/directory.ts#L613) — Is `content` a stale CodeGraph-generated `.gitignore` that should be
- `isStructuralPrompt(prompt: string)` — [`L508`](../../../../../raw/code/codegraph/src/directory.ts#L508) — Cheap, graph-free candidate gate for the front-load hook: could `prompt` be a
- `listDirectoryContents(projectRoot: string)` — [`L693`](../../../../../raw/code/codegraph/src/directory.ts#L693) — Get all files in the .codegraph directory
- `looksLikeProjectRoot(dir: string)` — [`L196`](../../../../../raw/code/codegraph/src/directory.ts#L196) — documented in [directory.ts](../../concepts/directory.ts.md)
- `planFrontload(cwd: string, prompt: string)` — [`L543`](../../../../../raw/code/codegraph/src/directory.ts#L543) — Decide what the front-load hook injects for a `prompt` issued from `cwd`, — documented in [directory.ts](../../concepts/directory.ts.md)
- `removeDirectory(projectRoot: string)` — [`L665`](../../../../../raw/code/codegraph/src/directory.ts#L665) — Remove the .codegraph directory — documented in [directory.ts](../../concepts/directory.ts.md)
- `unsafeIndexRootReason(projectRoot: string)` — [`L126`](../../../../../raw/code/codegraph/src/directory.ts#L126) — Reason a directory is unsafe to use as an index ROOT, or null when it's fine.
- `validateDirectory(projectRoot: string)` — [`L781`](../../../../../raw/code/codegraph/src/directory.ts#L781) — Check if the .codegraph directory has valid structure — documented in [directory.ts](../../concepts/directory.ts.md)

## Module values
- `CODEGRAPH_DIR` — [`L65`](../../../../../raw/code/codegraph/src/directory.ts#L65) — CodeGraph directory name — a load-time snapshot of {@link codeGraphDirName}.
- `DEFAULT_CODEGRAPH_DIR` — [`L12`](../../../../../raw/code/codegraph/src/directory.ts#L12) — The default per-project data directory name. — documented in [directory.ts](../../concepts/directory.ts.md)
- `DOC_DATA_EXT` — [`L446`](../../../../../raw/code/codegraph/src/directory.ts#L446) — Doc/data/asset file extensions — a `name.ext` of this kind is a file
- `GITIGNORE_CONTENT` — [`L593`](../../../../../raw/code/codegraph/src/directory.ts#L593) — Contents of `.codegraph/.gitignore`. A single wildcard ignore keeps every
- `GITIGNORE_MARKER` — [`L601`](../../../../../raw/code/codegraph/src/directory.ts#L601) — Header line that prefixes every .gitignore CodeGraph has auto-generated.
- `NOT_WORD_AFTER` — [`L246`](../../../../../raw/code/codegraph/src/directory.ts#L246)
- `NOT_WORD_BEFORE` — [`L245`](../../../../../raw/code/codegraph/src/directory.ts#L245) — Unicode-aware word-boundary emulation for the keyword lists below. JS's `\b`
- `STRUCTURAL_STEMS` — [`L323`](../../../../../raw/code/codegraph/src/directory.ts#L323) — Structural keyword STEMS matched as word PREFIXES (boundary on the left
- `STRUCTURAL_STEMS_RE` — [`L406`](../../../../../raw/code/codegraph/src/directory.ts#L406)
- `STRUCTURAL_UNSEGMENTED` — [`L442`](../../../../../raw/code/codegraph/src/directory.ts#L442) — Structural keywords matched as bare SUBSTRINGS, for languages where a
- `STRUCTURAL_WORDS` — [`L255`](../../../../../raw/code/codegraph/src/directory.ts#L255) — Structural keywords matched as EXACT words (boundary on both sides): short
- `STRUCTURAL_WORDS_RE` — [`L405`](../../../../../raw/code/codegraph/src/directory.ts#L405)
- `SUBPROJECT_SCAN_SKIP` — [`L180`](../../../../../raw/code/codegraph/src/directory.ts#L180) — Heavy/irrelevant directory names the sub-project scan never descends into. — documented in [directory.ts](../../concepts/directory.ts.md)
- `WORKSPACE_ROOT_MANIFESTS` — [`L189`](../../../../../raw/code/codegraph/src/directory.ts#L189) — Manifests that mark a directory as a project/workspace root. The down-scan — documented in [directory.ts](../../concepts/directory.ts.md)
- `errors` — [`L783`](../../../../../raw/code/codegraph/src/directory.ts#L783)
- `max` — [`L214`](../../../../../raw/code/codegraph/src/directory.ts#L214) — documented in [directory.ts](../../concepts/directory.ts.md)
- `maxDepth` — [`L214`](../../../../../raw/code/codegraph/src/directory.ts#L214) — documented in [directory.ts](../../concepts/directory.ts.md)
- `valid` — [`L782`](../../../../../raw/code/codegraph/src/directory.ts#L782)
- `warnedBadDirName` — [`L14`](../../../../../raw/code/codegraph/src/directory.ts#L14) — documented in [directory.ts](../../concepts/directory.ts.md)

