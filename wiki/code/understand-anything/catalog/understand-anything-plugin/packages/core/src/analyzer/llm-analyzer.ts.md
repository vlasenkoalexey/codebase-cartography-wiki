---
title: 'Module: understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/analyzer/`llm-analyzer.ts`/
symbols:
  parseFileAnalysisResponse: parseFileAnalysisResponse().
  parseProjectSummaryResponse: parseProjectSummaryResponse().
  buildProjectSummaryPrompt: buildProjectSummaryPrompt().
  LLMFileAnalysis.complexity: LLMFileAnalysis#complexity.
  LLMFileAnalysis.fileSummary: LLMFileAnalysis#fileSummary.
  buildFileAnalysisPrompt: buildFileAnalysisPrompt().
  LLMFileAnalysis.tags: LLMFileAnalysis#tags.
  LLMFileAnalysis.functionSummaries: LLMFileAnalysis#functionSummaries.
  LLMFileAnalysis.classSummaries: LLMFileAnalysis#classSummaries.
  LLMProjectSummary.description: LLMProjectSummary#description.
  LLMProjectSummary.frameworks: LLMProjectSummary#frameworks.
  LLMProjectSummary.layers: LLMProjectSummary#layers.
  LLMFileAnalysis: LLMFileAnalysis#
  LLMFileAnalysis.languageNotes: LLMFileAnalysis#languageNotes.
  LLMProjectSummary: LLMProjectSummary#
  buildProjectSummaryPrompt.sampleFiles-Array.typeLiteral1.path: buildProjectSummaryPrompt().(sampleFiles)Array:typeLiteral1:path.
  buildProjectSummaryPrompt.sampleFiles-Array.typeLiteral1.content: buildProjectSummaryPrompt().(sampleFiles)Array:typeLiteral1:content.
  extractJson: extractJson().
  VALID_COMPLEXITIES: VALID_COMPLEXITIES.
  LLMProjectSummary.layers.Array.typeLiteral0.name: LLMProjectSummary#layers.Array:typeLiteral0:name.
  LLMProjectSummary.layers.Array.typeLiteral0.description: LLMProjectSummary#layers.Array:typeLiteral0:description.
  LLMProjectSummary.layers.Array.typeLiteral0.filePatterns: LLMProjectSummary#layers.Array:typeLiteral0:filePatterns.
---
# Module: [`understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts)

## Classes
### `LLMFileAnalysis`
- def: [`understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts:1`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L1)
- signature: `interface LLMFileAnalysis`
- members:
  - `classSummaries` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L6)
  - `complexity` — [`L4`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L4)
  - `fileSummary` — [`L2`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L2)
  - `functionSummaries` — [`L5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L5)
  - `languageNotes` — [`L7`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L7)
  - `tags` — [`L3`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L3)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`llm-analyzer.test.ts`](llm-analyzer.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-analyzer-llm-analyzer.test.ts), [`parseFileAnalysisResponse`](llm-analyzer.ts.md#parseFileAnalysisResponse)

### `LLMProjectSummary`
- def: [`understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts:10`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L10)
- signature: `interface LLMProjectSummary`
- members:
  - `description` — [`L11`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L11)
  - `description` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L13)
  - `filePatterns` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L13)
  - `frameworks` — [`L12`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L12)
  - `layers` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L13)
  - `name` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L13)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`llm-analyzer.test.ts`](llm-analyzer.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-analyzer-llm-analyzer.test.ts), [`parseProjectSummaryResponse`](llm-analyzer.ts.md#parseProjectSummaryResponse)

## Functions
- `buildFileAnalysisPrompt(filePath: string, content: string, projectContext: string)` — [`L19`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L19) — Generates a prompt for analyzing a single source file with an LLM.
- `buildProjectSummaryPrompt(fileList: string[], sampleFiles: { path: string; content: string; }[])` — [`L48`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L48) — Generates a prompt for creating a project-level summary with an LLM.
- `extractJson(response: string)` — [`L81`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L81) — Extracts a JSON block from an LLM response, handling markdown fences.
- `parseFileAnalysisResponse(response: string)` — [`L102`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L102) — Parses an LLM response for file analysis. Returns null if parsing fails.
- `parseProjectSummaryResponse(response: string)` — [`L148`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L148) — Parses an LLM response for project summary. Returns null if parsing fails.

## Module values
- `VALID_COMPLEXITIES` — [`L97`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L97)
- `content` — [`L50`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L50)
- `path` — [`L50`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/llm-analyzer.ts#L50)

