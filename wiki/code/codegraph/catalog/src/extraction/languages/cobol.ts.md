---
title: 'Module: src/extraction/languages/cobol.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/cobol.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`cobol.ts`/
symbols:
  walkDataEntries: walkDataEntries().
  walkProcedureChildren: walkProcedureChildren().
  addRef: addRef().
  collectRefs: collectRefs().
  handleExec: handleExec().
  handleCopy: handleCopy().
  emitWriteRefs: emitWriteRefs().
  derefSameFileValue: derefSameFileValue().
  endLineOf: endLineOf().
  targetBaseName: targetBaseName().
  programName: programName().
  currentScope: currentScope().
  line: line().
  headerName: headerName().
  collapse: collapse().
  terminateSqlIncludes: terminateSqlIncludes().
  cobolExtractor: cobolExtractor.
  EXEC_CICS_PROGRAM_RE: EXEC_CICS_PROGRAM_RE.
  EXEC_CICS_TRANSID_RE: EXEC_CICS_TRANSID_RE.
  EXEC_SQL_INCLUDE_RE: EXEC_SQL_INCLUDE_RE.
  VALUE_LITERAL_RE: VALUE_LITERAL_RE.
  SPECIAL_REGISTER_RE: SPECIAL_REGISTER_RE.
---
# Module: [`src/extraction/languages/cobol.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts)

## Functions
- `addRef(ctx: ExtractorContext, fromNodeId: string | undefined, referenceName: string, referenceKind: "calls" | "imports" | "references", at: Node)` — [`L86`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L86)
- `collapse(text: string, cap?: number)` — [`L56`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L56) — Collapse whitespace runs so multi-line clauses read as one signature.
- `collectRefs(node: Node, fromNodeId: string | undefined, ctx: ExtractorContext)` — [`L302`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L302) — Collect call/import references from a statement subtree, attributed to the — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `currentScope(ctx: ExtractorContext)` — [`L61`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L61)
- `derefSameFileValue(name: string, ctx: ExtractorContext)` — [`L125`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L125) — A CICS option can name its target through a data item instead of a
- `emitWriteRefs(statement: Node, fields: string[], fromNodeId: string | undefined, ctx: ExtractorContext)` — [`L280`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L280) — Emit a `references` ref for every data item a statement WRITES (MOVE TO,
- `endLineOf(node: Node)` — [`L51`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L51)
- `handleCopy(node: Node, ctx: ExtractorContext)` — [`L104`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L104) — COPY <book> [IN/OF lib] — import node + imports reference.
- `handleExec(node: Node, ctx: ExtractorContext, fromNodeId: string | undefined)` — [`L144`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L144) — EXEC ... END-EXEC blocks are opaque single nodes. Mine the text for the
- `headerName(header: Node, source: string)` — [`L366`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L366) — "PARA-NAME." → "PARA-NAME"; "SEC-NAME SECTION." → "SEC-NAME".
- `line(node: Node)` — [`L47`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L47)
- `programName(programNode: Node, source: string)` — [`L425`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L425) — Program name from identification_division > program_name.
- `targetBaseName(target: Node, source: string)` — [`L262`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L262) — The base data name of an assignment target (first WORD, ignoring subscripts/OF-qualifiers).
- `terminateSqlIncludes(source: string)` — [`L72`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L72) — DB2 convention writes `EXEC SQL INCLUDE member END-EXEC` with no sentence
- `walkDataEntries(entries: Node[], ctx: ExtractorContext)` — [`L177`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L177) — Walk a run of DATA DIVISION entries (working-storage section children or a — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `walkProcedureChildren(children: Node[], divisionEndLine: number, ctx: ExtractorContext)` — [`L376`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L376) — Walk the flat PROCEDURE DIVISION (or a procedure copybook fragment): — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)

## Module values
- `EXEC_CICS_PROGRAM_RE` — [`L37`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L37) — EXEC CICS LINK/XCTL — program target, quoted literal or data name.
- `EXEC_CICS_TRANSID_RE` — [`L40`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L40) — EXEC CICS RETURN/START — next transaction, quoted literal or data name.
- `EXEC_SQL_INCLUDE_RE` — [`L43`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L43) — EXEC SQL INCLUDE <member> — the SQL flavor of COPY.
- `SPECIAL_REGISTER_RE` — [`L259`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L259) — Special registers and CICS/SQL communication areas — writes to these are
- `VALUE_LITERAL_RE` — [`L45`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L45) — The VALUE literal in a data item's signature ("PIC X(04) VALUE 'CB00'").
- `cobolExtractor` — [`L434`](../../../../../../../raw/code/codegraph/src/extraction/languages/cobol.ts#L434)

