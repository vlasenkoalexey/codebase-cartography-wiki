---
title: 'Module: src/extraction/languages/kotlin.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/kotlin.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`kotlin.ts`/
symbols:
  isFunInterfaceNode: isFunInterfaceNode().
  extractKotlinReturnType: extractKotlinReturnType().
  kotlinExtractor: kotlinExtractor.
  KOTLIN_NON_CLASS_RETURN: KOTLIN_NON_CLASS_RETURN.
---
# Module: [`src/extraction/languages/kotlin.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/kotlin.ts)

## Functions
- `extractKotlinReturnType(node: Node, source: string)` — [`L17`](../../../../../../../raw/code/codegraph/src/extraction/languages/kotlin.ts#L17) — A Kotlin function's declared return type, normalized to the bare class name a
- `isFunInterfaceNode(node: Node)` — [`L46`](../../../../../../../raw/code/codegraph/src/extraction/languages/kotlin.ts#L46) — Check if a node matches the `fun interface` misparse pattern

## Module values
- `KOTLIN_NON_CLASS_RETURN` — [`L6`](../../../../../../../raw/code/codegraph/src/extraction/languages/kotlin.ts#L6) — Kotlin return types that can't be a chained-call receiver (no class to chain on).
- `kotlinExtractor` — [`L71`](../../../../../../../raw/code/codegraph/src/extraction/languages/kotlin.ts#L71)

