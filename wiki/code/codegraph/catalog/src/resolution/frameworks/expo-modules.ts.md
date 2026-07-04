---
title: 'Module: src/resolution/frameworks/expo-modules.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/expo-modules.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`expo-modules.ts`/
symbols:
  extractExpoMethods: extractExpoMethods().
  isExpoModuleSource: isExpoModuleSource().
  EXPO_DECL_RE: EXPO_DECL_RE.
  expoModulesResolver: expoModulesResolver.
  EXPO_CLASS_RE: EXPO_CLASS_RE.
  EXPO_MODULE_NAME_RE: EXPO_MODULE_NAME_RE.
---
# Module: [`src/resolution/frameworks/expo-modules.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/expo-modules.ts)

## Functions
- `extractExpoMethods(filePath: string, source: string, language: "swift" | "kotlin")` — [`L101`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/expo-modules.ts#L101) — Extract Expo Module method declarations from a Swift / Kotlin source
- `isExpoModuleSource(source: string)` — [`L88`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/expo-modules.ts#L88) — Detect whether a file is plausibly an Expo Module — looking for both

## Module values
- `EXPO_CLASS_RE` — [`L78`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/expo-modules.ts#L78) — Heuristic class-name match — used as a fallback if `Name(...)` literal
- `EXPO_DECL_RE` — [`L63`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/expo-modules.ts#L63) — Match `Function("name")`, `AsyncFunction("name")`, or `Property("name")`
- `EXPO_MODULE_NAME_RE` — [`L71`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/expo-modules.ts#L71) — Match the module name literal `Name("ExpoX")`. Used to enrich each emitted
- `expoModulesResolver` — [`L152`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/expo-modules.ts#L152)

