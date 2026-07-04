---
title: 'Module: src/extraction/languages/objc.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/objc.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`objc.ts`/
symbols:
  collectTypeIdentifiers: collectTypeIdentifiers().
  extractObjcReturnType: extractObjcReturnType().
  extractObjcPropertyName: extractObjcPropertyName().
  findCompoundStatement: findCompoundStatement().
  extractObjcMethodName: extractObjcMethodName().
  objcExtractor: objcExtractor.
  OBJC_TYPE_QUALIFIERS: OBJC_TYPE_QUALIFIERS.
---
# Module: [`src/extraction/languages/objc.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/objc.ts)

## Functions
- `collectTypeIdentifiers(node: Node, source: string, out: string[])` — [`L44`](../../../../../../../raw/code/codegraph/src/extraction/languages/objc.ts#L44) — Collect the type identifiers under a `method_type`, in document order.
- `extractObjcMethodName(node: Node, source: string)` — [`L16`](../../../../../../../raw/code/codegraph/src/extraction/languages/objc.ts#L16) — Build ObjC selector: `greet`, `doThing:`, or `doThing:with:`.
- `extractObjcPropertyName(node: Node, source: string)` — [`L74`](../../../../../../../raw/code/codegraph/src/extraction/languages/objc.ts#L74)
- `extractObjcReturnType(node: Node, source: string)` — [`L61`](../../../../../../../raw/code/codegraph/src/extraction/languages/objc.ts#L61) — Capture an ObjC method's declared return type as a bare class name, for the
- `findCompoundStatement(node: Node)` — [`L5`](../../../../../../../raw/code/codegraph/src/extraction/languages/objc.ts#L5)

## Module values
- `OBJC_TYPE_QUALIFIERS` — [`L36`](../../../../../../../raw/code/codegraph/src/extraction/languages/objc.ts#L36) — Nullability / ARC qualifiers that sit where a return type's first type
- `objcExtractor` — [`L98`](../../../../../../../raw/code/codegraph/src/extraction/languages/objc.ts#L98)

