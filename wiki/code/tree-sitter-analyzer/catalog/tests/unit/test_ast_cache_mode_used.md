---
title: 'Module: tests/unit/test_ast_cache_mode_used.py'
type: catalog
provenance: extracted
module: tests/unit/test_ast_cache_mode_used.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ast_cache_mode_used`/
symbols:
  test_default_index_reports_incremental_mode: test_default_index_reports_incremental_mode().
  test_force_index_reports_full_mode: test_force_index_reports_full_mode().
  test_incremental_skips_unchanged_files: test_incremental_skips_unchanged_files().
  test_force_re_indexes_everything: test_force_re_indexes_everything().
  _make_project: _make_project().
---
# Module: [`tests/unit/test_ast_cache_mode_used.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_mode_used.py)

## Functions
- `_make_project(tmp_path: Path)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_mode_used.py#L26)
- `test_default_index_reports_incremental_mode(tmp_path: Path)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_mode_used.py#L32)
- `test_force_index_reports_full_mode(tmp_path: Path)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_mode_used.py#L45)
- `test_force_re_indexes_everything(tmp_path: Path)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_mode_used.py#L76) — ``force=True`` must wipe the index and re-parse every file.
- `test_incremental_skips_unchanged_files(tmp_path: Path)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_cache_mode_used.py#L57) — On second incremental call, all files should be cached, none re-indexed.

