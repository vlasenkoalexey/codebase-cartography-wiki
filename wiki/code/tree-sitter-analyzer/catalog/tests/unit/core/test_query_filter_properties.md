---
title: 'Module: tests/unit/core/test_query_filter_properties.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_query_filter_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_query_filter_properties`/
symbols:
  query_results_strategy: query_results_strategy().
  java_method_content_strategy: java_method_content_strategy().
  TestQueryFilterCorrectnessProperties.test_property_7_name_exact_filter_correctness: TestQueryFilterCorrectnessProperties#test_property_7_name_exact_filter_correctness().
  TestQueryFilterCorrectnessProperties.test_property_7_params_filter_correctness: TestQueryFilterCorrectnessProperties#test_property_7_params_filter_correctness().
  TestQueryFilterCorrectnessProperties.test_property_7_pattern_filter_correctness: TestQueryFilterCorrectnessProperties#test_property_7_pattern_filter_correctness().
  TestQueryFilterCorrectnessProperties.test_property_7_static_filter_correctness: TestQueryFilterCorrectnessProperties#test_property_7_static_filter_correctness().
  TestQueryFilterCorrectnessProperties.test_property_7_static_false_filter_correctness: TestQueryFilterCorrectnessProperties#test_property_7_static_false_filter_correctness().
  TestQueryFilterCorrectnessProperties.test_property_7_public_filter_correctness: TestQueryFilterCorrectnessProperties#test_property_7_public_filter_correctness().
  TestQueryFilterCorrectnessProperties.test_property_7_private_filter_correctness: TestQueryFilterCorrectnessProperties#test_property_7_private_filter_correctness().
  TestQueryFilterCorrectnessProperties.test_property_7_protected_filter_correctness: TestQueryFilterCorrectnessProperties#test_property_7_protected_filter_correctness().
  TestQueryFilterCorrectnessProperties.test_property_7_combined_filters_correctness: TestQueryFilterCorrectnessProperties#test_property_7_combined_filters_correctness().
  TestQueryFilterCorrectnessProperties.test_property_7_empty_filter_returns_all: TestQueryFilterCorrectnessProperties#test_property_7_empty_filter_returns_all().
  TestQueryFilterCorrectnessProperties.test_property_7_filtered_subset_of_original: TestQueryFilterCorrectnessProperties#test_property_7_filtered_subset_of_original().
  TestQueryFilterCorrectnessProperties.test_property_7_filter_preserves_result_structure: TestQueryFilterCorrectnessProperties#test_property_7_filter_preserves_result_structure().
  TestQueryFilterCorrectnessProperties.setup_method: TestQueryFilterCorrectnessProperties#setup_method().
  method_name_strategy: method_name_strategy().
  modifier_strategy: modifier_strategy().
  static_modifier_strategy: static_modifier_strategy().
  parameter_list_strategy: parameter_list_strategy().
  TestQueryFilterCorrectnessProperties: TestQueryFilterCorrectnessProperties#
---
# Module: [`tests/unit/core/test_query_filter_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py)

## Classes
### `TestQueryFilterCorrectnessProperties`
- def: [`tests/unit/core/test_query_filter_properties.py:114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L114)
- doc: Property-based tests for QueryFilter correctness.
- signature: `class TestQueryFilterCorrectnessProperties:`
- members:
  - `setup_method(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L122) — Set up test fixtures.
  - `test_property_7_combined_filters_correctness(self, results: list[dict])` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L274) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_empty_filter_returns_all(self, results: list[dict])` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L328) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_filter_preserves_result_structure(self, results: list[dict])` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L365) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_filtered_subset_of_original(self, results: list[dict])` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L346) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_name_exact_filter_correctness(self, results: list[dict])` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L128) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_params_filter_correctness(self, results: list[dict], param_count: int)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L252) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_pattern_filter_correctness(self, results: list[dict])` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L297) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_private_filter_correctness(self, results: list[dict])` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L211) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_protected_filter_correctness(self, results: list[dict])` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L230) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_public_filter_correctness(self, results: list[dict])` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L192) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_static_false_filter_correctness(self, results: list[dict])` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L173) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
  - `test_property_7_static_filter_correctness(self, results: list[dict])` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L154) — **Feature: test-coverage-improvement, Property 7: Query Filter Correctness**
- uses (calls/refs, reference-scoped): [`QueryFilter`](../../../tree_sitter_analyzer/core/query_filter.md#QueryFilter), [`filter_results`](../../../tree_sitter_analyzer/core/query_filter.md#QueryFilter.filter_results), [`_count_parameters`](../../../tree_sitter_analyzer/core/query_filter.md#QueryFilter._count_parameters), [`_extract_method_name`](../../../tree_sitter_analyzer/core/query_filter.md#QueryFilter._extract_method_name)  (1 test-only)

## Functions
- `java_method_content_strategy(draw: st.DrawFn)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L68) — Generate Java method content with known properties.
- `method_name_strategy(draw: st.DrawFn)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L25) — Generate valid method names.
- `modifier_strategy(draw: st.DrawFn)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L39) — Generate access modifiers.
- `parameter_list_strategy(draw: st.DrawFn)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L51) — Generate parameter list and count.
- `query_results_strategy(draw: st.DrawFn)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L102) — Generate a list of query results.
- `static_modifier_strategy(draw: st.DrawFn)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_query_filter_properties.py#L45) — Generate static modifier.

