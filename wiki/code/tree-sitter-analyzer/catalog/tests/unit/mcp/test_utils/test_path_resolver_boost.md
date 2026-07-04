---
title: 'Module: tests/unit/mcp/test_utils/test_path_resolver_boost.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_utils/test_path_resolver_boost.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_utils.test_path_resolver_boost`/TestValidatePathEdges#
symbols:
  TestValidatePathEdges.test_set_project_root_absolute: test_set_project_root_absolute().
  TestValidatePathEdges.test_set_project_root_none_clears: test_set_project_root_none_clears().
  TestValidatePathEdges.test_symlink_is_rejected: test_symlink_is_rejected().
  TestValidatePathEdges.test_symlink_check_oserror_passes: test_symlink_check_oserror_passes().
  TestValidatePathEdges.test_outside_project_root_rejected: test_outside_project_root_rejected().
  TestValidatePathEdges.test_validate_path_exception_handling: test_validate_path_exception_handling().
  TestValidatePathEdges.test_get_relative_path_cross_drive: test_get_relative_path_cross_drive().
  TestValidatePathEdges: ''
  TestValidatePathEdges.tmp_path: tmp_path().
---
# Module: [`tests/unit/mcp/test_utils/test_path_resolver_boost.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver_boost.py)

## Classes
### `TestValidatePathEdges`
- def: [`tests/unit/mcp/test_utils/test_path_resolver_boost.py:14`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver_boost.py#L14)
- signature: `class TestValidatePathEdges:`
- members:
  - `test_get_relative_path_cross_drive(self)` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver_boost.py#L84) — ValueError when paths don't share a prefix
  - `test_outside_project_root_rejected(self, tmp_path)` — [`L44`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver_boost.py#L44) — absolute path outside project_root → rejected
  - `test_set_project_root_absolute(self, tmp_path)` — [`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver_boost.py#L69)
  - `test_set_project_root_none_clears(self)` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver_boost.py#L75)
  - `test_symlink_check_oserror_passes(self, tmp_path)` — [`L36`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver_boost.py#L36) — is_symlink() raises OSError → swallowed, path accepted
  - `test_symlink_is_rejected(self, tmp_path)` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver_boost.py#L20) — is_symlink() returns True → rejected
  - `test_validate_path_exception_handling(self)` — [`L57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver_boost.py#L57) — general exception → error message
  - `tmp_path(self)` — [`L16`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver_boost.py#L16)
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.project_root), [`validate_path`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.validate_path), [`get_relative_path`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.get_relative_path), [`set_project_root`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.set_project_root)

