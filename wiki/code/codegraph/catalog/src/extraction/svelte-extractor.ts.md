---
title: 'Module: src/extraction/svelte-extractor.ts'
type: catalog
provenance: extracted
module: src/extraction/svelte-extractor.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`svelte-extractor.ts`/S
symbols:
  SvelteExtractor.processScriptBlock: velteExtractor#processScriptBlock().
  SvelteExtractor.extract: velteExtractor#extract().
  SvelteExtractor.createComponentNode: velteExtractor#createComponentNode().
  SvelteExtractor.extractTemplateCalls: velteExtractor#extractTemplateCalls().
  SvelteExtractor.extractTemplateComponents: velteExtractor#extractTemplateComponents().
  SvelteExtractor.filePath: velteExtractor#filePath.
  SvelteExtractor.source: velteExtractor#source.
  SvelteExtractor.unresolvedReferences: velteExtractor#unresolvedReferences.
  SvelteExtractor.errors: velteExtractor#errors.
  SvelteExtractor.-constructor: velteExtractor#`<constructor>`().
  SvelteExtractor.nodes: velteExtractor#nodes.
  SvelteExtractor.edges: velteExtractor#edges.
  SvelteExtractor.processScriptBlock.block-typeLiteral78.startLine: velteExtractor#processScriptBlock().(block)typeLiteral78:startLine.
  SvelteExtractor.extractScriptBlocks: velteExtractor#extractScriptBlocks().
  SVELTE_RUNES: VELTE_RUNES.
  SvelteExtractor: velteExtractor#
  SvelteExtractor.processScriptBlock.block-typeLiteral78.content: velteExtractor#processScriptBlock().(block)typeLiteral78:content.
  SvelteExtractor.processScriptBlock.block-typeLiteral78.isTypeScript: velteExtractor#processScriptBlock().(block)typeLiteral78:isTypeScript.
  SvelteExtractor.extractScriptBlocks.Array.typeLiteral35.content: velteExtractor#extractScriptBlocks().Array:typeLiteral35:content.
  SvelteExtractor.extractScriptBlocks.Array.typeLiteral35.startLine: velteExtractor#extractScriptBlocks().Array:typeLiteral35:startLine.
  SvelteExtractor.extractScriptBlocks.Array.typeLiteral35.isModule: velteExtractor#extractScriptBlocks().Array:typeLiteral35:isModule.
  SvelteExtractor.extractScriptBlocks.Array.typeLiteral35.isTypeScript: velteExtractor#extractScriptBlocks().Array:typeLiteral35:isTypeScript.
  SvelteExtractor.processScriptBlock.block-typeLiteral78.isModule: velteExtractor#processScriptBlock().(block)typeLiteral78:isModule.
  SvelteExtractor.extractTemplateCalls._scriptBlocks-Array.typeLiteral100.content: velteExtractor#extractTemplateCalls().(_scriptBlocks)Array:typeLiteral100:content.
  SvelteExtractor.extractTemplateCalls._scriptBlocks-Array.typeLiteral100.startLine: velteExtractor#extractTemplateCalls().(_scriptBlocks)Array:typeLiteral100:startLine.
---
# Module: [`src/extraction/svelte-extractor.ts`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts)

## Classes
### `SvelteExtractor`
- def: [`src/extraction/svelte-extractor.ts:24`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L24)
- doc: SvelteExtractor - Extracts code relationships from Svelte component files
- signature: `class SvelteExtractor`
- members:
  - `<constructor>(filePath: string, source: string)` — [`L32`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L32) — SvelteExtractor - Extracts code relationships from Svelte component files
  - `createComponentNode(method)` — [`L84`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L84) — Create a component node for the .svelte file
  - `extract(method)` — [`L40`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L40) — Extract from Svelte source
  - `extractScriptBlocks(method)` — [`L112`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L112) — Extract <script> blocks from the Svelte source
  - `extractTemplateCalls(method)` — [`L230`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L230) — Extract function calls from Svelte template expressions.
  - `extractTemplateComponents(method)` — [`L291`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L291) — Extract component usages from the Svelte template.
  - `processScriptBlock(method)` — [`L163`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L163) — Process a script block by delegating to TreeSitterExtractor
  - `content` — [`L113`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L113)
  - `content` — [`L164`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L164)
  - `content` — [`L232`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L232)
  - `edges` — [`L28`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L28)
  - `errors` — [`L30`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L30)
  - `filePath` — [`L25`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L25)
  - `isModule` — [`L115`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L115)
  - `isModule` — [`L164`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L164)
  - `isTypeScript` — [`L116`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L116)
  - `isTypeScript` — [`L164`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L164)
  - `nodes` — [`L27`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L27)
  - `source` — [`L26`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L26)
  - `startLine` — [`L114`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L114)
  - `startLine` — [`L164`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L164)
  - `startLine` — [`L232`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L232)
  - `unresolvedReferences` — [`L29`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L29)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`startLine`](../types.ts.md#Node.startLine), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`source`](../types.ts.md#Edge.source), [`extract`](tree-sitter.ts.md#TreeSitterExtractor.extract), [`kind`](../types.ts.md#Edge.kind), [`endLine`](../types.ts.md#Node.endLine), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`line`](../types.ts.md#UnresolvedReference.line), [`referenceName`](../types.ts.md#UnresolvedReference.referenceName), [`referenceKind`](../types.ts.md#UnresolvedReference.referenceKind), [`column`](../types.ts.md#UnresolvedReference.column), [`Language`](../types.ts.md#Language), [`endColumn`](../types.ts.md#Node.endColumn), [`startColumn`](../types.ts.md#Node.startColumn), [`updatedAt`](../types.ts.md#Node.updatedAt), [`line`](../types.ts.md#Edge.line), [`ExtractionResult`](../types.ts.md#ExtractionResult), [`nodes`](../types.ts.md#ExtractionResult.nodes), [`errors`](../types.ts.md#ExtractionResult.errors), [`generateNodeId`](tree-sitter-helpers.ts.md#generateNodeId), [`severity`](../types.ts.md#ExtractionError.severity), [`UnresolvedReference`](../types.ts.md#UnresolvedReference), [`message`](../types.ts.md#ExtractionError.message), [`<constructor>`](tree-sitter.ts.md#TreeSitterExtractor.-constructor), [`edges`](../types.ts.md#ExtractionResult.edges), [`isExported`](../types.ts.md#Node.isExported), [`unresolvedReferences`](../types.ts.md#ExtractionResult.unresolvedReferences), [`ExtractionError`](../types.ts.md#ExtractionError), [`language`](../types.ts.md#UnresolvedReference.language), [`code`](../types.ts.md#ExtractionError.code), [`isLanguageSupported`](grammars.ts.md#isLanguageSupported), [`filePath`](../types.ts.md#UnresolvedReference.filePath)  (+3 more)
- used by: [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`extractFromSource`](tree-sitter.ts.md#extractFromSource)

## Module values
- `SVELTE_RUNES` — [`L7`](../../../../../../raw/code/codegraph/src/extraction/svelte-extractor.ts#L7) — Svelte 5 rune names — compiler builtins, not real functions

