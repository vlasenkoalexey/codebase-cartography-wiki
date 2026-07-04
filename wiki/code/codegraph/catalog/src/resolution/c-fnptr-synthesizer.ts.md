---
title: 'Module: src/resolution/c-fnptr-synthesizer.ts'
type: catalog
provenance: extracted
module: src/resolution/c-fnptr-synthesizer.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`c-fnptr-synthesizer.ts`/
symbols:
  cFnPointerDispatchEdges: cFnPointerDispatchEdges().
  MacroDef: MacroDef#
  expandMacroCalls: expandMacroCalls().
  parseFunctionMacros: parseFunctionMacros().
  substituteMacro: substituteMacro().
  iterateFns: iterateFns().
  FieldInfo.name: FieldInfo#name.
  matchBrace: matchBrace().
  FieldInfo.isFnPtr: FieldInfo#isFnPtr.
  splitTopLevel: splitTopLevel().
  FANOUT_CAP: FANOUT_CAP.
  FieldInfo: FieldInfo#
  C_CPP_EXT: C_CPP_EXT.
  FieldInfo.type: FieldInfo#type.
  sliceLines: sliceLines().
  FieldInfo.index: FieldInfo#index.
  MacroDef.params: MacroDef#params.
  MacroDef.expansion: MacroDef#expansion.
  parseObjectMacros: parseObjectMacros().
  FNPTR_TYPEDEF_RE: FNPTR_TYPEDEF_RE.
  FNTYPE_TYPEDEF_STMT_RE: FNTYPE_TYPEDEF_STMT_RE.
  C_TYPE_KEYWORDS: C_TYPE_KEYWORDS.
  INCLUDE_RE: INCLUDE_RE.
  FN_KINDS: FN_KINDS.
  matchParen: matchParen().
  parseDefinedNames: parseDefinedNames().
  evalConditionals: evalConditionals().
  resolveTypeName: resolveTypeName().
  FNPTR_DECL_RE: FNPTR_DECL_RE.
  INCLUDABLE_EXT: INCLUDABLE_EXT.
---
# Module: [`src/resolution/c-fnptr-synthesizer.ts`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts)

## Classes
### `FieldInfo`
- def: [`src/resolution/c-fnptr-synthesizer.ts:62`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L62)
- doc: A struct field, in declaration order, flagged when it is a function pointer.
- signature: `interface FieldInfo`
- members:
  - `index` — [`L64`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L64)
  - `isFnPtr` — [`L65`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L65)
  - `name` — [`L63`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L63)
  - `type` — [`L68`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L68) — The field's declared type token (e.g. `redisCommand` for `struct redisCommand *cmd`),
- used by: [`cFnPointerDispatchEdges`](c-fnptr-synthesizer.ts.md#cFnPointerDispatchEdges)

### `MacroDef`
- def: [`src/resolution/c-fnptr-synthesizer.ts:123`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L123)
- doc: A function-like macro: `#define NAME(p0,p1,…) expansion`.
- signature: `interface MacroDef`
- members:
  - `expansion` — [`L125`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L125)
  - `params` — [`L124`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L124)
- used by: [`cFnPointerDispatchEdges`](c-fnptr-synthesizer.ts.md#cFnPointerDispatchEdges), [`expandMacroCalls`](c-fnptr-synthesizer.ts.md#expandMacroCalls), [`parseFunctionMacros`](c-fnptr-synthesizer.ts.md#parseFunctionMacros), [`substituteMacro`](c-fnptr-synthesizer.ts.md#substituteMacro)

## Functions
- `cFnPointerDispatchEdges(queries: QueryBuilder, ctx: ResolutionContext)` — [`L309`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L309) — documented in [index.ts](../../../concepts/index.ts.md)
- `evalConditionals(text: string, defined: Set<string>)` — [`L181`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L181) — Drop the inactive arms of `#ifdef`/`#ifndef`/`#if defined(X)`/`#else`/`#elif`/
- `expandMacroCalls(text: string, env: Map<string, MacroDef>)` — [`L266`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L266) — Expand known function-like macro calls in `text` to a fixpoint (depth-capped).
- `iterateFns(queries: QueryBuilder)` — [`L964`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L964) — C/C++ function + method nodes, streamed (memory-safe on symbol-dense repos).
- `matchBrace(src: string, open: number)` — [`L77`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L77) — Index of the `}` matching the `{` at `open` (which must point at a `{`). -1 if unbalanced.
- `matchParen(src: string, open: number)` — [`L109`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L109) — Index of the `)` matching the `(` at `open` (which must point at a `(`). -1 if unbalanced.
- `parseDefinedNames(stripped: string)` — [`L164`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L164) — All macro names a file `#define`s (value-ful or not) — the "defined" set for #ifdef.
- `parseFunctionMacros(stripped: string)` — [`L134`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L134) — Collect function-like macros from (comment-stripped) source, joining
- `parseObjectMacros(stripped: string)` — [`L153`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L153) — Collect object-like macros `#define NAME value` (NAME not immediately followed
- `resolveTypeName(name: string, objEnv: Map<string, string> | undefined)` — [`L242`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L242) — Resolve a type token through object-like macro aliases (transitive, capped).
- `sliceLines(content: string, startLine?: number | undefined, endLine?: number | undefined)` — [`L71`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L71)
- `splitTopLevel(body: string, sep: string)` — [`L91`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L91) — Split `body` on `sep` at brace/paren/bracket depth 0 (commas inside `{…}` / `(…)` stay together).
- `substituteMacro(def: MacroDef, args: string[])` — [`L254`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L254) — Substitute call args for the macro's params (whole-token) in its expansion.

## Module values
- `C_CPP_EXT` — [`L57`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L57)
- `C_TYPE_KEYWORDS` — [`L300`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L300) — Return-type keywords that must never be mistaken for the typedef's name.
- `FANOUT_CAP` — [`L59`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L59)
- `FNPTR_DECL_RE` — [`L292`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L292) — A fn-pointer field looks like `… (*name)(…)` — capture `name`. A
- `FNPTR_TYPEDEF_RE` — [`L295`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L295) — `typedef RET (*NAME)(…)` — a function-pointer typedef (CC/attr macro before
- `FNTYPE_TYPEDEF_STMT_RE` — [`L298`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L298) — A whole brace-free `typedef … ;` statement — capture the guts to spot the
- `FN_KINDS` — [`L58`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L58)
- `INCLUDABLE_EXT` — [`L307`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L307) — Included files worth scanning for registration tables (e.g. a generated `.def`).
- `INCLUDE_RE` — [`L305`](../../../../../../raw/code/codegraph/src/resolution/c-fnptr-synthesizer.ts#L305) — `#include "local/header"` — captured from RAW source (string contents survive).

