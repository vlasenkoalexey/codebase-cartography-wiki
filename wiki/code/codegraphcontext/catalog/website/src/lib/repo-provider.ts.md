---
title: 'Module: website/src/lib/repo-provider.ts'
type: catalog
provenance: extracted
module: website/src/lib/repo-provider.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/lib/`repo-provider.ts`/
symbols:
  repoRefFromRoute: repoRefFromRoute().
  RepoRef.provider: RepoRef#provider.
  parseRepoInput: parseRepoInput().
  listRepositoryFiles.Promise.typeLiteral100.commitSha: listRepositoryFiles().Promise:typeLiteral100:commitSha.
  RepoRef: RepoRef#
  RepoRef.fullPath: RepoRef#fullPath.
  RepoRef.repo: RepoRef#repo.
  RepoRef.owner: RepoRef#owner.
  getAuthenticatedZipUrl: getAuthenticatedZipUrl().
  getZipProxyUrl: getZipProxyUrl().
  getPublicZipUrl: getPublicZipUrl().
  getRawFileUrl: getRawFileUrl().
  flattenJsdelivrTree: flattenJsdelivrTree().
  getJsdelivrTotalSize: getJsdelivrTotalSize().
  estimateZipSize: estimateZipSize().
  resolveRepoMetadata.Promise.typeLiteral60.latestCommitSha: resolveRepoMetadata().Promise:typeLiteral60:latestCommitSha.
  getExploreRoute: getExploreRoute().
  getAuthHeaders: getAuthHeaders().
  getAuthTokenKey: getAuthTokenKey().
  getJsdelivrMetaUrl: getJsdelivrMetaUrl().
  getCdnFileUrl: getCdnFileUrl().
  getCacheKey: getCacheKey().
  getLegacyCacheKey: getLegacyCacheKey().
  getBranchesToTry: getBranchesToTry().
  JsdelivrFile.files: JsdelivrFile#files.
  RepoRef.host: RepoRef#host.
  resolveRepoMetadata: resolveRepoMetadata().
  listRepositoryFiles: listRepositoryFiles().
  JsdelivrFile.type: JsdelivrFile#type.
  RepoProvider: RepoProvider#
  GITHUB_HOST: GITHUB_HOST.
  cleanRepoPathSegment: cleanRepoPathSegment().
  listRepositoryFiles.Promise.typeLiteral100.branch: listRepositoryFiles().Promise:typeLiteral100:branch.
  JsdelivrFile: JsdelivrFile#
  detectProviderFromInput: detectProviderFromInput().
  GITLAB_HOST: GITLAB_HOST.
  listRepositoryFiles.Promise.typeLiteral100.files: listRepositoryFiles().Promise:typeLiteral100:files.
  JsdelivrFile.name: JsdelivrFile#name.
  JsdelivrFile.size: JsdelivrFile#size.
  DEFAULT_BRANCHES: DEFAULT_BRANCHES.
  resolveRepoMetadata.Promise.typeLiteral60.detectedBranch: resolveRepoMetadata().Promise:typeLiteral60:detectedBranch.
  estimateZipSize.Promise.typeLiteral206.estimatedZipSize: estimateZipSize().Promise:typeLiteral206:estimatedZipSize.
  estimateZipSize.Promise.typeLiteral206.isEstimateReliable: estimateZipSize().Promise:typeLiteral206:isEstimateReliable.
---
# Module: [`website/src/lib/repo-provider.ts`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts)

## Classes
### `JsdelivrFile`
- def: [`website/src/lib/repo-provider.ts:345`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L345) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- signature: `interface JsdelivrFile`
- members:
  - `files` — [`L349`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L349) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
  - `name` — [`L346`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L346) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
  - `size` — [`L348`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L348)
  - `type` — [`L347`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L347) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- used by: [`flattenJsdelivrTree`](repo-provider.ts.md#flattenJsdelivrTree), [`getJsdelivrTotalSize`](repo-provider.ts.md#getJsdelivrTotalSize)

### `RepoProvider`
- def: [`website/src/lib/repo-provider.ts:1`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L1) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- signature: `type RepoProvider`
- used by: [`repoRefFromRoute`](repo-provider.ts.md#repoRefFromRoute), [`provider`](repo-provider.ts.md#RepoRef.provider), [`detectProviderFromInput`](repo-provider.ts.md#detectProviderFromInput)

### `RepoRef`
- def: [`website/src/lib/repo-provider.ts:3`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L3) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- signature: `interface RepoRef`
- members:
  - `fullPath` — [`L10`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L10) — Full project path, e.g. `gitlab-org/gitlab` or `facebook/react`. — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
  - `host` — [`L11`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L11) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
  - `owner` — [`L6`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L6) — Namespace / owner segment (may contain slashes for nested GitLab groups). — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
  - `provider` — [`L4`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L4) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
  - `repo` — [`L8`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L8) — Project / repository name. — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- uses (calls/refs, reference-scoped): [`RepoProvider`](repo-provider.ts.md#RepoProvider)
- used by: [`Explore`](../pages/Explore.tsx.md#Explore), [`fetchRepositoryFiles`](repo-fetcher.ts.md#fetchRepositoryFiles), [`Explore.tsx`](../pages/Explore.tsx.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-pages-Explore.tsx), [`repo-fetcher.ts`](repo-fetcher.ts.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-lib-repo-fetcher.ts), [`repoRefFromRoute`](repo-provider.ts.md#repoRefFromRoute), [`parseRepoInput`](repo-provider.ts.md#parseRepoInput), [`commitSha`](repo-provider.ts.md#listRepositoryFiles.Promise.typeLiteral100.commitSha), [`getAuthenticatedZipUrl`](repo-provider.ts.md#getAuthenticatedZipUrl), [`estimateZipSize`](repo-provider.ts.md#estimateZipSize), [`getPublicZipUrl`](repo-provider.ts.md#getPublicZipUrl), [`getRawFileUrl`](repo-provider.ts.md#getRawFileUrl), [`getZipProxyUrl`](repo-provider.ts.md#getZipProxyUrl), [`getCachedGraph`](../pages/Explore.tsx.md#getCachedGraph), [`latestCommitSha`](repo-provider.ts.md#resolveRepoMetadata.Promise.typeLiteral60.latestCommitSha), [`getAuthHeaders`](repo-provider.ts.md#getAuthHeaders), [`getExploreRoute`](repo-provider.ts.md#getExploreRoute), [`cacheGraph`](../pages/Explore.tsx.md#cacheGraph), [`getAuthTokenKey`](repo-provider.ts.md#getAuthTokenKey), [`getCdnFileUrl`](repo-provider.ts.md#getCdnFileUrl), [`getJsdelivrMetaUrl`](repo-provider.ts.md#getJsdelivrMetaUrl), [`getCacheKey`](repo-provider.ts.md#getCacheKey), [`getLegacyCacheKey`](repo-provider.ts.md#getLegacyCacheKey), [`listRepositoryFiles`](repo-provider.ts.md#listRepositoryFiles), [`resolveRepoMetadata`](repo-provider.ts.md#resolveRepoMetadata)

## Functions
- `cleanRepoPathSegment(path: string)` — [`L20`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L20) — Strip trailing .git, /-/* UI paths, and query/hash from a repo path segment. — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `detectProviderFromInput(input: string)` — [`L116`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L116) — Guess provider from partial user input (URL or shorthand). Defaults to GitHub.
- `estimateZipSize(ref: RepoRef, branchesToTry: string[])` — [`L377`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L377) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `flattenJsdelivrTree(items: JsdelivrFile[], currentPath?: string)` — [`L352`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L352) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `getAuthHeaders(ref: RepoRef)` — [`L143`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L143) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `getAuthTokenKey(ref: RepoRef)` — [`L139`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L139) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `getAuthenticatedZipUrl(ref: RepoRef, branch: string)` — [`L225`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L225) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `getBranchesToTry(detectedBranch: string)` — [`L152`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L152)
- `getCacheKey(ref: RepoRef)` — [`L131`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L131)
- `getCdnFileUrl(ref: RepoRef, branch: string, filePath: string)` — [`L248`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L248) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `getExploreRoute(ref: RepoRef)` — [`L124`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L124)
- `getJsdelivrMetaUrl(ref: RepoRef, branch: string)` — [`L236`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L236) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `getJsdelivrTotalSize(items: JsdelivrFile[])` — [`L365`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L365)
- `getLegacyCacheKey(ref: RepoRef)` — [`L135`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L135)
- `getPublicZipUrl(ref: RepoRef, branch: string)` — [`L218`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L218) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `getRawFileUrl(ref: RepoRef, branch: string, filePath: string)` — [`L241`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L241) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `getZipProxyUrl(ref: RepoRef, branch: string)` — [`L211`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L211) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `listRepositoryFiles(ref: RepoRef, branchesToTry: string[])` — [`L256`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L256) — List all file paths in a repository (fallback when ZIP download fails).
- `parseRepoInput(input: string)` — [`L30`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L30) — Parse a user-supplied URL or `owner/repo` shorthand into a RepoRef. — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `repoRefFromRoute(provider: RepoProvider, owner: string, repo: string, gitlabSplat?: string)` — [`L83`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L83) — Build a RepoRef from route parameters. — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `resolveRepoMetadata(ref: RepoRef)` — [`L157`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L157) — Resolve default branch and latest commit SHA for a repository.

## Module values
- `DEFAULT_BRANCHES` — [`L17`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L17)
- `GITHUB_HOST` — [`L14`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L14) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `GITLAB_HOST` — [`L15`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L15) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `branch` — [`L259`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L259)
- `commitSha` — [`L259`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L259) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)
- `detectedBranch` — [`L159`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L159)
- `estimatedZipSize` — [`L380`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L380)
- `files` — [`L259`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L259)
- `isEstimateReliable` — [`L380`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L380)
- `latestCommitSha` — [`L159`](../../../../../../../raw/code/codegraphcontext/website/src/lib/repo-provider.ts#L159) — documented in [website-src-lib-repo-provider.ts](../../../../concepts/website-src-lib-repo-provider.ts.md)

