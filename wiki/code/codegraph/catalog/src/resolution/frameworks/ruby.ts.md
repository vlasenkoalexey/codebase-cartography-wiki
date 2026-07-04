---
title: 'Module: src/resolution/frameworks/ruby.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/ruby.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`ruby.ts`/
symbols:
  railsResolver: railsResolver.
  resolveControllerAction: resolveControllerAction().
  resolveModel: resolveModel().
  resolveController: resolveController().
  resolveHelper: resolveHelper().
  resolveService: resolveService().
  RESTFUL_ROUTES.Record.typeLiteral128.path: RESTFUL_ROUTES.Record:typeLiteral128:path.
  RESTFUL_ROUTES.Record.typeLiteral128.method: RESTFUL_ROUTES.Record:typeLiteral128:method.
  RESTFUL_ROUTES: RESTFUL_ROUTES.
  PLURAL_ACTIONS: PLURAL_ACTIONS.
  SINGULAR_ACTIONS: SINGULAR_ACTIONS.
  pluralize: pluralize().
  camelize: camelize().
---
# Module: [`src/resolution/frameworks/ruby.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts)

## Functions
- `camelize(s: string)` — [`L217`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L217) — snake_case → CamelCase (`user_profiles` → `UserProfiles`).
- `pluralize(w: string)` — [`L210`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L210) — Naive ActiveSupport-style pluralize — covers the common resource names.
- `resolveController(name: string, context: ResolutionContext)` — [`L268`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L268)
- `resolveControllerAction(ctrlPath: string, action: string, context: ResolutionContext)` — [`L222`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L222) — Resolve a `controller#action` route ref to the action method in that controller.
- `resolveHelper(name: string, context: ResolutionContext)` — [`L299`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L299)
- `resolveModel(name: string, context: ResolutionContext)` — [`L238`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L238)
- `resolveService(name: string, context: ResolutionContext)` — [`L316`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L316)

## Module values
- `PLURAL_ACTIONS` — [`L206`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L206)
- `RESTFUL_ROUTES` — [`L197`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L197)
- `SINGULAR_ACTIONS` — [`L207`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L207)
- `method` — [`L197`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L197)
- `path` — [`L197`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L197)
- `railsResolver` — [`L11`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/ruby.ts#L11) — documented in [extraction-index.ts](../../../../concepts/extraction-index.ts.md)

