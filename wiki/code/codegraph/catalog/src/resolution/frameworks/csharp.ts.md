---
title: 'Module: src/resolution/frameworks/csharp.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/csharp.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`csharp.ts`/
symbols:
  aspnetResolver: aspnetResolver.
  resolveByNameAndKind: resolveByNameAndKind().
  CLASS_KINDS: CLASS_KINDS.
  SERVICE_KINDS: SERVICE_KINDS.
  joinCsPath: joinCsPath().
  extractCSharpTailIdent: extractCSharpTailIdent().
  CONTROLLER_DIRS: CONTROLLER_DIRS.
  SERVICE_DIRS: SERVICE_DIRS.
  REPO_DIRS: REPO_DIRS.
  MODEL_DIRS: MODEL_DIRS.
  VIEWMODEL_DIRS: VIEWMODEL_DIRS.
---
# Module: [`src/resolution/frameworks/csharp.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts)

## Functions
- `extractCSharpTailIdent(expr: string)` — [`L235`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L235) — Extract last identifier from an expression like `MyService.Handler` or `Handler`.
- `joinCsPath(prefix: string, sub: string)` — [`L229`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L229) — Join a class-level [Route] prefix and an action's path into one normalized `/path`.
- `resolveByNameAndKind(name: string, kinds: Set<string>, preferredDirPatterns: string[], context: ResolutionContext)` — [`L254`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L254) — Resolve a symbol by name using indexed queries instead of scanning all files.

## Module values
- `CLASS_KINDS` — [`L248`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L248)
- `CONTROLLER_DIRS` — [`L242`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L242)
- `MODEL_DIRS` — [`L245`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L245)
- `REPO_DIRS` — [`L244`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L244)
- `SERVICE_DIRS` — [`L243`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L243)
- `SERVICE_KINDS` — [`L249`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L249)
- `VIEWMODEL_DIRS` — [`L246`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L246)
- `aspnetResolver` — [`L11`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/csharp.ts#L11) — documented in [extraction-index.ts](../../../../concepts/extraction-index.ts.md)

