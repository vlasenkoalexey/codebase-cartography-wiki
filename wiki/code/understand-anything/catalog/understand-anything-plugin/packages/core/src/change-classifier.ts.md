---
title: 'Module: understand-anything-plugin/packages/core/src/change-classifier.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/change-classifier.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/`change-classifier.ts`/
symbols:
  classifyUpdate: classifyUpdate().
  UpdateDecision.action: UpdateDecision#action.
  UpdateDecision.rerunArchitecture: UpdateDecision#rerunArchitecture.
  summarizeChanges: summarizeChanges().
  UpdateDecision.filesToReanalyze: UpdateDecision#filesToReanalyze.
  UpdateDecision.rerunTour: UpdateDecision#rerunTour.
  UpdateDecision.reason: UpdateDecision#reason.
  detectDirectoryChanges: detectDirectoryChanges().
  topDirectory: topDirectory().
  UpdateDecision: UpdateDecision#
---
# Module: [`understand-anything-plugin/packages/core/src/change-classifier.ts`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts)

## Classes
### `UpdateDecision`
- def: [`understand-anything-plugin/packages/core/src/change-classifier.ts:4`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts#L4)
- signature: `interface UpdateDecision`
- members:
  - `action` — [`L5`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts#L5)
  - `filesToReanalyze` — [`L6`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts#L6)
  - `reason` — [`L9`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts#L9)
  - `rerunArchitecture` — [`L7`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts#L7)
  - `rerunTour` — [`L8`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts#L8)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`classifyUpdate`](change-classifier.ts.md#classifyUpdate), [`change-classifier.test.ts`](__tests__/change-classifier.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-change-classifier.test.ts)

## Functions
- `classifyUpdate(analysis: ChangeAnalysis, totalFilesInGraph: number, allKnownFiles?: string[])` — [`L21`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts#L21) — Classify the type of graph update needed based on structural change analysis.
- `detectDirectoryChanges(newFiles: string[], deletedFiles: string[], allKnownFiles: string[])` — [`L94`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts#L94) — Detect if the changes affect the directory structure (new or removed directories).
- `summarizeChanges(analysis: ChangeAnalysis)` — [`L129`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts#L129) — Produce a concise human-readable summary of structural changes.
- `topDirectory(filePath: string)` — [`L119`](../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/change-classifier.ts#L119) — Get the top-level directory of a file path (first path segment).

