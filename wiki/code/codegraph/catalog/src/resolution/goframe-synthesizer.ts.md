---
title: 'Module: src/resolution/goframe-synthesizer.ts'
type: catalog
provenance: extracted
module: src/resolution/goframe-synthesizer.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`goframe-synthesizer.ts`/
symbols:
  goframeRouteEdges: goframeRouteEdges().
  selectHandler: selectHandler().
  addonRoot: addonRoot().
  FANOUT_CAP: FANOUT_CAP.
  pointerParamTypes: pointerParamTypes().
---
# Module: [`src/resolution/goframe-synthesizer.ts`](../../../../../../raw/code/codegraph/src/resolution/goframe-synthesizer.ts)

## Functions
- `addonRoot(p: string)` — [`L55`](../../../../../../raw/code/codegraph/src/resolution/goframe-synthesizer.ts#L55) — The addon/plugin module a path lives under (`addons/hgexample/…` → `hgexample`),
- `goframeRouteEdges(ctx: ResolutionContext)` — [`L76`](../../../../../../raw/code/codegraph/src/resolution/goframe-synthesizer.ts#L76)
- `pointerParamTypes(sig: string)` — [`L40`](../../../../../../raw/code/codegraph/src/resolution/goframe-synthesizer.ts#L40) — Pointer-parameter types in a Go method signature, in both qualified and bare
- `selectHandler(candidates: Node[], routeFile: string)` — [`L66`](../../../../../../raw/code/codegraph/src/resolution/goframe-synthesizer.ts#L66) — Pick the one handler for a route from same-request-type candidates. Usually a

## Module values
- `FANOUT_CAP` — [`L30`](../../../../../../raw/code/codegraph/src/resolution/goframe-synthesizer.ts#L30)

