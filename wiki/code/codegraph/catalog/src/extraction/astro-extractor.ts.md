---
title: 'Module: src/extraction/astro-extractor.ts'
type: catalog
provenance: extracted
module: src/extraction/astro-extractor.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`astro-extractor.ts`/A
symbols:
  AstroExtractor.processScriptContent: stroExtractor#processScriptContent().
  AstroExtractor.extract: stroExtractor#extract().
  AstroExtractor.createComponentNode: stroExtractor#createComponentNode().
  AstroExtractor.extractTemplateComponents: stroExtractor#extractTemplateComponents().
  AstroExtractor.extractTemplateCalls: stroExtractor#extractTemplateCalls().
  AstroExtractor.filePath: stroExtractor#filePath.
  AstroExtractor.source: stroExtractor#source.
  AstroExtractor.unresolvedReferences: stroExtractor#unresolvedReferences.
  AstroExtractor.errors: stroExtractor#errors.
  AstroExtractor.-constructor: stroExtractor#`<constructor>`().
  AstroExtractor.nodes: stroExtractor#nodes.
  AstroExtractor.edges: stroExtractor#edges.
  AstroExtractor.processScriptContent.block-typeLiteral88.startLine: stroExtractor#processScriptContent().(block)typeLiteral88:startLine.
  AstroExtractor.extractFrontmatter: stroExtractor#extractFrontmatter().
  AstroExtractor.extractScriptBlocks: stroExtractor#extractScriptBlocks().
  AstroExtractor.getCoveredRanges: stroExtractor#getCoveredRanges().
  ASTRO_BUILTIN_COMPONENTS: STRO_BUILTIN_COMPONENTS.
  AstroExtractor: stroExtractor#
  AstroExtractor.processScriptContent.block-typeLiteral88.content: stroExtractor#processScriptContent().(block)typeLiteral88:content.
  AstroExtractor.extractScriptBlocks.Array.typeLiteral56.content: stroExtractor#extractScriptBlocks().Array:typeLiteral56:content.
  AstroExtractor.extractScriptBlocks.Array.typeLiteral56.startLine: stroExtractor#extractScriptBlocks().Array:typeLiteral56:startLine.
---
# Module: [`src/extraction/astro-extractor.ts`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts)

## Classes
### `AstroExtractor`
- def: [`src/extraction/astro-extractor.ts:28`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L28)
- doc: AstroExtractor - Extracts code relationships from Astro component files
- signature: `class AstroExtractor`
- members:
  - `<constructor>(filePath: string, source: string)` — [`L36`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L36) — AstroExtractor - Extracts code relationships from Astro component files
  - `createComponentNode(method)` — [`L90`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L90) — Create a component node for the .astro file
  - `extract(method)` — [`L44`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L44) — Extract from Astro source
  - `extractFrontmatter(method)` — [`L123`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L123) — Extract the frontmatter block: the content between the opening `---`
  - `extractScriptBlocks(method)` — [`L156`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L156) — Extract <script> blocks from the template portion
  - `extractTemplateCalls(method)` — [`L278`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L278) — Extract function calls from Astro template expressions.
  - `extractTemplateComponents(method)` — [`L336`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L336) — Extract component usages from the Astro template.
  - `getCoveredRanges(method)` — [`L247`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L247) — Line ranges (0-indexed, inclusive) the template scans must skip:
  - `processScriptContent(method)` — [`L185`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L185) — Process frontmatter / script content by delegating to TreeSitterExtractor.
  - `content` — [`L156`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L156)
  - `content` — [`L186`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L186)
  - `edges` — [`L32`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L32)
  - `errors` — [`L34`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L34)
  - `filePath` — [`L29`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L29)
  - `nodes` — [`L31`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L31)
  - `source` — [`L30`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L30)
  - `startLine` — [`L156`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L156)
  - `startLine` — [`L186`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L186)
  - `unresolvedReferences` — [`L33`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L33)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`startLine`](../types.ts.md#Node.startLine), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`source`](../types.ts.md#Edge.source), [`extract`](tree-sitter.ts.md#TreeSitterExtractor.extract), [`kind`](../types.ts.md#Edge.kind), [`endLine`](../types.ts.md#Node.endLine), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`line`](../types.ts.md#UnresolvedReference.line), [`referenceName`](../types.ts.md#UnresolvedReference.referenceName), [`referenceKind`](../types.ts.md#UnresolvedReference.referenceKind), [`column`](../types.ts.md#UnresolvedReference.column), [`endColumn`](../types.ts.md#Node.endColumn), [`startColumn`](../types.ts.md#Node.startColumn), [`updatedAt`](../types.ts.md#Node.updatedAt), [`line`](../types.ts.md#Edge.line), [`ExtractionResult`](../types.ts.md#ExtractionResult), [`nodes`](../types.ts.md#ExtractionResult.nodes), [`errors`](../types.ts.md#ExtractionResult.errors), [`generateNodeId`](tree-sitter-helpers.ts.md#generateNodeId), [`severity`](../types.ts.md#ExtractionError.severity), [`UnresolvedReference`](../types.ts.md#UnresolvedReference), [`message`](../types.ts.md#ExtractionError.message), [`<constructor>`](tree-sitter.ts.md#TreeSitterExtractor.-constructor), [`edges`](../types.ts.md#ExtractionResult.edges), [`isExported`](../types.ts.md#Node.isExported), [`unresolvedReferences`](../types.ts.md#ExtractionResult.unresolvedReferences), [`ExtractionError`](../types.ts.md#ExtractionError), [`language`](../types.ts.md#UnresolvedReference.language), [`code`](../types.ts.md#ExtractionError.code), [`isLanguageSupported`](grammars.ts.md#isLanguageSupported), [`filePath`](../types.ts.md#UnresolvedReference.filePath), [`durationMs`](../types.ts.md#ExtractionResult.durationMs)  (+2 more)
- used by: [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`extractFromSource`](tree-sitter.ts.md#extractFromSource)

## Module values
- `ASTRO_BUILTIN_COMPONENTS` — [`L10`](../../../../../../raw/code/codegraph/src/extraction/astro-extractor.ts#L10) — Astro built-in components — compiler-provided (`<Fragment>`) or shipped by

