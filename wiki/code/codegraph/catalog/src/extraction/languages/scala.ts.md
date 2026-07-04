---
title: 'Module: src/extraction/languages/scala.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/scala.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`scala.ts`/
symbols:
  emitScalaTypeRefs: emitScalaTypeRefs().
  extractVisibility: extractVisibility().
  getValVarName: getValVarName().
  extractScalaReturnType: extractScalaReturnType().
  scalaExtractor: scalaExtractor.
  SCALA_BUILTIN_TYPES: SCALA_BUILTIN_TYPES.
  emitScalaTypeRefs.ctx-typeLiteral9.addUnresolvedReference: emitScalaTypeRefs().(ctx)typeLiteral9:addUnresolvedReference.
---
# Module: [`src/extraction/languages/scala.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/scala.ts)

## Functions
- `emitScalaTypeRefs(typeNode: Node, fromId: string, ctx: { addUnresolvedReference: (r: { fromNodeId: string; referenceName: string; referenceKind: "references"; line: number; column: number; }) => void; }, source: string)` — [`L27`](../../../../../../../raw/code/codegraph/src/extraction/languages/scala.ts#L27) — Emit `references` edges for every type identifier in a Scala type subtree
- `extractScalaReturnType(node: Node, source: string)` — [`L56`](../../../../../../../raw/code/codegraph/src/extraction/languages/scala.ts#L56) — Capture a Scala method's declared return type as a bare type name, for the
- `extractVisibility(node: Node)` — [`L69`](../../../../../../../raw/code/codegraph/src/extraction/languages/scala.ts#L69)
- `getValVarName(node: Node, source: string)` — [`L5`](../../../../../../../raw/code/codegraph/src/extraction/languages/scala.ts#L5)

## Module values
- `SCALA_BUILTIN_TYPES` — [`L14`](../../../../../../../raw/code/codegraph/src/extraction/languages/scala.ts#L14)
- `addUnresolvedReference` — [`L27`](../../../../../../../raw/code/codegraph/src/extraction/languages/scala.ts#L27)
- `scalaExtractor` — [`L82`](../../../../../../../raw/code/codegraph/src/extraction/languages/scala.ts#L82)

