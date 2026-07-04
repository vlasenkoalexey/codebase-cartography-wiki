---
title: 'Module: src/extraction/languages/erlang.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/erlang.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`erlang.ts`/
symbols:
  handleFunDecl: handleFunDecl().
  handleAppResourceTuple: handleAppResourceTuple().
  handleBehaviour: handleBehaviour().
  handleRecordDecl: handleRecordDecl().
  moduleExports: moduleExports().
  handlePpDefine: handlePpDefine().
  handleTypeAlias: handleTypeAlias().
  atomText: atomText().
  precedingSpec: precedingSpec().
  clauseHeader: clauseHeader().
  collapseWs: collapseWs().
  lastFnId: lastFnId.
  exportsFile: exportsFile.
  exportsMemo: exportsMemo.
  lastFnFile: lastFnFile.
  lastFnName: lastFnName.
  erlangExtractor: erlangExtractor.
---
# Module: [`src/extraction/languages/erlang.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts)

## Functions
- `atomText(node: Node, source: string)` — [`L27`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L27) — Text of an atom with quoted-atom quotes stripped (`'EXIT'` → `EXIT`).
- `clauseHeader(clause: Node, source: string)` — [`L93`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L93) — `name(Args) when Guard` — the clause text up to the `->`.
- `collapseWs(text: string)` — [`L31`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L31)
- `handleAppResourceTuple(node: Node, ctx: ExtractorContext)` — [`L226`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L226) — OTP application resource file (`<app>.app.src` / `<app>.app`): a single — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `handleBehaviour(node: Node, ctx: ExtractorContext)` — [`L198`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L198) — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `handleFunDecl(node: Node, ctx: ExtractorContext)` — [`L99`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L99) — documented in [extraction-tree-sitter-helpers.ts](../../../../concepts/extraction-tree-sitter-helpers.ts.md)
- `handlePpDefine(node: Node, ctx: ExtractorContext)` — [`L175`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L175)
- `handleRecordDecl(node: Node, ctx: ExtractorContext)` — [`L145`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L145) — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `handleTypeAlias(node: Node, ctx: ExtractorContext)` — [`L164`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L164)
- `moduleExports(node: Node, source: string, filePath: string)` — [`L53`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L53)
- `precedingSpec(node: Node, name: string, source: string)` — [`L82`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L82) — The -spec directly above a function (comments may sit between), if it names it.

## Module values
- `erlangExtractor` — [`L262`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L262)
- `exportsFile` — [`L39`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L39) — Exported function names for the current file ('all' for -compile(export_all)).
- `exportsMemo` — [`L40`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L40)
- `lastFnFile` — [`L49`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L49) — Clause-merge state: the previous fun_decl's name and node id. A fun_decl
- `lastFnId` — [`L51`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L51)
- `lastFnName` — [`L50`](../../../../../../../raw/code/codegraph/src/extraction/languages/erlang.ts#L50)

