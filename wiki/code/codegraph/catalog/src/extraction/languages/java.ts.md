---
title: 'Module: src/extraction/languages/java.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/java.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`java.ts`/
symbols:
  synthesizeLombokMembers: synthesizeLombokMembers().
  lombokAnnotationNames: lombokAnnotationNames().
  normalizeJavaType: normalizeJavaType().
  modifierTextOf: modifierTextOf().
  extractJavaReturnType: extractJavaReturnType().
  lombokGetterName: lombokGetterName().
  lombokSetterName: lombokSetterName().
  capitalizeJava: capitalizeJava().
  javaExtractor: javaExtractor.
  JAVA_NON_CLASS_RETURN_NODES: JAVA_NON_CLASS_RETURN_NODES.
  LOMBOK_LOG_ANNOTATIONS: LOMBOK_LOG_ANNOTATIONS.
---
# Module: [`src/extraction/languages/java.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts)

## Functions
- `capitalizeJava(name: string)` — [`L79`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L79)
- `extractJavaReturnType(node: Node, source: string)` — [`L41`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L41) — A Java method's declared return type. Reads the `type` field; constructors
- `lombokAnnotationNames(node: Node)` — [`L59`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L59) — Simple names of every annotation in a node's `modifiers` child (`@lombok.Getter` → `Getter`).
- `lombokGetterName(fieldName: string, isBooleanPrimitive: boolean)` — [`L84`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L84) — Lombok getter name: `getX`, or `isX` for a primitive boolean (keeping an existing `isFoo` field name).
- `lombokSetterName(fieldName: string, isBooleanPrimitive: boolean)` — [`L92`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L92) — Lombok setter name: `setX` (a primitive boolean field `isFoo` sets via `setFoo`).
- `modifierTextOf(node: Node)` — [`L74`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L74) — Text of a declaration's `modifiers` child (keyword modifiers are anonymous, so match on text).
- `normalizeJavaType(typeNode: Node | null, source: string)` — [`L24`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L24) — Normalize a Java type node to the bare class name a chained
- `synthesizeLombokMembers(classNode: Node, ctx: ExtractorContext)` — [`L118`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L118) — Synthesize the members Lombok generates at compile time. Covers the common, — documented in [extraction-tree-sitter-types.ts](../../../../concepts/extraction-tree-sitter-types.ts.md)

## Module values
- `JAVA_NON_CLASS_RETURN_NODES` — [`L10`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L10) — Tree-sitter-java node types for a method's `type` (return) field that can
- `LOMBOK_LOG_ANNOTATIONS` — [`L54`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L54) — Lombok logging annotations — all generate a field named `log` by default.
- `javaExtractor` — [`L253`](../../../../../../../raw/code/codegraph/src/extraction/languages/java.ts#L253)

