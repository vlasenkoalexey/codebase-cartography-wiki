---
title: 'Module: src/resolution/frameworks/python.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/python.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`python.ts`/
symbols:
  djangoResolver: djangoResolver.
  extractDecoratorRoutes: extractDecoratorRoutes().
  fastapiResolver: fastapiResolver.
  extractFlaskRestful: extractFlaskRestful().
  flaskResolver: flaskResolver.
  resolveModelIterableIter: resolveModelIterableIter().
  resolveByNameAndKind: resolveByNameAndKind().
  DecoratorRouteOpts.methodGroup: DecoratorRouteOpts#methodGroup.
  DecoratorRouteOpts.methodFromGroup: DecoratorRouteOpts#methodFromGroup.
  DecoratorRouteOpts.decoratorRegex: DecoratorRouteOpts#decoratorRegex.
  DecoratorRouteOpts.defaultMethod: DecoratorRouteOpts#defaultMethod.
  DecoratorRouteOpts.pathGroup: DecoratorRouteOpts#pathGroup.
  DecoratorRouteOpts.handlerGroup: DecoratorRouteOpts#handlerGroup.
  DecoratorRouteOpts.findHandler: DecoratorRouteOpts#findHandler.
  DecoratorRouteOpts.language: DecoratorRouteOpts#language.
  CLASS_KINDS: CLASS_KINDS.
  VARIABLE_KINDS: VARIABLE_KINDS.
  resolveHandlerName: resolveHandlerName().
  DecoratorRouteOpts: DecoratorRouteOpts#
  MODEL_DIRS: MODEL_DIRS.
  VIEW_DIRS: VIEW_DIRS.
  FORM_DIRS: FORM_DIRS.
  ROUTER_DIRS: ROUTER_DIRS.
  DEP_DIRS: DEP_DIRS.
  VIEW_KINDS: VIEW_KINDS.
  FUNCTION_KINDS: FUNCTION_KINDS.
---
# Module: [`src/resolution/frameworks/python.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts)

## Classes
### `DecoratorRouteOpts`
- def: [`src/resolution/frameworks/python.ts:275`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L275)
- signature: `interface DecoratorRouteOpts`
- members:
  - `decoratorRegex` — [`L276`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L276)
  - `defaultMethod` — [`L277`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L277)
  - `findHandler` — [`L282`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L282)
  - `handlerGroup` — [`L281`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L281)
  - `language` — [`L283`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L283)
  - `methodFromGroup` — [`L279`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L279)
  - `methodGroup` — [`L278`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L278)
  - `pathGroup` — [`L280`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L280)
- used by: [`extractDecoratorRoutes`](python.ts.md#extractDecoratorRoutes), [`fastapiResolver`](python.ts.md#fastapiResolver), [`flaskResolver`](python.ts.md#flaskResolver)

## Functions
- `extractDecoratorRoutes(filePath: string, content: string, opts: DecoratorRouteOpts)` — [`L286`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L286)
- `extractFlaskRestful(filePath: string, safe: string)` — [`L347`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L347) — Flask-RESTful: `api.add_resource(ResourceClass, '/path'[, '/path2'])`
- `resolveByNameAndKind(name: string, kinds: Set<string>, preferredDirPatterns: string[], context: ResolutionContext)` — [`L401`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L401) — Resolve a symbol by name using indexed queries instead of scanning all files.
- `resolveHandlerName(expr: string)` — [`L161`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L161) — Parse a Django URL handler expression and return the symbol/module to link.
- `resolveModelIterableIter(context: ResolutionContext)` — [`L148`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L148) — Find ModelIterable.__iter__ — the default iterable QuerySet invokes via

## Module values
- `CLASS_KINDS` — [`L393`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L393)
- `DEP_DIRS` — [`L391`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L391)
- `FORM_DIRS` — [`L389`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L389)
- `FUNCTION_KINDS` — [`L396`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L396)
- `MODEL_DIRS` — [`L387`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L387)
- `ROUTER_DIRS` — [`L390`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L390)
- `VARIABLE_KINDS` — [`L395`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L395)
- `VIEW_DIRS` — [`L388`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L388)
- `VIEW_KINDS` — [`L394`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L394)
- `djangoResolver` — [`L11`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L11) — documented in [types.ts](../../../../concepts/types.ts.md)
- `fastapiResolver` — [`L232`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L232)
- `flaskResolver` — [`L179`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/python.ts#L179)

