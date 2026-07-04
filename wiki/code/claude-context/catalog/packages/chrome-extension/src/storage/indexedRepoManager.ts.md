---
title: 'Module: packages/chrome-extension/src/storage/indexedRepoManager.ts'
type: catalog
provenance: extracted
module: packages/chrome-extension/src/storage/indexedRepoManager.ts
status: fresh
symbol_base: scip-typescript npm @zilliz/claude-context-chrome-extension 0.1.4 src/storage/`indexedRepoManager.ts`/IndexedRepo
symbols:
  IndexedRepoManager.addIndexedRepo: Manager#addIndexedRepo().
  IndexedRepoManager.getIndexedRepos: Manager#getIndexedRepos().
  IndexedRepoManager.updateLastSearchTime: Manager#updateLastSearchTime().
  IndexedRepoManager.removeIndexedRepo: Manager#removeIndexedRepo().
  IndexedRepoManager.isRepoIndexed: Manager#isRepoIndexed().
  IndexedRepoManager.getRecentlyIndexedRepos: Manager#getRecentlyIndexedRepos().
  IndexedRepoManager.cleanupOldRepos: Manager#cleanupOldRepos().
  IndexedRepoManager: Manager#
  IndexedRepository: sitory#
  IndexedRepository.id: sitory#id.
  IndexedRepoManager.STORAGE_KEY: Manager#STORAGE_KEY.
  IndexedRepository.indexedAt: sitory#indexedAt.
  IndexedRepository.owner: sitory#owner.
  IndexedRepository.repo: sitory#repo.
  IndexedRepository.totalFiles: sitory#totalFiles.
  IndexedRepository.totalChunks: sitory#totalChunks.
  IndexedRepository.lastSearchAt: sitory#lastSearchAt.
  IndexedRepository.collectionName: sitory#collectionName.
---
# Module: [`packages/chrome-extension/src/storage/indexedRepoManager.ts`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts)

## Classes
### `IndexedRepoManager`
- def: [`packages/chrome-extension/src/storage/indexedRepoManager.ts:12`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L12) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
- signature: `class IndexedRepoManager`
- members:
  - `addIndexedRepo(method)` — [`L15`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L15) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `cleanupOldRepos(method)` — [`L105`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L105) — documented in [packages-chrome-extension-src-storage-indexedRepoManager.ts](../../../../../concepts/packages-chrome-extension-src-storage-indexedRepoManager.ts.md)
  - `getIndexedRepos(method)` — [`L41`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L41) — documented in [packages-chrome-extension-src-storage-indexedRepoManager.ts](../../../../../concepts/packages-chrome-extension-src-storage-indexedRepoManager.ts.md)
  - `getRecentlyIndexedRepos(method)` — [`L98`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L98) — documented in [packages-chrome-extension-src-storage-indexedRepoManager.ts](../../../../../concepts/packages-chrome-extension-src-storage-indexedRepoManager.ts.md)
  - `isRepoIndexed(method)` — [`L53`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L53) — documented in [packages-chrome-extension-src-storage-indexedRepoManager.ts](../../../../../concepts/packages-chrome-extension-src-storage-indexedRepoManager.ts.md)
  - `removeIndexedRepo(method)` — [`L58`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L58) — documented in [packages-chrome-extension-src-storage-indexedRepoManager.ts](../../../../../concepts/packages-chrome-extension-src-storage-indexedRepoManager.ts.md)
  - `updateLastSearchTime(method)` — [`L76`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L76) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `STORAGE_KEY` — [`L13`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L13) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
- uses (calls/refs, reference-scoped): [`IndexedRepository`](indexedRepoManager.ts.md#IndexedRepository), [`id`](indexedRepoManager.ts.md#IndexedRepository.id), [`indexedAt`](indexedRepoManager.ts.md#IndexedRepository.indexedAt), [`lastSearchAt`](indexedRepoManager.ts.md#IndexedRepository.lastSearchAt)
- used by: [`handleIndexRepo`](../background.ts.md#handleIndexRepo), [`background.ts`](../background.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-background.ts), [`handleSearchCode`](../background.ts.md#handleSearchCode), [`handleCheckIndexStatus`](../background.ts.md#handleCheckIndexStatus), [`handleClearIndex`](../background.ts.md#handleClearIndex), [`handleGetIndexedRepos`](../background.ts.md#handleGetIndexedRepos)

### `IndexedRepository`
- def: [`packages/chrome-extension/src/storage/indexedRepoManager.ts:1`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L1) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
- signature: `interface IndexedRepository`
- members:
  - `collectionName` — [`L9`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L9)
  - `id` — [`L2`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L2) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `indexedAt` — [`L5`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L5) — documented in [packages-chrome-extension-src-background.ts](../../../../../concepts/packages-chrome-extension-src-background.ts.md)
  - `lastSearchAt` — [`L8`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L8) — documented in [packages-chrome-extension-src-storage-indexedRepoManager.ts](../../../../../concepts/packages-chrome-extension-src-storage-indexedRepoManager.ts.md)
  - `owner` — [`L3`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L3)
  - `repo` — [`L4`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L4)
  - `totalChunks` — [`L7`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L7)
  - `totalFiles` — [`L6`](../../../../../../../../raw/code/claude-context/packages/chrome-extension/src/storage/indexedRepoManager.ts#L6)
- used by: [`handleIndexRepo`](../background.ts.md#handleIndexRepo), [`background.ts`](../background.ts.md#scip-typescript-npm-zilliz-claude-context-chrome-extension-0.1.4-src-background.ts), [`addIndexedRepo`](indexedRepoManager.ts.md#IndexedRepoManager.addIndexedRepo), [`getIndexedRepos`](indexedRepoManager.ts.md#IndexedRepoManager.getIndexedRepos), [`updateLastSearchTime`](indexedRepoManager.ts.md#IndexedRepoManager.updateLastSearchTime), [`removeIndexedRepo`](indexedRepoManager.ts.md#IndexedRepoManager.removeIndexedRepo), [`getRecentlyIndexedRepos`](indexedRepoManager.ts.md#IndexedRepoManager.getRecentlyIndexedRepos), [`isRepoIndexed`](indexedRepoManager.ts.md#IndexedRepoManager.isRepoIndexed), [`cleanupOldRepos`](indexedRepoManager.ts.md#IndexedRepoManager.cleanupOldRepos)

