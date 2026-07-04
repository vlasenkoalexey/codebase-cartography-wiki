---
title: 'Module: src/agent/utils.ts'
type: catalog
provenance: extracted
module: src/agent/utils.ts
status: fresh
symbol_base: scip-typescript npm openwiki 0.0.1 src/agent/`utils.ts`/
symbols:
  writeLastUpdateMetadata: writeLastUpdateMetadata().
  readLastUpdate: readLastUpdate().
  createGitSummary: createGitSummary().
  createRunContext: createRunContext().
  addDirectoryToSnapshot: addDirectoryToSnapshot().
  runGit: runGit().
  createOpenWikiContentSnapshot: createOpenWikiContentSnapshot().
  formatGitSection: formatGitSection().
  getGitHead: getGitHead().
  readSnapshotFile: readSnapshotFile().
  isExpectedSnapshotRaceError: isExpectedSnapshotRaceError().
  execFileAsync: execFileAsync.
  OpenWikiContentSnapshot: OpenWikiContentSnapshot#
  isFileNotFoundError: isFileNotFoundError().
  isExecError: isExecError().
---
# Module: [`src/agent/utils.ts`](../../../../../../raw/code/openwiki/src/agent/utils.ts)

## Classes
### `OpenWikiContentSnapshot`
- def: [`src/agent/utils.ts:12`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L12)
- signature: `type OpenWikiContentSnapshot`
- used by: [`createOpenWikiContentSnapshot`](utils.ts.md#createOpenWikiContentSnapshot)

## Functions
- `addDirectoryToSnapshot(hash: any, directory: string, relativeDirectory: string)` — [`L113`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L113) — Recursively adds stable file paths and bytes to the OpenWiki content snapshot.
- `createGitSummary(command: OpenWikiCommand, cwd: string, lastUpdate: UpdateMetadata | null)` — [`L181`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L181) — Produces the git evidence block passed to init/update prompts. — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `createOpenWikiContentSnapshot(cwd: string)` — [`L63`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L63) — Hashes OpenWiki content, excluding run metadata, to detect real documentation changes. — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `createRunContext(command: OpenWikiCommand, cwd: string)` — [`L17`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L17) — Builds the per-run context the prompt uses to reason about prior docs and git changes. — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `formatGitSection(command: string, output: string)` — [`L281`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L281)
- `getGitHead(cwd: string)` — [`L248`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L248)
- `isExecError(error: unknown)` — [`L305`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L305)
- `isExpectedSnapshotRaceError(error: unknown)` — [`L295`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L295)
- `isFileNotFoundError(error: unknown)` — [`L287`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L287)
- `readLastUpdate(cwd: string)` — [`L77`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L77) — Reads prior run metadata if it exists and is structurally valid. — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)
- `readSnapshotFile(filePath: string)` — [`L166`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L166) — Reads snapshot bytes while tolerating files that move mid-scan.
- `runGit(cwd: string, args: string[])` — [`L257`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L257) — Runs git commands without failing the whole run for normal git command errors.
- `writeLastUpdateMetadata(command: OpenWikiCommand, cwd: string, modelId: string)` — [`L39`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L39) — Records a successful init/update run so future updates can diff from this git head. — documented in [openwiki-agent-index.ts](../../../concepts/openwiki-agent-index.ts.md)

## Module values
- `execFileAsync` — [`L10`](../../../../../../raw/code/openwiki/src/agent/utils.ts#L10)

