---
title: 'Module: tests/unit/test_health_history.py'
type: catalog
provenance: extracted
module: tests/unit/test_health_history.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_health_history`/
symbols:
  test_history_schema_migration_idempotent: test_history_schema_migration_idempotent().
  test_history_coexists_with_existing_health_scores_table: test_history_coexists_with_existing_health_scores_table().
  _import_history: _import_history().
  history: history().
  pytestmark: pytestmark.
  project_root: project_root().
  test_append_then_last_returns_appended: test_append_then_last_returns_appended().
  test_last_returns_none_for_unknown_file: test_last_returns_none_for_unknown_file().
  test_last_returns_most_recent_row_when_multiple: test_last_returns_most_recent_row_when_multiple().
  test_prune_keeps_last_n: test_prune_keeps_last_n().
  test_prune_does_not_touch_other_files: test_prune_does_not_touch_other_files().
  test_prune_keep_n_larger_than_rows_is_noop: test_prune_keep_n_larger_than_rows_is_noop().
  test_append_records_trigger_source: test_append_records_trigger_source().
---
# Module: [`tests/unit/test_health_history.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py)

## Functions
- `_import_history()` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L29) — Lazy import to ensure each test gets a clean failure on missing module.
- `history(project_root: str)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L43)
- `project_root(tmp_path: Path)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L37)
- `test_append_records_trigger_source(history, project_root: str)` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L227) — Each appended row records its trigger ('watch' | 'cli' | 'mcp').
- `test_append_then_last_returns_appended(history)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L55) — append(file, score, grade) → last(file) returns (grade, score).
- `test_history_coexists_with_existing_health_scores_table(project_root: str)` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L171) — If health_scores.db already exists (from HealthScoreCache),
- `test_history_schema_migration_idempotent(project_root: str)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L150) — Opening HealthHistory twice on the same project must not raise.
- `test_last_returns_most_recent_row_when_multiple(history)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L72) — Multiple appends for one file → last() returns the latest by computed_at.
- `test_last_returns_none_for_unknown_file(history)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L67) — A file that was never appended returns None — no implicit zero row.
- `test_prune_does_not_touch_other_files(history)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L126) — prune(fileA, keep=1) must NOT delete rows for fileB.
- `test_prune_keep_n_larger_than_rows_is_noop(history)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L140) — If keep_n > existing rows, prune deletes nothing and does not raise.
- `test_prune_keeps_last_n(history, project_root: str)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L87) — append 60 rows → prune(file, keep=10) → exactly 10 rows, the latest by time.

## Module values
- `pytestmark` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_history.py#L26)

