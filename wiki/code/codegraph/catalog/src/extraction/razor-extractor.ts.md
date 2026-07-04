---
title: 'Module: src/extraction/razor-extractor.ts'
type: catalog
provenance: extracted
module: src/extraction/razor-extractor.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`razor-extractor.ts`/
symbols:
  RazorExtractor.extract: RazorExtractor#extract().
  RazorExtractor.createComponentNode: RazorExtractor#createComponentNode().
  RazorExtractor.processCodeBlocks: RazorExtractor#processCodeBlocks().
  RazorExtractor.pushRef: RazorExtractor#pushRef().
  RazorExtractor.extractDirectives: RazorExtractor#extractDirectives().
  RazorExtractor.extractComponentTags: RazorExtractor#extractComponentTags().
  RazorExtractor.filePath: RazorExtractor#filePath.
  RazorExtractor.source: RazorExtractor#source.
  RazorExtractor.-constructor: RazorExtractor#`<constructor>`().
  RazorExtractor.extractCodeBlocks: RazorExtractor#extractCodeBlocks().
  RazorExtractor.unresolvedReferences: RazorExtractor#unresolvedReferences.
  RazorExtractor.nodes: RazorExtractor#nodes.
  RazorExtractor.errors: RazorExtractor#errors.
  RazorExtractor.typeNames: RazorExtractor#typeNames().
  RazorExtractor.edges: RazorExtractor#edges.
  RazorExtractor.lastSegment: RazorExtractor#lastSegment().
  RazorExtractor.extractCodeBlocks.Array.typeLiteral98.content: RazorExtractor#extractCodeBlocks().Array:typeLiteral98:content.
  BLAZOR_BUILTIN_COMPONENTS: BLAZOR_BUILTIN_COMPONENTS.
  RazorExtractor: RazorExtractor#
  RazorExtractor.matchBrace: RazorExtractor#matchBrace().
  RazorExtractor.extractCodeBlocks.Array.typeLiteral98.lineOffset: RazorExtractor#extractCodeBlocks().Array:typeLiteral98:lineOffset.
---
# Module: [`src/extraction/razor-extractor.ts`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts)

## Classes
### `RazorExtractor`
- def: [`src/extraction/razor-extractor.ts:50`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L50)
- signature: `class RazorExtractor`
- members:
  - `<constructor>(filePath: string, source: string)` — [`L58`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L58)
  - `createComponentNode(method)` — [`L94`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L94)
  - `extract(method)` — [`L63`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L63)
  - `extractCodeBlocks(method)` — [`L225`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L225) — `@code { … }` / `@functions { … }` (Blazor) and `@{ … }` (Razor) C# blocks.
  - `extractComponentTags(method)` — [`L166`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L166)
  - `extractDirectives(method)` — [`L148`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L148)
  - `lastSegment(method)` — [`L117`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L117) — Last `.`-segment (`App.ViewModels.RegisterModel` → `RegisterModel`).
  - `matchBrace(method)` — [`L192`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L192) — Find the matching `}` for the `{` at `openIdx`, skipping string literals and
  - `processCodeBlocks(method)` — [`L252`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L252) — Delegate each `@code`/`@functions`/`@{` block's C# to the tree-sitter C#
  - `pushRef(method)` — [`L136`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L136)
  - `typeNames(method)` — [`L127`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L127) — Split a type expression into the capitalized type names it contains — base
  - `content` — [`L225`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L225)
  - `edges` — [`L54`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L54)
  - `errors` — [`L56`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L56)
  - `filePath` — [`L51`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L51)
  - `lineOffset` — [`L225`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L225)
  - `nodes` — [`L53`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L53)
  - `source` — [`L52`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L52)
  - `unresolvedReferences` — [`L55`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L55)
- uses (calls/refs, reference-scoped): [`id`](../types.ts.md#Node.id), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`name`](../types.ts.md#Node.name), [`startLine`](../types.ts.md#Node.startLine), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`extract`](tree-sitter.ts.md#TreeSitterExtractor.extract), [`endLine`](../types.ts.md#Node.endLine), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`line`](../types.ts.md#UnresolvedReference.line), [`referenceName`](../types.ts.md#UnresolvedReference.referenceName), [`referenceKind`](../types.ts.md#UnresolvedReference.referenceKind), [`column`](../types.ts.md#UnresolvedReference.column), [`endColumn`](../types.ts.md#Node.endColumn), [`startColumn`](../types.ts.md#Node.startColumn), [`updatedAt`](../types.ts.md#Node.updatedAt), [`ExtractionResult`](../types.ts.md#ExtractionResult), [`nodes`](../types.ts.md#ExtractionResult.nodes), [`errors`](../types.ts.md#ExtractionResult.errors), [`generateNodeId`](tree-sitter-helpers.ts.md#generateNodeId), [`severity`](../types.ts.md#ExtractionError.severity), [`UnresolvedReference`](../types.ts.md#UnresolvedReference), [`message`](../types.ts.md#ExtractionError.message), [`<constructor>`](tree-sitter.ts.md#TreeSitterExtractor.-constructor), [`edges`](../types.ts.md#ExtractionResult.edges), [`isExported`](../types.ts.md#Node.isExported), [`unresolvedReferences`](../types.ts.md#ExtractionResult.unresolvedReferences), [`ExtractionError`](../types.ts.md#ExtractionError), [`language`](../types.ts.md#UnresolvedReference.language), [`code`](../types.ts.md#ExtractionError.code), [`isLanguageSupported`](grammars.ts.md#isLanguageSupported), [`filePath`](../types.ts.md#UnresolvedReference.filePath), [`durationMs`](../types.ts.md#ExtractionResult.durationMs), [`BLAZOR_BUILTIN_COMPONENTS`](razor-extractor.ts.md#BLAZOR_BUILTIN_COMPONENTS)
- used by: [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`extractFromSource`](tree-sitter.ts.md#extractFromSource)

## Module values
- `BLAZOR_BUILTIN_COMPONENTS` — [`L39`](../../../../../../raw/code/codegraph/src/extraction/razor-extractor.ts#L39) — Blazor framework-provided components — invoked by the runtime, not defined

