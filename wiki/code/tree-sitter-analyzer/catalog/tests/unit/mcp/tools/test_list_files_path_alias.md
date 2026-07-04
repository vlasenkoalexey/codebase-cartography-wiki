---
title: 'Module: tests/unit/mcp/tools/test_list_files_path_alias.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_list_files_path_alias.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_list_files_path_alias`/test_
symbols:
  test_path_is_declared_in_schema: path_is_declared_in_schema().
  test_path_maps_to_roots_when_roots_absent: path_maps_to_roots_when_roots_absent().
  test_explicit_roots_wins_over_path: explicit_roots_wins_over_path().
  test_empty_path_is_rejected_not_silently_widened: empty_path_is_rejected_not_silently_widened().
  test_consumed_path_alias_is_removed: consumed_path_alias_is_removed().
  test_nonexistent_path_is_rejected_not_silently_widened: nonexistent_path_is_rejected_not_silently_widened().
---
# Module: [`tests/unit/mcp/tools/test_list_files_path_alias.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_list_files_path_alias.py)

## Functions
- `test_consumed_path_alias_is_removed(tmp_path)` — [`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_list_files_path_alias.py#L49) — Once mapped to roots, the ``path`` alias is popped so it never lingers
- `test_empty_path_is_rejected_not_silently_widened(tmp_path)` — [`L41`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_list_files_path_alias.py#L41) — Review issue 2: an explicit-but-empty ``path`` must be a user error, NOT
- `test_explicit_roots_wins_over_path(tmp_path)` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_list_files_path_alias.py#L32)
- `test_nonexistent_path_is_rejected_not_silently_widened(tmp_path)` — [`L60`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_list_files_path_alias.py#L60) — A non-existent ``path`` must surface an error — NOT silently fall back to
- `test_path_is_declared_in_schema()` — [`L19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_list_files_path_alias.py#L19) — ``path`` must be in the inner schema or the facade whitelist drops it.
- `test_path_maps_to_roots_when_roots_absent(tmp_path)` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_list_files_path_alias.py#L25)

