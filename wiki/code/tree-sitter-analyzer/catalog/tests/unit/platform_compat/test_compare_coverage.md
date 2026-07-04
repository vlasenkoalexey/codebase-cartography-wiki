---
title: 'Module: tests/unit/platform_compat/test_compare_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/platform_compat/test_compare_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.platform_compat.test_compare_coverage`/
symbols:
  _make_profile: _make_profile().
  _make_behavior: _make_behavior().
  test_missing_construct_in_b: test_missing_construct_in_b().
  test_missing_construct_in_a: test_missing_construct_in_a().
  test_error_mismatch: test_error_mismatch().
  test_count_mismatch: test_count_mismatch().
  test_behavior_difference_fields: test_behavior_difference_fields().
  test_profile_comparison_has_differences: test_profile_comparison_has_differences().
  test_attribute_mismatch: test_attribute_mismatch().
  test_no_differences: test_no_differences().
  test_diff_report_with_differences: test_diff_report_with_differences().
  test_diff_report_no_differences: test_diff_report_no_differences().
---
# Module: [`tests/unit/platform_compat/test_compare_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py)

## Functions
- `_make_behavior(construct_id="f1", node_type="function", element_count=3, attributes=None, has_error=False, known_issues=None)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L16)
- `_make_profile(platform_key="linux-3.12", behaviors=None)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L34)
- `test_attribute_mismatch()` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L95) — Cover attribute_mismatch with DeepDiff (line 100-116).
- `test_behavior_difference_fields()` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L145) — Cover BehaviorDifference dataclass instantiation.
- `test_count_mismatch()` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L83) — Cover count_mismatch branch (line 91-99).
- `test_diff_report_no_differences()` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L130) — Cover generate_diff_report when has_differences is False.
- `test_diff_report_with_differences()` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L118) — Cover generate_diff_report when has_differences is True.
- `test_error_mismatch()` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L71) — Cover error_mismatch branch.
- `test_missing_construct_in_a()` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L60) — Cover key in keys_b - keys_a.
- `test_missing_construct_in_b()` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L48) — Cover key in keys_a - keys_b (line 60).
- `test_no_differences()` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L103) — Cover the happy path with no differences.
- `test_profile_comparison_has_differences()` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/platform_compat/test_compare_coverage.py#L158) — Cover ProfileComparison.has_differences property.

