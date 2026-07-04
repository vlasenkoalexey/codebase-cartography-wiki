---
title: 'Module: tests/unit/mcp/test_utils/test_path_resolver.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_utils/test_path_resolver.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_utils.test_path_resolver`/
symbols:
  _normalize_test_path: _normalize_test_path().
  TestPathResolverIntegration.test_full_workflow: TestPathResolverIntegration#test_full_workflow().
  TestPathResolverInit.test_init_without_project_root: TestPathResolverInit#test_init_without_project_root().
  TestPathResolverCache.test_cache_size_limit: TestPathResolverCache#test_cache_size_limit().
  TestPathResolverCache.test_clear_cache: TestPathResolverCache#test_clear_cache().
  TestPathResolverCache.test_get_cache_stats: TestPathResolverCache#test_get_cache_stats().
  TestPathResolverSetProjectRoot.test_set_project_root_absolute: TestPathResolverSetProjectRoot#test_set_project_root_absolute().
  TestPathResolverInit.test_init_with_absolute_project_root: TestPathResolverInit#test_init_with_absolute_project_root().
  TestPathResolverResolve.test_resolve_absolute_path: TestPathResolverResolve#test_resolve_absolute_path().
  TestPathResolverResolve.test_resolve_relative_path_with_project_root: TestPathResolverResolve#test_resolve_relative_path_with_project_root().
  TestPathResolverResolve.test_resolve_relative_path_without_project_root: TestPathResolverResolve#test_resolve_relative_path_without_project_root().
  TestPathResolverResolve.test_resolve_path_normalization: TestPathResolverResolve#test_resolve_path_normalization().
  TestPathResolverCache.test_cache_hit: TestPathResolverCache#test_cache_hit().
  TestPathResolverGetProjectRoot.test_get_project_root_set: TestPathResolverGetProjectRoot#test_get_project_root_set().
  TestPathResolverSetProjectRoot.test_set_project_root_relative: TestPathResolverSetProjectRoot#test_set_project_root_relative().
  TestPathResolverSetProjectRoot.test_set_project_root_none: TestPathResolverSetProjectRoot#test_set_project_root_none().
  TestPathResolverIntegration.test_cross_platform_workflow: TestPathResolverIntegration#test_cross_platform_workflow().
  TestPathResolverInit.test_init_with_relative_project_root: TestPathResolverInit#test_init_with_relative_project_root().
  TestPathResolverInit.test_cache_initialization: TestPathResolverInit#test_cache_initialization().
  TestPathResolverResolve.test_resolve_empty_path: TestPathResolverResolve#test_resolve_empty_path().
  TestPathResolverResolve.test_resolve_none_path: TestPathResolverResolve#test_resolve_none_path().
  TestPathResolverResolve.test_resolve_non_string_path: TestPathResolverResolve#test_resolve_non_string_path().
  TestPathResolverResolve.test_resolve_windows_path_on_posix: TestPathResolverResolve#test_resolve_windows_path_on_posix().
  TestPathResolverResolve.test_resolve_unix_path_on_windows: TestPathResolverResolve#test_resolve_unix_path_on_windows().
  TestPathResolverResolve.test_resolve_with_cache: TestPathResolverResolve#test_resolve_with_cache().
  TestPathResolverIsRelative.test_relative_path: TestPathResolverIsRelative#test_relative_path().
  TestPathResolverIsRelative.test_absolute_path: TestPathResolverIsRelative#test_absolute_path().
  TestPathResolverIsRelative.test_dot_path: TestPathResolverIsRelative#test_dot_path().
  TestPathResolverGetRelativePath.test_get_relative_path_with_project_root: TestPathResolverGetRelativePath#test_get_relative_path_with_project_root().
  TestPathResolverGetRelativePath.test_get_relative_path_without_project_root: TestPathResolverGetRelativePath#test_get_relative_path_without_project_root().
  TestPathResolverGetRelativePath.test_get_relative_path_non_absolute: TestPathResolverGetRelativePath#test_get_relative_path_non_absolute().
  TestPathResolverGetRelativePath.test_get_relative_path_different_drives: TestPathResolverGetRelativePath#test_get_relative_path_different_drives().
  TestPathResolverValidatePath.test_validate_existing_file: TestPathResolverValidatePath#test_validate_existing_file().
  TestPathResolverValidatePath.test_validate_nonexistent_file: TestPathResolverValidatePath#test_validate_nonexistent_file().
  TestPathResolverValidatePath.test_validate_directory: TestPathResolverValidatePath#test_validate_directory().
  TestPathResolverValidatePath.test_validate_symlink: TestPathResolverValidatePath#test_validate_symlink().
  TestPathResolverValidatePath.test_validate_path_outside_project_root: TestPathResolverValidatePath#test_validate_path_outside_project_root().
  TestPathResolverValidatePath.test_validate_path_without_project_root: TestPathResolverValidatePath#test_validate_path_without_project_root().
  TestPathResolverValidatePath.test_validate_path_exception_handling: TestPathResolverValidatePath#test_validate_path_exception_handling().
  TestPathResolverGetProjectRoot.test_get_project_root_not_set: TestPathResolverGetProjectRoot#test_get_project_root_not_set().
  TestResolvePathFunction.test_resolve_path_with_project_root: TestResolvePathFunction#test_resolve_path_with_project_root().
  TestResolvePathFunction.test_resolve_path_without_project_root: TestResolvePathFunction#test_resolve_path_without_project_root().
  TestNormalizePathCrossPlatform.test_empty_path: TestNormalizePathCrossPlatform#test_empty_path().
  TestNormalizePathCrossPlatform.test_none_path: TestNormalizePathCrossPlatform#test_none_path().
  TestNormalizePathCrossPlatform.test_posix_normal_path: TestNormalizePathCrossPlatform#test_posix_normal_path().
  TestNormalizePathCrossPlatform.test_windows_normal_path: TestNormalizePathCrossPlatform#test_windows_normal_path().
  TestNormalizePathCrossPlatform.test_macos_system_volumes_data_prefix: TestNormalizePathCrossPlatform#test_macos_system_volumes_data_prefix().
  TestNormalizePathCrossPlatform.test_macos_private_var_prefix: TestNormalizePathCrossPlatform#test_macos_private_var_prefix().
  TestNormalizePathCrossPlatform.test_macos_var_prefix_unchanged: TestNormalizePathCrossPlatform#test_macos_var_prefix_unchanged().
  TestNormalizePathCrossPlatform.test_windows_short_path_not_called_on_posix: TestNormalizePathCrossPlatform#test_windows_short_path_not_called_on_posix().
  TestIsWindowsAbsolutePath.test_empty_path: TestIsWindowsAbsolutePath#test_empty_path().
  TestIsWindowsAbsolutePath.test_short_path: TestIsWindowsAbsolutePath#test_short_path().
  TestIsWindowsAbsolutePath.test_windows_backslash_path: TestIsWindowsAbsolutePath#test_windows_backslash_path().
  TestIsWindowsAbsolutePath.test_windows_forward_slash_path: TestIsWindowsAbsolutePath#test_windows_forward_slash_path().
  TestIsWindowsAbsolutePath.test_non_windows_path: TestIsWindowsAbsolutePath#test_non_windows_path().
  TestIsWindowsAbsolutePath.test_path_without_colon: TestIsWindowsAbsolutePath#test_path_without_colon().
  TestIsWindowsAbsolutePath.test_non_alpha_drive_letter: TestIsWindowsAbsolutePath#test_non_alpha_drive_letter().
  TestNormalizePathCrossPlatform: TestNormalizePathCrossPlatform#
  TestIsWindowsAbsolutePath: TestIsWindowsAbsolutePath#
  TestPathResolverInit: TestPathResolverInit#
  TestPathResolverResolve: TestPathResolverResolve#
  TestPathResolverCache: TestPathResolverCache#
  TestPathResolverIsRelative: TestPathResolverIsRelative#
  TestPathResolverGetRelativePath: TestPathResolverGetRelativePath#
  TestPathResolverValidatePath: TestPathResolverValidatePath#
  TestPathResolverGetProjectRoot: TestPathResolverGetProjectRoot#
  TestPathResolverSetProjectRoot: TestPathResolverSetProjectRoot#
  TestResolvePathFunction: TestResolvePathFunction#
  TestPathResolverIntegration: TestPathResolverIntegration#
---
# Module: [`tests/unit/mcp/test_utils/test_path_resolver.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py)

## Classes
### `TestIsWindowsAbsolutePath`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:83`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L83)
- doc: Tests for _is_windows_absolute_path function.
- signature: `class TestIsWindowsAbsolutePath:`
- members:
  - `test_empty_path(self)` — [`L86`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L86) — Test that empty path returns False.
  - `test_non_alpha_drive_letter(self)` — [`L110`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L110) — Test non-alpha drive letter returns False.
  - `test_non_windows_path(self)` — [`L102`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L102) — Test non-Windows path returns False.
  - `test_path_without_colon(self)` — [`L106`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L106) — Test path without drive letter returns False.
  - `test_short_path(self)` — [`L90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L90) — Test that short paths return False.
  - `test_windows_backslash_path(self)` — [`L94`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L94) — Test Windows path with backslash.
  - `test_windows_forward_slash_path(self)` — [`L98`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L98) — Test Windows path with forward slash.
- uses (calls/refs, reference-scoped): [`_is_windows_absolute_path`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#_is_windows_absolute_path)

### `TestNormalizePathCrossPlatform`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L34)
- doc: Tests for _normalize_path_cross_platform function.
- signature: `class TestNormalizePathCrossPlatform:`
- members:
  - `test_empty_path(self)` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L37) — Test that empty path is returned as-is.
  - `test_macos_private_var_prefix(self, monkeypatch)` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L63) — Test macOS /private/var to /var normalization.
  - `test_macos_system_volumes_data_prefix(self, monkeypatch)` — [`L57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L57) — Test macOS /System/Volumes/Data prefix removal.
  - `test_macos_var_prefix_unchanged(self, monkeypatch)` — [`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L69) — Test that /var paths are kept as-is on macOS.
  - `test_none_path(self)` — [`L42`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L42) — Test that None path is returned as-is.
  - `test_posix_normal_path(self)` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L47) — Test that normal POSIX paths are unchanged.
  - `test_windows_normal_path(self)` — [`L52`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L52) — Test that normal Windows paths are unchanged.
  - `test_windows_short_path_not_called_on_posix(self, monkeypatch)` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L75) — Test that Windows API is not called on POSIX systems.
- uses (calls/refs, reference-scoped): [`_normalize_path_cross_platform`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#_normalize_path_cross_platform)

### `TestPathResolverCache`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:250`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L250)
- doc: Tests for PathResolver caching.
- signature: `class TestPathResolverCache:`
- members:
  - `test_cache_hit(self, tmp_path)` — [`L253`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L253) — Test that cache returns cached values.
  - `test_cache_size_limit(self)` — [`L267`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L267) — Test that cache respects size limit.
  - `test_clear_cache(self, tmp_path)` — [`L283`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L283) — Test that cache can be cleared.
  - `test_get_cache_stats(self)` — [`L297`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L297) — Test getting cache statistics.
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`resolve`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.resolve), [`_cache`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver._cache), [`_add_to_cache`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver._add_to_cache), [`_cache_size_limit`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver._cache_size_limit), [`get_cache_stats`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.get_cache_stats), [`clear_cache`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.clear_cache)

### `TestPathResolverGetProjectRoot`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:467`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L467)
- doc: Tests for PathResolver.get_project_root method.
- signature: `class TestPathResolverGetProjectRoot:`
- members:
  - `test_get_project_root_not_set(self)` — [`L477`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L477) — Test getting unset project root.
  - `test_get_project_root_set(self, tmp_path)` — [`L470`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L470) — Test getting set project root.
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`get_project_root`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.get_project_root)  (1 test-only)

### `TestPathResolverGetRelativePath`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:339`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L339)
- doc: Tests for PathResolver.get_relative_path method.
- signature: `class TestPathResolverGetRelativePath:`
- members:
  - `test_get_relative_path_different_drives(self)` — [`L370`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L370) — Test getting relative path across different drives on Windows.
  - `test_get_relative_path_non_absolute(self)` — [`L363`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L363) — Test that non-absolute path raises ValueError.
  - `test_get_relative_path_with_project_root(self, tmp_path)` — [`L342`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L342) — Test getting relative path with project root.
  - `test_get_relative_path_without_project_root(self)` — [`L351`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L351) — Test getting relative path without project root.
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`get_relative_path`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.get_relative_path)

### `TestPathResolverInit`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:115`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L115)
- doc: Tests for PathResolver initialization.
- signature: `class TestPathResolverInit:`
- members:
  - `test_cache_initialization(self)` — [`L140`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L140) — Test that cache is initialized correctly.
  - `test_init_with_absolute_project_root(self, tmp_path)` — [`L125`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L125) — Test initialization with absolute project root.
  - `test_init_with_relative_project_root(self)` — [`L134`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L134) — Test initialization with relative project root.
  - `test_init_without_project_root(self)` — [`L118`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L118) — Test initialization without project root.
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.project_root), [`_cache`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver._cache), [`_cache_size_limit`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver._cache_size_limit)  (1 test-only)

### `TestPathResolverIntegration`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:541`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L541)
- doc: Integration tests for PathResolver.
- signature: `class TestPathResolverIntegration:`
- members:
  - `test_cross_platform_workflow(self, tmp_path)` — [`L576`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L576) — Test cross-platform path handling.
  - `test_full_workflow(self, tmp_path)` — [`L544`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L544) — Test complete path resolution workflow.
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`resolve`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.resolve), [`validate_path`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.validate_path), [`get_relative_path`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.get_relative_path), [`get_cache_stats`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.get_cache_stats), [`is_relative`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.is_relative)  (1 test-only)

### `TestPathResolverIsRelative`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:311`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L311)
- doc: Tests for PathResolver.is_relative method.
- signature: `class TestPathResolverIsRelative:`
- members:
  - `test_absolute_path(self)` — [`L321`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L321) — Test that absolute paths are not identified as relative.
  - `test_dot_path(self)` — [`L333`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L333) — Test that . is considered relative.
  - `test_relative_path(self)` — [`L314`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L314) — Test that relative paths are identified.
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`is_relative`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.is_relative)

### `TestPathResolverResolve`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:147`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L147)
- doc: Tests for PathResolver.resolve method.
- signature: `class TestPathResolverResolve:`
- members:
  - `test_resolve_absolute_path(self, tmp_path)` — [`L168`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L168) — Test resolving absolute path.
  - `test_resolve_empty_path(self)` — [`L150`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L150) — Test that empty path raises ValueError.
  - `test_resolve_non_string_path(self)` — [`L162`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L162) — Test that non-string path raises TypeError.
  - `test_resolve_none_path(self)` — [`L156`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L156) — Test that None path raises ValueError.
  - `test_resolve_path_normalization(self, tmp_path)` — [`L236`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L236) — Test that path separators are normalized.
  - `test_resolve_relative_path_with_project_root(self, tmp_path)` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L178) — Test resolving relative path with project root.
  - `test_resolve_relative_path_without_project_root(self, tmp_path)` — [`L189`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L189) — Test resolving relative path without project root.
  - `test_resolve_unix_path_on_windows(self, tmp_path)` — [`L215`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L215) — Test Unix absolute path on Windows.
  - `test_resolve_windows_path_on_posix(self, monkeypatch)` — [`L206`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L206) — Test Windows absolute path on POSIX system.
  - `test_resolve_with_cache(self, tmp_path)` — [`L224`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L224) — Test that caching works correctly.
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`resolve`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.resolve)  (1 test-only)

### `TestPathResolverSetProjectRoot`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:484`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L484)
- doc: Tests for PathResolver.set_project_root method.
- signature: `class TestPathResolverSetProjectRoot:`
- members:
  - `test_set_project_root_absolute(self, tmp_path)` — [`L487`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L487) — Test setting absolute project root.
  - `test_set_project_root_none(self)` — [`L503`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L503) — Test setting project root to None.
  - `test_set_project_root_relative(self)` — [`L496`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L496) — Test setting relative project root.
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.project_root), [`set_project_root`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.set_project_root)  (1 test-only)

### `TestPathResolverValidatePath`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:382`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L382)
- doc: Tests for PathResolver.validate_path method.
- signature: `class TestPathResolverValidatePath:`
- members:
  - `test_validate_directory(self, tmp_path)` — [`L402`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L402) — Test validating a directory.
  - `test_validate_existing_file(self, tmp_path)` — [`L385`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L385) — Test validating an existing file.
  - `test_validate_nonexistent_file(self, tmp_path)` — [`L395`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L395) — Test validating a non-existent file.
  - `test_validate_path_exception_handling(self, tmp_path)` — [`L457`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L457) — Test exception handling during validation.
  - `test_validate_path_outside_project_root(self, tmp_path)` — [`L435`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L435) — Test validating path outside project root.
  - `test_validate_path_without_project_root(self, tmp_path)` — [`L447`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L447) — Test validating path without project root.
  - `test_validate_symlink(self, tmp_path)` — [`L412`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L412) — Test validating a symlink.
- uses (calls/refs, reference-scoped): [`PathResolver`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver), [`validate_path`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#PathResolver.validate_path)

### `TestResolvePathFunction`
- def: [`tests/unit/mcp/test_utils/test_path_resolver.py:511`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L511)
- doc: Tests for resolve_path convenience function.
- signature: `class TestResolvePathFunction:`
- members:
  - `test_resolve_path_with_project_root(self, tmp_path)` — [`L514`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L514) — Test resolve_path with project root.
  - `test_resolve_path_without_project_root(self, tmp_path)` — [`L524`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L524) — Test resolve_path without project root.
- uses (calls/refs, reference-scoped): [`resolve_path`](../../../../tree_sitter_analyzer/mcp/utils/path_resolver.md#resolve_path)  (1 test-only)

## Functions
- `_normalize_test_path(path: str)` — [`L21`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_path_resolver.py#L21) — Normalize path to handle macOS /var -> /private/var symlinks

