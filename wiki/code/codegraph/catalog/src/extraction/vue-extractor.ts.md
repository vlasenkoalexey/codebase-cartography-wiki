---
title: 'Module: src/extraction/vue-extractor.ts'
type: catalog
provenance: extracted
module: src/extraction/vue-extractor.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`vue-extractor.ts`/
symbols:
  VueExtractor.processScriptBlock: VueExtractor#processScriptBlock().
  VueExtractor.extract: VueExtractor#extract().
  VueExtractor.createComponentNode: VueExtractor#createComponentNode().
  VueExtractor.extractTemplateComponents: VueExtractor#extractTemplateComponents().
  VueExtractor.filePath: VueExtractor#filePath.
  VueExtractor.source: VueExtractor#source.
  VueExtractor.errors: VueExtractor#errors.
  VueExtractor.-constructor: VueExtractor#`<constructor>`().
  VueExtractor.nodes: VueExtractor#nodes.
  VueExtractor.edges: VueExtractor#edges.
  VueExtractor.unresolvedReferences: VueExtractor#unresolvedReferences.
  VueExtractor.processScriptBlock.block-typeLiteral79.startLine: VueExtractor#processScriptBlock().(block)typeLiteral79:startLine.
  VueExtractor.extractScriptBlocks: VueExtractor#extractScriptBlocks().
  VUE_BUILTIN_COMPONENTS: VUE_BUILTIN_COMPONENTS.
  kebabToPascal: kebabToPascal().
  VueExtractor: VueExtractor#
  VueExtractor.processScriptBlock.block-typeLiteral79.content: VueExtractor#processScriptBlock().(block)typeLiteral79:content.
  VueExtractor.processScriptBlock.block-typeLiteral79.isTypeScript: VueExtractor#processScriptBlock().(block)typeLiteral79:isTypeScript.
  VueExtractor.extractScriptBlocks.Array.typeLiteral36.content: VueExtractor#extractScriptBlocks().Array:typeLiteral36:content.
  VueExtractor.extractScriptBlocks.Array.typeLiteral36.startLine: VueExtractor#extractScriptBlocks().Array:typeLiteral36:startLine.
  VueExtractor.extractScriptBlocks.Array.typeLiteral36.isSetup: VueExtractor#extractScriptBlocks().Array:typeLiteral36:isSetup.
  VueExtractor.extractScriptBlocks.Array.typeLiteral36.isTypeScript: VueExtractor#extractScriptBlocks().Array:typeLiteral36:isTypeScript.
  VueExtractor.processScriptBlock.block-typeLiteral79.isSetup: VueExtractor#processScriptBlock().(block)typeLiteral79:isSetup.
---
# Module: [`src/extraction/vue-extractor.ts`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts)

## Classes
### `VueExtractor`
- def: [`src/extraction/vue-extractor.ts:38`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L38)
- doc: VueExtractor - Extracts code relationships from Vue Single-File Component files
- signature: `class VueExtractor`
- members:
  - `<constructor>(filePath: string, source: string)` — [`L46`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L46) — VueExtractor - Extracts code relationships from Vue Single-File Component files
  - `createComponentNode(method)` — [`L92`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L92) — Create a component node for the .vue file
  - `extract(method)` — [`L54`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L54) — Extract from Vue source
  - `extractScriptBlocks(method)` — [`L120`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L120) — Extract <script> and <script setup> blocks from the Vue source
  - `extractTemplateComponents(method)` — [`L245`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L245) — Extract component usages from the Vue `<template>`.
  - `processScriptBlock(method)` — [`L171`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L171) — Process a script block by delegating to TreeSitterExtractor
  - `content` — [`L121`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L121)
  - `content` — [`L172`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L172)
  - `edges` — [`L42`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L42)
  - `errors` — [`L44`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L44)
  - `filePath` — [`L39`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L39)
  - `isSetup` — [`L123`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L123)
  - `isSetup` — [`L172`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L172)
  - `isTypeScript` — [`L124`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L124)
  - `isTypeScript` — [`L172`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L172)
  - `nodes` — [`L41`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L41)
  - `source` — [`L40`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L40)
  - `startLine` — [`L122`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L122)
  - `startLine` — [`L172`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L172)
  - `unresolvedReferences` — [`L43`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L43)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`startLine`](../types.ts.md#Node.startLine), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`source`](../types.ts.md#Edge.source), [`extract`](tree-sitter.ts.md#TreeSitterExtractor.extract), [`kind`](../types.ts.md#Edge.kind), [`endLine`](../types.ts.md#Node.endLine), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`line`](../types.ts.md#UnresolvedReference.line), [`referenceName`](../types.ts.md#UnresolvedReference.referenceName), [`referenceKind`](../types.ts.md#UnresolvedReference.referenceKind), [`column`](../types.ts.md#UnresolvedReference.column), [`Language`](../types.ts.md#Language), [`endColumn`](../types.ts.md#Node.endColumn), [`startColumn`](../types.ts.md#Node.startColumn), [`updatedAt`](../types.ts.md#Node.updatedAt), [`line`](../types.ts.md#Edge.line), [`ExtractionResult`](../types.ts.md#ExtractionResult), [`nodes`](../types.ts.md#ExtractionResult.nodes), [`errors`](../types.ts.md#ExtractionResult.errors), [`generateNodeId`](tree-sitter-helpers.ts.md#generateNodeId), [`severity`](../types.ts.md#ExtractionError.severity), [`UnresolvedReference`](../types.ts.md#UnresolvedReference), [`message`](../types.ts.md#ExtractionError.message), [`<constructor>`](tree-sitter.ts.md#TreeSitterExtractor.-constructor), [`edges`](../types.ts.md#ExtractionResult.edges), [`isExported`](../types.ts.md#Node.isExported), [`unresolvedReferences`](../types.ts.md#ExtractionResult.unresolvedReferences), [`ExtractionError`](../types.ts.md#ExtractionError), [`language`](../types.ts.md#UnresolvedReference.language), [`isLanguageSupported`](grammars.ts.md#isLanguageSupported), [`filePath`](../types.ts.md#UnresolvedReference.filePath), [`durationMs`](../types.ts.md#ExtractionResult.durationMs)  (+3 more)
- used by: [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`extractFromSource`](tree-sitter.ts.md#extractFromSource)

## Functions
- `kebabToPascal(name: string)` — [`L22`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L22) — `my-component` → `MyComponent` (Vue allows either form in templates).

## Module values
- `VUE_BUILTIN_COMPONENTS` — [`L11`](../../../../../../raw/code/codegraph/src/extraction/vue-extractor.ts#L11) — Vue built-in components — skipped so a `<Transition>` / `<KeepAlive>` in the

