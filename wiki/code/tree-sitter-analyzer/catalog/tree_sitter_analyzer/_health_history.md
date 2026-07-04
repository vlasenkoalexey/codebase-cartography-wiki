---
title: 'Module: tree_sitter_analyzer/_health_history.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_health_history.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._health_history`/
symbols:
  HealthHistory._conn: HealthHistory#_conn.
  HealthHistory._init_db: HealthHistory#_init_db().
  HealthHistory.append: HealthHistory#append().
  HealthHistory: HealthHistory#
  HealthHistory.last: HealthHistory#last().
  HealthHistory.prune: HealthHistory#prune().
  HealthHistory.enabled: HealthHistory#enabled().
  HealthHistory.close: HealthHistory#close().
  HealthHistory._db_path: HealthHistory#_db_path.
  HealthHistory._enabled: HealthHistory#_enabled.
  logger: logger.
  _SCHEMA: _SCHEMA.
  _default_db_path: _default_db_path().
  HealthHistory.__init__: HealthHistory#__init__().
  HealthHistory._project_root: HealthHistory#_project_root.
---
# Module: [`tree_sitter_analyzer/_health_history.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py)

## Classes
### `HealthHistory`
- def: [`tree_sitter_analyzer/_health_history.py:53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L53)
- doc: Append-only history of per-file health scores.
- signature: `class HealthHistory:`
- members:
  - `append(self, file_path: str, score: float, grade: str, *, dimensions: dict[str, Any] | None = None, trigger: str = "watch", computed_at: float | None = None)` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L99) — Append a new history row.
  - `close(self)` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L89)
  - `enabled(self)` — [`L86`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L86)
  - `last(self, file_path: str)` — [`L146`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L146) — Return ``(grade, score)`` for the most recent row, or ``None``.
  - `prune(self, file_path: str, keep_n: int)` — [`L165`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L165) — Delete all rows for ``file_path`` except the latest ``keep_n``.
- protocol/private: `__init__`[`L62`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L62), `_conn`[`L65`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L65), `_db_path`[`L64`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L64), `_enabled`[`L66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L66), `_init_db`[`L68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L68), `_project_root`[`L63`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L63)
- uses (calls/refs, reference-scoped): [`logger`](_health_history.md#logger), [`_SCHEMA`](_health_history.md#_SCHEMA), [`_default_db_path`](_health_history.md#_default_db_path)
- used by: [`_process_one`](health_homeostasis.md#HealthHomeostasisLoop._process_one), [`run_watch_health`](health_homeostasis.md#run_watch_health), [`__init__`](health_homeostasis.md#HealthHomeostasisLoop.__init__), [`_on_sync`](health_homeostasis.md#run_watch_health._on_sync)  (5 test-only)

## Functions
- `_default_db_path(project_root: str)` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L48)

## Module values
- `_SCHEMA` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L33)
- `logger` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_history.py#L30)

