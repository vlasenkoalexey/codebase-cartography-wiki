---
title: 'Module: src/db/migrations.ts'
type: catalog
provenance: extracted
module: src/db/migrations.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/db/`migrations.ts`/
symbols:
  runMigrations: runMigrations().
  migrations: migrations.
  Migration.version: Migration#version.
  getCurrentVersion: getCurrentVersion().
  getPendingMigrations: getPendingMigrations().
  recordMigration: recordMigration().
  needsMigration: needsMigration().
  getMigrationHistory: getMigrationHistory().
  Migration.description: Migration#description.
  Migration.up: Migration#up.
  CURRENT_SCHEMA_VERSION: CURRENT_SCHEMA_VERSION.
  Migration: Migration#
  getMigrationHistory.Array.typeLiteral50.version: getMigrationHistory().Array:typeLiteral50:version.
  getMigrationHistory.Array.typeLiteral50.appliedAt: getMigrationHistory().Array:typeLiteral50:appliedAt.
  getMigrationHistory.Array.typeLiteral50.description: getMigrationHistory().Array:typeLiteral50:description.
---
# Module: [`src/db/migrations.ts`](../../../../../../raw/code/codegraph/src/db/migrations.ts)

## Classes
### `Migration`
- def: [`src/db/migrations.ts:17`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L17)
- doc: Migration definition
- signature: `interface Migration`
- members:
  - `description` — [`L19`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L19)
  - `up` — [`L20`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L20)
  - `version` — [`L18`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L18)
- uses (calls/refs, reference-scoped): [`SqliteDatabase`](sqlite-adapter.ts.md#SqliteDatabase)
- used by: [`runMigrations`](migrations.ts.md#runMigrations), [`migrations`](migrations.ts.md#migrations), [`getPendingMigrations`](migrations.ts.md#getPendingMigrations)

## Functions
- `getCurrentVersion(db: SqliteDatabase)` — [`L127`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L127) — Get the current schema version from the database — documented in [db-sqlite-adapter.ts](../../../concepts/db-sqlite-adapter.ts.md)
- `getMigrationHistory(db: SqliteDatabase)` — [`L191`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L191) — Get migration history from database
- `getPendingMigrations(db: SqliteDatabase)` — [`L181`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L181) — Get list of pending migrations — documented in [db-sqlite-adapter.ts](../../../concepts/db-sqlite-adapter.ts.md)
- `needsMigration(db: SqliteDatabase)` — [`L173`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L173) — Check if the database needs migration
- `recordMigration(db: SqliteDatabase, version: number, description: string)` — [`L142`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L142) — Record a migration as applied
- `runMigrations(db: SqliteDatabase, fromVersion: number)` — [`L151`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L151) — Run all pending migrations — documented in [db-sqlite-adapter.ts](../../../concepts/db-sqlite-adapter.ts.md)

## Module values
- `CURRENT_SCHEMA_VERSION` — [`L12`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L12) — Current schema version
- `appliedAt` — [`L193`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L193)
- `description` — [`L193`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L193)
- `migrations` — [`L29`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L29) — All migrations in order
- `version` — [`L193`](../../../../../../raw/code/codegraph/src/db/migrations.ts#L193)

