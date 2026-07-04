---
title: 'Module: tests/fixtures/typescript_advanced.ts'
type: catalog
provenance: extracted
module: tests/fixtures/typescript_advanced.ts
status: fresh
symbol_base: scip-typescript npm . . tests/fixtures/`typescript_advanced.ts`/
symbols:
  UserModule: UserModule#
  UserService.-constructor: UserService#`<constructor>`().
  UserService.getById: UserService#getById().
  UserService: UserService#
  IUserRepository: IUserRepository#
  IUserRepository.findById: IUserRepository#findById().
  USER_REPOSITORY: USER_REPOSITORY.
  IUserRepository.save: IUserRepository#save().
  UserStatus: UserStatus#
  UserStatus.Active: UserStatus#Active.
  UserStatus.Inactive: UserStatus#Inactive.
  UserStatus.Suspended: UserStatus#Suspended.
  UserId: UserId#
  DEFAULT_ROLES: DEFAULT_ROLES.
  USER_CONFIG: USER_CONFIG.
  UserService.create: UserService#create().
  UserService.bulkCreate: UserService#bulkCreate().
---
# Module: [`tests/fixtures/typescript_advanced.ts`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts)

## Classes
### `IUserRepository`
- def: [`tests/fixtures/typescript_advanced.ts:23`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L23)
- signature: `interface IUserRepository`
- members:
  - `findById(method)` — [`L24`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L24)
  - `save(method)` — [`L25`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L25)
- used by: (2 test-only callers)

### `UserId`
- def: [`tests/fixtures/typescript_advanced.ts:34`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L34)
- signature: `type UserId`

### `UserModule`
- def: [`tests/fixtures/typescript_advanced.ts:73`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L73)
- signature: `class UserModule`
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `UserService`
- def: [`tests/fixtures/typescript_advanced.ts:50`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L50)
- signature: `class UserService`
- members:
  - `<constructor>(repo: IUserRepository)` — [`L51`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L51)
  - `bulkCreate(method)` — [`L57`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L57)
  - `create(method)` — [`L53`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L53)
  - `getById(method)` — [`L61`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L61)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `UserStatus`
- def: [`tests/fixtures/typescript_advanced.ts:28`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L28)
- signature: `enum UserStatus`
- members:
  - `Active` — [`L29`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L29)
  - `Inactive` — [`L30`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L30)
  - `Suspended` — [`L31`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L31)

## Module values
- `DEFAULT_ROLES` — [`L38`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L38)
- `USER_CONFIG` — [`L40`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L40)
- `USER_REPOSITORY` — [`L36`](../../../../../../raw/code/graphify/tests/fixtures/typescript_advanced.ts#L36)

