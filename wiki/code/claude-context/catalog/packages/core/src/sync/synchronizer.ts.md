---
title: 'Module: packages/core/src/sync/synchronizer.ts'
type: catalog
provenance: extracted
module: packages/core/src/sync/synchronizer.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-core 0.1.15 src/sync/`synchronizer.ts`/FileSynchronizer#
symbols:
  FileSynchronizer.checkForChanges: checkForChanges().
  FileSynchronizer.-constructor: '`<constructor>`().'
  FileSynchronizer.loadSnapshot: loadSnapshot().
  FileSynchronizer.generateFileHashes: generateFileHashes().
  FileSynchronizer.initialize: initialize().
  FileSynchronizer.fileHashes: fileHashes.
  FileSynchronizer.saveSnapshot: saveSnapshot().
  FileSynchronizer.buildMerkleDAG: buildMerkleDAG().
  FileSynchronizer: ''
  FileSynchronizer.merkleDAG: merkleDAG.
  FileSynchronizer.compareStates: compareStates().
  FileSynchronizer.shouldIgnore: shouldIgnore().
  FileSynchronizer.snapshotPath: snapshotPath.
  FileSynchronizer.rootDir: rootDir.
  FileSynchronizer.ignoreMatcher: ignoreMatcher.
  FileSynchronizer.getFileHash: getFileHash().
  FileSynchronizer.supportedExtensions: supportedExtensions.
  FileSynchronizer.deleteSnapshot: deleteSnapshot().
  FileSynchronizer.compareStates.typeLiteral111.added: compareStates().typeLiteral111:added.
  FileSynchronizer.compareStates.typeLiteral111.removed: compareStates().typeLiteral111:removed.
  FileSynchronizer.compareStates.typeLiteral111.modified: compareStates().typeLiteral111:modified.
  FileSynchronizer.getSnapshotPath: getSnapshotPath().
  FileSynchronizer.hashFile: hashFile().
  FileSynchronizer.checkForChanges.Promise.typeLiteral98.added: checkForChanges().Promise:typeLiteral98:added.
  FileSynchronizer.checkForChanges.Promise.typeLiteral98.removed: checkForChanges().Promise:typeLiteral98:removed.
  FileSynchronizer.checkForChanges.Promise.typeLiteral98.modified: checkForChanges().Promise:typeLiteral98:modified.
---
# Module: [`packages/core/src/sync/synchronizer.ts`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts)

## Classes
### `FileSynchronizer`
- def: [`packages/core/src/sync/synchronizer.ts:8`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L8)
- signature: `class FileSynchronizer`
- members:
  - `<constructor>(rootDir: string, ignorePatterns?: string[], supportedExtensions?: string[])` — [`L16`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L16) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `buildMerkleDAG(method)` — [`L109`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L109) — documented in [packages-core-src-sync-merkle.ts](../../../../../concepts/packages-core-src-sync-merkle.ts.md)
  - `checkForChanges(method)` — [`L138`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L138) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `compareStates(method)` — [`L164`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L164) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `deleteSnapshot(method)` — [`L243`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L243) — Delete snapshot file for a given codebase path
  - `generateFileHashes(method)` — [`L45`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L45) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `getFileHash(method)` — [`L190`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L190)
  - `getSnapshotPath(method)` — [`L25`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L25) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `hashFile(method)` — [`L35`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L35) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `initialize(method)` — [`L131`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L131) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `loadSnapshot(method)` — [`L213`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L213) — documented in [packages-core-src-context.ts](../../../../../concepts/packages-core-src-context.ts.md)
  - `saveSnapshot(method)` — [`L194`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L194) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `shouldIgnore(method)` — [`L105`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L105) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `added` — [`L138`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L138)
  - `added` — [`L164`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L164)
  - `fileHashes` — [`L9`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L9) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `ignoreMatcher` — [`L14`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L14)
  - `merkleDAG` — [`L10`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L10) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `modified` — [`L138`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L138)
  - `modified` — [`L164`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L164)
  - `removed` — [`L138`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L138)
  - `removed` — [`L164`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L164)
  - `rootDir` — [`L11`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L11) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `snapshotPath` — [`L12`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L12) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
  - `supportedExtensions` — [`L13`](../../../../../../../../raw/code/claude-context/packages/core/src/sync/synchronizer.ts#L13) — documented in [packages-core-src-sync-synchronizer.ts](../../../../../concepts/packages-core-src-sync-synchronizer.ts.md)
- uses (calls/refs, reference-scoped): [`addNode`](merkle.ts.md#MerkleDAG.addNode), [`compare`](merkle.ts.md#MerkleDAG.compare), [`deserialize`](merkle.ts.md#MerkleDAG.deserialize), [`ignores`](../utils/ignore-matcher.ts.md#IgnoreMatcher.ignores), [`MerkleDAG`](merkle.ts.md#MerkleDAG), [`<constructor>`](merkle.ts.md#MerkleDAG.-constructor), [`serialize`](merkle.ts.md#MerkleDAG.serialize), [`<constructor>`](../utils/ignore-matcher.ts.md#IgnoreMatcher.-constructor), [`IgnoreMatcher`](../utils/ignore-matcher.ts.md#IgnoreMatcher), [`added`](merkle.ts.md#MerkleDAG.compare.typeLiteral23.added), [`removed`](merkle.ts.md#MerkleDAG.compare.typeLiteral23.removed)
- used by: [`context.splitter.test.ts`](../context.splitter.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.splitter.test.ts), [`context.ignore-patterns.test.ts`](../context.ignore-patterns.test.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ignore-patterns.test.ts), [`context.ts`](../context.ts.md#scip-typescript-npm-zilliz-claude-context-core-0.1.15-src-context.ts), [`modified`](../context.ts.md#Context.reindexByChange.Promise.typeLiteral121.modified), [`execute`](../../../vscode-extension/src/commands/indexCommand.ts.md#IndexCommand.execute), [`clearIndex`](../context.ts.md#Context.clearIndex), [`synchronizers`](../context.ts.md#Context.synchronizers), [`setSynchronizer`](../context.ts.md#Context.setSynchronizer), [`getSynchronizers`](../context.ts.md#Context.getSynchronizers)

