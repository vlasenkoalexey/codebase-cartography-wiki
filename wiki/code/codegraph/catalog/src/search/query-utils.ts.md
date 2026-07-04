---
title: 'Module: src/search/query-utils.ts'
type: catalog
provenance: extracted
module: src/search/query-utils.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/search/`query-utils.ts`/
symbols:
  extractSearchTerms: extractSearchTerms().
  scorePathRelevance: scorePathRelevance().
  isTestFile: isTestFile().
  kindBonus: kindBonus().
  deriveProjectNameTokens: deriveProjectNameTokens().
  normalizeNameToken: normalizeNameToken().
  getStemVariants: getStemVariants().
  isDistinctiveIdentifier: isDistinctiveIdentifier().
  STOP_WORDS: STOP_WORDS.
  nameMatchBonus: nameMatchBonus().
  extractSearchTerms.options-typeLiteral38.stems: extractSearchTerms().(options)typeLiteral38:stems.
  matchesNonProductionDir: matchesNonProductionDir().
---
# Module: [`src/search/query-utils.ts`](../../../../../../raw/code/codegraph/src/search/query-utils.ts)

## Functions
- `deriveProjectNameTokens(projectRoot: string)` — [`L29`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L29) — Tokens that name the PROJECT as a whole — its `go.mod` module, `package.json`
- `extractSearchTerms(query: string, options?: { stems?: boolean | undefined; } | undefined)` — [`L156`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L156) — Extract meaningful search terms from a natural language query.
- `getStemVariants(term: string)` — [`L85`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L85) — Generate stem variants of a search term by removing common English suffixes.
- `isDistinctiveIdentifier(token: string)` — [`L433`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L433) — Whether a query token looks like a code identifier the user deliberately typed
- `isTestFile(filePath: string)` — [`L280`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L280) — Check if a file path looks like a test file
- `kindBonus(kind: "function" | "file" | "module" | "class" | "struct" | "interface" | "trait" | "protocol" | "method" | "property" | "field" | "variable" | "constant" | "enum" | "enum_member" | ... 6 more ... | "component")` — [`L388`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L388) — Kind-based bonus for search ranking
- `matchesNonProductionDir(lowerPath: string)` — [`L325`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L325) — Check if a path is in a non-production directory (integration, sample, example, etc.)
- `nameMatchBonus(nodeName: string, query: string)` — [`L343`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L343) — Bonus when a node's name matches the search query.
- `normalizeNameToken(raw: string)` — [`L12`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L12) — Normalize a name to a comparable token: lowercase, alphanumerics only.
- `scorePathRelevance(filePath: string, query: string, projectNameTokens?: Set<string> | undefined)` — [`L221`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L221) — Score path relevance to a query

## Module values
- `STOP_WORDS` — [`L60`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L60) — Common stop words to filter from search queries.
- `stems` — [`L156`](../../../../../../raw/code/codegraph/src/search/query-utils.ts#L156)

