---
title: 'Module: src/extraction/languages/r.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/r.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`r.ts`/
symbols:
  extractClassMembers: extractClassMembers().
  emitMethodArg: emitMethodArg().
  literalOrIdentifier: literalOrIdentifier().
  firstArgValue: firstArgValue().
  calleeName: calleeName().
  ASSIGN_LEFT: ASSIGN_LEFT.
  CLASS_FNS: CLASS_FNS.
  GENERIC_FNS: GENERIC_FNS.
  CONSTANT_NAME: CONSTANT_NAME.
  rExtractor: rExtractor.
  ASSIGN_RIGHT: ASSIGN_RIGHT.
  IMPORT_FNS: IMPORT_FNS.
---
# Module: [`src/extraction/languages/r.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts)

## Functions
- `calleeName(call: Node, source: string)` — [`L46`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L46) — The call's callee name when it is a bare identifier or `pkg::fn` (→ `fn`).
- `emitMethodArg(entry: Node, ctx: ExtractorContext)` — [`L84`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L84) — Emit one `name = function(…)` argument entry as a method in the current scope.
- `extractClassMembers(classCall: Node, classId: string, ctx: ExtractorContext)` — [`L110`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L110) — Extract a class call's methods. Two shapes: — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)
- `firstArgValue(call: Node)` — [`L58`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L58) — First positional argument's value node of a call.
- `literalOrIdentifier(node: Node | null, source: string)` — [`L70`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L70) — Text of a string node's content, or an identifier's text.

## Module values
- `ASSIGN_LEFT` — [`L37`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L37) — R language extractor (#828).
- `ASSIGN_RIGHT` — [`L38`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L38)
- `CLASS_FNS` — [`L40`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L40)
- `CONSTANT_NAME` — [`L43`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L43) — ALL_CAPS or DOTTED.CAPS top-level assignment → constant.
- `GENERIC_FNS` — [`L41`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L41)
- `IMPORT_FNS` — [`L39`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L39)
- `rExtractor` — [`L165`](../../../../../../../raw/code/codegraph/src/extraction/languages/r.ts#L165)

