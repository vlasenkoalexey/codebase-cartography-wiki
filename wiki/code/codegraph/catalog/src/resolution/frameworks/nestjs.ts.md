---
title: 'Module: src/resolution/frameworks/nestjs.ts'
type: catalog
provenance: extracted
module: src/resolution/frameworks/nestjs.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/resolution/frameworks/`nestjs.ts`/
symbols:
  nestjsResolver: nestjsResolver.
  parseRouteObjects: parseRouteObjects().
  findDecorators: findDecorators().
  buildClassScopes: buildClassScopes().
  walkRoutesTree: walkRoutesTree().
  collectModuleControllers: collectModuleControllers().
  scopeFor: scopeFor().
  DecoratorHit.index: DecoratorHit#index.
  collectRouterModuleRegistrations: collectRouterModuleRegistrations().
  parseRoutesArray: parseRoutesArray().
  applyModulePrefix: applyModulePrefix().
  RouteItem: RouteItem#
  DecoratorHit.args: DecoratorHit#args.
  methodNameAfter: methodNameAfter().
  DecoratorHit.end: DecoratorHit#end.
  ClassScope.kind: ClassScope#kind.
  DecoratorHit.length: DecoratorHit#length.
  detectLanguage: detectLanguage().
  parseArrayField: parseArrayField().
  DecoratorHit.name: DecoratorHit#name.
  readArgs: readArgs().
  parseStringArg: parseStringArg().
  RouteItem.moduleName: RouteItem#moduleName.
  parseControllerPrefix: parseControllerPrefix().
  parseControllersField: parseControllersField().
  classNameAfter: classNameAfter().
  ClassKind: ClassKind#
  ClassScope: ClassScope#
  joinHttpPath: joinHttpPath().
  RouteItem.children: RouteItem#children.
  DecoratorHit: DecoratorHit#
  ClassScope.prefix: ClassScope#prefix.
  RouteItem.path: RouteItem#path.
  matchingClose: matchingClose().
  JsLang: JsLang#
  HTTP_METHODS: HTTP_METHODS.
  GQL_OPS: GQL_OPS.
  PROVIDER_CONVENTIONS: PROVIDER_CONVENTIONS.
  ClassScope.start: ClassScope#start.
  ClassScope.end: ClassScope#end.
  parseGatewayNamespace: parseGatewayNamespace().
  parseGraphqlName: parseGraphqlName().
  lineAt: lineAt().
  splitTopLevelObjects: splitTopLevelObjects().
  parseStringField: parseStringField().
  parseIdentField: parseIdentField().
---
# Module: [`src/resolution/frameworks/nestjs.ts`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts)

## Classes
### `ClassKind`
- def: [`src/resolution/frameworks/nestjs.ts:413`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L413)
- signature: `type ClassKind`
- used by: [`buildClassScopes`](nestjs.ts.md#buildClassScopes), [`kind`](nestjs.ts.md#ClassScope.kind)

### `ClassScope`
- def: [`src/resolution/frameworks/nestjs.ts:415`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L415)
- signature: `interface ClassScope`
- members:
  - `end` — [`L420`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L420)
  - `kind` — [`L416`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L416)
  - `prefix` — [`L418`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L418) — HTTP prefix (controller) or WS namespace (gateway); '' otherwise.
  - `start` — [`L419`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L419)
- uses (calls/refs, reference-scoped): [`ClassKind`](nestjs.ts.md#ClassKind)
- used by: [`nestjsResolver`](nestjs.ts.md#nestjsResolver), [`buildClassScopes`](nestjs.ts.md#buildClassScopes), [`scopeFor`](nestjs.ts.md#scopeFor)

### `DecoratorHit`
- def: [`src/resolution/frameworks/nestjs.ts:289`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L289)
- signature: `interface DecoratorHit`
- members:
  - `args` — [`L293`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L293) — Raw text between the decorator's parentheses.
  - `end` — [`L297`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L297) — Index just past the decorator's closing `)`.
  - `index` — [`L295`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L295) — Index of the leading `@` in the (comment-stripped) source.
  - `length` — [`L299`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L299) — Character length of the whole `@Name(...)` decorator.
  - `name` — [`L291`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L291) — Decorator name without the leading `@` (e.g. `Get`).
- used by: [`nestjsResolver`](nestjs.ts.md#nestjsResolver), [`findDecorators`](nestjs.ts.md#findDecorators), [`buildClassScopes`](nestjs.ts.md#buildClassScopes), [`collectModuleControllers`](nestjs.ts.md#collectModuleControllers)

### `JsLang`
- def: [`src/resolution/frameworks/nestjs.ts:40`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L40)
- signature: `type JsLang`
- used by: [`detectLanguage`](nestjs.ts.md#detectLanguage)

### `RouteItem`
- def: [`src/resolution/frameworks/nestjs.ts:545`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L545)
- signature: `interface RouteItem`
- members:
  - `children` — [`L548`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L548)
  - `moduleName` — [`L547`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L547)
  - `path` — [`L546`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L546)
- used by: [`parseRouteObjects`](nestjs.ts.md#parseRouteObjects), [`walkRoutesTree`](nestjs.ts.md#walkRoutesTree), [`parseRoutesArray`](nestjs.ts.md#parseRoutesArray)

## Functions
- `applyModulePrefix(route: Node, prefix: string)` — [`L664`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L664) — Recompute a route node's `name` by prepending `prefix` to the *original*
- `buildClassScopes(safe: string)` — [`L429`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L429) — Build the list of class-level decorator scopes, sorted by position. Each
- `classNameAfter(safe: string, start: number)` — [`L627`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L627) — Starting just after a class decorator's `)`, return the name of the class
- `collectModuleControllers(safe: string, out: Map<string, string>)` — [`L601`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L601) — Walk every `@Module(...)` decorator and populate `out` with
- `collectRouterModuleRegistrations(safe: string, out: Map<string, string>)` — [`L532`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L532) — Walk every `RouterModule.register([...])` call (and the equivalent
- `detectLanguage(filePath: string)` — [`L514`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L514)
- `findDecorators(safe: string, names: string[])` — [`L308`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L308) — Find every `@Name(...)` decorator whose name is in `names`. Uses a
- `joinHttpPath(prefix: string, sub: string)` — [`L503`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L503) — Join a controller prefix and method path into a single normalised `/path`.
- `lineAt(safe: string, index: number)` — [`L510`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L510)
- `matchingClose(s: string, open: number)` — [`L682`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L682) — Return the index of the bracket that closes the one at `open`, or -1.
- `methodNameAfter(safe: string, start: number)` — [`L365`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L365) — Starting just after a method decorator's `)`, return the name of the method
- `parseArrayField(obj: string, name: string)` — [`L758`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L758) — Read an array-valued field — `key: [ ... ]` — as the raw inner text.
- `parseControllerPrefix(args: string)` — [`L473`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L473) — `@Controller('users')` | `@Controller({ path: 'users', host })` | `@Controller(['a','b'])` | `@Controller()`.
- `parseControllersField(args: string)` — [`L613`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L613)
- `parseGatewayNamespace(args: string)` — [`L480`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L480) — `@WebSocketGateway({ namespace: 'chat' })` | `@WebSocketGateway(81, { namespace: '/chat' })` | `@WebSocketGateway()`.
- `parseGraphqlName(args: string, handler: string | null)` — [`L490`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L490) — GraphQL operation name. Prefers an explicit `{ name: 'x' }` or a leading
- `parseIdentField(obj: string, name: string)` — [`L751`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L751) — Read an identifier-valued field — `key: SomeIdent` — out of one object body.
- `parseRouteObjects(s: string)` — [`L566`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L566)
- `parseRoutesArray(args: string)` — [`L557`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L557) — Parse a `[ {...}, {...} ]` argument list into a list of `RouteItem`s. The
- `parseStringArg(args: string)` — [`L467`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L467) — First string literal anywhere in the args, or '' (covers `'x'`, `{ k: 'x' }`).
- `parseStringField(obj: string, name: string)` — [`L744`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L744) — Read a string-valued field — `key: 'value'` — out of one object literal's
- `readArgs(s: string, openIndex: number)` — [`L333`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L333) — Read a balanced `(...)` starting at `openIndex` (which must point at `(`).
- `scopeFor(scopes: ClassScope[], index: number)` — [`L455`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L455)
- `splitTopLevelObjects(s: string)` — [`L709`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L709) — Split `s` into the contents of each top-level object literal. Brackets and
- `walkRoutesTree(items: RouteItem[], parentPrefix: string, out: Map<string, string>)` — [`L578`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L578)

## Module values
- `GQL_OPS` — [`L43`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L43)
- `HTTP_METHODS` — [`L42`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L42)
- `PROVIDER_CONVENTIONS` — [`L273`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L273)
- `nestjsResolver` — [`L45`](../../../../../../../raw/code/codegraph/src/resolution/frameworks/nestjs.ts#L45) — documented in [extraction-index.ts](../../../../concepts/extraction-index.ts.md)

