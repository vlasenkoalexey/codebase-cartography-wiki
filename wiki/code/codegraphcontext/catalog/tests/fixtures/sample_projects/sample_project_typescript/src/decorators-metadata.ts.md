---
title: 'Module: tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts
status: fresh
symbol_base: scip-typescript npm sample_project_typescript 1.0.0 src/`decorators-metadata.ts`/
symbols:
  User: User#
  User.id: User#id.
  User.username: User#username.
  User.email: User#email.
  User.-constructor: User#`<constructor>`().
  User.getInfo: User#getInfo().
  User.-get-isAdult: User#`<get>isAdult`().
  User.updateAge: User#updateAge().
  METADATA_KEYS: METADATA_KEYS.
  UserService.findById: UserService#findById().
  ValidationEngine.validate: ValidationEngine#validate().
  User.deleteUser: User#deleteUser().
  Log: Log().
  Column: Column().
  Column.options-typeLiteral131.name: Column().(options)typeLiteral131:name.
  Column.options-typeLiteral131.type: Column().(options)typeLiteral131:type.
  SerializableProperty: SerializableProperty().
  decoratorExamples: decoratorExamples.
  Injectable: Injectable().
  Serializable: Serializable().
  Validate: Validate().
  Cache: Cache().
  RequireRole: RequireRole().
  MinLength: MinLength().
  Max: Max().
  ValidateParam: ValidateParam().
  MetadataReader.getInjectableInfo: MetadataReader#getInjectableInfo().
  UserService.-constructor: UserService#`<constructor>`().
  Required: Required().
  MetadataReader: MetadataReader#
  User.age: User#age.
  User.syncWithExternalService: User#syncWithExternalService().
  Inject: Inject().
  MetadataReader.getClassMetadata: MetadataReader#getClassMetadata().
  User.currentUserRole: User#currentUserRole.
  Entity: Entity().
  Component: Component().
  Component.config-typeLiteral8.selector: Component().(config)typeLiteral8:selector.
  Component.config-typeLiteral8.template: Component().(config)typeLiteral8:template.
  Retry: Retry().
  Computed: Computed().
  ValidationEngine: ValidationEngine#
  ValidationEngine.validate.typeLiteral228.valid: ValidationEngine#validate().typeLiteral228:valid.
  ValidationEngine.validate.typeLiteral228.errors: ValidationEngine#validate().typeLiteral228:errors.
  Column.options-typeLiteral131.nullable: Column().(options)typeLiteral131:nullable.
  Getter: Getter().
  Setter: Setter().
  MetadataReader.getMethodMetadata: MetadataReader#getMethodMetadata().
  MetadataReader.getPropertyMetadata: MetadataReader#getPropertyMetadata().
  MetadataReader.getAllMethodNames: MetadataReader#getAllMethodNames().
  MetadataReader.getValidationRules: MetadataReader#getValidationRules().
  User.password: User#password.
  UserService: UserService#
---
# Module: [`tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts)

## Classes
### `MetadataReader`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts:281`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L281)
- signature: `class MetadataReader`
- members:
  - `getAllMethodNames(method)` — [`L294`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L294)
  - `getClassMetadata(method)` — [`L282`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L282)
  - `getInjectableInfo(method)` — [`L315`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L315)
  - `getMethodMetadata(method)` — [`L286`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L286)
  - `getPropertyMetadata(method)` — [`L290`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L290)
  - `getValidationRules(method)` — [`L311`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L311)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `User`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts:324`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L324)
- signature: `class User`
- members:
  - `<constructor>(id: number, username: string, email: string, age: number)` — [`L349`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L349)
  - `<get>isAdult` — [`L385`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L385)
  - `deleteUser(method)` — [`L371`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L371)
  - `getInfo(method)` — [`L358`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L358)
  - `syncWithExternalService(method)` — [`L376`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L376)
  - `updateAge(method)` — [`L363`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L363)
  - `age` — [`L344`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L344)
  - `currentUserRole` — [`L347`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L347)
  - `email` — [`L339`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L339)
  - `id` — [`L328`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L328)
  - `password` — [`L346`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L346)
  - `username` — [`L334`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L334)
- uses (calls/refs, reference-scoped): (20 test-only callers)
- used by: (3 test-only callers)

### `UserService`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts:391`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L391)
- signature: `class UserService`
- members:
  - `<constructor>(userRepo: any, logger: any)` — [`L392`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L392)
  - `findById(method)` — [`L398`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L398)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (1 test-only callers)

### `ValidationEngine`
- def: [`tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts:406`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L406)
- signature: `class ValidationEngine`
- members:
  - `validate(method)` — [`L407`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L407)
  - `errors` — [`L407`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L407)
  - `valid` — [`L407`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L407)
- used by: (1 test-only callers)

## Functions
- `Cache(ttl?: number)` — [`L106`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L106)
- `Column(options?: { name?: string; type?: string; nullable?: boolean; })` — [`L177`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L177)
- `Component(config: { selector: string; template?: string; })` — [`L37`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L37)
- `Computed()` — [`L236`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L236)
- `Entity(tableName?: string)` — [`L23`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L23)
- `Getter()` — [`L266`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L266)
- `Inject(token?: string)` — [`L245`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L245)
- `Injectable()` — [`L30`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L30)
- `Log(message?: string)` — [`L69`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L69)
- `Max(value: number)` — [`L209`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L209)
- `MinLength(length: number)` — [`L196`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L196)
- `RequireRole(role: string)` — [`L155`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L155)
- `Required()` — [`L188`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L188)
- `Retry(maxAttempts?: number, delay?: number)` — [`L132`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L132)
- `Serializable()` — [`L44`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L44)
- `SerializableProperty(alias?: string)` — [`L222`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L222)
- `Setter()` — [`L273`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L273)
- `Validate()` — [`L85`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L85)
- `ValidateParam(validator: (value: any) => boolean, message: string)` — [`L253`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L253)

## Module values
- `METADATA_KEYS` — [`L11`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L11)
- `decoratorExamples` — [`L441`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L441)
- `name` — [`L177`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L177)
- `nullable` — [`L177`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L177)
- `selector` — [`L37`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L37)
- `template` — [`L37`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L37)
- `type` — [`L177`](../../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project_typescript/src/decorators-metadata.ts#L177)

