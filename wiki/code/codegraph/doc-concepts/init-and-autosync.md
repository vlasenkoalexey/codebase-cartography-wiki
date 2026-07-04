---
title: Init, the daemon, and never-stale auto-sync
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Init, the daemon, and never-stale auto-sync

## Definition
CodeGraph's per-project lifecycle is deliberately one-command and self-maintaining. `codegraph init` creates the local `.codegraph/` directory **and** builds the full graph in the same step. From then on **auto-sync is on by default**: a native OS file watcher (FSEvents / inotify / ReadDirectoryChangesW) sees every create/modify/delete, debounces, and incrementally re-indexes — so "the index is never stale, and there is nothing to re-run." Indexing is always the *user's* decision (the installer wires agents but never indexes); once a project has a `.codegraph/`, the agent uses CodeGraph automatically.

## In codegraph (grounded)
The library entry point **`src/index.ts`** exposes the `CodeGraph` class that drives the whole lifecycle:

- **init / build.** [`CodeGraph.init`](../catalog/src/index.ts.md#CodeGraph.init) creates the project and [`CodeGraph.indexAll`](../catalog/src/index.ts.md#CodeGraph.indexAll) builds the graph — the README's "one command, done." Incremental updates go through [`CodeGraph.sync`](../catalog/src/index.ts.md#CodeGraph.sync).
- **The `.codegraph/` directory.** Managed in **`src/directory.ts`** — [`getCodeGraphDir`](../catalog/src/directory.ts.md#getCodeGraphDir) / [`createDirectory`](../catalog/src/directory.ts.md#createDirectory) resolve and create it (honoring `CODEGRAPH_DIR`), [`isInitialized`](../catalog/src/directory.ts.md#isInitialized) gates whether a project is ready, and [`findNearestCodeGraphRoot`](../catalog/src/directory.ts.md#findNearestCodeGraphRoot) locates it from a nested path (the monorepo / `projectPath` case).
- **Auto-sync watcher.** [`CodeGraph.watch`](../catalog/src/index.ts.md#CodeGraph.watch) starts the [`FileWatcher`](../catalog/src/sync/watcher.ts.md#FileWatcher) in **`src/sync/watcher.ts`**: [`FileWatcher.start`](../catalog/src/sync/watcher.ts.md#FileWatcher.start) attaches native watchers, [`FileWatcher.handleChange`](../catalog/src/sync/watcher.ts.md#FileWatcher.handleChange) collapses bursts, and [`FileWatcher.scheduleSync`](../catalog/src/sync/watcher.ts.md#FileWatcher.scheduleSync) fires the re-index after the debounce window (default 2000ms, `CODEGRAPH_WATCH_DEBOUNCE_MS`). The staleness signal the README describes comes from [`CodeGraph.getPendingFiles`](../catalog/src/index.ts.md#CodeGraph.getPendingFiles) / [`FileWatcher.getPendingFiles`](../catalog/src/sync/watcher.ts.md#FileWatcher.getPendingFiles) and [`CodeGraph.isIndexStale`](../catalog/src/index.ts.md#CodeGraph.isIndexStale), which drive the `⚠️` per-file banner telling the agent to Read a still-pending file directly.
- **One shared background server.** The README's "auto-sync while the MCP server runs" is the daemon in **`src/mcp/daemon.ts`** — [`Daemon.start`](../catalog/src/mcp/daemon.ts.md#Daemon.start) binds a local socket so multiple agent sessions share one indexing process, [`Daemon.handleConnection`](../catalog/src/mcp/daemon.ts.md#Daemon.handleConnection) does connect-time catch-up reconciliation, and [`tryAcquireDaemonLock`](../catalog/src/mcp/daemon.ts.md#tryAcquireDaemonLock) guards single-instance ownership. `CODEGRAPH_NO_DAEMON=1` skips it (per-session in-process serving).

## Why it matters / when it applies
This is what lets the agent trust that a query reflects the code *right now* without the user ever running `codegraph sync`. The three freshness layers the README calls out — debounced watcher, per-file staleness banner, connect-time catch-up — exist precisely so the agent never gets a silent wrong answer in the window between an edit and the next sync. Manual `codegraph sync` is only for the edge cases: watcher disabled (sandboxes, `CODEGRAPH_NO_DAEMON=1`) or scripting against the index outside an agent session.

## Connections
- Code concepts: [index.ts](../concepts/index.ts.md) — the `CodeGraph` class wiring all layers; [sync-watcher.ts](../concepts/sync-watcher.ts.md) — the debounced native file watcher in depth; [mcp-daemon.ts](../concepts/mcp-daemon.ts.md) — the shared background server and its lock/lifecycle; [directory.ts](../concepts/directory.ts.md) — `.codegraph/` resolution and project-root discovery; [extraction-index.ts](../concepts/extraction-index.ts.md) — the indexing the watcher triggers.
- Module catalogs: [index.ts](../catalog/src/index.ts.md), [sync/watcher.ts](../catalog/src/sync/watcher.ts.md), [mcp/daemon.ts](../catalog/src/mcp/daemon.ts.md), [directory.ts](../catalog/src/directory.ts.md).
- Related doc-concepts: [local-first-grounding](local-first-grounding.md) — the extraction that init/sync run; [mcp-tool-surface](mcp-tool-surface.md) — what serves the freshly-synced graph to the agent.

## Source
Extracted from `README.md` (kept in place) — the "Get Started", "How auto-syncing works", "How It Works", and "CLI Reference" sections.
