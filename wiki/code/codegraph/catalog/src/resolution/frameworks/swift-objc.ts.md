---
title: 'Module: src/resolution/frameworks/swift-objc.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/swift-objc.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`swift-objc.ts`/
symbols:
  resolveObjcCallToSwift: resolveObjcCallToSwift().
  buildObjcMap: buildObjcMap().
  declarationSourceWindow: declarationSourceWindow().
  resolveSwiftCallToObjc: resolveSwiftCallToObjc().
  objcByCandidateSwiftBase: objcByCandidateSwiftBase.
  swiftObjcBridgeResolver: swiftObjcBridgeResolver.
  GENERIC_NAMES: GENERIC_NAMES.
  SOURCE_PROBE_LINES: SOURCE_PROBE_LINES.
---
# Module: [`src/resolution/frameworks/swift-objc.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/swift-objc.ts)

## Functions
- `buildObjcMap(context: ResolutionContext)` — [`L116`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/swift-objc.ts#L116)
- `declarationSourceWindow(node: Node, context: ResolutionContext)` — [`L157`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/swift-objc.ts#L157) — Read a small window of source ending at `node.startLine`, used to
- `resolveObjcCallToSwift(ref: UnresolvedRef, context: ResolutionContext)` — [`L213`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/swift-objc.ts#L213) — Try to resolve an ObjC caller's selector reference to a Swift `@objc`
- `resolveSwiftCallToObjc(ref: UnresolvedRef, context: ResolutionContext)` — [`L173`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/swift-objc.ts#L173) — Try to resolve a Swift caller's bare reference to an ObjC implementation.

## Module values
- `GENERIC_NAMES` — [`L76`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/swift-objc.ts#L76) — Names that are too generic to bridge with any precision. These are common
- `SOURCE_PROBE_LINES` — [`L150`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/swift-objc.ts#L150) — Window of source text around a Swift declaration used by `isObjcExposed`
- `objcByCandidateSwiftBase` — [`L50`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/swift-objc.ts#L50) — Memoized "Swift base name → ObjC method nodes" map.
- `swiftObjcBridgeResolver` — [`L248`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/swift-objc.ts#L248)

