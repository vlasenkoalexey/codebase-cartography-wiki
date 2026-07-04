---
title: 'Module: tests/integration/platform/test_compare_properties.py'
type: catalog
provenance: extracted
module: tests/integration/platform/test_compare_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.platform.test_compare_properties`/
symbols:
  behavior_profile_strategy: behavior_profile_strategy().
  parsing_behavior_strategy: parsing_behavior_strategy().
  TestCompareProperties.test_profile_comparison_accuracy: TestCompareProperties#test_profile_comparison_accuracy().
  test_compare_missing_construct: test_compare_missing_construct().
  test_compare_no_differences: test_compare_no_differences().
  test_compare_count_mismatch: test_compare_count_mismatch().
  test_compare_error_mismatch: test_compare_error_mismatch().
  TestCompareProperties.test_profile_comparison_identity: TestCompareProperties#test_profile_comparison_identity().
  TestCompareProperties: TestCompareProperties#
---
# Module: [`tests/integration/platform/test_compare_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_compare_properties.py)

## Classes
### `TestCompareProperties`
- def: [`tests/integration/platform/test_compare_properties.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_compare_properties.py#L37)
- signature: `class TestCompareProperties:`
- members:
  - `test_profile_comparison_accuracy(self, profile)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_compare_properties.py#L52) — Property 9: Profile comparison accuracy (Differences)
  - `test_profile_comparison_identity(self, profile)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_compare_properties.py#L40) — Property 9: Profile comparison accuracy (Identity)
- uses (calls/refs, reference-scoped): [`compare_profiles`](../../../tree_sitter_analyzer/platform_compat/compare.md#compare_profiles), [`diff_type`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.diff_type), [`differences`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.differences), [`has_differences`](../../../tree_sitter_analyzer/platform_compat/compare.md#ProfileComparison.has_differences), [`construct_id`](../../../tree_sitter_analyzer/platform_compat/compare.md#BehaviorDifference.construct_id)  (1 test-only)

## Functions
- `behavior_profile_strategy(draw)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_compare_properties.py#L26)
- `parsing_behavior_strategy(draw)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_compare_properties.py#L14)
- `test_compare_count_mismatch()` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_compare_properties.py#L114)
- `test_compare_error_mismatch()` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_compare_properties.py#L131)
- `test_compare_missing_construct()` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_compare_properties.py#L80)
- `test_compare_no_differences()` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_compare_properties.py#L96)

