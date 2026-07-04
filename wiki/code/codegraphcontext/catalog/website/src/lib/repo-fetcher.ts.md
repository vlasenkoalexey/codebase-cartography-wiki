---
title: 'Module: website/src/lib/repo-fetcher.ts'
type: catalog
provenance: extracted
module: website/src/lib/repo-fetcher.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/lib/`repo-fetcher.ts`/
symbols:
  fetchRepositoryFiles: fetchRepositoryFiles().
  SOURCE_FILE_PATTERN: SOURCE_FILE_PATTERN.
  RepoFetchCallbacks.onProgressText: RepoFetchCallbacks#onProgressText.
  RepoFetchCallbacks.onProgressValue: RepoFetchCallbacks#onProgressValue.
  RepoFetchCallbacks.isPathIgnored: RepoFetchCallbacks#isPathIgnored.
  RepoFetchCallbacks.fetchWithProgress: RepoFetchCallbacks#fetchWithProgress.
  RepoFetchCallbacks.fetchWithFallbackProxies: RepoFetchCallbacks#fetchWithFallbackProxies.
  isZipResponse: isZipResponse.
  FetchedRepoFiles: FetchedRepoFiles#
  FetchedRepoFiles.files: FetchedRepoFiles#files.
  FetchedRepoFiles.fileContents: FetchedRepoFiles#fileContents.
  FetchedRepoFiles.latestCommitSha: FetchedRepoFiles#latestCommitSha.
  RepoFetchCallbacks: RepoFetchCallbacks#
  FetchedRepoFiles.detectedBranch: FetchedRepoFiles#detectedBranch.
---
# Module: [`website/src/lib/repo-fetcher.ts`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts)

## Classes
### `FetchedRepoFiles`
- def: [`website/src/lib/repo-fetcher.ts:19`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L19)
- signature: `interface FetchedRepoFiles`
- members:
  - `detectedBranch` — [`L23`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L23)
  - `fileContents` — [`L21`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L21)
  - `files` — [`L20`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L20)
  - `latestCommitSha` — [`L22`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L22)
- used by: [`Explore`](../pages/Explore.tsx.md#Explore), [`fetchRepositoryFiles`](repo-fetcher.ts.md#fetchRepositoryFiles)

### `RepoFetchCallbacks`
- def: [`website/src/lib/repo-fetcher.ts:26`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L26)
- signature: `interface RepoFetchCallbacks`
- members:
  - `fetchWithFallbackProxies` — [`L31`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L31)
  - `fetchWithProgress` — [`L30`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L30)
  - `isPathIgnored` — [`L29`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L29)
  - `onProgressText` — [`L27`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L27)
  - `onProgressValue` — [`L28`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L28)
- used by: [`Explore`](../pages/Explore.tsx.md#Explore), [`fetchRepositoryFiles`](repo-fetcher.ts.md#fetchRepositoryFiles)

## Functions
- `fetchRepositoryFiles(ref: RepoRef, callbacks: RepoFetchCallbacks)` — [`L42`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L42) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)

## Module values
- `SOURCE_FILE_PATTERN` — [`L17`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L17)
- `isZipResponse` — [`L37`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-fetcher.ts#L37)

