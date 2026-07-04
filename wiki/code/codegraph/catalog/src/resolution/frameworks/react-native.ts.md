---
title: 'Module: src/resolution/frameworks/react-native.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/react-native.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`react-native.ts`/
symbols:
  buildRNMaps: buildRNMaps().
  parseObjcRNExports.Array.typeLiteral1.jsName: parseObjcRNExports().Array:typeLiteral1:jsName.
  NativeMethod.node: NativeMethod#node.
  NativeMethod: NativeMethod#
  parseJvmRNExports.Array.typeLiteral49.jsName: parseJvmRNExports().Array:typeLiteral49:jsName.
  nativeMethodMaps: nativeMethodMaps.
  parseObjcRNExports: parseObjcRNExports().
  parseObjcRNExports.Array.typeLiteral1.moduleName: parseObjcRNExports().Array:typeLiteral1:moduleName.
  NativeMethod.moduleName: NativeMethod#moduleName.
  NativeMethod.jsName: NativeMethod#jsName.
  parseObjcRNExports.Array.typeLiteral1.nativeSelectorFirstKw: parseObjcRNExports().Array:typeLiteral1:nativeSelectorFirstKw.
  RN_EMITTER_BUILTINS: RN_EMITTER_BUILTINS.
  reactNativeBridgeResolver: reactNativeBridgeResolver.
  nativeMethodMaps.WeakMap.typeLiteral0.byJsName: nativeMethodMaps.WeakMap:typeLiteral0:byJsName.
  parseObjcRNExports.Array.typeLiteral1.line: parseObjcRNExports().Array:typeLiteral1:line.
  findObjcClassName: findObjcClassName().
  defaultObjcModuleName: defaultObjcModuleName().
  parseJvmRNExports: parseJvmRNExports().
  parseJvmRNExports.Array.typeLiteral49.moduleName: parseJvmRNExports().Array:typeLiteral49:moduleName.
  parseTurboModuleSpec: parseTurboModuleSpec().
  buildRNMaps.typeLiteral103.byJsName: buildRNMaps().typeLiteral103:byJsName.
---
# Module: [`src/resolution/frameworks/react-native.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts)

## Classes
### `NativeMethod`
- def: [`src/resolution/frameworks/react-native.ts:50`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L50)
- doc: One native RN method known to the resolver. Indexed by JS-visible name.
- signature: `interface NativeMethod`
- members:
  - `jsName` — [`L54`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L54) — JS-visible method name.
  - `moduleName` — [`L52`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L52) — Module name as seen from JS (`Geolocation`, `RNSVGRenderableModule`, …).
  - `node` — [`L56`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L56) — Native implementation node (ObjC method / Java method / Kotlin function).
- uses (calls/refs, reference-scoped): [`Node`](../../types.ts.md#Node)
- used by: [`react-native.ts`](react-native.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-resolution-frameworks-react-native.ts), [`buildRNMaps`](react-native.ts.md#buildRNMaps), [`byJsName`](react-native.ts.md#nativeMethodMaps.WeakMap.typeLiteral0.byJsName)

## Functions
- `buildRNMaps(context: ResolutionContext)` — [`L263`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L263)
- `defaultObjcModuleName(className: string)` — [`L74`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L74) — Default ObjC module name when `RCT_EXPORT_MODULE()` has no argument:
- `findObjcClassName(source: string)` — [`L152`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L152) — Find the `@implementation` class name in an ObjC file — used as the
- `parseJvmRNExports(source: string)` — [`L171`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L171) — Parse a Java/Kotlin source file for `@ReactMethod` annotated methods
- `parseObjcRNExports(source: string, className: string | null)` — [`L99`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L99) — Parse an ObjC `.m`/`.mm` file's source for `RCT_EXPORT_MODULE` and
- `parseTurboModuleSpec(source: string)` — [`L212`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L212) — Parse a TS file for a TurboModule spec declaration. The spec file is

## Module values
- `RN_EMITTER_BUILTINS` — [`L254`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L254) — RCTEventEmitter built-ins that every emitter subclass inherits. JS code
- `byJsName` — [`L62`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L62)
- `byJsName` — [`L263`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L263)
- `jsName` — [`L102`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L102)
- `jsName` — [`L173`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L173)
- `line` — [`L102`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L102)
- `moduleName` — [`L102`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L102)
- `moduleName` — [`L173`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L173)
- `nativeMethodMaps` — [`L60`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L60) — Per-context lazy map cache.
- `nativeSelectorFirstKw` — [`L102`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L102)
- `reactNativeBridgeResolver` — [`L362`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/react-native.ts#L362)

