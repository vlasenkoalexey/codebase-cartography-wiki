---
title: 'Module: understand-anything-plugin/packages/core/src/staleness.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/staleness.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/`staleness.ts`/
symbols:
  mergeGraphUpdate: mergeGraphUpdate().
  isStale: isStale().
  getChangedFiles: getChangedFiles().
  StalenessResult: StalenessResult#
  StalenessResult.stale: StalenessResult#stale.
  StalenessResult.changedFiles: StalenessResult#changedFiles.
---
# Module: [`understand-anything-plugin/packages/core/src/staleness.ts`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/staleness.ts)

## Classes
### `StalenessResult`
- def: [`understand-anything-plugin/packages/core/src/staleness.ts:4`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/staleness.ts#L4)
- signature: `interface StalenessResult`
- members:
  - `changedFiles` — [`L6`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/staleness.ts#L6)
  - `stale` — [`L5`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/staleness.ts#L5)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`isStale`](staleness.ts.md#isStale)

## Functions
- `getChangedFiles(projectDir: string, lastCommitHash: string)` — [`L13`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/staleness.ts#L13) — Get the list of files that changed between a given commit and HEAD.
- `isStale(projectDir: string, lastCommitHash: string)` — [`L34`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/staleness.ts#L34) — Check whether the knowledge graph is stale relative to the current HEAD.
- `mergeGraphUpdate(existingGraph: KnowledgeGraph, changedFilePaths: string[], newNodes: GraphNode[], newEdges: GraphEdge[], newCommitHash: string)` — [`L54`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/staleness.ts#L54) — Merge new analysis results into an existing knowledge graph.

