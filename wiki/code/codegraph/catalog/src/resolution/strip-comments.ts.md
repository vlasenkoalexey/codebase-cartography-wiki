---
title: 'Module: src/resolution/strip-comments.ts'
type: catalog
provenance: extracted
module: src/resolution/strip-comments.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`strip-comments.ts`/
symbols:
  stripCommentsForRegex: stripCommentsForRegex().
  blankRange: blankRange().
  stripPython: stripPython().
  stripRuby: stripRuby().
  stripCStyle: stripCStyle().
  stripPhp: stripPhp().
  stripGo: stripGo().
  stripRust: stripRust().
  stripErlang: stripErlang().
  CommentLang: CommentLang#
---
# Module: [`src/resolution/strip-comments.ts`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts)

## Classes
### `CommentLang`
- def: [`src/resolution/strip-comments.ts:26`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts#L26)
- doc: Per-language comment stripper for framework route extractors.
- signature: `type CommentLang`
- used by: [`stripCommentsForRegex`](strip-comments.ts.md#stripCommentsForRegex), [`dynamic-boundaries.ts`](../mcp/dynamic-boundaries.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-mcp-dynamic-boundaries.ts), [`commentLang`](../mcp/dynamic-boundaries.ts.md#commentLang)

## Functions
- `blankRange(buf: string[], start: number, end: number, src: string)` — [`L72`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts#L72) — Replace every char in a slice with spaces, but keep newlines so line
- `stripCStyle(src: string, allowSingleQuoteStrings: boolean)` — [`L220`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts#L220)
- `stripCommentsForRegex(content: string, lang: CommentLang)` — [`L41`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts#L41) — documented in [mcp-tools.ts](../../../concepts/mcp-tools.ts.md)
- `stripErlang(src: string)` — [`L486`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts#L486) — Erlang: `%` starts a line comment unless it sits inside a `"string"`, a
- `stripGo(src: string)` — [`L332`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts#L332)
- `stripPhp(src: string)` — [`L272`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts#L272)
- `stripPython(src: string)` — [`L80`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts#L80)
- `stripRuby(src: string)` — [`L142`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts#L142)
- `stripRust(src: string)` — [`L405`](../../../../../../raw/code/codegraph/src/resolution/strip-comments.ts#L405)

