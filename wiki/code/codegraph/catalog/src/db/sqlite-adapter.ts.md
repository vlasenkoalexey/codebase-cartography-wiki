---
title: 'Module: src/db/sqlite-adapter.ts'
type: catalog
provenance: extracted
module: src/db/sqlite-adapter.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/db/`sqlite-adapter.ts`/
symbols:
  SqliteDatabase.prepare: SqliteDatabase#prepare().
  SqliteStatement.all: SqliteStatement#all().
  SqliteStatement: SqliteStatement#
  SqliteDatabase: SqliteDatabase#
  NodeSqliteAdapter.prepare: NodeSqliteAdapter#prepare().
  SqliteDatabase.exec: SqliteDatabase#exec().
  SqliteStatement.run: SqliteStatement#run().
  createDatabase: createDatabase().
  SqliteDatabase.transaction: SqliteDatabase#transaction().
  SqliteStatement.get: SqliteStatement#get().
  NodeSqliteAdapter._db: NodeSqliteAdapter#_db.
  SqliteDatabase.pragma: SqliteDatabase#pragma().
  SqliteBackend: SqliteBackend#
  createDatabase.typeLiteral47.db: createDatabase().typeLiteral47:db.
  NodeSqliteAdapter.pragma: NodeSqliteAdapter#pragma().
  SqliteDatabase.close: SqliteDatabase#close().
  NodeSqliteAdapter.-constructor: NodeSqliteAdapter#`<constructor>`().
  createDatabase.typeLiteral47.backend: createDatabase().typeLiteral47:backend.
  NodeSqliteAdapter: NodeSqliteAdapter#
  NodeSqliteAdapter.-get-open: NodeSqliteAdapter#`<get>open`().
  NodeSqliteAdapter.exec: NodeSqliteAdapter#exec().
  NodeSqliteAdapter.transaction: NodeSqliteAdapter#transaction().
  NodeSqliteAdapter.close: NodeSqliteAdapter#close().
  SqliteStatement.iterate: SqliteStatement#iterate().
  SqliteStatement.run.typeLiteral0.changes: SqliteStatement#run().typeLiteral0:changes.
  SqliteStatement.run.typeLiteral0.lastInsertRowid: SqliteStatement#run().typeLiteral0:lastInsertRowid.
  SqliteDatabase.open: SqliteDatabase#open.
  NodeSqliteAdapter.pragma.options-typeLiteral27.simple: NodeSqliteAdapter#pragma().(options)typeLiteral27:simple.
  SqliteDatabase.pragma.options-typeLiteral1.simple: SqliteDatabase#pragma().(options)typeLiteral1:simple.
---
# Module: [`src/db/sqlite-adapter.ts`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts)

## Classes
### `NodeSqliteAdapter`  ·  implements/extends SqliteDatabase
- def: [`src/db/sqlite-adapter.ts:50`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L50)
- doc: Wraps Node's built-in `node:sqlite` (`DatabaseSync`) to match the
- signature: `class NodeSqliteAdapter`
- members:
  - `<constructor>(dbPath: string)` — [`L53`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L53) — Wraps Node's built-in `node:sqlite` (`DatabaseSync`) to match the
  - `<get>open` — [`L59`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L59)
  - `close(method)` — [`L123`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L123)
  - `exec(method)` — [`L88`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L88)
  - `pragma(method)` — [`L92`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L92)
  - `prepare(method)` — [`L63`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L63) — documented in [db-sqlite-adapter.ts](../../../concepts/db-sqlite-adapter.ts.md)
  - `transaction(method)` — [`L109`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L109)
  - `simple` — [`L92`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L92)
- protocol/private: `_db`[`L51`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L51)
- uses (calls/refs, reference-scoped): [`all`](sqlite-adapter.ts.md#SqliteStatement.all), [`SqliteStatement`](sqlite-adapter.ts.md#SqliteStatement), [`SqliteDatabase`](sqlite-adapter.ts.md#SqliteDatabase), [`run`](sqlite-adapter.ts.md#SqliteStatement.run), [`get`](sqlite-adapter.ts.md#SqliteStatement.get), [`iterate`](sqlite-adapter.ts.md#SqliteStatement.iterate), [`changes`](sqlite-adapter.ts.md#SqliteStatement.run.typeLiteral0.changes), [`lastInsertRowid`](sqlite-adapter.ts.md#SqliteStatement.run.typeLiteral0.lastInsertRowid)
- used by: [`prepare`](sqlite-adapter.ts.md#SqliteDatabase.prepare), [`SqliteDatabase`](sqlite-adapter.ts.md#SqliteDatabase), [`exec`](sqlite-adapter.ts.md#SqliteDatabase.exec), [`createDatabase`](sqlite-adapter.ts.md#createDatabase), [`transaction`](sqlite-adapter.ts.md#SqliteDatabase.transaction), [`pragma`](sqlite-adapter.ts.md#SqliteDatabase.pragma), [`close`](sqlite-adapter.ts.md#SqliteDatabase.close)

### `SqliteBackend`
- def: [`src/db/sqlite-adapter.ts:39`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L39)
- doc: The active SQLite backend. Only one now (`node:sqlite`); kept as a named type
- signature: `type SqliteBackend`
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-db-index.ts), [`openedInode`](index.ts.md#DatabaseConnection.openedInode), [`createDatabase`](sqlite-adapter.ts.md#createDatabase), [`getBackend`](index.ts.md#DatabaseConnection.getBackend), [`backend`](index.ts.md#DatabaseConnection.backend)

### `SqliteDatabase`
- def: [`src/db/sqlite-adapter.ts:26`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L26) — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
- signature: `interface SqliteDatabase`
- members:
  - `close(method)` — [`L31`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L31)
  - `exec(method)` — [`L28`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L28)
  - `pragma(method)` — [`L29`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L29)
  - `prepare(method)` — [`L27`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L27) — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `transaction(method)` — [`L30`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L30)
  - `open` — [`L32`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L32)
  - `simple` — [`L29`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L29)
- uses (calls/refs, reference-scoped): [`SqliteStatement`](sqlite-adapter.ts.md#SqliteStatement), [`prepare`](sqlite-adapter.ts.md#NodeSqliteAdapter.prepare), [`pragma`](sqlite-adapter.ts.md#NodeSqliteAdapter.pragma), [`NodeSqliteAdapter`](sqlite-adapter.ts.md#NodeSqliteAdapter), [`close`](sqlite-adapter.ts.md#NodeSqliteAdapter.close), [`exec`](sqlite-adapter.ts.md#NodeSqliteAdapter.exec), [`transaction`](sqlite-adapter.ts.md#NodeSqliteAdapter.transaction)
- used by: [`searchNodes`](queries.ts.md#QueryBuilder.searchNodes), [`db`](queries.ts.md#QueryBuilder.db), [`queries.ts`](queries.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-db-queries.ts), [`insertNode`](queries.ts.md#QueryBuilder.insertNode), [`updateNode`](queries.ts.md#QueryBuilder.updateNode), [`getNodeById`](queries.ts.md#QueryBuilder.getNodeById), [`getOutgoingEdges`](queries.ts.md#QueryBuilder.getOutgoingEdges), [`getUnresolvedReferencesBatch`](queries.ts.md#QueryBuilder.getUnresolvedReferencesBatch), [`getUnresolvedByName`](queries.ts.md#QueryBuilder.getUnresolvedByName), [`getUnresolvedReferencesByFiles`](queries.ts.md#QueryBuilder.getUnresolvedReferencesByFiles), [`getStats`](queries.ts.md#QueryBuilder.getStats), [`getUnresolvedReferences`](queries.ts.md#QueryBuilder.getUnresolvedReferences), [`getIncomingEdges`](queries.ts.md#QueryBuilder.getIncomingEdges), [`getNodesByKind`](queries.ts.md#QueryBuilder.getNodesByKind), [`getNodesByIds`](queries.ts.md#QueryBuilder.getNodesByIds), [`findNodesByExactName`](queries.ts.md#QueryBuilder.findNodesByExactName), [`insertUnresolvedRef`](queries.ts.md#QueryBuilder.insertUnresolvedRef), [`searchNodesFuzzy`](queries.ts.md#QueryBuilder.searchNodesFuzzy), [`upsertFile`](queries.ts.md#QueryBuilder.upsertFile), [`insertEdge`](queries.ts.md#QueryBuilder.insertEdge), [`index.ts`](index.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-db-index.ts), [`searchNodesFTS`](queries.ts.md#QueryBuilder.searchNodesFTS), [`searchNodesLike`](queries.ts.md#QueryBuilder.searchNodesLike), [`initialize`](index.ts.md#DatabaseConnection.initialize), [`iterateNodesByKind`](queries.ts.md#QueryBuilder.iterateNodesByKind), [`findNodesByNameSubstring`](queries.ts.md#QueryBuilder.findNodesByNameSubstring), [`insertEdges`](queries.ts.md#QueryBuilder.insertEdges), [`getAllFiles`](queries.ts.md#QueryBuilder.getAllFiles), [`insertNameSegments`](queries.ts.md#QueryBuilder.insertNameSegments), [`getFileByPath`](queries.ts.md#QueryBuilder.getFileByPath), [`getNodesByName`](queries.ts.md#QueryBuilder.getNodesByName), [`searchAllByFilters`](queries.ts.md#QueryBuilder.searchAllByFilters), [`getNodesByFile`](queries.ts.md#QueryBuilder.getNodesByFile), [`getNodesByQualifiedNameExact`](queries.ts.md#QueryBuilder.getNodesByQualifiedNameExact), [`getNodesByLowerName`](queries.ts.md#QueryBuilder.getNodesByLowerName), [`deleteSpecificResolvedReferences`](queries.ts.md#QueryBuilder.deleteSpecificResolvedReferences), [`openedInode`](index.ts.md#DatabaseConnection.openedInode), [`deleteFile`](queries.ts.md#QueryBuilder.deleteFile), [`runMigrations`](migrations.ts.md#runMigrations), [`deleteNodesByFile`](queries.ts.md#QueryBuilder.deleteNodesByFile)  (+53 more)

### `SqliteStatement`
- def: [`src/db/sqlite-adapter.ts:13`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L13) — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
- doc: SQLite Adapter
- signature: `interface SqliteStatement`
- members:
  - `all(method)` — [`L16`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L16) — documented in [db-queries.ts](../../../concepts/db-queries.ts.md)
  - `get(method)` — [`L15`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L15)
  - `iterate(method)` — [`L23`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L23) — Lazily yield result rows one at a time instead of materializing the whole
  - `run(method)` — [`L14`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L14)
  - `changes` — [`L14`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L14)
  - `lastInsertRowid` — [`L14`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L14)
- used by: [`searchNodes`](queries.ts.md#QueryBuilder.searchNodes), [`queries.ts`](queries.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-db-queries.ts), [`insertNode`](queries.ts.md#QueryBuilder.insertNode), [`updateNode`](queries.ts.md#QueryBuilder.updateNode), [`prepare`](sqlite-adapter.ts.md#SqliteDatabase.prepare), [`getNodeById`](queries.ts.md#QueryBuilder.getNodeById), [`getOutgoingEdges`](queries.ts.md#QueryBuilder.getOutgoingEdges), [`getUnresolvedReferencesBatch`](queries.ts.md#QueryBuilder.getUnresolvedReferencesBatch), [`getUnresolvedByName`](queries.ts.md#QueryBuilder.getUnresolvedByName), [`getUnresolvedReferencesByFiles`](queries.ts.md#QueryBuilder.getUnresolvedReferencesByFiles), [`getStats`](queries.ts.md#QueryBuilder.getStats), [`getUnresolvedReferences`](queries.ts.md#QueryBuilder.getUnresolvedReferences), [`getIncomingEdges`](queries.ts.md#QueryBuilder.getIncomingEdges), [`getNodesByKind`](queries.ts.md#QueryBuilder.getNodesByKind), [`getNodesByIds`](queries.ts.md#QueryBuilder.getNodesByIds), [`findNodesByExactName`](queries.ts.md#QueryBuilder.findNodesByExactName), [`insertUnresolvedRef`](queries.ts.md#QueryBuilder.insertUnresolvedRef), [`searchNodesFuzzy`](queries.ts.md#QueryBuilder.searchNodesFuzzy), [`upsertFile`](queries.ts.md#QueryBuilder.upsertFile), [`insertEdge`](queries.ts.md#QueryBuilder.insertEdge), [`searchNodesFTS`](queries.ts.md#QueryBuilder.searchNodesFTS), [`searchNodesLike`](queries.ts.md#QueryBuilder.searchNodesLike), [`initialize`](index.ts.md#DatabaseConnection.initialize), [`iterateNodesByKind`](queries.ts.md#QueryBuilder.iterateNodesByKind), [`findNodesByNameSubstring`](queries.ts.md#QueryBuilder.findNodesByNameSubstring), [`getAllFiles`](queries.ts.md#QueryBuilder.getAllFiles), [`insertNameSegments`](queries.ts.md#QueryBuilder.insertNameSegments), [`getFileByPath`](queries.ts.md#QueryBuilder.getFileByPath), [`getNodesByName`](queries.ts.md#QueryBuilder.getNodesByName), [`searchAllByFilters`](queries.ts.md#QueryBuilder.searchAllByFilters), [`getNodesByFile`](queries.ts.md#QueryBuilder.getNodesByFile), [`getNodesByQualifiedNameExact`](queries.ts.md#QueryBuilder.getNodesByQualifiedNameExact), [`getNodesByLowerName`](queries.ts.md#QueryBuilder.getNodesByLowerName), [`deleteSpecificResolvedReferences`](queries.ts.md#QueryBuilder.deleteSpecificResolvedReferences), [`prepare`](sqlite-adapter.ts.md#NodeSqliteAdapter.prepare), [`deleteFile`](queries.ts.md#QueryBuilder.deleteFile), [`deleteNodesByFile`](queries.ts.md#QueryBuilder.deleteNodesByFile), [`findEdgesBetweenNodes`](queries.ts.md#QueryBuilder.findEdgesBetweenNodes), [`getCrossFileIncomingEdgesWithTarget`](queries.ts.md#QueryBuilder.getCrossFileIncomingEdgesWithTarget), [`getUnresolvedReferencesCount`](queries.ts.md#QueryBuilder.getUnresolvedReferencesCount)  (+59 more)

## Functions
- `createDatabase(dbPath: string)` — [`L137`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L137) — Create a database connection backed by `node:sqlite`.

## Module values
- `backend` — [`L137`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L137)
- `db` — [`L137`](../../../../../../raw/code/codegraph/src/db/sqlite-adapter.ts#L137)

