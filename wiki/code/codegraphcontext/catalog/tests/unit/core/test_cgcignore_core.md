---
title: 'Module: tests/unit/core/test_cgcignore_core.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_cgcignore_core.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.core.test_cgcignore_core`/test_
symbols:
  test_safe_walk_directory_pruning_and_error_handling: safe_walk_directory_pruning_and_error_handling().
  test_safe_walk_directory_pruning_and_error_handling.mock_walk: safe_walk_directory_pruning_and_error_handling().mock_walk().
  test_parse_cgcignore_lines_skips_comments_and_blanks: parse_cgcignore_lines_skips_comments_and_blanks().
  test_build_ignore_spec_merges_default_and_user_patterns: build_ignore_spec_merges_default_and_user_patterns().
  test_build_ignore_spec_auto_creates_cgcignore_with_defaults: build_ignore_spec_auto_creates_cgcignore_with_defaults().
  test_read_cgcignore_patterns_merges_defaults_with_user_patterns: read_cgcignore_patterns_merges_defaults_with_user_patterns().
  test_find_cgcignore_does_not_escape_non_git_root: find_cgcignore_does_not_escape_non_git_root().
  test_build_ignore_spec_prefers_local_over_explicit_context_file: build_ignore_spec_prefers_local_over_explicit_context_file().
  test_build_ignore_spec_auto_creates_local_even_with_explicit_context_file: build_ignore_spec_auto_creates_local_even_with_explicit_context_file().
---
# Module: [`tests/unit/core/test_cgcignore_core.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_core.py)

## Functions
- `mock_walk(top, topdown=True, onerror=None, followlinks=False)` — [`L166`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_core.py#L166)
- `test_build_ignore_spec_auto_creates_cgcignore_with_defaults(tmp_path: Path)` — [`L40`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_core.py#L40)
- `test_build_ignore_spec_auto_creates_local_even_with_explicit_context_file(tmp_path: Path)` — [`L110`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_core.py#L110)
- `test_build_ignore_spec_merges_default_and_user_patterns(tmp_path: Path)` — [`L23`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_core.py#L23)
- `test_build_ignore_spec_prefers_local_over_explicit_context_file(tmp_path: Path)` — [`L87`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_core.py#L87)
- `test_find_cgcignore_does_not_escape_non_git_root(tmp_path: Path)` — [`L68`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_core.py#L68)
- `test_parse_cgcignore_lines_skips_comments_and_blanks()` — [`L10`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_core.py#L10)
- `test_read_cgcignore_patterns_merges_defaults_with_user_patterns(tmp_path: Path)` — [`L59`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_core.py#L59)
- `test_safe_walk_directory_pruning_and_error_handling(tmp_path: Path, monkeypatch)` — [`L131`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_core.py#L131)

