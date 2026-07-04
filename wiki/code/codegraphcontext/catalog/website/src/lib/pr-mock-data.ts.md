---
title: 'Module: website/src/lib/pr-mock-data.ts'
type: catalog
provenance: extracted
module: website/src/lib/pr-mock-data.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/lib/`pr-mock-data.ts`/
symbols:
  PRLink.source: PRLink#source.
  PRLink.target: PRLink#target.
  PRNode.name: PRNode#name.
  PRNode.id: PRNode#id.
  PRNode.type: PRNode#type.
  PRNode.prZone: PRNode#prZone.
  PRNode.status: PRNode#status.
  PRNode.gitDiff: PRNode#gitDiff.
  PRNode.file: PRNode#file.
  PRNode.layer: PRNode#layer.
  PRNode.val: PRNode#val.
  PRLink.type: PRLink#type.
  PRNode: PRNode#
  PRLink.id: PRLink#id.
  PRLink: PRLink#
  PRGraphData: PRGraphData#
  PRGraphData.nodes: PRGraphData#nodes.
  PRGraphData.links: PRGraphData#links.
  PRGraphData.files: PRGraphData#files.
  PRLink.isViolation: PRLink#isViolation.
  PRNode.complexityDelta: PRNode#complexityDelta.
  PRNode.isOrphan: PRNode#isOrphan.
  prMockData: prMockData.
  PRNode.fileChurn: PRNode#fileChurn.
  PRNode.signatureChanged: PRNode#signatureChanged.
  PRLink.violationMessage: PRLink#violationMessage.
  PRGraphData.fileContents: PRGraphData#fileContents.
  PRGraphData.metadata: PRGraphData#metadata.
  PRGraphData.metadata.typeLiteral0.prTitle: PRGraphData#metadata.typeLiteral0:prTitle.
  PRGraphData.metadata.typeLiteral0.prNumber: PRGraphData#metadata.typeLiteral0:prNumber.
  PRGraphData.metadata.typeLiteral0.author: PRGraphData#metadata.typeLiteral0:author.
  PRGraphData.metadata.typeLiteral0.sourceBranch: PRGraphData#metadata.typeLiteral0:sourceBranch.
  PRGraphData.metadata.typeLiteral0.targetBranch: PRGraphData#metadata.typeLiteral0:targetBranch.
  PRGraphData.metadata.typeLiteral0.repo: PRGraphData#metadata.typeLiteral0:repo.
  PRGraphData.metadata.typeLiteral0.commit: PRGraphData#metadata.typeLiteral0:commit.
  PRGraphData.metadata.typeLiteral0.timestamp: PRGraphData#metadata.typeLiteral0:timestamp.
  PRGraphData.metadata.typeLiteral0.directChanges: PRGraphData#metadata.typeLiteral0:directChanges.
  PRGraphData.metadata.typeLiteral0.impactedCount: PRGraphData#metadata.typeLiteral0:impactedCount.
  PRGraphData.metadata.typeLiteral0.violationsCount: PRGraphData#metadata.typeLiteral0:violationsCount.
  PRGraphData.metadata.typeLiteral0.orphansCount: PRGraphData#metadata.typeLiteral0:orphansCount.
  PRNode.prevSignature: PRNode#prevSignature.
  PRNode.newSignature: PRNode#newSignature.
  PRNode.affectedCallers: PRNode#affectedCallers.
  PRNode.line_number: PRNode#line_number.
---
# Module: [`website/src/lib/pr-mock-data.ts`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts)

## Classes
### `PRGraphData`
- def: [`website/src/lib/pr-mock-data.ts:30`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L30) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- signature: `interface PRGraphData`
- members:
  - `author` — [`L38`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L38)
  - `commit` — [`L42`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L42)
  - `directChanges` — [`L44`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L44)
  - `fileContents` — [`L34`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L34)
  - `files` — [`L33`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L33)
  - `impactedCount` — [`L45`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L45)
  - `links` — [`L32`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L32) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `metadata` — [`L35`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L35)
  - `nodes` — [`L31`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L31)
  - `orphansCount` — [`L47`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L47)
  - `prNumber` — [`L37`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L37)
  - `prTitle` — [`L36`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L36)
  - `repo` — [`L41`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L41)
  - `sourceBranch` — [`L39`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L39)
  - `targetBranch` — [`L40`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L40)
  - `timestamp` — [`L43`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L43)
  - `violationsCount` — [`L46`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L46)
- uses (calls/refs, reference-scoped): [`PRNode`](pr-mock-data.ts.md#PRNode), [`PRLink`](pr-mock-data.ts.md#PRLink)
- used by: [`computePRInsights`](pr-insights.ts.md#computePRInsights), [`pr-mock-data.ts`](pr-mock-data.ts.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-lib-pr-mock-data.ts), [`PRReviewerPage`](../pages/PRReviewerPage.tsx.md#PRReviewerPage), [`PRReviewerPage.tsx`](../pages/PRReviewerPage.tsx.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-pages-PRReviewerPage.tsx), [`pr-insights.ts`](pr-insights.ts.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-lib-pr-insights.ts)

### `PRLink`
- def: [`website/src/lib/pr-mock-data.ts:21`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L21)
- signature: `interface PRLink`
- members:
  - `id` — [`L22`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L22)
  - `isViolation` — [`L26`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L26)
  - `source` — [`L23`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L23) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `target` — [`L24`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L24) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `type` — [`L25`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L25) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `violationMessage` — [`L27`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L27)
- used by: [`computePRInsights`](pr-insights.ts.md#computePRInsights), [`pr-mock-data.ts`](pr-mock-data.ts.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-lib-pr-mock-data.ts), [`PRReviewerPage`](../pages/PRReviewerPage.tsx.md#PRReviewerPage), [`PRReviewerPage.tsx`](../pages/PRReviewerPage.tsx.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-pages-PRReviewerPage.tsx), [`isMeaningfulOrphan`](pr-insights.ts.md#isMeaningfulOrphan), [`pr-insights.ts`](pr-insights.ts.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-lib-pr-insights.ts), [`links`](pr-mock-data.ts.md#PRGraphData.links)

### `PRNode`
- def: [`website/src/lib/pr-mock-data.ts:1`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L1) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- signature: `interface PRNode`
- members:
  - `affectedCallers` — [`L15`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L15)
  - `complexityDelta` — [`L8`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L8)
  - `file` — [`L5`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L5) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `fileChurn` — [`L9`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L9)
  - `gitDiff` — [`L16`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L16) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `id` — [`L2`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L2) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `isOrphan` — [`L11`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L11)
  - `layer` — [`L10`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L10)
  - `line_number` — [`L17`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L17)
  - `name` — [`L3`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L3) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `newSignature` — [`L14`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L14)
  - `prZone` — [`L6`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L6) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `prevSignature` — [`L13`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L13)
  - `signatureChanged` — [`L12`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L12)
  - `status` — [`L7`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L7) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `type` — [`L4`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L4) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
  - `val` — [`L18`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L18)
- used by: [`computePRInsights`](pr-insights.ts.md#computePRInsights), [`pr-mock-data.ts`](pr-mock-data.ts.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-lib-pr-mock-data.ts), [`PRReviewerPage`](../pages/PRReviewerPage.tsx.md#PRReviewerPage), [`PRReviewerPage.tsx`](../pages/PRReviewerPage.tsx.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-pages-PRReviewerPage.tsx), [`isMeaningfulOrphan`](pr-insights.ts.md#isMeaningfulOrphan), [`isLikelyNoiseNode`](pr-insights.ts.md#isLikelyNoiseNode), [`pr-insights.ts`](pr-insights.ts.md#scip-typescript-npm-vite_react_shadcn_ts-0.0.0-src-lib-pr-insights.ts), [`nodes`](pr-mock-data.ts.md#PRGraphData.nodes)

## Module values
- `prMockData` — [`L51`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-mock-data.ts#L51)

