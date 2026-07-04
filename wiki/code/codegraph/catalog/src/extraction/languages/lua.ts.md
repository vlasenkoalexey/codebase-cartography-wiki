---
title: 'Module: src/extraction/languages/lua.ts'
type: catalog
provenance: extracted
module: src/extraction/languages/lua.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/languages/`lua.ts`/
symbols:
  requireModule: requireModule().
  findDescendant: findDescendant().
  luaExtractor: luaExtractor.
---
# Module: [`src/extraction/languages/lua.ts`](../../../../../../../raw/code/codegraph/src/extraction/languages/lua.ts)

## Functions
- `findDescendant(node: Node, type: string)` — [`L9`](../../../../../../../raw/code/codegraph/src/extraction/languages/lua.ts#L9) — First descendant of a given type (breadth-first), or null.
- `requireModule(callNode: Node, source: string)` — [`L28`](../../../../../../../raw/code/codegraph/src/extraction/languages/lua.ts#L28) — If `callNode` is a `require(...)` call, return the module name; otherwise null.

## Module values
- `luaExtractor` — [`L62`](../../../../../../../raw/code/codegraph/src/extraction/languages/lua.ts#L62)

