---
title: Cross-language native bridging
type: doc-concept
provenance: doc
source: docs/design/mixed-ios-and-react-native-bridging.md
updated: 2026-07-04
status: fresh
---
# Cross-language native bridging

## Definition
A **cross-language native bridge** is a dispatch "shape" where a single call
edge spans two ecosystems: a JS/TS React Native (or Expo) callsite that at
runtime reaches native Objective-C / Swift / Java / Kotlin code, or a Swift
call that lands on an Objective-C selector in the same iOS app. codegraph
indexes each language correctly **in isolation**, but the value of a
`trace` / `callers` / `impact` query is in the flow that crosses the
boundary — and a plain tree-sitter parse breaks there: the JS callsite has no
outgoing edge to the native handler, and the native handler has no incoming
edge from JS. This concept captures how codegraph rebuilds that edge so the
graph reflects that "a JS call actually reaches native code."

## The problem (the gap)
`useEffect(() => NativeModules.Geolocation.getCurrentPosition(cb))` in `App.js`
runs `RCT_EXPORT_METHOD(getCurrentPosition:...)` in `RNCGeolocation.m` at
runtime, but statically the two files share no reference — the JS property
chain resolves nowhere and the ObjC method node has zero callers. Same break
for `await ExpoCamera.takePictureAsync(...)` → Swift `AsyncFunction("takePictureAsync")`,
and for Swift `imageDownloader.download(url:completion:)` → ObjC
`-[ImageDownloader downloadURL:completion:]`. An agent asked to trace such a
flow gets no path and falls back to reading both files — which is exactly the
Read/Grep fallback codegraph exists to eliminate. The load-bearing rule from
the doc: **partial coverage is worse than none** — a half-bridged flow reveals
one hop the agent then drills to finish, so every channel (both directions,
legacy bridge *and* TurboModules) must close before measuring.

## The recognizer approach
The key insight is that in every one of these channels **a matching name
exists on both sides** — Swift's auto-bridged ObjC selector, the literal
first argument of `RCT_EXPORT_METHOD`, an Expo `Function("name")` string, a
TurboModule spec's `Native<Name>` export. So these are **resolver** patterns
(the bridging rule is deterministic from a name), not whole-graph
correlation. The work is: extract the bridging-side names, then let a resolver
match them and emit a `references` edge with `provenance:'heuristic'` and
`metadata.synthesizedBy:'<channel>'`. The one exception is native→JS events,
which look like the in-language EventEmitter pattern and so are handled as a
**synthesizer** channel instead.

The doc enumerates eleven channels grouped by direction:
- **Swift ↔ ObjC** (methods, `@objc` exposure, properties, initializers,
  protocols) — resolved by the auto-name selector mapping (`func move(to:)`
  ↔ `-moveTo:`, `init(name:)` ↔ `-initWithName:`), stored as an alternate
  name on the declaration node so ordinary name resolution finds the peer.
- **JS → native (RN legacy bridge)** — `NativeModules.<Mod>.<fn>` matched to
  `RCT_EXPORT_METHOD` / `RCT_REMAP_METHOD`, keyed by the `RCT_EXPORT_MODULE()`
  module name (ObjC) or `@ReactMethod` on a `getName()`-bearing class (JVM).
- **JS ↔ native (TurboModules / Codegen)** — the TS spec file is read as
  ground truth (`TurboModuleRegistry.get<Spec>('Name')` + the `Spec` methods).
- **Native → JS events** — `[self sendEventWithName:@"x"]` ↔
  `new NativeEventEmitter(...).addListener('x', cb)`.
- **JS → native (Expo modules)** — `requireNativeModule('X').fn(...)` ↔
  Swift/Kotlin `Function("fn") { ... }` inside a `Module` with `Name("X")`.
- **JS → native (Fabric view components)** — `<MyView prop=v/>` ↔
  Codegen view spec + native impl class (composes with the JSX synthesizer).

## In codegraph (grounded)
This design is implemented as a **family of passes**, split between the
callback synthesizer and the per-framework resolvers.

The **synthesizer** family lives in the callback synthesizer module
([`src/resolution/callback-synthesizer.ts`](../catalog/src/resolution/callback-synthesizer.ts.md)) —
each pass is one bridge channel:
- [`rnEventEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#rnEventEdges)
  — the native→JS event channel (Phase 3): `sendEventWithName:` on an
  `RCTEventEmitter` linked to the JS `addListener('name', cb)`, keyed by the
  literal event name (it reuses the in-language event-fanout cap and, for the
  subscribe-wrapper pattern, attributes the listener to the enclosing JS
  function).
- [`rnCrossPlatformEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#rnCrossPlatformEdges)
  and [`expoCrossPlatformEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#expoCrossPlatformEdges)
  — pair a native module's iOS and Android implementations that expose the
  same JS-visible name, so a JS callsite reaches both platforms' native code.
- [`fabricNativeImplEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#fabricNativeImplEdges)
  — the Fabric view channel (Phase 6): walks each `fabric-component` node and
  emits a `calls` edge to the native class matching its name with RN's
  convention suffixes (`View` / `ViewManager` / `ComponentView` / `Manager`),
  composing with [`reactJsxChildEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#reactJsxChildEdges)
  to close the full JSX → native flow. It shares the same EventEmitter
  machinery as [`eventEmitterEdges`](../catalog/src/resolution/callback-synthesizer.ts.md#eventEmitterEdges).

The **resolver** family lives under `frameworks/`, one module per channel:
- React Native ([`src/resolution/frameworks/react-native.ts`](../catalog/src/resolution/frameworks/react-native.ts.md)):
  [`reactNativeBridgeResolver`](../catalog/src/resolution/frameworks/react-native.ts.md#reactNativeBridgeResolver)
  matches `NativeModules.<Mod>.<fn>` against native maps built by
  [`parseObjcRNExports`](../catalog/src/resolution/frameworks/react-native.ts.md#parseObjcRNExports),
  [`parseJvmRNExports`](../catalog/src/resolution/frameworks/react-native.ts.md#parseJvmRNExports),
  and [`parseTurboModuleSpec`](../catalog/src/resolution/frameworks/react-native.ts.md#parseTurboModuleSpec)
  (module name via [`defaultObjcModuleName`](../catalog/src/resolution/frameworks/react-native.ts.md#defaultObjcModuleName)).
- Expo ([`src/resolution/frameworks/expo-modules.ts`](../catalog/src/resolution/frameworks/expo-modules.ts.md)):
  [`expoModulesResolver`](../catalog/src/resolution/frameworks/expo-modules.ts.md#expoModulesResolver)
  with [`extractExpoMethods`](../catalog/src/resolution/frameworks/expo-modules.ts.md#extractExpoMethods)
  synthesizing a `method` node per `Function("X")` / `AsyncFunction("X")`.
- Fabric ([`src/resolution/frameworks/fabric.ts`](../catalog/src/resolution/frameworks/fabric.ts.md)):
  [`fabricViewResolver`](../catalog/src/resolution/frameworks/fabric.ts.md#fabricViewResolver)
  and [`extractFabricNodes`](../catalog/src/resolution/frameworks/fabric.ts.md#extractFabricNodes)
  parse `codegenNativeComponent<Props>('Name')` specs into component + prop nodes.
- Swift ↔ ObjC ([`src/resolution/frameworks/swift-objc.ts`](../catalog/src/resolution/frameworks/swift-objc.ts.md)):
  [`swiftObjcBridgeResolver`](../catalog/src/resolution/frameworks/swift-objc.ts.md#swiftObjcBridgeResolver)
  with [`resolveSwiftCallToObjc`](../catalog/src/resolution/frameworks/swift-objc.ts.md#resolveSwiftCallToObjc)
  and [`resolveObjcCallToSwift`](../catalog/src/resolution/frameworks/swift-objc.ts.md#resolveObjcCallToSwift),
  driven by the pure auto-name mapping in
  [`src/resolution/swift-objc-bridge.ts`](../catalog/src/resolution/swift-objc-bridge.ts.md)
  ([`objcSelectorForSwiftMethod`](../catalog/src/resolution/swift-objc-bridge.ts.md#objcSelectorForSwiftMethod),
  [`objcSelectorForSwiftInit`](../catalog/src/resolution/swift-objc-bridge.ts.md#objcSelectorForSwiftInit),
  [`objcAccessorsForSwiftProperty`](../catalog/src/resolution/swift-objc-bridge.ts.md#objcAccessorsForSwiftProperty),
  [`swiftBaseNamesForObjcSelector`](../catalog/src/resolution/swift-objc-bridge.ts.md#swiftBaseNamesForObjcSelector)).

The bridging-side **names** these passes match on are surfaced by the
cross-language function-reference extraction in
[`src/extraction/function-ref.ts`](../catalog/src/extraction/function-ref.ts.md)
(per-language callable-reference specs). Every synthesized bridge edge is an
[`Edge`](../catalog/src/types.ts.md#Edge) of an appropriate
[`EdgeKind`](../catalog/src/types.ts.md#EdgeKind) (`references` / `calls`)
carrying `provenance:'heuristic'` + `metadata.synthesizedBy`, so the MCP read
tools surface it inline with no extra plumbing.

## Why it matters / when it applies
This applies to any mixed iOS app (Swift + Objective-C) or React Native / Expo
project — exactly the codebases where the interesting flow crosses the
boundary. The doc calls out sharp precision hazards the passes must respect:
NSObject-universal selectors (`init`, `description`, `copy`, …) and every
`RCTEventEmitter`'s built-in `addListener` / `removeListeners` are
**blocklisted**, because bridging them produces noise instead of signal
(RNFirebase dropped from 78 edges — 60 false positives — to 18 precise ones
after the blocklist). A cap of `EVENT_FANOUT_CAP = 6` makes over-connected
generic event names **skip rather than over-link** — silent beats wrong. The
doc also records a latent architecture bug the work surfaced: framework
resolvers whose `detect()` reads the indexed file list ran `initialize()`
before any files were indexed and silently dropped themselves; the fix reruns
`initialize()` after extraction. Explicitly out of scope: dynamic/computed
bridge keys (`NativeModules[someVar]`), bare JSI, `performSelector:`, and
Swift generics over ObjC protocols.

## Connections
- Code concepts: [resolution-callback-synthesizer.ts](../concepts/resolution-callback-synthesizer.ts.md)
  — the deep page on the synthesizer family that owns `rnEventEdges`,
  `rnCrossPlatformEdges`, `expoCrossPlatformEdges`, and `fabricNativeImplEdges`;
  [extraction-function-ref.ts](../concepts/extraction-function-ref.ts.md)
  — the cross-language callable-reference extraction that surfaces the
  bridging-side names; [types.ts](../concepts/types.ts.md) — `Edge` /
  `EdgeKind` / the `heuristic` provenance + `synthesizedBy` metadata every
  bridge edge carries.
- Module catalogs:
  [callback-synthesizer.ts](../catalog/src/resolution/callback-synthesizer.ts.md) ·
  [frameworks/react-native.ts](../catalog/src/resolution/frameworks/react-native.ts.md) ·
  [frameworks/expo-modules.ts](../catalog/src/resolution/frameworks/expo-modules.ts.md) ·
  [frameworks/fabric.ts](../catalog/src/resolution/frameworks/fabric.ts.md) ·
  [frameworks/swift-objc.ts](../catalog/src/resolution/frameworks/swift-objc.ts.md) ·
  [swift-objc-bridge.ts](../catalog/src/resolution/swift-objc-bridge.ts.md) ·
  [extraction/function-ref.ts](../catalog/src/extraction/function-ref.ts.md) ·
  [types.ts](../catalog/src/types.ts.md)
- Related doc-concepts: [dynamic-dispatch-coverage](dynamic-dispatch-coverage.md)
  (this is one row of that coverage matrix — the cross-language rows) ·
  [value-reference-edges](value-reference-edges.md) ·
  [template-markup-parsing](template-markup-parsing.md) (the JSX/markup hop the
  Fabric channel composes with).

## Source
Extracted from `docs/design/mixed-ios-and-react-native-bridging.md` (kept in place).
