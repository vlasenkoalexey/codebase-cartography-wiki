---
title: 'Module: src/search/query-parser.ts'
type: catalog
provenance: extracted
module: src/search/query-parser.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/search/`query-parser.ts`/
symbols:
  parseQuery: parseQuery().
  ParsedQuery.kinds: ParsedQuery#kinds.
  ParsedQuery.languages: ParsedQuery#languages.
  KIND_VALUES: KIND_VALUES.
  LANGUAGE_VALUES: LANGUAGE_VALUES.
  ParsedQuery.text: ParsedQuery#text.
  ParsedQuery.pathFilters: ParsedQuery#pathFilters.
  ParsedQuery.nameFilters: ParsedQuery#nameFilters.
  ParsedQuery: ParsedQuery#
  boundedEditDistance: boundedEditDistance().
  unquote: unquote().
---
# Module: [`src/search/query-parser.ts`](../../../../../../raw/code/codegraph/src/search/query-parser.ts)

## Classes
### `ParsedQuery`
- def: [`src/search/query-parser.ts:34`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L34)
- signature: `interface ParsedQuery`
- members:
  - `kinds` — [`L38`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L38) — kind: filters (OR'd). Empty when none specified.
  - `languages` — [`L40`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L40) — lang:/language: filters (OR'd). Empty when none specified.
  - `nameFilters` — [`L44`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L44) — name: filters (OR'd, case-insensitive substring of node.name).
  - `pathFilters` — [`L42`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L42) — path: filters (OR'd, case-insensitive substring of file_path). Empty when none.
  - `text` — [`L36`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L36) — Free-text portion to feed to FTS / LIKE. May be empty.
- uses (calls/refs, reference-scoped): [`Language`](../types.ts.md#Language), [`NodeKind`](../types.ts.md#NodeKind)
- used by: [`searchNodes`](../db/queries.ts.md#QueryBuilder.searchNodes), [`parseQuery`](query-parser.ts.md#parseQuery)

## Functions
- `boundedEditDistance(a: string, b: string, maxDist: number)` — [`L157`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L157) — Damerau-Levenshtein-ish bounded edit distance. Returns `maxDist + 1`
- `parseQuery(raw: string)` — [`L66`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L66) — Parse a raw query into structured filters + remaining text. — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
- `unquote(s: string)` — [`L57`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L57) — Strip a surrounding pair of double quotes from `s`. Allows users to

## Module values
- `KIND_VALUES` — [`L50`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L50)
- `LANGUAGE_VALUES` — [`L51`](../../../../../../raw/code/codegraph/src/search/query-parser.ts#L51)

