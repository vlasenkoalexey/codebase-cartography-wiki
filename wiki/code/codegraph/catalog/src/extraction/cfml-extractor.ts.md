---
title: 'Module: src/extraction/cfml-extractor.ts'
type: catalog
provenance: extracted
module: src/extraction/cfml-extractor.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`cfml-extractor.ts`/
symbols:
  CfmlExtractor.extractComponent: CfmlExtractor#extractComponent().
  CfmlExtractor.delegateScriptTag: CfmlExtractor#delegateScriptTag().
  CfmlExtractor.extractFunctionTag: CfmlExtractor#extractFunctionTag().
  CfmlExtractor.delegateQueryTag: CfmlExtractor#delegateQueryTag().
  CfmlExtractor.extractBareScript: CfmlExtractor#extractBareScript().
  CfmlExtractor.extract: CfmlExtractor#extract().
  CfmlExtractor.createFileNode: CfmlExtractor#createFileNode().
  CfmlExtractor.extractTagBased: CfmlExtractor#extractTagBased().
  CfmlExtractor.tagAttr: CfmlExtractor#tagAttr().
  CfmlExtractor.walkProgram: CfmlExtractor#walkProgram().
  CfmlExtractor.filePath: CfmlExtractor#filePath.
  CfmlExtractor.delegateNestedTags: CfmlExtractor#delegateNestedTags().
  CfmlExtractor.language: CfmlExtractor#language.
  CfmlExtractor.-constructor: CfmlExtractor#`<constructor>`().
  CfmlExtractor.errors: CfmlExtractor#errors.
  CfmlExtractor.source: CfmlExtractor#source.
  CfmlExtractor.nodes: CfmlExtractor#nodes.
  CfmlExtractor.edges: CfmlExtractor#edges.
  CfmlExtractor.unresolvedReferences: CfmlExtractor#unresolvedReferences.
  CfmlExtractor.componentNameFromPath: CfmlExtractor#componentNameFromPath().
  CfmlExtractor: CfmlExtractor#
  isBareScriptCfml: isBareScriptCfml().
---
# Module: [`src/extraction/cfml-extractor.ts`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts)

## Classes
### `CfmlExtractor`
- def: [`src/extraction/cfml-extractor.ts:20`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L20)
- doc: CfmlExtractor - Extracts code relationships from CFML source (.cfc/.cfm).
- signature: `class CfmlExtractor`
- members:
  - `<constructor>(filePath: string, source: string, language?: "typescript" | "javascript" | "tsx" | "jsx" | "python" | "go" | "rust" | "java" | "c" | "cpp" | "csharp" | "razor" | "php" | "ruby" | "swift" | ... 24 more ... | "unknown")` — [`L30`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L30) — CfmlExtractor - Extracts code relationships from CFML source (.cfc/.cfm).
  - `componentNameFromPath(method)` — [`L462`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L462)
  - `createFileNode(method)` — [`L120`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L120) — Build the file's own `kind:'file'` node, spanning the whole source. Tag-based files need this explicitly — unlike `extractBareScript` (which delegates the whole file to `TreeSitterExtractor` and inherits its file node), `extractTagBased` walks the tree itself and has no other source of one.
  - `delegateNestedTags(method)` — [`L308`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L308) — Recursively delegates any `cf_script_tag`/`cf_query_tag` found within
  - `delegateQueryTag(method)` — [`L407`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L407) — Delegate a `<cfquery>...</cfquery>` tag's SQL body to the `cfquery` grammar.
  - `delegateScriptTag(method)` — [`L335`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L335) — Delegate a `<cfscript>...</cfscript>` tag body to the cfscript grammar.
  - `extract(method)` — [`L36`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L36)
  - `extractBareScript(method)` — [`L63`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L63) — Modern bare-script `.cfc`/`.cfm`: delegate the whole file to the cfscript grammar.
  - `extractComponent(method)` — [`L175`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L175) — `<cfcomponent extends="Base" implements="IFoo,IBar">...</cfcomponent>`. — documented in [extraction-tree-sitter-helpers.ts](../../../concepts/extraction-tree-sitter-helpers.ts.md)
  - `extractFunctionTag(method)` — [`L259`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L259) — `<cffunction name="..." access="..." returntype="...">...</cffunction>`. — documented in [extraction-tree-sitter-helpers.ts](../../../concepts/extraction-tree-sitter-helpers.ts.md)
  - `extractTagBased(method)` — [`L94`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L94) — Legacy tag-based CFML: walk `<cfcomponent>`/`<cffunction>`, delegating `<cfscript>` bodies.
  - `tagAttr(method)` — [`L432`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L432) — Read a `cf_attribute`'s value by name from a tag node's direct `cf_attribute`/`cf_tag_attributes` children.
  - `walkProgram(method)` — [`L147`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L147) — Walks `program`'s named children with a single forward cursor (not an
  - `edges` — [`L25`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L25)
  - `errors` — [`L27`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L27)
  - `filePath` — [`L21`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L21)
  - `language` — [`L23`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L23)
  - `nodes` — [`L24`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L24)
  - `source` — [`L22`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L22)
  - `unresolvedReferences` — [`L26`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L26)
- uses (calls/refs, reference-scoped): [`<get>type`](../web-tree-sitter.d.ts.md#Node.-get-type), [`id`](../types.ts.md#Node.id), [`Node`](../web-tree-sitter.d.ts.md#Node), [`Node`](../types.ts.md#Node), [`kind`](../types.ts.md#Node.kind), [`filePath`](../types.ts.md#Node.filePath), [`<get>namedChildren`](../web-tree-sitter.d.ts.md#Node.-get-namedChildren), [`name`](../types.ts.md#Node.name), [`startLine`](../types.ts.md#Node.startLine), [`namedChild`](../web-tree-sitter.d.ts.md#Node.namedChild), [`startPosition`](../web-tree-sitter.d.ts.md#Node.startPosition), [`Edge`](../types.ts.md#Edge), [`language`](../types.ts.md#Node.language), [`<get>namedChildCount`](../web-tree-sitter.d.ts.md#Node.-get-namedChildCount), [`target`](../types.ts.md#Edge.target), [`qualifiedName`](../types.ts.md#Node.qualifiedName), [`source`](../types.ts.md#Edge.source), [`extract`](tree-sitter.ts.md#TreeSitterExtractor.extract), [`kind`](../types.ts.md#Edge.kind), [`endLine`](../types.ts.md#Node.endLine), [`fromNodeId`](../types.ts.md#UnresolvedReference.fromNodeId), [`line`](../types.ts.md#UnresolvedReference.line), [`referenceName`](../types.ts.md#UnresolvedReference.referenceName), [`referenceKind`](../types.ts.md#UnresolvedReference.referenceKind), [`column`](../types.ts.md#UnresolvedReference.column), [`Language`](../types.ts.md#Language), [`row`](../web-tree-sitter.d.ts.md#Point.row), [`column`](../web-tree-sitter.d.ts.md#Point.column), [`endColumn`](../types.ts.md#Node.endColumn), [`startColumn`](../types.ts.md#Node.startColumn), [`updatedAt`](../types.ts.md#Node.updatedAt), [`line`](../types.ts.md#Edge.line), [`startIndex`](../web-tree-sitter.d.ts.md#Node.startIndex), [`ExtractionResult`](../types.ts.md#ExtractionResult), [`<get>endIndex`](../web-tree-sitter.d.ts.md#Node.-get-endIndex), [`nodes`](../types.ts.md#ExtractionResult.nodes), [`errors`](../types.ts.md#ExtractionResult.errors), [`generateNodeId`](tree-sitter-helpers.ts.md#generateNodeId), [`severity`](../types.ts.md#ExtractionError.severity), [`UnresolvedReference`](../types.ts.md#UnresolvedReference)  (+19 more)
- used by: [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`extractFromSource`](tree-sitter.ts.md#extractFromSource)

## Functions
- `isBareScriptCfml(source: string)` — [`L476`](../../../../../../raw/code/codegraph/src/extraction/cfml-extractor.ts#L476) — Sniff whether CFML source is bare-script (`component { ... }`, modern style)

