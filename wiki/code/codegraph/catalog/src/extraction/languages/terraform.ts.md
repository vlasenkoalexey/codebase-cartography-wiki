---
title: 'Module: src/extraction/languages/terraform.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/terraform.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`terraform.ts`/
symbols:
  terraformExtractor: terraformExtractor.
  emitModuleWiring: emitModuleWiring().
  emitLocals: emitLocals().
  emitModuleProvidersRefs: emitModuleProvidersRefs().
  emitReferencesInBody: emitReferencesInBody().
  emitProviderSelectionRef: emitProviderSelectionRef().
  emitRefFromVariableExpr: emitRefFromVariableExpr().
  readStringAttr: readStringAttr().
  providerSelectionFromExpr: providerSelectionFromExpr().
  readBlockHeader: readBlockHeader().
  stringLitValue: stringLitValue().
  collectReferences: collectReferences().
  findStringLit: findStringLit().
  getBlockBody: getBlockBody().
  describeBlock: describeBlock().
  BlockDecl.kind: BlockDecl#kind.
  BlockDecl.name: BlockDecl#name.
  BlockDecl.qualifiedName: BlockDecl#qualifiedName.
  BlockDecl.signature: BlockDecl#signature.
  EmitRefsOptions.skipTopAttrs: EmitRefsOptions#skipTopAttrs.
  BUILTIN_HEADS: BUILTIN_HEADS.
  BUILTIN_KEYWORDS: BUILTIN_KEYWORDS.
  qualifyReference: qualifyReference().
  MODULE_META_ARGS: MODULE_META_ARGS.
  BlockDecl: BlockDecl#
  EmitRefsOptions: EmitRefsOptions#
  EmitRefsOptions.suppressScoped: EmitRefsOptions#suppressScoped.
---
# Module: [`src/extraction/languages/terraform.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts)

## Classes
### `BlockDecl`
- def: [`src/extraction/languages/terraform.ts:404`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L404)
- signature: `interface BlockDecl`
- members:
  - `kind` — [`L405`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L405)
  - `name` — [`L406`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L406)
  - `qualifiedName` — [`L407`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L407)
  - `signature` — [`L408`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L408)
- used by: [`terraformExtractor`](terraform.ts.md#terraformExtractor), [`describeBlock`](terraform.ts.md#describeBlock)

### `EmitRefsOptions`
- def: [`src/extraction/languages/terraform.ts:508`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L508)
- signature: `interface EmitRefsOptions`
- members:
  - `skipTopAttrs` — [`L512`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L512) — Direct attributes of `body` to skip (meta-arguments handled explicitly elsewhere).
  - `suppressScoped` — [`L510`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L510) — Drop `:`-scoped module refs (moved/import blocks name resources INSIDE a module instance).
- used by: [`emitReferencesInBody`](terraform.ts.md#emitReferencesInBody)

## Functions
- `collectReferences(expr: Node, source: string, onRef: (qualifiedName: string, line: number, column: number) => void)` — [`L89`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L89) — Walk an `expression` subtree and emit a reference for every dotted name
- `describeBlock(type: string, labels: string[])` — [`L411`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L411)
- `emitLocals(body: Node | null, ctx: ExtractorContext)` — [`L473`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L473) — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `emitModuleProvidersRefs(body: Node, ctx: ExtractorContext, fromNodeId: string)` — [`L603`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L603) — `providers = { aws = aws.east, aws.dns = aws.dns }` in a module block maps — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `emitModuleWiring(moduleName: string, block: Node, body: Node, ctx: ExtractorContext, fromNodeId: string)` — [`L353`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L353) — Bridge a `module "M" { ... }` block across the module boundary with — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `emitProviderSelectionRef(body: Node, ctx: ExtractorContext, fromNodeId: string)` — [`L573`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L573) — `provider = aws.east` (or bare `provider = google-beta`) in a resource/data — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `emitRefFromVariableExpr(varExpr: Node, source: string, onRef: (qualifiedName: string, line: number, column: number) => void)` — [`L111`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L111)
- `emitReferencesInBody(body: Node, ctx: ExtractorContext, fromNodeId: string, opts?: EmitRefsOptions | undefined)` — [`L515`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L515) — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `findStringLit(expr: Node)` — [`L392`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L392) — First string_lit anywhere under an expression (source = "./modules/x").
- `getBlockBody(block: Node)` — [`L73`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L73) — Find the `body` child of a block (it's after the labels and block_start).
- `providerSelectionFromExpr(expr: Node, source: string)` — [`L644`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L644) — Read a provider-configuration address (`aws`, `aws.east`, `google-beta`)
- `qualifyReference(head: string, attrs: string[])` — [`L145`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L145)
- `readBlockHeader(block: Node, source: string)` — [`L51`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L51) — Block "type" and its label values. Returns null if the block is malformed.
- `readStringAttr(body: Node, name: string, source: string)` — [`L555`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L555) — Value of a direct string attribute of a body (`alias = "east"`), or null.
- `stringLitValue(node: Node, source: string)` — [`L42`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L42) — Read a string_lit value (skipping the quotes / template start/end tokens).

## Module values
- `BUILTIN_HEADS` — [`L30`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L30) — Built-in references that should NOT be resolved to project nodes.
- `BUILTIN_KEYWORDS` — [`L39`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L39) — Bare strings that we never want to treat as references.
- `MODULE_META_ARGS` — [`L336`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L336) — Module meta-arguments — attributes of a `module` block that configure the
- `terraformExtractor` — [`L185`](../../../../../../../raw/code/codegraph/src/extraction/languages/terraform.ts#L185)

