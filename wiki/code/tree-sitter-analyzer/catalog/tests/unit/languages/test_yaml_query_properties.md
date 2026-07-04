---
title: 'Module: tests/unit/languages/test_yaml_query_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_query_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_query_properties`/
symbols:
  TestYAMLQueryProperties.test_property_11_query_result_correctness_getter_functions: TestYAMLQueryProperties#test_property_11_query_result_correctness_getter_functions().
  TestYAMLQueryProperties.test_property_11_query_result_correctness_consistency_across_interfaces: TestYAMLQueryProperties#test_property_11_query_result_correctness_consistency_across_interfaces().
  TestYAMLQueryProperties.test_property_11_query_result_correctness_all_queries_consistency: TestYAMLQueryProperties#test_property_11_query_result_correctness_all_queries_consistency().
  YAML_AVAILABLE: YAML_AVAILABLE.
  TestYAMLQueryProperties.test_property_11_query_result_correctness_description_exists: TestYAMLQueryProperties#test_property_11_query_result_correctness_description_exists().
  TestYAMLQueryProperties.test_property_11_query_result_correctness_invalid_query_handling: TestYAMLQueryProperties#test_property_11_query_result_correctness_invalid_query_handling().
  TestYAMLQueryProperties.test_property_11_query_result_correctness_tree_sitter_compilation: TestYAMLQueryProperties#test_property_11_query_result_correctness_tree_sitter_compilation().
  TestYAMLQueryProperties.test_property_11_query_result_correctness_all_queries_compile: TestYAMLQueryProperties#test_property_11_query_result_correctness_all_queries_compile().
  TestYAMLQueryProperties.test_property_11_query_result_correctness_syntax_validity: TestYAMLQueryProperties#test_property_11_query_result_correctness_syntax_validity().
  TestYAMLQueryProperties.test_property_11_query_result_correctness_no_empty_queries: TestYAMLQueryProperties#test_property_11_query_result_correctness_no_empty_queries().
  TestYAMLQueryProperties.test_property_11_query_result_correctness_query_coverage: TestYAMLQueryProperties#test_property_11_query_result_correctness_query_coverage().
  TestYAMLQueryProperties: TestYAMLQueryProperties#
---
# Module: [`tests/unit/languages/test_yaml_query_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py)

## Classes
### `TestYAMLQueryProperties`
- def: [`tests/unit/languages/test_yaml_query_properties.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L37)
- doc: Property-based tests for YAML query definitions.
- signature: `class TestYAMLQueryProperties:`
- members:
  - `test_property_11_query_result_correctness_all_queries_compile(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L290) — Feature: yaml-language-support, Property 11: Query Result Correctness
  - `test_property_11_query_result_correctness_all_queries_consistency(self, query_name: str)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L114) — Feature: yaml-language-support, Property 11: Query Result Correctness
  - `test_property_11_query_result_correctness_consistency_across_interfaces(self)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L352) — Feature: yaml-language-support, Property 11: Query Result Correctness
  - `test_property_11_query_result_correctness_description_exists(self, query_name: str)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L81) — Feature: yaml-language-support, Property 11: Query Result Correctness
  - `test_property_11_query_result_correctness_getter_functions(self, query_name: str)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L153) — Feature: yaml-language-support, Property 11: Query Result Correctness
  - `test_property_11_query_result_correctness_invalid_query_handling(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L223) — Feature: yaml-language-support, Property 11: Query Result Correctness
  - `test_property_11_query_result_correctness_no_empty_queries(self)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L195) — Feature: yaml-language-support, Property 11: Query Result Correctness
  - `test_property_11_query_result_correctness_query_coverage(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L321) — Feature: yaml-language-support, Property 11: Query Result Correctness
  - `test_property_11_query_result_correctness_syntax_validity(self, query_name: str)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L42) — Feature: yaml-language-support, Property 11: Query Result Correctness
  - `test_property_11_query_result_correctness_tree_sitter_compilation(self, query_name: str)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L259) — Feature: yaml-language-support, Property 11: Query Result Correctness
- uses (calls/refs, reference-scoped): [`YAML_QUERIES`](../../../tree_sitter_analyzer/queries/yaml.md#YAML_QUERIES.YAML_QUERIES), [`ALL_QUERIES`](../../../tree_sitter_analyzer/queries/yaml.md#ALL_QUERIES.ALL_QUERIES), [`YAML_QUERY_DESCRIPTIONS`](../../../tree_sitter_analyzer/queries/yaml.md#YAML_QUERY_DESCRIPTIONS.YAML_QUERY_DESCRIPTIONS), [`get_available_yaml_queries`](../../../tree_sitter_analyzer/queries/yaml.md#get_available_yaml_queries), [`get_query`](../../../tree_sitter_analyzer/queries/yaml.md#get_query), [`get_yaml_query`](../../../tree_sitter_analyzer/queries/yaml.md#get_yaml_query), [`list_queries`](../../../tree_sitter_analyzer/queries/yaml.md#list_queries), [`get_all_queries`](../../../tree_sitter_analyzer/queries/yaml.md#get_all_queries), [`get_yaml_query_description`](../../../tree_sitter_analyzer/queries/yaml.md#get_yaml_query_description)  (1 test-only)

## Module values
- `YAML_AVAILABLE` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_query_properties.py#L32)

