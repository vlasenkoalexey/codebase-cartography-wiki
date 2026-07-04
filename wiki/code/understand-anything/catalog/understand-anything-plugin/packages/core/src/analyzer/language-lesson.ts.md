---
title: 'Module: understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts'
type: catalog
provenance: extracted
module: understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts
status: fresh
symbol_base: scip-typescript npm @understand-anything/core 0.1.0 src/analyzer/`language-lesson.ts`/
symbols:
  buildLanguageLessonPrompt: buildLanguageLessonPrompt().
  detectLanguageConcepts: detectLanguageConcepts().
  parseLanguageLessonResponse: parseLanguageLessonResponse().
  LanguageLessonResult.concepts: LanguageLessonResult#concepts.
  buildConceptPatterns: buildConceptPatterns().
  LanguageLessonResult.languageNotes: LanguageLessonResult#languageNotes.
  getLanguageDisplayName: getLanguageDisplayName().
  LanguageLessonResult: LanguageLessonResult#
  LanguageLessonResult.concepts.Array.typeLiteral0.name: LanguageLessonResult#concepts.Array:typeLiteral0:name.
  LanguageLessonResult.concepts.Array.typeLiteral0.explanation: LanguageLessonResult#concepts.Array:typeLiteral0:explanation.
  BASE_CONCEPT_PATTERNS: BASE_CONCEPT_PATTERNS.
  extractJson: extractJson().
---
# Module: [`understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts)

## Classes
### `LanguageLessonResult`
- def: [`understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts:4`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L4)
- signature: `interface LanguageLessonResult`
- members:
  - `concepts` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L6)
  - `explanation` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L6)
  - `languageNotes` — [`L5`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L5)
  - `name` — [`L6`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L6)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-index.ts), [`language-lesson.test.ts`](../__tests__/language-lesson.test.ts.md#scip-typescript-npm-understand-anything-core-0.1.0-src-__tests__-language-lesson.test.ts), [`parseLanguageLessonResponse`](language-lesson.ts.md#parseLanguageLessonResponse)

## Functions
- `buildConceptPatterns(langConfig?: any)` — [`L48`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L48) — Build the full concept patterns map by merging base patterns with — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
- `buildLanguageLessonPrompt(node: GraphNode, edges: GraphEdge[], language: string, langConfig?: any)` — [`L112`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L112) — Builds a prompt that asks an LLM to produce a language-specific lesson for a given node. — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
- `detectLanguageConcepts(node: GraphNode, language: string, langConfig?: any)` — [`L69`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L69) — Detects language concepts present in a graph node based on its tags, summary, and languageNotes. — documented in [understand-anything-plugin-packages-core-src-languages-types.ts](../../../../../../concepts/understand-anything-plugin-packages-core-src-languages-types.ts.md)
- `extractJson(response: string)` — [`L160`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L160) — Extracts a JSON block from an LLM response, handling markdown fences.
- `getLanguageDisplayName(language: string, langConfig?: any)` — [`L99`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L99) — Get the display name for a language.
- `parseLanguageLessonResponse(response: string)` — [`L178`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L178) — Parses an LLM response for language lesson content.

## Module values
- `BASE_CONCEPT_PATTERNS` — [`L13`](../../../../../../../../../raw/code/understand-anything/understand-anything-plugin/packages/core/src/analyzer/language-lesson.ts#L13) — Base concept patterns that apply across all languages.

