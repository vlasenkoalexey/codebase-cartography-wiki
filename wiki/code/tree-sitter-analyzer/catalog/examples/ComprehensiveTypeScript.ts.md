---
title: 'Module: examples/ComprehensiveTypeScript.ts'
type: catalog
provenance: extracted
module: examples/ComprehensiveTypeScript.ts
status: fresh
symbol_base: scip-typescript npm . . examples/`ComprehensiveTypeScript.ts`/
symbols:
  Application.initialize: Application#initialize().
  Application.-constructor: Application#`<constructor>`().
  User: User#
  main: main().
  UserService: UserService#
  Application.setupEventHandlers: Application#setupEventHandlers().
  handleUser: handleUser().
  UserService.save: UserService#save().
  Application.demonstrateUserSearch: Application#demonstrateUserSearch().
  Application.demonstrateStreamProcessing: Application#demonstrateStreamProcessing().
  UserService.findAll: UserService#findAll().
  Application.userService: Application#userService.
  Application.batchProcessor: Application#batchProcessor.
  UserService.users: UserService#users.
  UserService.eventEmitter: UserService#eventEmitter.
  UserService.onUserSaved: UserService#onUserSaved().
  BaseEntity.-constructor: BaseEntity#`<constructor>`().
  User.id: User#id.
  BatchProcessor.config: DataProcessing/BatchProcessor#config.
  User.name: User#name.
  UserService.getInstance: UserService#getInstance().
  UserService.findById: UserService#findById().
  UserService.onUserDeleted: UserService#onUserDeleted().
  AsyncDataProcessor.fetchData: AsyncDataProcessor#fetchData().
  BatchProcessor.-constructor: DataProcessing/BatchProcessor#`<constructor>`().
  BatchProcessor.processBatch: DataProcessing/BatchProcessor#processBatch().
  BatchProcessor.createBatches: DataProcessing/BatchProcessor#createBatches().
  BatchProcessor.processSingleBatch: DataProcessing/BatchProcessor#processSingleBatch().
  isAdminUser: isAdminUser().
  AdminUser: AdminUser#
  UserService.instance: UserService#instance.
  Repository.findAll: Repository#findAll().
  UserService.delete: UserService#delete().
  UserUpdate: UserUpdate#
  processUser: processUser().
  User.preferences: User#preferences.
  Repository: Repository#
  ValidatedUser: ValidatedUser#
  ValidatedUser.name: ValidatedUser#name.
  Application.dataProcessor: Application#dataProcessor.
  AdminUser.permissions: AdminUser#permissions.
  BaseEntity: BaseEntity#
  ValidatedUser.age: ValidatedUser#age.
  ValidatedUser.greet: ValidatedUser#greet().
  Partial: Partial#
  User.age: User#age.
  EventHandler: EventHandler#
  AsyncDataProcessor: AsyncDataProcessor#
  AsyncDataProcessor.cache: AsyncDataProcessor#cache.
  ProcessorConfig.batchSize: DataProcessing/ProcessorConfig#batchSize.
  Repository.findById: Repository#findById().
  Repository.save: Repository#save().
  Repository.delete: Repository#delete().
  BaseEntity.validate: BaseEntity#validate().
  BaseEntity.updateTimestamp: BaseEntity#updateTimestamp().
  BaseEntity.getId: BaseEntity#getId().
  UserService.validate: UserService#validate().
  UserKeys: UserKeys#
  UserValues: UserValues#
  AsyncDataProcessor.fetchMultipleData: AsyncDataProcessor#fetchMultipleData().
  stringValue: stringValue.
  anotherStringValue: anotherStringValue.
  isUser: isUser().
  UserID: UserID#
  User.email: User#email.
  UserPreferences: UserPreferences#
  UserPreferences.theme: UserPreferences#theme.
  UserPreferences.language: UserPreferences#language.
  UserPreferences.notifications: UserPreferences#notifications.
  Permission: Permission#
  BaseEntity.id: BaseEntity#id.
  BaseEntity.updatedAt: BaseEntity#updatedAt.
  Validate: Validate().
  ProcessorConfig: DataProcessing/ProcessorConfig#
  ProcessorConfig.timeout: DataProcessing/ProcessorConfig#timeout.
  unknownValue: unknownValue.
  StringOrNumber: StringOrNumber#
  Callback: Callback#
  UserRole: UserRole#
  HttpStatusCode: HttpStatusCode#
  BaseEntity.createdAt: BaseEntity#createdAt.
  Log: Log().
  AsyncDataProcessor.simulateApiCall: AsyncDataProcessor#simulateApiCall().
  AsyncDataProcessor.processDataStream: AsyncDataProcessor#processDataStream().
  ProcessorConfig.retries: DataProcessing/ProcessorConfig#retries.
  BatchProcessor: DataProcessing/BatchProcessor#
  Application: Application#
  NonNullable: NonNullable#
  ReturnType: ReturnType#
  Required: Required#
  EventName: EventName#
  CSSProperty: CSSProperty#
  AdminUser.lastLogin: AdminUser#lastLogin.
  Permission.resource: Permission#resource.
  Permission.actions: Permission#actions.
  UserRole.GUEST: UserRole#GUEST.
  UserRole.USER: UserRole#USER.
  UserRole.ADMIN: UserRole#ADMIN.
  UserRole.SUPER_ADMIN: UserRole#SUPER_ADMIN.
  HttpStatusCode.OK: HttpStatusCode#OK.
  HttpStatusCode.CREATED: HttpStatusCode#CREATED.
  HttpStatusCode.BAD_REQUEST: HttpStatusCode#BAD_REQUEST.
  HttpStatusCode.UNAUTHORIZED: HttpStatusCode#UNAUTHORIZED.
  HttpStatusCode.NOT_FOUND: HttpStatusCode#NOT_FOUND.
  HttpStatusCode.INTERNAL_SERVER_ERROR: HttpStatusCode#INTERNAL_SERVER_ERROR.
  Direction: Direction#
  Direction.Up: Direction#Up.
  Direction.Down: Direction#Down.
  Direction.Left: Direction#Left.
  Direction.Right: Direction#Right.
  ApiResponse: ApiResponse#
  getProperty: getProperty().
  createValidator: createValidator().
  add: add.
  multiply: multiply.
  compose: compose.
---
# Module: [`examples/ComprehensiveTypeScript.ts`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts)

## Classes
### `AdminUser`
- def: [`examples/ComprehensiveTypeScript.ts:63`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L63)
- signature: `interface AdminUser`
- members:
  - `lastLogin` — [`L65`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L65)
  - `permissions` — [`L64`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L64)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (3 test-only callers)

### `ApiResponse`
- def: [`examples/ComprehensiveTypeScript.ts:294`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L294)
- signature: `type ApiResponse`

### `Application`
- def: [`examples/ComprehensiveTypeScript.ts:442`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L442)
- doc: アプリケーションのメインクラス
- signature: `class Application`
- members:
  - `<constructor>()` — [`L447`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L447) — アプリケーションのメインクラス
  - `demonstrateStreamProcessing(method)` — [`L529`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L529) — データストリーム処理のデモ (Data stream processing demo)
  - `demonstrateUserSearch(method)` — [`L515`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L515) — ユーザー検索のデモ (User search demo)
  - `initialize(method)` — [`L473`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L473) — アプリケーションの初期化
  - `setupEventHandlers(method)` — [`L459`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L459)
  - `batchProcessor` — [`L445`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L445)
  - `dataProcessor` — [`L444`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L444)
  - `userService` — [`L443`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L443)
- uses (calls/refs, reference-scoped): (25 test-only callers)
- used by: (2 test-only callers)

### `AsyncDataProcessor`
- def: [`examples/ComprehensiveTypeScript.ts:311`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L311)
- doc: 非同期データ処理クラス
- signature: `class AsyncDataProcessor`
- members:
  - `fetchData(method)` — [`L318`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L318) — データを非同期で取得
  - `fetchMultipleData(method)` — [`L350`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L350) — 複数のデータを並行取得
  - `processDataStream(method)` — [`L358`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L358) — ジェネレーター関数 (Generator function)
  - `simulateApiCall(method)` — [`L334`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L334)
  - `cache` — [`L312`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L312)
- used by: (4 test-only callers)

### `BaseEntity`
- def: [`examples/ComprehensiveTypeScript.ts:123`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L123)
- doc: 抽象基底クラス
- signature: `class BaseEntity`
- members:
  - `<constructor>(id: string)` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L128) — 抽象基底クラス
  - `getId(method)` — [`L140`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L140)
  - `updateTimestamp(method)` — [`L136`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L136)
  - `validate(method)` — [`L134`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L134)
  - `createdAt` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L125)
  - `id` — [`L124`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L124)
  - `updatedAt` — [`L126`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L126)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `BatchProcessor`
- def: [`examples/ComprehensiveTypeScript.ts:376`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L376)
- signature: `class BatchProcessor`
- members:
  - `<constructor>(config: ProcessorConfig)` — [`L379`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L379)
  - `createBatches(method)` — [`L395`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L395)
  - `processBatch(method)` — [`L383`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L383)
  - `processSingleBatch(method)` — [`L403`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L403)
  - `config` — [`L377`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L377)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (3 test-only callers)

### `CSSProperty`
- def: [`examples/ComprehensiveTypeScript.ts:39`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L39)
- signature: `type CSSProperty`

### `Callback`
- def: [`examples/ComprehensiveTypeScript.ts:22`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L22)
- signature: `type Callback`
- used by: (1 test-only callers)

### `Direction`
- def: [`examples/ComprehensiveTypeScript.ts:110`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L110)
- signature: `enum Direction`
- members:
  - `Down` — [`L112`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L112)
  - `Left` — [`L113`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L113)
  - `Right` — [`L114`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L114)
  - `Up` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L111)

### `EventHandler`
- def: [`examples/ComprehensiveTypeScript.ts:82`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L82)
- signature: `interface EventHandler`
- used by: (3 test-only callers)

### `EventName`
- def: [`examples/ComprehensiveTypeScript.ts:38`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L38)
- signature: `type EventName`

### `HttpStatusCode`
- def: [`examples/ComprehensiveTypeScript.ts:100`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L100)
- signature: `enum HttpStatusCode`
- members:
  - `BAD_REQUEST` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L103)
  - `CREATED` — [`L102`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L102)
  - `INTERNAL_SERVER_ERROR` — [`L106`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L106)
  - `NOT_FOUND` — [`L105`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L105)
  - `OK` — [`L101`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L101)
  - `UNAUTHORIZED` — [`L104`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L104)
- used by: (1 test-only callers)

### `NonNullable`
- def: [`examples/ComprehensiveTypeScript.ts:25`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L25)
- signature: `type NonNullable`

### `Partial`
- def: [`examples/ComprehensiveTypeScript.ts:29`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L29)
- signature: `type Partial`
- used by: (3 test-only callers)

### `Permission`
- def: [`examples/ComprehensiveTypeScript.ts:68`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L68)
- signature: `interface Permission`
- members:
  - `actions` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L70)
  - `resource` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L69)
- used by: (2 test-only callers)

### `ProcessorConfig`
- def: [`examples/ComprehensiveTypeScript.ts:370`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L370)
- signature: `interface ProcessorConfig`
- members:
  - `batchSize` — [`L371`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L371)
  - `retries` — [`L373`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L373)
  - `timeout` — [`L372`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L372)
- used by: (5 test-only callers)

### `Repository`
- def: [`examples/ComprehensiveTypeScript.ts:74`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L74)
- signature: `interface Repository`
- members:
  - `delete(method)` — [`L77`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L77)
  - `findAll(method)` — [`L78`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L78)
  - `findById(method)` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L75)
  - `save(method)` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L76)
- uses (calls/refs, reference-scoped): (6 test-only callers)
- used by: (2 test-only callers)

### `Required`
- def: [`examples/ComprehensiveTypeScript.ts:33`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L33)
- signature: `type Required`

### `ReturnType`
- def: [`examples/ComprehensiveTypeScript.ts:26`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L26)
- signature: `type ReturnType`

### `StringOrNumber`
- def: [`examples/ComprehensiveTypeScript.ts:20`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L20)
- signature: `type StringOrNumber`
- used by: (1 test-only callers)

### `User`
- def: [`examples/ComprehensiveTypeScript.ts:47`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L47)
- doc: ユーザー情報を表すインターフェース
- signature: `interface User`
- members:
  - `age` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L51)
  - `email` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L50)
  - `id` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L48)
  - `name` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L49)
  - `preferences` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L52)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (19 test-only callers)

### `UserID`
- def: [`examples/ComprehensiveTypeScript.ts:21`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L21)
- signature: `type UserID`
- used by: (2 test-only callers)

### `UserKeys`
- def: [`examples/ComprehensiveTypeScript.ts:290`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L290)
- signature: `type UserKeys`
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `UserPreferences`
- def: [`examples/ComprehensiveTypeScript.ts:56`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L56)
- signature: `interface UserPreferences`
- members:
  - `language` — [`L58`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L58)
  - `notifications` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L59)
  - `theme` — [`L57`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L57)
- used by: (3 test-only callers)

### `UserRole`
- def: [`examples/ComprehensiveTypeScript.ts:92`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L92)
- doc: ユーザーの役割を表す列挙型
- signature: `enum UserRole`
- members:
  - `ADMIN` — [`L95`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L95)
  - `GUEST` — [`L93`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L93)
  - `SUPER_ADMIN` — [`L96`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L96)
  - `USER` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L94)
- used by: (1 test-only callers)

### `UserService`  ·  implements/extends BaseEntity, Repository
- def: [`examples/ComprehensiveTypeScript.ts:149`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L149)
- doc: ユーザーサービスクラス
- signature: `class UserService`
- members:
  - `delete(method)` — [`L193`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L193)
  - `findAll(method)` — [`L201`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L201)
  - `findById(method)` — [`L169`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L169)
  - `getInstance(method)` — [`L161`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L161)
  - `onUserDeleted(method)` — [`L225`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L225)
  - `onUserSaved(method)` — [`L221`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L221)
  - `save(method)` — [`L175`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L175)
  - `validate(method)` — [`L216`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L216)
  - `eventEmitter` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L152)
  - `instance` — [`L150`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L150)
  - `users` — [`L151`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L151)
- uses (calls/refs, reference-scoped): (6 test-only callers)
- used by: (14 test-only callers)

### `UserUpdate`
- def: [`examples/ComprehensiveTypeScript.ts:289`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L289)
- signature: `type UserUpdate`
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `UserValues`
- def: [`examples/ComprehensiveTypeScript.ts:291`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L291)
- signature: `type UserValues`
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `ValidatedUser`
- def: [`examples/ComprehensiveTypeScript.ts:273`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L273)
- signature: `class ValidatedUser`
- members:
  - `greet(method)` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L281)
  - `age` — [`L278`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L278)
  - `name` — [`L275`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L275)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

## Functions
- `Log(target: any, propertyName: string, descriptor: PropertyDescriptor)` — [`L236`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L236) — ログ出力デコレーター
- `Validate(validator: (value: any) => boolean)` — [`L251`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L251) — バリデーションデコレーター
- `createValidator(predicate: (value: T) => boolean, errorMessage: string)` — [`L417`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L417) — 高階関数の例 (Higher-order function example)
- `getProperty(obj: T, key: K)` — [`L301`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L301)
- `handleUser(user: User | AdminUser)` — [`L589`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L589)
- `isAdminUser(user: User)` — [`L584`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L584)
- `isUser(obj: any)` — [`L577`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L577)
- `main()` — [`L599`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L599)
- `processUser(user: User)` — [`L571`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L571)

## Module values
- `add` — [`L430`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L430)
- `anotherStringValue` — [`L568`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L568)
- `compose` — [`L434`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L434)
- `multiply` — [`L431`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L431)
- `stringValue` — [`L567`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L567)
- `unknownValue` — [`L566`](../../../../../raw/code/tree-sitter-analyzer/examples/ComprehensiveTypeScript.ts#L566)

