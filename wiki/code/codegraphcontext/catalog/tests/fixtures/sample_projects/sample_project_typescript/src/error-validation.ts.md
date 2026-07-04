---
title: 'Module: tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts
status: fresh
symbol_base: scip-typescript npm sample_project_typescript 1.0.0 src/`error-validation.ts`/
symbols:
  SchemaValidator.validate: SchemaValidator#validate().
  SchemaValidator.validateObject: SchemaValidator#validateObject().
  Result: Result#
  ValidationError.-constructor: ValidationError#`<constructor>`().
  Err: Err.
  fetchUser: fetchUser().
  safeProcessUser: safeProcessUser.
  ApplicationError: ApplicationError#
  ValidationRules: ValidationRules.
  errorBoundary: errorBoundary.
  ValidationError: ValidationError#
  Ok: Ok.
  safeParseInt: safeParseInt().
  safeParse: safeParse().
  userSchema: userSchema.
  safeParseFloat: safeParseFloat().
  ApplicationError.-constructor: ApplicationError#`<constructor>`().
  ValidationRule: ValidationRule#
  ValidationRule.validate: ValidationRule#validate.
  ValidationRule.message: ValidationRule#message.
  tryCatch: tryCatch().
  tryCatchAsync: tryCatchAsync().
  validateUser.Result.typeLiteral165.age: validateUser().Result:typeLiteral165:age.
  safeJsonParse: safeJsonParse().
  map: map().
  mapError: mapError().
  Schema.rules: Schema#rules.
  ErrorBoundary.handle: ErrorBoundary#handle().
  isOk: isOk().
  isObject: isObject().
  NotFoundError.-constructor: NotFoundError#`<constructor>`().
  NetworkError.-constructor: NetworkError#`<constructor>`().
  Schema: Schema#
  isErr: isErr().
  validateUser: validateUser().
  flatMap: flatMap().
  assertIsString: assertIsString().
  assertIsNumber: assertIsNumber().
  assertIsObject: assertIsObject().
  assertHasProperty: assertHasProperty().
  hasProperty: hasProperty().
  ErrorBoundary.onError: ErrorBoundary#onError().
  Schema.transform: Schema#transform.
  ErrorBoundary.onGlobalError: ErrorBoundary#onGlobalError().
  ErrorBoundary.wrap: ErrorBoundary#wrap().
  ErrorBoundary.globalHandler: ErrorBoundary#globalHandler.
  NotFoundError: NotFoundError#
  UnauthorizedError: UnauthorizedError#
  NetworkError: NetworkError#
  isArray: isArray().
  hasProperties: hasProperties().
  ValidationError.field: ValidationError#field.
  isString: isString().
  isNumber: isNumber().
  Schema.optional: Schema#optional.
  SchemaValidator: SchemaValidator#
  ErrorBoundary.errorHandlers: ErrorBoundary#errorHandlers.
  ApplicationError.code: ApplicationError#code.
  ApplicationError.timestamp: ApplicationError#timestamp.
  ApplicationError.context: ApplicationError#context.
  ValidationError.value: ValidationError#value.
  NotFoundError.resource: NotFoundError#resource.
  NotFoundError.identifier: NotFoundError#identifier.
  NetworkError.statusCode: NetworkError#statusCode.
  NetworkError.url: NetworkError#url.
  ErrorBoundary: ErrorBoundary#
  validateUser.Result.typeLiteral165.id: validateUser().Result:typeLiteral165:id.
  UnauthorizedError.-constructor: UnauthorizedError#`<constructor>`().
  isInstanceOf: isInstanceOf().
  isOneOf: isOneOf().
  assert: assert().
  assertNever: assertNever().
  validateUser.Result.typeLiteral165.name: validateUser().Result:typeLiteral165:name.
  validateUser.Result.typeLiteral165.email: validateUser().Result:typeLiteral165:email.
  errorHandlingExamples: errorHandlingExamples.
---
# Module: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts)

## Classes
### `ApplicationError`  ·  implements/extends Error
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts:8`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L8)
- doc: Error Handling and Validation
- signature: `class ApplicationError`
- members:
  - `<constructor>(message: string, code: string, context?: Record<string, any>)` — [`L13`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L13) — Error Handling and Validation
  - `code` — [`L9`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L9)
  - `context` — [`L11`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L11)
  - `timestamp` — [`L10`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L10)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (5 test-only callers)

### `ErrorBoundary`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts:350`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L350)
- signature: `class ErrorBoundary`
- members:
  - `handle(method)` — [`L362`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L362)
  - `onError(method)` — [`L354`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L354)
  - `onGlobalError(method)` — [`L358`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L358)
  - `wrap(method)` — [`L374`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L374)
  - `errorHandlers` — [`L351`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L351)
  - `globalHandler` — [`L352`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L352)
- used by: (2 test-only callers)

### `NetworkError`  ·  implements/extends ApplicationError, Error
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts:58`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L58)
- signature: `class NetworkError`
- members:
  - `<constructor>(message: string, statusCode?: number, url?: string, context?: Record<string, any>)` — [`L62`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L62)
  - `statusCode` — [`L59`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L59)
  - `url` — [`L60`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L60)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `NotFoundError`  ·  implements/extends ApplicationError, Error
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts:39`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L39)
- signature: `class NotFoundError`
- members:
  - `<constructor>(resource: string, identifier: any, context?: Record<string, any>)` — [`L43`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L43)
  - `identifier` — [`L41`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L41)
  - `resource` — [`L40`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L40)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `Result`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts:71`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L71)
- signature: `type Result`
- used by: (19 test-only callers)

### `Schema`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts:198`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L198)
- signature: `interface Schema`
- members:
  - `optional` — [`L200`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L200)
  - `rules` — [`L199`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L199)
  - `transform` — [`L201`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L201)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (3 test-only callers)

### `SchemaValidator`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts:204`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L204)
- signature: `class SchemaValidator`
- members:
  - `validate(method)` — [`L205`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L205)
  - `validateObject(method)` — [`L237`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L237)
- uses (calls/refs, reference-scoped): (14 test-only callers)
- used by: (1 test-only callers)

### `UnauthorizedError`  ·  implements/extends ApplicationError, Error
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts:51`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L51)
- signature: `class UnauthorizedError`
- members:
  - `<constructor>(message?: string, context?: Record<string, any>)` — [`L52`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L52)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `ValidationError`  ·  implements/extends ApplicationError, Error
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts:27`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L27)
- signature: `class ValidationError`
- members:
  - `<constructor>(message: string, field?: string, value?: any, context?: Record<string, any>)` — [`L31`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L31)
  - `field` — [`L28`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L28)
  - `value` — [`L29`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L29)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (18 test-only callers)

### `ValidationRule`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts:193`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L193)
- signature: `interface ValidationRule`
- members:
  - `message` — [`L195`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L195)
  - `validate` — [`L194`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L194)
- used by: (3 test-only callers)

## Functions
- `assert(condition: any, message?: string)` — [`L155`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L155)
- `assertHasProperty(obj: unknown, prop: K)` — [`L179`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L179)
- `assertIsNumber(value: unknown)` — [`L167`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L167)
- `assertIsObject(value: unknown)` — [`L173`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L173)
- `assertIsString(value: unknown)` — [`L161`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L161)
- `assertNever(value: never)` — [`L188`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L188)
- `fetchUser(id: number)` — [`L459`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L459)
- `flatMap(result: Result<T, E>, fn: (data: T) => Result<U, E>)` — [`L94`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L94)
- `hasProperties(obj: unknown, ...props: K[])` — [`L132`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L132)
- `hasProperty(obj: unknown, prop: K)` — [`L125`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L125)
- `isArray(value: unknown, elementGuard: (item: unknown) => item is T)` — [`L121`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L121)
- `isErr(result: Result<T, E>)` — [`L82`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L82)
- `isInstanceOf(...args: any[])` — [`L140`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L140)
- `isNumber(value: unknown)` — [`L113`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L113)
- `isObject(value: unknown)` — [`L117`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L117)
- `isOk(result: Result<T, E>)` — [`L78`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L78)
- `isOneOf(values: T, value: unknown)` — [`L147`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L147)
- `isString(value: unknown)` — [`L109`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L109)
- `map(result: Result<T, E>, fn: (data: T) => U)` — [`L87`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L87)
- `mapError(result: Result<T, E>, fn: (error: E) => F)` — [`L101`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L101)
- `safeJsonParse(json: string)` — [`L345`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L345)
- `safeParse(value: string, parser: (str: string) => T)` — [`L330`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L330)
- `safeParseFloat(value: string)` — [`L322`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L322)
- `safeParseInt(value: string)` — [`L314`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L314)
- `tryCatch(fn: () => T)` — [`L399`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L399)
- `tryCatchAsync(fn: () => Promise<T>)` — [`L407`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L407)
- `validateUser(userData: unknown)` — [`L450`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L450)

## Module values
- `Err` — [`L76`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L76)
- `Ok` — [`L75`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L75)
- `ValidationRules` — [`L266`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L266)
- `age` — [`L454`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L454)
- `email` — [`L453`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L453)
- `errorBoundary` — [`L485`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L485)
- `errorHandlingExamples` — [`L518`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L518)
- `id` — [`L451`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L451)
- `name` — [`L452`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L452)
- `safeProcessUser` — [`L500`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L500)
- `userSchema` — [`L418`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/error-validation.ts#L418)

