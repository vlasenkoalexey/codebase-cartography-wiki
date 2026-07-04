---
title: 'Module: src/db/index.ts'
type: catalog
provenance: extracted
module: src/db/index.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/db/`index.ts`/
symbols:
  DatabaseConnection.initialize: DatabaseConnection#initialize().
  DatabaseConnection.open: DatabaseConnection#open().
  DatabaseConnection.openedInode: DatabaseConnection#openedInode.
  DatabaseConnection.db: DatabaseConnection#db.
  DatabaseConnection: DatabaseConnection#
  getDatabasePath: getDatabasePath().
  DatabaseConnection.getDb: DatabaseConnection#getDb().
  DatabaseConnection.getSchemaVersion: DatabaseConnection#getSchemaVersion().
  DatabaseConnection.isReplacedOnDisk: DatabaseConnection#isReplacedOnDisk().
  configureConnection: configureConnection().
  DatabaseConnection.runMaintenance: DatabaseConnection#runMaintenance().
  DatabaseConnection.close: DatabaseConnection#close().
  DatabaseConnection.getBackend: DatabaseConnection#getBackend().
  DatabaseConnection.getJournalMode: DatabaseConnection#getJournalMode().
  DatabaseConnection.optimize: DatabaseConnection#optimize().
  DatabaseConnection.transaction: DatabaseConnection#transaction().
  DatabaseConnection.isOpen: DatabaseConnection#isOpen().
  DatabaseConnection.backend: DatabaseConnection#backend.
  removeDatabaseFiles: removeDatabaseFiles().
  DatabaseConnection.dbPath: DatabaseConnection#dbPath.
  DatabaseConnection.getPath: DatabaseConnection#getPath().
  DatabaseConnection.getSize: DatabaseConnection#getSize().
  statInode: statInode().
  DATABASE_FILENAME: DATABASE_FILENAME.
  WAL_SIDECAR_SUFFIXES: WAL_SIDECAR_SUFFIXES.
---
# Module: [`src/db/index.ts`](../../../../../../raw/code/codegraph/src/db/index.ts)

## Classes
### `DatabaseConnection`
- def: [`src/db/index.ts:43`](../../../../../../raw/code/codegraph/src/db/index.ts#L43)
- doc: Database connection wrapper with lifecycle management
- signature: `class DatabaseConnection`
- members:
  - `close(method)` — [`L233`](../../../../../../raw/code/codegraph/src/db/index.ts#L233) — Close the database connection
  - `getBackend(method)` — [`L130`](../../../../../../raw/code/codegraph/src/db/index.ts#L130) — Get the SQLite backend serving this connection. Per-instance so
  - `getDb(method)` — [`L121`](../../../../../../raw/code/codegraph/src/db/index.ts#L121) — Get the underlying database instance
  - `getJournalMode(method)` — [`L151`](../../../../../../raw/code/codegraph/src/db/index.ts#L151) — The journal mode actually in effect (e.g. 'wal', 'delete').
  - `getPath(method)` — [`L137`](../../../../../../raw/code/codegraph/src/db/index.ts#L137) — Get database file path
  - `getSchemaVersion(method)` — [`L163`](../../../../../../raw/code/codegraph/src/db/index.ts#L163) — Get current schema version
  - `getSize(method)` — [`L187`](../../../../../../raw/code/codegraph/src/db/index.ts#L187) — Get database file size in bytes
  - `initialize(method)` — [`L67`](../../../../../../raw/code/codegraph/src/db/index.ts#L67) — Initialize a new database at the given path — documented in [db-sqlite-adapter.ts](../../../concepts/db-sqlite-adapter.ts.md)
  - `isOpen(method)` — [`L240`](../../../../../../raw/code/codegraph/src/db/index.ts#L240) — Check if the database connection is open
  - `isReplacedOnDisk(method)` — [`L255`](../../../../../../raw/code/codegraph/src/db/index.ts#L255) — True when the DB file at our path has been REPLACED on disk since we opened
  - `open(method)` — [`L98`](../../../../../../raw/code/codegraph/src/db/index.ts#L98) — Open an existing database
  - `optimize(method)` — [`L195`](../../../../../../raw/code/codegraph/src/db/index.ts#L195) — Optimize database (vacuum and analyze)
  - `runMaintenance(method)` — [`L217`](../../../../../../raw/code/codegraph/src/db/index.ts#L217) — Lightweight, non-blocking maintenance to run after bulk writes
  - `transaction(method)` — [`L180`](../../../../../../raw/code/codegraph/src/db/index.ts#L180) — Execute a function within a transaction
  - `backend` — [`L46`](../../../../../../raw/code/codegraph/src/db/index.ts#L46)
  - `db` — [`L44`](../../../../../../raw/code/codegraph/src/db/index.ts#L44) — documented in [db-sqlite-adapter.ts](../../../concepts/db-sqlite-adapter.ts.md)
  - `dbPath` — [`L45`](../../../../../../raw/code/codegraph/src/db/index.ts#L45)
  - `openedInode` — [`L55`](../../../../../../raw/code/codegraph/src/db/index.ts#L55) — `dev:ino` of the DB file at the moment we opened it (or null when the — documented in [db-sqlite-adapter.ts](../../../concepts/db-sqlite-adapter.ts.md)
- uses (calls/refs, reference-scoped): [`prepare`](sqlite-adapter.ts.md#SqliteDatabase.prepare), [`SqliteDatabase`](sqlite-adapter.ts.md#SqliteDatabase), [`exec`](sqlite-adapter.ts.md#SqliteDatabase.exec), [`runMigrations`](migrations.ts.md#runMigrations), [`run`](sqlite-adapter.ts.md#SqliteStatement.run), [`createDatabase`](sqlite-adapter.ts.md#createDatabase), [`getCurrentVersion`](migrations.ts.md#getCurrentVersion), [`transaction`](sqlite-adapter.ts.md#SqliteDatabase.transaction), [`get`](sqlite-adapter.ts.md#SqliteStatement.get), [`pragma`](sqlite-adapter.ts.md#SqliteDatabase.pragma), [`configureConnection`](index.ts.md#configureConnection), [`SqliteBackend`](sqlite-adapter.ts.md#SqliteBackend), [`db`](sqlite-adapter.ts.md#createDatabase.typeLiteral47.db), [`CURRENT_SCHEMA_VERSION`](migrations.ts.md#CURRENT_SCHEMA_VERSION), [`close`](sqlite-adapter.ts.md#SqliteDatabase.close), [`backend`](sqlite-adapter.ts.md#createDatabase.typeLiteral47.backend), [`SchemaVersion`](../types.ts.md#SchemaVersion), [`statInode`](index.ts.md#statInode), [`open`](sqlite-adapter.ts.md#SqliteDatabase.open)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-index.ts), [`indexAll`](../index.ts.md#CodeGraph.indexAll), [`sync`](../index.ts.md#CodeGraph.sync), [`open`](../index.ts.md#CodeGraph.open), [`watcher`](../index.ts.md#CodeGraph.watcher), [`init`](../index.ts.md#CodeGraph.init), [`openSync`](../index.ts.md#CodeGraph.openSync), [`recreate`](../index.ts.md#CodeGraph.recreate), [`reopenIfReplaced`](../index.ts.md#CodeGraph.reopenIfReplaced), [`getStats`](../index.ts.md#CodeGraph.getStats), [`initSync`](../index.ts.md#CodeGraph.initSync), [`close`](../index.ts.md#CodeGraph.close), [`db`](../index.ts.md#CodeGraph.db), [`getBackend`](../index.ts.md#CodeGraph.getBackend), [`getJournalMode`](../index.ts.md#CodeGraph.getJournalMode), [`optimize`](../index.ts.md#CodeGraph.optimize)

## Functions
- `configureConnection(db: SqliteDatabase)` — [`L30`](../../../../../../raw/code/codegraph/src/db/index.ts#L30) — Apply connection-level PRAGMAs. Shared by `initialize` and `open` so the two
- `getDatabasePath(projectRoot: string)` — [`L294`](../../../../../../raw/code/codegraph/src/db/index.ts#L294) — Get the default database path for a project — documented in [directory.ts](../../../concepts/directory.ts.md)
- `removeDatabaseFiles(dbPath: string)` — [`L317`](../../../../../../raw/code/codegraph/src/db/index.ts#L317) — Delete a database file and its WAL sidecars (`-wal`/`-shm`).
- `statInode(p: string)` — [`L269`](../../../../../../raw/code/codegraph/src/db/index.ts#L269) — `dev:ino` for a path, or null if it can't be stat'd or the platform doesn't

## Module values
- `DATABASE_FILENAME` — [`L282`](../../../../../../raw/code/codegraph/src/db/index.ts#L282) — Default database filename
- `WAL_SIDECAR_SUFFIXES` — [`L289`](../../../../../../raw/code/codegraph/src/db/index.ts#L289) — SQLite's sidecar files in WAL mode — the write-ahead log and its shared-memory

