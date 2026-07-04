---
title: SQLite Adapter — Insulating the Query Layer from the SQLite Driver
type: concept
provenance: mixed
concept: db-sqlite-adapter.ts
updated: 2026-07-04
status: fresh
---
# SQLite Adapter — Insulating the Query Layer from the SQLite Driver

## Overview
`sqlite-adapter.ts` is the seam between codegraph's storage layer and whichever
SQLite binding actually executes the SQL. It defines two interfaces —
[`SqliteDatabase`](../catalog/src/db/sqlite-adapter.ts.md#SqliteDatabase) and
[`SqliteStatement`](../catalog/src/db/sqlite-adapter.ts.md#SqliteStatement) —
shaped after the popular `better-sqlite3` native binding's API, plus one
concrete implementation, `NodeSqliteAdapter`, that satisfies that shape by
wrapping Node's built-in `node:sqlite` (`DatabaseSync`). Everything else in
`src/db/` — the entire prepared-statement query layer and the
connection/migration bootstrap — is written against the interface type, never
against a concrete driver: `queries.ts`'s [`db`](../catalog/src/db/queries.ts.md#QueryBuilder.db)
property is typed `SqliteDatabase`, and every one of its dozens of methods
([`insertNode`](../catalog/src/db/queries.ts.md#QueryBuilder.insertNode),
[`getNodeById`](../catalog/src/db/queries.ts.md#QueryBuilder.getNodeById),
[`getOutgoingEdges`](../catalog/src/db/queries.ts.md#QueryBuilder.getOutgoingEdges),
and so on) calls `db.`[`prepare`](../catalog/src/db/sqlite-adapter.ts.md#SqliteDatabase.prepare)`(...)`
without knowing or caring which SQLite is underneath. The payoff already
happened once: codegraph's own `BUNDLING.md` records that the project dropped
the native `better-sqlite3` addon *and* an earlier wasm fallback in favor of
the zero-native-build `node:sqlite` module — a driver swap that, because of
this file, touched exactly one module instead of every call site in `src/db/`.

## Diagram
```mermaid
classDiagram
    class SqliteDatabase {
        <<interface>>
        +prepare(sql) SqliteStatement
        +exec(sql)
        +pragma(str, options)
        +transaction(fn)
        +close()
        +open: boolean
    }
    class SqliteStatement {
        <<interface>>
        +run(...params)
        +get(...params)
        +all(...params)
        +iterate(...params)
    }
    class NodeSqliteAdapter {
        -_db: DatabaseSync
        +prepare(sql) SqliteStatement
    }
    NodeSqliteAdapter ..|> SqliteDatabase : implements
    SqliteDatabase --> SqliteStatement : prepare() returns
    QueryBuilder --> SqliteDatabase : db property
    DatabaseConnection --> SqliteDatabase : db property
    NodeSqliteAdapter --> DatabaseSync : wraps node:sqlite
```

## Design rationale (why it's built this way)
The obvious first guess about a "SQLite adapter" file is that it exists so the
tool can swap between a native binding and a bundled/WASM one at runtime,
matching the README's "100% local, no native build required" pitch. Reading
the file corrects that: **there is currently exactly one implementation.**
The header comment is explicit — "CodeGraph ships with a bundled Node runtime,
so `node:sqlite`... is always available — there is no native build step and
no wasm fallback" — and the `SqliteBackend` type is a union of one string
literal (`'node-sqlite'`), annotated "Only one now... kept as a named type so
`codegraph status` and the per-instance reporting have a stable shape." So the
guess is right about *history*, wrong about the *present*: `BUNDLING.md`
confirms codegraph used to ship `better-sqlite3` (a native addon requiring a
per-platform compiled binary) with a wasm fallback for when the native build
failed — and that the wasm path was itself a source of bugs ("no more
`database is locked`", issue #238). The interface predates the swap to
`node:sqlite`, and the swap is exactly what it was built to absorb: because
[`SqliteDatabase`](../catalog/src/db/sqlite-adapter.ts.md#SqliteDatabase) and
[`SqliteStatement`](../catalog/src/db/sqlite-adapter.ts.md#SqliteStatement)
were already the vocabulary every other file used, retiring two backends for
one new one meant rewriting only `NodeSqliteAdapter`, not `queries.ts`,
`index.ts`, or `migrations.ts`.

The interface is deliberately shaped like `better-sqlite3`'s API rather than
`node:sqlite`'s native shape (which exposes `isOpen` instead of `open`, and
has no `.pragma()` or `.transaction()` convenience methods at all) — so
`NodeSqliteAdapter` absorbs every naming/ergonomics mismatch in one place:
its `open` getter reads `this._db.isOpen`, its `pragma()` hand-parses
write-vs-read pragmas and re-implements better-sqlite3's `{ simple: true }`
single-value convenience, and its `transaction()` hand-rolls a
`BEGIN`/`COMMIT`/`ROLLBACK` wrapper that `node:sqlite` doesn't provide
natively. None of these three methods carry their own graph nodes in this
packet's subgraph (only [`prepare`](../catalog/src/db/sqlite-adapter.ts.md#NodeSqliteAdapter.prepare)
does), but they're visible directly in the source and are the concrete price
this file pays so callers don't have to know `node:sqlite` exists.

> [!inferred] The `SqliteBackend` union staying at one member, rather than
> being collapsed to a plain string, reads as leaving room for a future
> second backend (e.g. an in-memory or WASM path for a sandboxed target)
> rather than pure naming inertia — but nothing in the source or docs commits
> to that plan.

## Entry points
- [`prepare`](../catalog/src/db/sqlite-adapter.ts.md#SqliteDatabase.prepare) — the single interface method every caller in `src/db/` invokes to get a statement handle; it is the front door of the whole adapter, and virtually every read or write in the query layer starts by calling it.
- [`prepare`](../catalog/src/db/sqlite-adapter.ts.md#NodeSqliteAdapter.prepare) — the concrete override that runs when the interface method above is invoked at runtime. The packet's subgraph marks the edge from the interface method to this one as `(virtual)` — a dynamic-dispatch edge recovered by class-hierarchy analysis rather than a static call — which is exactly the base→override binding this file exists to hide from callers.
- [`db`](../catalog/src/db/queries.ts.md#QueryBuilder.db) — the property that hands a `SqliteDatabase` to the ~40 `QueryBuilder` methods making up codegraph's SQL surface, including [`insertNode`](../catalog/src/db/queries.ts.md#QueryBuilder.insertNode), [`getOutgoingEdges`](../catalog/src/db/queries.ts.md#QueryBuilder.getOutgoingEdges), and [`searchNodes`](../catalog/src/db/queries.ts.md#QueryBuilder.searchNodes); control reaches the adapter here on every graph read or write.
- [`initialize`](../catalog/src/db/index.ts.md#DatabaseConnection.initialize) — where a project's database connection is first constructed, calling [`getCurrentVersion`](../catalog/src/db/migrations.ts.md#getCurrentVersion) and `prepare` against a fresh `SqliteDatabase` before any query-layer code runs.

## Mechanism (step-by-step)
1. [`SqliteDatabase`](../catalog/src/db/sqlite-adapter.ts.md#SqliteDatabase) and [`SqliteStatement`](../catalog/src/db/sqlite-adapter.ts.md#SqliteStatement) fix the vocabulary the rest of the db layer is allowed to use — a connection is something with `prepare`/`exec`/`pragma`/`transaction`/`close`/`open`, and a prepared statement is something with `run`/`get`/`all`/`iterate`. Nothing downstream imports a driver-specific type; it imports these two interfaces.
2. `NodeSqliteAdapter`'s [`prepare`](../catalog/src/db/sqlite-adapter.ts.md#NodeSqliteAdapter.prepare) implements the contract by asking `node:sqlite` for a real prepared statement, then wrapping it in a plain object whose `run`, `get`, and `all` methods forward to it — `all` in particular satisfies [`SqliteStatement`](../catalog/src/db/sqlite-adapter.ts.md#SqliteStatement)'s [`all`](../catalog/src/db/sqlite-adapter.ts.md#SqliteStatement.all) member one-for-one, since `node:sqlite`'s own `all()` already returns the same shape better-sqlite3's callers expect.
3. `QueryBuilder` never sees `node:sqlite` at all: its [`db`](../catalog/src/db/queries.ts.md#QueryBuilder.db) field is typed `SqliteDatabase`, and its query methods — [`insertNode`](../catalog/src/db/queries.ts.md#QueryBuilder.insertNode), [`updateNode`](../catalog/src/db/queries.ts.md#QueryBuilder.updateNode), [`getNodeById`](../catalog/src/db/queries.ts.md#QueryBuilder.getNodeById), [`getIncomingEdges`](../catalog/src/db/queries.ts.md#QueryBuilder.getIncomingEdges), [`searchNodesFTS`](../catalog/src/db/queries.ts.md#QueryBuilder.searchNodesFTS), and dozens more — all reach SQLite exclusively by calling `this.db.prepare(...)`. This is the payoff of step 1: the entire SQL surface of codegraph is one `db.prepare()` call away from being driver-agnostic.
4. The connection/migration bootstrap is written against the same interface, not a parallel one: [`initialize`](../catalog/src/db/index.ts.md#DatabaseConnection.initialize) and migrations.ts's [`runMigrations`](../catalog/src/db/migrations.ts.md#runMigrations), [`getCurrentVersion`](../catalog/src/db/migrations.ts.md#getCurrentVersion), and [`getPendingMigrations`](../catalog/src/db/migrations.ts.md#getPendingMigrations) all take or hold a `SqliteDatabase` parameter, so schema versioning shares the exact same seam as row-level queries.
5. `SqliteStatement`'s `iterate` member exists as a deliberate escape hatch from `all`: its own doc comment explains it's for unbounded scans so memory stays O(1) rather than O(rows), citing a real production incident (#610) where `all()`-ing every symbol on a dense project spiked the heap into an OOM. Consumers pick accordingly — [`getAllNodes`](../catalog/src/db/queries.ts.md#QueryBuilder.getAllNodes) and most lookups use `all`, while [`iterateNodesByKind`](../catalog/src/db/queries.ts.md#QueryBuilder.iterateNodesByKind) (whose own doc says "Stream every node of a kind one at a time (lazy) instead of materializing") uses `iterate` for exactly the scan pattern the comment warns about.

## Key data structures
- [`SqliteDatabase`](../catalog/src/db/sqlite-adapter.ts.md#SqliteDatabase) — a six-member contract (`prepare`, `exec`, `pragma`, `transaction`, `close`, `open`) standing in for "a database connection" everywhere in `src/db/`. `NodeSqliteAdapter` is currently its only implementer.
- [`SqliteStatement`](../catalog/src/db/sqlite-adapter.ts.md#SqliteStatement) — a four-member contract (`run`, `get`, `all`, `iterate`) standing in for "a prepared statement." The `all`/`iterate` split is the materialized-vs-streaming choice every scan-heavy query method has to make.
- [`db`](../catalog/src/db/queries.ts.md#QueryBuilder.db) and [`db`](../catalog/src/db/index.ts.md#DatabaseConnection.db) — the two places that actually hold a live `SqliteDatabase` instance, one per `QueryBuilder` and one per `DatabaseConnection`. Neither is a module-level singleton.
- [`openedInode`](../catalog/src/db/index.ts.md#DatabaseConnection.openedInode) — a `DatabaseConnection` field recording the `dev:ino` of the DB file at open time, sitting alongside `db` as per-connection state used to notice if the underlying file has since been replaced.

## Dynamics (design intent)
`node:sqlite`'s `DatabaseSync` is, as the name implies, fully synchronous —
every `SqliteStatement` method blocks the caller until SQLite returns, so
there is no interleaving to reason about within a single adapter instance.
The interface is instantiated per connection rather than as a process
singleton: `index.ts`
(the `DatabaseConnection` module) constructs and holds its own `db`, and
`QueryBuilder`'s [`db`](../catalog/src/db/queries.ts.md#QueryBuilder.db) is
likewise instance state, not a shared global.

> [!inferred] Reading the source directly (not the subgraph): the adapter's
> factory function documents that this per-instance design is deliberate
> because an MCP server process can have more than one project's database
> open at once, and a process-global connection would race across them. The
> factory itself isn't a subgraph symbol in this packet, so it's noted here
> rather than cited.

> [!inferred] `NodeSqliteAdapter`'s `transaction()` is a hand-rolled
> `BEGIN`/`COMMIT`/`ROLLBACK` wrapper, not `better-sqlite3`'s native
> transaction implementation — which also handles `SAVEPOINT`-based nesting.
> Whether a nested `transaction()` call (a transaction started from inside
> another) behaves correctly here isn't something this file or packet settles
> statically.

## Edge cases
- `close()` is written to be idempotent — it checks the underlying `isOpen`
  flag before calling into `node:sqlite`, because `DatabaseSync.close()`
  throws if the database is already closed, while callers elsewhere are
  allowed to close more than once.
- `run()`'s return value is defensively normalized (`Number(...)` on
  `changes`, defaulting `lastInsertRowid` to `0`) rather than passed through
  raw, suggesting the author didn't fully trust `node:sqlite`'s result shape
  to always populate both fields.
- `pragma()` branches purely on whether the input string contains `=` to
  decide "write" vs "read" pragma — a string-shape check, not a schema-aware
  parse, so a pragma name that happens to contain `=` in an unexpected
  position would misroute.
- The factory that constructs the adapter wraps the `require('node:sqlite')`
  call in a try/catch and rethrows a friendlier, actionable error naming
  Node 22.5+ or the bundled release — so an old-Node failure surfaces as
  guidance rather than a raw `MODULE_NOT_FOUND`.

## Open questions
- Is a second `SqliteBackend` value actually planned, or is the union type
  purely a vestige of the pre-`node:sqlite` era described in `BUNDLING.md`?
  Neither this file nor the packet's subgraph says.
- Does `NodeSqliteAdapter#transaction` support reentrant/nested calls the way
  `better-sqlite3`'s native `.transaction()` does? Not verifiable from this
  file alone.
- The many call sites recorded as "called by: all" (and similarly for
  `prepare`) in the subgraph's edge counts suggest very high fan-in from the
  query layer, but the packet doesn't resolve them to distinct named callers
  beyond what's cited above — a finer-grained caller breakdown would need the
  full `queries.ts` packet.

## See also
- [QueryBuilder — CodeGraph's SQL Query & Search Layer](db-queries.ts.md) — the module that consumes this adapter on nearly every line; if `SqliteDatabase`/`SqliteStatement` is the seam, `QueryBuilder` is the seam's heaviest user.
- [The Node/Edge graph model](types.ts.md) — the `Node`/`Edge` records that `QueryBuilder` reads and writes through this adapter; this file is agnostic to their shape, but they're what ultimately rides over `prepare`/`all`/`run`.
- [mcp-daemon.ts.md](mcp-daemon.ts.md) — the background daemon that keeps a project's database warm across MCP calls is the concrete reason a `SqliteDatabase` is constructed per-connection instead of as a process-global.
- [mcp-query-pool.ts.md](mcp-query-pool.ts.md) — a worker pool serving MCP queries is another consumer for which "one `SqliteDatabase` per connection, not a shared singleton" is load-bearing rather than incidental.
