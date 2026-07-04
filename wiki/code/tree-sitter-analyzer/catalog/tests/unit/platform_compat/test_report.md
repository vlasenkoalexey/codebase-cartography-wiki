---
title: 'Module: tests/unit/platform_compat/test_report.py'
type: catalog
provenance: extracted
module: tests/unit/platform_compat/test_report.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.platform_compat.test_report`/
symbols:
  _make_profile: _make_profile().
  TestGenerateCompatibilityMatrix.test_single_profile_no_errors: TestGenerateCompatibilityMatrix#test_single_profile_no_errors().
  TestGenerateCompatibilityMatrix.test_profile_with_error_shows_warning: TestGenerateCompatibilityMatrix#test_profile_with_error_shows_warning().
  TestGenerateCompatibilityMatrix.test_missing_construct_shows_missing: TestGenerateCompatibilityMatrix#test_missing_construct_shows_missing().
  TestGenerateCompatibilityMatrix.test_profiles_sorted_by_platform_key: TestGenerateCompatibilityMatrix#test_profiles_sorted_by_platform_key().
  TestGenerateCompatibilityMatrix.test_invalid_json_skipped: TestGenerateCompatibilityMatrix#test_invalid_json_skipped().
  TestGenerateCompatibilityMatrix.test_json_without_platform_key_skipped: TestGenerateCompatibilityMatrix#test_json_without_platform_key_skipped().
  TestGenerateCompatibilityMatrix.test_markdown_table_format: TestGenerateCompatibilityMatrix#test_markdown_table_format().
  TestGenerateCompatibilityMatrix.test_empty_dir_returns_no_profiles: TestGenerateCompatibilityMatrix#test_empty_dir_returns_no_profiles().
  TestGenerateCompatibilityMatrix: TestGenerateCompatibilityMatrix#
---
# Module: [`tests/unit/platform_compat/test_report.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py)

## Classes
### `TestGenerateCompatibilityMatrix`
- def: [`tests/unit/platform_compat/test_report.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py#L42)
- doc: Tests for generate_compatibility_matrix.
- signature: `class TestGenerateCompatibilityMatrix:`
- members:
  - `test_empty_dir_returns_no_profiles(self, tmp_path: Path)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py#L45)
  - `test_invalid_json_skipped(self, tmp_path: Path)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py#L122)
  - `test_json_without_platform_key_skipped(self, tmp_path: Path)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py#L140)
  - `test_markdown_table_format(self, tmp_path: Path)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py#L158)
  - `test_missing_construct_shows_missing(self, tmp_path: Path)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py#L79)
  - `test_profile_with_error_shows_warning(self, tmp_path: Path)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py#L65)
  - `test_profiles_sorted_by_platform_key(self, tmp_path: Path)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py#L105)
  - `test_single_profile_no_errors(self, tmp_path: Path)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py#L49)
- uses (calls/refs, reference-scoped): [`ParsingBehavior`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior), [`generate_compatibility_matrix`](../../../tree_sitter_analyzer/platform_compat/report.md#generate_compatibility_matrix), [`node_type`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior.node_type), [`has_error`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior.has_error), [`attributes`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior.attributes), [`construct_id`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior.construct_id), [`element_count`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior.element_count)  (1 test-only)

## Functions
- `_make_profile(tmp_path: Path, platform_key: str, behaviors: dict[str, ParsingBehavior])` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_report.py#L10) — Create a profile.json under the expected directory structure.

