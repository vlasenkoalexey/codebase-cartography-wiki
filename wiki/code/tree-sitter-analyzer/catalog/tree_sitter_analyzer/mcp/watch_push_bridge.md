---
title: 'Module: tree_sitter_analyzer/mcp/watch_push_bridge.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/watch_push_bridge.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.watch_push_bridge`/
symbols:
  _drive_subscriptions._push: _drive_subscriptions()._push().
  _drive_subscriptions: _drive_subscriptions().
  _drive_subscriptions._evaluate: _drive_subscriptions()._evaluate().
  _send_update: _send_update().
  collect_changed_pairs: collect_changed_pairs().
  make_on_sync_callback: make_on_sync_callback().
  logger: logger.
  make_on_sync_callback._on_sync: make_on_sync_callback()._on_sync().
  _handle_push_result: _handle_push_result().
---
# Module: [`tree_sitter_analyzer/mcp/watch_push_bridge.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/watch_push_bridge.py)

## Functions
- `_drive_subscriptions(project_root: str | None, sync_result: dict[str, Any])` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/watch_push_bridge.py#L45) — Re-evaluate each subscription and push deltas.  Called on the watcher thread.
- `_evaluate(session_id: str, selector: str)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/watch_push_bridge.py#L54)
- `_handle_push_result(future: Any, session_id: str, selector: str, registry: Any)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/watch_push_bridge.py#L138) — Callback on push future completion — GC dead sessions.
- `_on_sync(sync_result: dict[str, Any])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/watch_push_bridge.py#L39)
- `_push(session_id: str, selector: str)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/watch_push_bridge.py#L76)
- `_send_update(session_id: str, uri: str)` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/watch_push_bridge.py#L122) — Coroutine that sends resource-updated; runs on the captured loop.
- `collect_changed_pairs(registry: Any, evaluate: Any)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/watch_push_bridge.py#L100) — Return the ``(session_id, selector)`` pairs whose result changed.
- `make_on_sync_callback(project_root: str | None)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/watch_push_bridge.py#L30) — Return an ``on_sync`` callable suitable for ``FileWatcherDaemon``.

## Module values
- `logger` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/watch_push_bridge.py#L27)

