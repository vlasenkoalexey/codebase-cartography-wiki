---
title: 'Module: src/resolution/swift-objc-bridge.ts'
type: catalog
provenance: extracted
module: src/resolution/swift-objc-bridge.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/`swift-objc-bridge.ts`/
symbols:
  swiftBaseNamesForObjcSelector: swiftBaseNamesForObjcSelector().
  capFirst: capFirst().
  objcSelectorForSwiftMethod: objcSelectorForSwiftMethod().
  objcSelectorForSwiftInit: objcSelectorForSwiftInit().
  objcAccessorsForSwiftProperty: objcAccessorsForSwiftProperty().
  isObjcExposed: isObjcExposed().
  lowerFirst: lowerFirst().
  detectExplicitObjcName: detectExplicitObjcName().
---
# Module: [`src/resolution/swift-objc-bridge.ts`](../../../../../../raw/code/codegraph/src/resolution/swift-objc-bridge.ts)

## Functions
- `capFirst(s: string)` — [`L42`](../../../../../../raw/code/codegraph/src/resolution/swift-objc-bridge.ts#L42) — Capitalize the first character of a string. Used for the "With"-prefix
- `detectExplicitObjcName(sourceSlice: string)` — [`L257`](../../../../../../raw/code/codegraph/src/resolution/swift-objc-bridge.ts#L257) — Detect whether a Swift method `@objc` declaration uses the `@objc(custom:)`
- `isObjcExposed(sourceSlice: string)` — [`L273`](../../../../../../raw/code/codegraph/src/resolution/swift-objc-bridge.ts#L273) — Detect whether a Swift declaration is `@objc`-exposed by scanning the
- `lowerFirst(s: string)` — [`L50`](../../../../../../raw/code/codegraph/src/resolution/swift-objc-bridge.ts#L50) — Lowercase the first character. Used in reverse: `setName:` setter ↔
- `objcAccessorsForSwiftProperty(swiftName: string, explicitObjcName?: string | null | undefined)` — [`L160`](../../../../../../raw/code/codegraph/src/resolution/swift-objc-bridge.ts#L160) — Compute the bridged ObjC getter + setter for a Swift `@objc` property.
- `objcSelectorForSwiftInit(externalLabels: (string | null)[], internalNames: string[], explicitObjcName?: string | null | undefined)` — [`L117`](../../../../../../raw/code/codegraph/src/resolution/swift-objc-bridge.ts#L117) — Compute the bridged ObjC selector for a Swift `init(...)` declaration.
- `objcSelectorForSwiftMethod(baseName: string, externalLabels: (string | null)[], explicitObjcName?: string | null | undefined)` — [`L76`](../../../../../../raw/code/codegraph/src/resolution/swift-objc-bridge.ts#L76) — Compute the auto-bridged ObjC selector for a Swift method declaration.
- `swiftBaseNamesForObjcSelector(selector: string)` — [`L196`](../../../../../../raw/code/codegraph/src/resolution/swift-objc-bridge.ts#L196) — Reverse: from an ObjC selector, return the candidate Swift base names

