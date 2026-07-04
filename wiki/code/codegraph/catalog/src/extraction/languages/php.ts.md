---
title: 'Module: src/extraction/languages/php.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/php.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`php.ts`/
symbols:
  extractPhpReturnType: extractPhpReturnType().
  phpStaticIncludePath: phpStaticIncludePath().
  PHP_INCLUDE_TYPES: PHP_INCLUDE_TYPES.
  phpExtractor: phpExtractor.
  PHP_NON_CLASS_RETURN: PHP_NON_CLASS_RETURN.
---
# Module: [`src/extraction/languages/php.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/php.ts)

## Functions
- `extractPhpReturnType(node: Node, source: string)` — [`L50`](../../../../../../../raw/code/codegraph/src/extraction/languages/php.ts#L50) — A method/function's declared return type, normalized to the class a chained
- `phpStaticIncludePath(node: Node, source: string)` — [`L22`](../../../../../../../raw/code/codegraph/src/extraction/languages/php.ts#L22) — Extract a static string-literal path from a PHP include/require expression.

## Module values
- `PHP_INCLUDE_TYPES` — [`L8`](../../../../../../../raw/code/codegraph/src/extraction/languages/php.ts#L8)
- `PHP_NON_CLASS_RETURN` — [`L37`](../../../../../../../raw/code/codegraph/src/extraction/languages/php.ts#L37) — PHP built-in return types that can't be a method receiver (so no class to chain on).
- `phpExtractor` — [`L68`](../../../../../../../raw/code/codegraph/src/extraction/languages/php.ts#L68)

