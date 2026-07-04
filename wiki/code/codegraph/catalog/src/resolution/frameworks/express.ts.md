---
title: 'Module: src/resolution/frameworks/express.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/express.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`express.ts`/
symbols:
  expressResolver: expressResolver.
  resolveControllerMethod: resolveControllerMethod().
  resolveMiddleware: resolveMiddleware().
  resolveServiceMethod: resolveServiceMethod().
  matchDelim: matchDelim().
  extractTailIdent: extractTailIdent().
  RESERVED_CALLS: RESERVED_CALLS.
  isMiddlewareName: isMiddlewareName().
  detectLanguage: detectLanguage().
---
# Module: [`src/resolution/frameworks/express.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/express.ts)

## Functions
- `detectLanguage(filePath: string)` — [`L331`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/express.ts#L331) — Detect language from file extension
- `extractTailIdent(expr: string)` — [`L11`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/express.ts#L11)
- `isMiddlewareName(name: string)` — [`L227`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/express.ts#L227) — Check if a name looks like middleware
- `matchDelim(s: string, open: number, oc: string, cc: string)` — [`L21`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/express.ts#L21) — Index of the delimiter matching the one at `open`, skipping string/template
- `resolveControllerMethod(controller: string, method: string, context: ResolutionContext)` — [`L279`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/express.ts#L279) — Resolve controller method using name-based lookup
- `resolveMiddleware(name: string, context: ResolutionContext)` — [`L249`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/express.ts#L249) — Resolve middleware reference using name-based lookup
- `resolveServiceMethod(serviceName: string, method: string, context: ResolutionContext)` — [`L310`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/express.ts#L310) — Resolve service/helper method using name-based lookup

## Module values
- `RESERVED_CALLS` — [`L39`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/express.ts#L39)
- `expressResolver` — [`L50`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/express.ts#L50) — documented in [extraction-index.ts](../../../../concepts/extraction-index.ts.md)

