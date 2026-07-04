---
title: 'Module: tests/unit/tools/test_writer_path_normalization.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_writer_path_normalization.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_writer_path_normalization`/
symbols:
  _make_writer: _make_writer().
  TestPathConsistencyEndToEnd.test_write_and_delete_use_same_path_format: TestPathConsistencyEndToEnd#test_write_and_delete_use_same_path_format().
  _make_writer_with_delete_mocks: _make_writer_with_delete_mocks().
  TestNormalizePrefix.test_fix_resolves_the_bug: TestNormalizePrefix#test_fix_resolves_the_bug().
  TestAddRepositoryToGraph.test_stored_path_uses_forward_slashes: TestAddRepositoryToGraph#test_stored_path_uses_forward_slashes().
  TestAddRepositoryToGraph.test_stored_path_is_absolute: TestAddRepositoryToGraph#test_stored_path_is_absolute().
  TestDeleteRepositoryFromGraph.test_normalized_path_used_for_lookup: TestDeleteRepositoryFromGraph#test_normalized_path_used_for_lookup().
  TestDeleteRepositoryFromGraph.test_prefix_uses_forward_slash: TestDeleteRepositoryFromGraph#test_prefix_uses_forward_slash().
  TestDeleteRepositoryFromGraph.test_returns_false_for_nonexistent_repo: TestDeleteRepositoryFromGraph#test_returns_false_for_nonexistent_repo().
  TestDeleteFileFromGraph.test_normalized_path_used: TestDeleteFileFromGraph#test_normalized_path_used().
  TestGetRepoClassLookup.test_prefix_uses_forward_slash: TestGetRepoClassLookup#test_prefix_uses_forward_slash().
  TestDeleteRelationshipLinks.test_prefix_uses_forward_slash: TestDeleteRelationshipLinks#test_prefix_uses_forward_slash().
  TestAddMinimalFileNode.test_stored_paths_use_forward_slashes: TestAddMinimalFileNode#test_stored_paths_use_forward_slashes().
  TestNormalizePrefix.make_mock: TestNormalizePrefix#make_mock().
  _make_writer_with_delete_mocks._side_effect: _make_writer_with_delete_mocks()._side_effect().
  TestPathConsistencyEndToEnd.capture_write: TestPathConsistencyEndToEnd#capture_write().
  TestPathConsistencyEndToEnd._delete_side_effect: TestPathConsistencyEndToEnd#_delete_side_effect().
  TestNormalizePath: TestNormalizePath#
  TestNormalizePath.test_forward_slash_path_unchanged: TestNormalizePath#test_forward_slash_path_unchanged().
  TestNormalizePath.test_windows_style_backslash_path: TestNormalizePath#test_windows_style_backslash_path().
  TestNormalizePath.test_returns_string: TestNormalizePath#test_returns_string().
  TestNormalizePath.test_path_object_input: TestNormalizePath#test_path_object_input().
  TestNormalizePath.test_string_input: TestNormalizePath#test_string_input().
  TestNormalizePath.test_resolves_relative_path: TestNormalizePath#test_resolves_relative_path().
  TestNormalizePath.test_no_trailing_slash: TestNormalizePath#test_no_trailing_slash().
  TestNormalizePrefix: TestNormalizePrefix#
  TestNormalizePrefix.test_ends_with_forward_slash: TestNormalizePrefix#test_ends_with_forward_slash().
  TestNormalizePrefix.test_no_backslashes: TestNormalizePrefix#test_no_backslashes().
  TestNormalizePrefix.test_is_normalize_path_plus_slash: TestNormalizePrefix#test_is_normalize_path_plus_slash().
  TestNormalizePrefix.test_starts_with_query_correctness: TestNormalizePrefix#test_starts_with_query_correctness().
  TestNormalizePrefix.test_windows_backslash_does_not_match_without_fix: TestNormalizePrefix#test_windows_backslash_does_not_match_without_fix().
  TestAddRepositoryToGraph: TestAddRepositoryToGraph#
  TestDeleteRepositoryFromGraph: TestDeleteRepositoryFromGraph#
  TestDeleteFileFromGraph: TestDeleteFileFromGraph#
  TestGetRepoClassLookup: TestGetRepoClassLookup#
  TestDeleteRelationshipLinks: TestDeleteRelationshipLinks#
  TestAddMinimalFileNode: TestAddMinimalFileNode#
  TestPathConsistencyEndToEnd: TestPathConsistencyEndToEnd#
---
# Module: [`tests/unit/tools/test_writer_path_normalization.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py)

## Classes
### `TestAddMinimalFileNode`
- def: [`tests/unit/tools/test_writer_path_normalization.py:320`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L320)
- signature: `class TestAddMinimalFileNode:`
- members:
  - `test_stored_paths_use_forward_slashes(self, tmp_path)` — [`L321`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L321)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestAddRepositoryToGraph`
- def: [`tests/unit/tools/test_writer_path_normalization.py:199`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L199)
- signature: `class TestAddRepositoryToGraph:`
- members:
  - `test_stored_path_is_absolute(self, tmp_path)` — [`L215`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L215)
  - `test_stored_path_uses_forward_slashes(self, tmp_path)` — [`L200`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L200)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestDeleteFileFromGraph`
- def: [`tests/unit/tools/test_writer_path_normalization.py:273`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L273)
- signature: `class TestDeleteFileFromGraph:`
- members:
  - `test_normalized_path_used(self, tmp_path)` — [`L275`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L275)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestDeleteRelationshipLinks`
- def: [`tests/unit/tools/test_writer_path_normalization.py:302`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L302)
- signature: `class TestDeleteRelationshipLinks:`
- members:
  - `test_prefix_uses_forward_slash(self, tmp_path)` — [`L303`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L303)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestDeleteRepositoryFromGraph`
- def: [`tests/unit/tools/test_writer_path_normalization.py:228`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L228)
- signature: `class TestDeleteRepositoryFromGraph:`
- members:
  - `test_normalized_path_used_for_lookup(self, tmp_path)` — [`L230`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L230) — delete_repository_from_graph normalizes before querying.
  - `test_prefix_uses_forward_slash(self, tmp_path)` — [`L247`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L247) — The STARTS WITH prefix must end with '/' not '\'.
  - `test_returns_false_for_nonexistent_repo(self, tmp_path)` — [`L265`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L265)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestGetRepoClassLookup`
- def: [`tests/unit/tools/test_writer_path_normalization.py:289`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L289)
- signature: `class TestGetRepoClassLookup:`
- members:
  - `test_prefix_uses_forward_slash(self, tmp_path)` — [`L290`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L290)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestNormalizePath`
- def: [`tests/unit/tools/test_writer_path_normalization.py:35`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L35)
- doc: _normalize_path always returns a forward-slash absolute path string.
- signature: `class TestNormalizePath:`
- members:
  - `test_forward_slash_path_unchanged(self, tmp_path)` — [`L38`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L38)
  - `test_no_trailing_slash(self, tmp_path)` — [`L76`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L76) — _normalize_path does NOT add a trailing slash.
  - `test_path_object_input(self, tmp_path)` — [`L59`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L59) — Accepts a Path object, not just a string.
  - `test_resolves_relative_path(self)` — [`L71`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L71) — Relative paths become absolute.
  - `test_returns_string(self, tmp_path)` — [`L55`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L55)
  - `test_string_input(self, tmp_path)` — [`L65`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L65) — Accepts a plain string path.
  - `test_windows_style_backslash_path(self)` — [`L43`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L43) — Simulate what str(Path(...).resolve()) returns on Windows.

### `TestNormalizePrefix`
- def: [`tests/unit/tools/test_writer_path_normalization.py:82`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L82)
- doc: _normalize_prefix always ends with a single '/' and uses forward slashes.
- signature: `class TestNormalizePrefix:`
- members:
  - `make_mock(p)` — [`L136`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L136)
  - `test_ends_with_forward_slash(self, tmp_path)` — [`L85`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L85)
  - `test_fix_resolves_the_bug(self)` — [`L129`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L129) — With _normalize_path applied to both stored path and prefix,
  - `test_is_normalize_path_plus_slash(self, tmp_path)` — [`L93`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L93)
  - `test_no_backslashes(self, tmp_path)` — [`L89`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L89)
  - `test_starts_with_query_correctness(self, tmp_path)` — [`L96`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L96) — Simulate the exact STARTS WITH scenario from issue #1080.
  - `test_windows_backslash_does_not_match_without_fix(self)` — [`L113`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L113) — Demonstrate the original bug: backslash path vs forward-slash prefix.

### `TestPathConsistencyEndToEnd`
- def: [`tests/unit/tools/test_writer_path_normalization.py:343`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L343)
- doc: Verify that the path written by add_repository_to_graph is the same
- signature: `class TestPathConsistencyEndToEnd:`
- members:
  - `capture_write(original_session_run, query, **kwargs)` — [`L356`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L356)
  - `test_write_and_delete_use_same_path_format(self, tmp_path)` — [`L350`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L350)
- protocol/private: `_delete_side_effect`[`L372`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L372)
- uses (calls/refs, reference-scoped): (1 test-only callers)

## Functions
- `_make_writer()` — [`L160`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L160) — Return a GraphWriter with a fully mocked driver and db_manager.
- `_make_writer_with_delete_mocks()` — [`L178`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L178) — Return a GraphWriter with a mocked driver that returns proper values
- `_side_effect(*_a, **_kw)` — [`L188`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_writer_path_normalization.py#L188)

