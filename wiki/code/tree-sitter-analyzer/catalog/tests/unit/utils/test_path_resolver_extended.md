---
title: 'Module: tests/unit/utils/test_path_resolver_extended.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_path_resolver_extended.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_path_resolver_extended`/
symbols:
  TestPathResolverExtended.resolver: TestPathResolverExtended#resolver.
  TestPathResolverExtended.project_root: TestPathResolverExtended#project_root.
  TestPathResolverExtended.test_get_relative_path_with_absolute_path: TestPathResolverExtended#test_get_relative_path_with_absolute_path().
  TestPathResolverExtended.test_set_project_root_with_valid_path: TestPathResolverExtended#test_set_project_root_with_valid_path().
  TestPathResolverExtended.test_file: TestPathResolverExtended#test_file.
  TestPathResolverExtended.test_cache_functionality: TestPathResolverExtended#test_cache_functionality().
  TestPathResolverExtended.test_resolve_with_relative_path_dot: TestPathResolverExtended#test_resolve_with_relative_path_dot().
  TestPathResolverExtended.test_resolve_with_relative_path_double_dot: TestPathResolverExtended#test_resolve_with_relative_path_double_dot().
  TestPathResolverExtended.test_resolve_with_mixed_separators: TestPathResolverExtended#test_resolve_with_mixed_separators().
  TestPathResolverExtended.test_validate_path_with_directory: TestPathResolverExtended#test_validate_path_with_directory().
  TestPathResolverExtended.test_validate_path_with_permission_error: TestPathResolverExtended#test_validate_path_with_permission_error().
  TestPathResolverExtended.test_validate_path_with_symlink: TestPathResolverExtended#test_validate_path_with_symlink().
  TestPathResolverExtended.test_get_relative_path_with_path_outside_project: TestPathResolverExtended#test_get_relative_path_with_path_outside_project().
  TestPathResolverExtended.test_get_relative_path_with_none_project_root: TestPathResolverExtended#test_get_relative_path_with_none_project_root().
  TestPathResolverExtended.test_is_relative_with_absolute_path: TestPathResolverExtended#test_is_relative_with_absolute_path().
  TestPathResolverExtended.test_path_normalization: TestPathResolverExtended#test_path_normalization().
  TestPathResolverExtended.test_set_project_root_with_none: TestPathResolverExtended#test_set_project_root_with_none().
  TestPathResolverExtended.test_set_project_root_with_empty_string: TestPathResolverExtended#test_set_project_root_with_empty_string().
  TestPathResolverExtended.test_error_handling: TestPathResolverExtended#test_error_handling().
  normalize_path_for_comparison: normalize_path_for_comparison().
  TestPathResolverExtended.test_resolve_with_none_project_root: TestPathResolverExtended#test_resolve_with_none_project_root().
  TestPathResolverExtended.test_resolve_with_empty_string_project_root: TestPathResolverExtended#test_resolve_with_empty_string_project_root().
  TestPathResolverExtended.test_is_relative_with_relative_path: TestPathResolverExtended#test_is_relative_with_relative_path().
  TestPathResolverExtended.test_is_relative_with_empty_path: TestPathResolverExtended#test_is_relative_with_empty_path().
  TestPathResolverExtended.test_is_relative_with_none_path: TestPathResolverExtended#test_is_relative_with_none_path().
  TestPathResolverExtended.test_resolve_path_function_with_valid_project_root: TestPathResolverExtended#test_resolve_path_function_with_valid_project_root().
  TestPathResolverExtended.test_cross_platform_path_handling: TestPathResolverExtended#test_cross_platform_path_handling().
  TestPathResolverExtended.test_edge_cases: TestPathResolverExtended#test_edge_cases().
  TestPathResolverExtended.temp_dir: TestPathResolverExtended#temp_dir.
  TestPathResolverExtended.teardown_method: TestPathResolverExtended#teardown_method().
  TestPathResolverExtended.test_resolve_path_function_with_none_project_root: TestPathResolverExtended#test_resolve_path_function_with_none_project_root().
  TestPathResolverExtended.test_resolve_path_function_with_empty_project_root: TestPathResolverExtended#test_resolve_path_function_with_empty_project_root().
  TestPathResolverExtended: TestPathResolverExtended#
  TestPathResolverExtended.setup_method: TestPathResolverExtended#setup_method().
---
# Module: [`tests/unit/utils/test_path_resolver_extended.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py)

## Classes
### `TestPathResolverExtended`
- def: [`tests/unit/utils/test_path_resolver_extended.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L71)
- doc: Extended test cases for PathResolver class
- signature: `class TestPathResolverExtended:`
- members:
  - `setup_method(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L74) — Set up test fixtures
  - `teardown_method(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L87) — Clean up test fixtures
  - `test_cache_functionality(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L354) — Test cache functionality.
  - `test_cross_platform_path_handling(self)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L264) — Test cross-platform path handling.
  - `test_edge_cases(self)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L322) — Test various edge cases.
  - `test_error_handling(self)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L339) — Test error handling in various scenarios.
  - `test_get_relative_path_with_absolute_path(self)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L166) — Test get_relative_path method with absolute path.
  - `test_get_relative_path_with_none_project_root(self)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L194) — Test get_relative_path method when project_root is None.
  - `test_get_relative_path_with_path_outside_project(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L186) — Test get_relative_path method with path outside project.
  - `test_is_relative_with_absolute_path(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L200) — Test is_relative method with absolute path.
  - `test_is_relative_with_empty_path(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L210) — Test is_relative method with empty path.
  - `test_is_relative_with_none_path(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L215) — Test is_relative method with None path.
  - `test_is_relative_with_relative_path(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L205) — Test is_relative method with relative path.
  - `test_path_normalization(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L220) — Test path normalization.
  - `test_resolve_path_function_with_empty_project_root(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L252) — Test resolve_path function with empty project_root.
  - `test_resolve_path_function_with_none_project_root(self)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L246) — Test resolve_path function with None project_root.
  - `test_resolve_path_function_with_valid_project_root(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L258) — Test resolve_path function with valid project_root.
  - `test_resolve_with_empty_string_project_root(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L99) — Test resolve method with empty string project_root.
  - `test_resolve_with_mixed_separators(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L122) — Test resolve method with mixed path separators.
  - `test_resolve_with_none_project_root(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L92) — Test resolve method when project_root is None.
  - `test_resolve_with_relative_path_dot(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L106) — Test resolve method with relative path starting with dot.
  - `test_resolve_with_relative_path_double_dot(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L112) — Test resolve method with relative path starting with double dot.
  - `test_set_project_root_with_empty_string(self)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L231) — Test set_project_root method with empty string.
  - `test_set_project_root_with_none(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L226) — Test set_project_root method with None.
  - `test_set_project_root_with_valid_path(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L236) — Test set_project_root method with valid path.
  - `test_validate_path_with_directory(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L129) — Test validate_path with directory path.
  - `test_validate_path_with_permission_error(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L140) — Test validate_path with permission error.
  - `test_validate_path_with_symlink(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L153) — Test validate_path with symlink.
  - `project_root` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L77)
  - `resolver` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L85)
  - `temp_dir` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L76)
  - `test_file` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L81)
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`resolve`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.resolve), [`project_root`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.project_root), [`validate_path`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.validate_path), [`get_relative_path`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.get_relative_path), [`set_project_root`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.set_project_root), [`resolve_path`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#resolve_path), [`get_cache_stats`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.get_cache_stats), [`is_relative`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.is_relative), [`clear_cache`](../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.clear_cache)  (1 test-only)

## Functions
- `normalize_path_for_comparison(path_str)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_path_resolver_extended.py#L17) — Normalize path for comparison, handling platform-specific differences.

