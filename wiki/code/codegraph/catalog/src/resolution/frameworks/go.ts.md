---
title: 'Module: src/resolution/frameworks/go.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/go.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`go.ts`/
symbols:
  goResolver: goResolver.
  resolveByNameAndKind: resolveByNameAndKind().
  extractGoTailIdent: extractGoTailIdent().
  HANDLER_DIRS: HANDLER_DIRS.
  SERVICE_DIRS: SERVICE_DIRS.
  MIDDLEWARE_DIRS: MIDDLEWARE_DIRS.
  MODEL_DIRS: MODEL_DIRS.
  SERVICE_KINDS: SERVICE_KINDS.
---
# Module: [`src/resolution/frameworks/go.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/go.ts)

## Functions
- `extractGoTailIdent(expr: string)` — [`L139`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/go.ts#L139) — Extract the last identifier from an expression like `pkg.Sub.handler` or `handler`.
- `resolveByNameAndKind(name: string, kind: string | null, preferredDirs: string[], context: ResolutionContext, kinds?: Set<string> | undefined)` — [`L156`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/go.ts#L156) — Resolve a symbol by name using indexed queries instead of scanning all files.

## Module values
- `HANDLER_DIRS` — [`L146`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/go.ts#L146)
- `MIDDLEWARE_DIRS` — [`L148`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/go.ts#L148)
- `MODEL_DIRS` — [`L149`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/go.ts#L149)
- `SERVICE_DIRS` — [`L147`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/go.ts#L147)
- `SERVICE_KINDS` — [`L150`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/go.ts#L150)
- `goResolver` — [`L11`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/go.ts#L11) — documented in [types.ts](../../../../concepts/types.ts.md)

