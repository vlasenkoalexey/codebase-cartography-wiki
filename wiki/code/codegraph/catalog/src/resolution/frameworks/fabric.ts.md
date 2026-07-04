---
title: 'Module: src/resolution/frameworks/fabric.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/fabric.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`fabric.ts`/
symbols:
  extractFabricNodes: extractFabricNodes().
  extractLegacyViewManagerNodes: extractLegacyViewManagerNodes().
  extractJvmViewManagerNodes: extractJvmViewManagerNodes().
  fabricViewResolver: fabricViewResolver.
  CODEGEN_DECL_RE: CODEGEN_DECL_RE.
  RCT_VIEW_PROP_RE: RCT_VIEW_PROP_RE.
  deriveComponentNameFromManager: deriveComponentNameFromManager().
  OBJC_IMPL_RE: OBJC_IMPL_RE.
  isFabricSpec: isFabricSpec().
  findNativePropsBody: findNativePropsBody().
  extractPropNames: extractPropNames().
---
# Module: [`src/resolution/frameworks/fabric.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts)

## Functions
- `deriveComponentNameFromManager(className: string)` — [`L84`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L84) — Derive the JS-visible component name from a native ViewManager class.
- `extractFabricNodes(filePath: string, source: string)` — [`L293`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L293)
- `extractJvmViewManagerNodes(filePath: string, source: string)` — [`L225`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L225) — Java/Kotlin `@ReactProp("name")` extraction. The annotation precedes a
- `extractLegacyViewManagerNodes(filePath: string, source: string)` — [`L145`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L145) — Extract legacy Paper view-manager declarations from a .m/.mm file.
- `extractPropNames(body: string)` — [`L116`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L116) — Parse the NativeProps interface body and return prop names.
- `findNativePropsBody(source: string)` — [`L105`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L105) — Pull the `NativeProps` interface body out of a Fabric spec source.
- `isFabricSpec(source: string)` — [`L97`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L97) — Cheap source-level detector — must contain `codegenNativeComponent` to

## Module values
- `CODEGEN_DECL_RE` — [`L52`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L52)
- `OBJC_IMPL_RE` — [`L75`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L75) — ObjC `@implementation Foo` extraction. Used to identify the ViewManager
- `RCT_VIEW_PROP_RE` — [`L67`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L67) — Legacy Paper view manager macros — older RN libs (still very common,
- `fabricViewResolver` — [`L364`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/fabric.ts#L364)

