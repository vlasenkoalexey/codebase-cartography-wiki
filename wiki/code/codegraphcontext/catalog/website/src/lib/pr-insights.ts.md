---
title: 'Module: website/src/lib/pr-insights.ts'
type: catalog
provenance: extracted
module: website/src/lib/pr-insights.ts
status: fresh
symbol_base: scip-typescript npm vite_react_shadcn_ts 0.0.0 src/lib/`pr-insights.ts`/
symbols:
  computePRInsights: computePRInsights().
  isMeaningfulOrphan: isMeaningfulOrphan().
  isLikelyNoiseNode: isLikelyNoiseNode().
  PRInsights.riskLevel: PRInsights#riskLevel.
  PRInsights.keySymbols: PRInsights#keySymbols.
  PRInsights.meaningfulCallPaths: PRInsights#meaningfulCallPaths.
  getNodeLabel: getNodeLabel().
  PRRiskLevel: PRRiskLevel#
  PRKeySymbol: PRKeySymbol#
  PRKeySymbol.id: PRKeySymbol#id.
  PRKeySymbol.name: PRKeySymbol#name.
  PRKeySymbol.file: PRKeySymbol#file.
  PRKeySymbol.reason: PRKeySymbol#reason.
  PRCallPath: PRCallPath#
  diffAddsOrRemovesSymbol: diffAddsOrRemovesSymbol().
  PRInsights: PRInsights#
  PRInsights.riskScore: PRInsights#riskScore.
  PRInsights.summary: PRInsights#summary.
  PRInsights.reviewVerdict: PRInsights#reviewVerdict.
  PRInsights.signalNodeCount: PRInsights#signalNodeCount.
  PRInsights.noiseNodeCount: PRInsights#noiseNodeCount.
  PRInsights.noiseRatio: PRInsights#noiseRatio.
  PRInsights.meaningfulOrphanCount: PRInsights#meaningfulOrphanCount.
  PRInsights.falsePositiveOrphanCount: PRInsights#falsePositiveOrphanCount.
  PRInsights.recommendations: PRInsights#recommendations.
  PRInsights.changedFileCount: PRInsights#changedFileCount.
  PRInsights.primaryImpactCount: PRInsights#primaryImpactCount.
  nodeName: nodeName().
  hasAnchorBodyEdit: hasAnchorBodyEdit().
  PRCallPath.source: PRCallPath#source.
  PRCallPath.target: PRCallPath#target.
  PRCallPath.sourceName: PRCallPath#sourceName.
  PRCallPath.targetName: PRCallPath#targetName.
  PRCallPath.type: PRCallPath#type.
  PRCallPath.label: PRCallPath#label.
---
# Module: [`website/src/lib/pr-insights.ts`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts)

## Classes
### `PRCallPath`
- def: [`website/src/lib/pr-insights.ts:12`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L12)
- signature: `interface PRCallPath`
- members:
  - `label` — [`L18`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L18)
  - `source` — [`L13`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L13)
  - `sourceName` — [`L15`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L15)
  - `target` — [`L14`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L14)
  - `targetName` — [`L16`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L16)
  - `type` — [`L17`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L17)
- used by: [`computePRInsights`](pr-insights.ts.md#computePRInsights), [`meaningfulCallPaths`](pr-insights.ts.md#PRInsights.meaningfulCallPaths)

### `PRInsights`
- def: [`website/src/lib/pr-insights.ts:21`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L21)
- signature: `interface PRInsights`
- members:
  - `changedFileCount` — [`L34`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L34)
  - `falsePositiveOrphanCount` — [`L32`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L32)
  - `keySymbols` — [`L26`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L26)
  - `meaningfulCallPaths` — [`L27`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L27)
  - `meaningfulOrphanCount` — [`L31`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L31)
  - `noiseNodeCount` — [`L29`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L29)
  - `noiseRatio` — [`L30`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L30)
  - `primaryImpactCount` — [`L35`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L35)
  - `recommendations` — [`L33`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L33)
  - `reviewVerdict` — [`L25`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L25)
  - `riskLevel` — [`L22`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L22)
  - `riskScore` — [`L23`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L23)
  - `signalNodeCount` — [`L28`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L28)
  - `summary` — [`L24`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L24)
- uses (calls/refs, reference-scoped): [`PRCallPath`](pr-insights.ts.md#PRCallPath), [`PRKeySymbol`](pr-insights.ts.md#PRKeySymbol), [`PRRiskLevel`](pr-insights.ts.md#PRRiskLevel)
- used by: [`computePRInsights`](pr-insights.ts.md#computePRInsights)

### `PRKeySymbol`
- def: [`website/src/lib/pr-insights.ts:5`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L5)
- signature: `interface PRKeySymbol`
- members:
  - `file` — [`L8`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L8)
  - `id` — [`L6`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L6)
  - `name` — [`L7`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L7)
  - `reason` — [`L9`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L9)
- used by: [`computePRInsights`](pr-insights.ts.md#computePRInsights), [`keySymbols`](pr-insights.ts.md#PRInsights.keySymbols)

### `PRRiskLevel`
- def: [`website/src/lib/pr-insights.ts:3`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L3)
- signature: `type PRRiskLevel`
- used by: [`computePRInsights`](pr-insights.ts.md#computePRInsights), [`riskLevel`](pr-insights.ts.md#PRInsights.riskLevel)

## Functions
- `computePRInsights(data: PRGraphData)` — [`L97`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L97) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `diffAddsOrRemovesSymbol(diff: string, name: string, kind: "class" | "def")` — [`L42`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L42)
- `getNodeLabel(id: string)` — [`L265`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L265)
- `hasAnchorBodyEdit(diff: string)` — [`L47`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L47)
- `isLikelyNoiseNode(node: PRNode, directNodes: PRNode[])` — [`L56`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L56) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `isMeaningfulOrphan(node: PRNode, links: PRLink[])` — [`L85`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L85) — documented in [website-src-components-PRReviewer.tsx](../../../../concepts/website-src-components-PRReviewer.tsx.md)
- `nodeName(id: string)` — [`L38`](../../../../../../../raw/code/codegraphcontext/website/src/lib/pr-insights.ts#L38)

