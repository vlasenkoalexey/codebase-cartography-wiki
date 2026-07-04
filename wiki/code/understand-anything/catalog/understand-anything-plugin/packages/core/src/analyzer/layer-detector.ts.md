---
title: 'Module: understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/analyzer/`layer-detector.ts`/
symbols:
  detectLayers: detectLayers().
  applyLLMLayers: applyLLMLayers().
  LAYER_PATTERNS.Array.typeLiteral0.description: LAYER_PATTERNS.Array:typeLiteral0:description.
  parseLayerDetectionResponse: parseLayerDetectionResponse().
  buildLayerDetectionPrompt: buildLayerDetectionPrompt().
  LAYER_PATTERNS.Array.typeLiteral0.layerName: LAYER_PATTERNS.Array:typeLiteral0:layerName.
  LAYER_PATTERNS.Array.typeLiteral0.patterns: LAYER_PATTERNS.Array:typeLiteral0:patterns.
  matchFileToLayer: matchFileToLayer().
  LLMLayerResponse.name: LLMLayerResponse#name.
  LLMLayerResponse: LLMLayerResponse#
  LLMLayerResponse.filePatterns: LLMLayerResponse#filePatterns.
  LLMLayerResponse.description: LLMLayerResponse#description.
  LAYER_PATTERNS: LAYER_PATTERNS.
  toLayerId: toLayerId().
---
# Module: [`understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts)

## Classes
### `LLMLayerResponse`
- def: [`understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts:6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L6)
- doc: LLM layer response structure — what the LLM returns for each layer.
- signature: `interface LLMLayerResponse`
- members:
  - `description` — [`L8`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L8)
  - `filePatterns` — [`L9`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L9)
  - `name` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L7)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`layer-detector.test.ts`](../__tests__/layer-detector.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-layer-detector.test.ts), [`applyLLMLayers`](layer-detector.ts.md#applyLLMLayers), [`parseLayerDetectionResponse`](layer-detector.ts.md#parseLayerDetectionResponse)

## Functions
- `applyLLMLayers(graph: KnowledgeGraph, llmLayers: LLMLayerResponse[])` — [`L227`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L227) — Applies LLM-provided layer definitions to a knowledge graph.
- `buildLayerDetectionPrompt(graph: KnowledgeGraph)` — [`L150`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L150) — Builds an LLM prompt that asks the model to identify logical layers
- `detectLayers(graph: KnowledgeGraph)` — [`L105`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L105) — Heuristic layer detection — assigns file nodes to layers based on
- `matchFileToLayer(filePath: string)` — [`L80`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L80) — Determine which layer a file path belongs to based on directory patterns.
- `parseLayerDetectionResponse(response: string)` — [`L177`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L177) — Parses an LLM response for layer detection.
- `toLayerId(name: string)` — [`L72`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L72) — Convert a layer name to a kebab-case layer ID.

## Module values
- `LAYER_PATTERNS` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L16) — Directory-pattern to layer-name mapping for heuristic detection.
- `description` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L16)
- `layerName` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L16)
- `patterns` — [`L16`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/layer-detector.ts#L16)

