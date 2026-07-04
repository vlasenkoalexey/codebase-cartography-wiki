---
title: 'Module: extensions/vscode/src/providers/editorProviders.ts'
type: catalog
provenance: extracted
module: extensions/vscode/src/providers/editorProviders.ts
status: fresh
symbol_base: scip-typescript npm codegraphcontext-vscode 0.1.0 src/providers/`editorProviders.ts`/
symbols:
  CgcCodeLensProvider._fetchAll: CgcCodeLensProvider#_fetchAll().
  CgcDeadCodeDiagnostics.refreshForDocument: CgcDeadCodeDiagnostics#refreshForDocument().
  CgcCodeLensProvider.provideCodeLenses: CgcCodeLensProvider#provideCodeLenses().
  collectDefinitionLines.Array.typeLiteral4.symbol: collectDefinitionLines().Array:typeLiteral4:symbol.
  CgcHoverProvider.provideHover: CgcHoverProvider#provideHover().
  CgcCodeLensProvider.invalidate: CgcCodeLensProvider#invalidate().
  collectDefinitionLines: collectDefinitionLines().
  lensCache: lensCache.
  CgcDeadCodeDiagnostics.dispose: CgcDeadCodeDiagnostics#dispose().
  CgcDeadCodeDiagnostics.index: CgcDeadCodeDiagnostics#index.
  CgcCodeLensProvider._fetchingDocs: CgcCodeLensProvider#_fetchingDocs.
  CgcCodeLensProvider.-constructor: CgcCodeLensProvider#`<constructor>`().
  CgcHoverProvider.-constructor: CgcHoverProvider#`<constructor>`().
  CgcDeadCodeDiagnostics.-constructor: CgcDeadCodeDiagnostics#`<constructor>`().
  CgcCodeLensProvider._onDidChange: CgcCodeLensProvider#_onDidChange.
  CgcDeadCodeCodeActionProvider: CgcDeadCodeCodeActionProvider#
  CgcCodeLensProvider.onDidChangeCodeLenses: CgcCodeLensProvider#onDidChangeCodeLenses.
  collectDefinitionLines.Array.typeLiteral4.line: collectDefinitionLines().Array:typeLiteral4:line.
  CgcDeadCodeDiagnostics.collection: CgcDeadCodeDiagnostics#collection.
  CgcDeadCodeDiagnostics.strikeDecoration: CgcDeadCodeDiagnostics#strikeDecoration.
  DEF_PATTERN: DEF_PATTERN.
  symbolAtPosition: symbolAtPosition().
  collectDefinitionLines.Array.typeLiteral4.type: collectDefinitionLines().Array:typeLiteral4:type.
  CgcCodeLensProvider: CgcCodeLensProvider#
  CgcHoverProvider: CgcHoverProvider#
  CgcDeadCodeDiagnostics: CgcDeadCodeDiagnostics#
  CgcDeadCodeCodeActionProvider.providedCodeActionKinds: CgcDeadCodeCodeActionProvider#providedCodeActionKinds.
  CgcDeadCodeCodeActionProvider.provideCodeActions: CgcDeadCodeCodeActionProvider#provideCodeActions().
---
# Module: [`extensions/vscode/src/providers/editorProviders.ts`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts)

## Classes
### `CgcCodeLensProvider`
- def: [`extensions/vscode/src/providers/editorProviders.ts:35`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L35)
- signature: `class CgcCodeLensProvider`
- members:
  - `<constructor>(service: CgcService)` — [`L39`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L39) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `invalidate(method)` — [`L114`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L114)
  - `provideCodeLenses(method)` — [`L41`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L41)
  - `onDidChangeCodeLenses` — [`L37`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L37)
- protocol/private: `_fetchAll`[`L86`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L86), `_fetchingDocs`[`L84`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L84), `_onDidChange`[`L36`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L36)
- uses (calls/refs, reference-scoped): [`CgcService`](../mcp/service.ts.md#CgcService), [`findCallers`](../mcp/service.ts.md#CgcService.findCallers), [`findCallees`](../mcp/service.ts.md#CgcService.findCallees), [`symbol`](editorProviders.ts.md#collectDefinitionLines.Array.typeLiteral4.symbol), [`getComplexity`](../mcp/service.ts.md#CgcService.getComplexity), [`collectDefinitionLines`](editorProviders.ts.md#collectDefinitionLines), [`lensCache`](editorProviders.ts.md#lensCache), [`line`](editorProviders.ts.md#collectDefinitionLines.Array.typeLiteral4.line), [`type`](editorProviders.ts.md#collectDefinitionLines.Array.typeLiteral4.type)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts)

### `CgcDeadCodeCodeActionProvider`
- def: [`extensions/vscode/src/providers/editorProviders.ts:250`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L250)
- signature: `class CgcDeadCodeCodeActionProvider`
- members:
  - `provideCodeActions(method)` — [`L253`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L253)
  - `providedCodeActionKinds` — [`L251`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L251)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts)

### `CgcDeadCodeDiagnostics`
- def: [`extensions/vscode/src/providers/editorProviders.ts:196`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L196)
- signature: `class CgcDeadCodeDiagnostics`
- members:
  - `<constructor>(service: CgcService)` — [`L204`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L204) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `dispose(method)` — [`L206`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L206)
  - `refreshForDocument(method)` — [`L211`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L211)
  - `collection` — [`L197`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L197)
  - `index` — [`L202`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L202) — documented in [extensions-vscode-src-types-cgc.ts](../../../../../concepts/extensions-vscode-src-types-cgc.ts.md)
  - `strikeDecoration` — [`L198`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L198)
- uses (calls/refs, reference-scoped): [`CgcService`](../mcp/service.ts.md#CgcService), [`findDeadCode`](../mcp/service.ts.md#CgcService.findDeadCode), [`DeadCodeEntry`](../types/cgc.ts.md#DeadCodeEntry), [`line_number`](../types/cgc.ts.md#DeadCodeEntry.line_number), [`class_name`](../types/cgc.ts.md#DeadCodeEntry.class_name), [`function_name`](../types/cgc.ts.md#DeadCodeEntry.function_name), [`path`](../types/cgc.ts.md#DeadCodeEntry.path)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts)

### `CgcHoverProvider`
- def: [`extensions/vscode/src/providers/editorProviders.ts:123`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L123)
- signature: `class CgcHoverProvider`
- members:
  - `<constructor>(service: CgcService)` — [`L124`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L124) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
  - `provideHover(method)` — [`L126`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L126) — documented in [extensions-vscode-src-mcp-service.ts](../../../../../concepts/extensions-vscode-src-mcp-service.ts.md)
- uses (calls/refs, reference-scoped): [`CgcService`](../mcp/service.ts.md#CgcService), [`findCallers`](../mcp/service.ts.md#CgcService.findCallers), [`findCallees`](../mcp/service.ts.md#CgcService.findCallees), [`getComplexity`](../mcp/service.ts.md#CgcService.getComplexity), [`symbolAtPosition`](editorProviders.ts.md#symbolAtPosition)
- used by: [`activate`](../extension.ts.md#activate), [`extension.ts`](../extension.ts.md#scip-typescript-npm-codegraphcontext-vscode-0.1.0-src-extension.ts)

## Functions
- `collectDefinitionLines(document: vscode.TextDocument)` — [`L15`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L15)
- `symbolAtPosition(document: vscode.TextDocument, position: vscode.Position)` — [`L10`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L10)

## Module values
- `DEF_PATTERN` — [`L7`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L7)
- `lensCache` — [`L33`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L33)
- `line` — [`L15`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L15)
- `symbol` — [`L15`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L15)
- `type` — [`L15`](../../../../../../../../raw/code/codegraphcontext/extensions/vscode/src/providers/editorProviders.ts#L15)

