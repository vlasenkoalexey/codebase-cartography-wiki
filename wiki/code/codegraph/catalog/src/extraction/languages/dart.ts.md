---
title: 'Module: src/extraction/languages/dart.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/dart.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`dart.ts`/
symbols:
  dartCtorInfo: dartCtorInfo().
  extractDartReturnType: extractDartReturnType().
  dartEnclosingTypeName: dartEnclosingTypeName().
  dartCalleeOfArgPart: dartCalleeOfArgPart().
  dartInnerSignature: dartInnerSignature().
  dartConstructorSignature: dartConstructorSignature().
  dartExtractor: dartExtractor.
---
# Module: [`src/extraction/languages/dart.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/dart.ts)

## Functions
- `dartCalleeOfArgPart(argPart: Node)` — [`L100`](../../../../../../../raw/code/codegraph/src/extraction/languages/dart.ts#L100) — The callee name of the Dart call whose `argument_part` selector is `argPart`
- `dartConstructorSignature(node: Node)` — [`L25`](../../../../../../../raw/code/codegraph/src/extraction/languages/dart.ts#L25) — The factory/named-constructor signature inside a node, if any. A constructor
- `dartCtorInfo(node: Node)` — [`L61`](../../../../../../../raw/code/codegraph/src/extraction/languages/dart.ts#L61) — Validated constructor info for `node`, or undefined if it isn't genuinely a
- `dartEnclosingTypeName(node: Node)` — [`L38`](../../../../../../../raw/code/codegraph/src/extraction/languages/dart.ts#L38) — The name of the class/mixin/extension/enum lexically enclosing `node`.
- `dartInnerSignature(node: Node)` — [`L9`](../../../../../../../raw/code/codegraph/src/extraction/languages/dart.ts#L9) — The `function_signature` carrying a method's return type — unwrapped from a
- `extractDartReturnType(node: Node, source: string)` — [`L80`](../../../../../../../raw/code/codegraph/src/extraction/languages/dart.ts#L80) — Capture a Dart method/function's declared return type as a bare type name, for

## Module values
- `dartExtractor` — [`L118`](../../../../../../../raw/code/codegraph/src/extraction/languages/dart.ts#L118)

