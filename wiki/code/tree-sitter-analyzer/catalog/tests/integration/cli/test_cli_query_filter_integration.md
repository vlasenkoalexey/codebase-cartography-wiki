---
title: 'Module: tests/integration/cli/test_cli_query_filter_integration.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_query_filter_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_cli_query_filter_integration`/TestCLIQueryFilter
symbols:
  TestCLIQueryFilterEdgeCases.temp_file: EdgeCases#temp_file.
  TestCLIQueryFilterIntegration.base_args: Integration#base_args.
  TestCLIQueryFilterIntegration.temp_file: Integration#temp_file.
  TestCLIQueryFilterIntegration.test_cli_query_with_name_filter: Integration#test_cli_query_with_name_filter().
  TestCLIQueryFilterIntegration.test_cli_query_with_pattern_filter: Integration#test_cli_query_with_pattern_filter().
  TestCLIQueryFilterIntegration.test_cli_query_with_parameter_filter: Integration#test_cli_query_with_parameter_filter().
  TestCLIQueryFilterIntegration.test_cli_query_with_modifier_filter: Integration#test_cli_query_with_modifier_filter().
  TestCLIQueryFilterIntegration.test_cli_query_with_multiple_filters: Integration#test_cli_query_with_multiple_filters().
  TestCLIQueryFilterIntegration.test_cli_query_filter_no_matches: Integration#test_cli_query_filter_no_matches().
  TestCLIQueryFilterIntegration.test_cli_custom_query_with_filter: Integration#test_cli_custom_query_with_filter().
  TestCLIQueryFilterIntegration.test_cli_query_without_filter: Integration#test_cli_query_without_filter().
  TestCLIQueryFilterEdgeCases.test_filter_overloaded_methods_by_params: EdgeCases#test_filter_overloaded_methods_by_params().
  TestCLIQueryFilterEdgeCases.test_filter_methods_with_annotations: EdgeCases#test_filter_methods_with_annotations().
  TestCLIQueryFilterEdgeCases.test_filter_generic_methods: EdgeCases#test_filter_generic_methods().
  TestCLIQueryFilterIntegration.teardown_method: Integration#teardown_method().
  TestCLIQueryFilterEdgeCases.teardown_method: EdgeCases#teardown_method().
  TestCLIQueryFilterIntegration.java_code: Integration#java_code.
  TestCLIQueryFilterEdgeCases.edge_case_code: EdgeCases#edge_case_code.
  TestCLIQueryFilterIntegration: Integration#
  TestCLIQueryFilterIntegration.setup_method: Integration#setup_method().
  TestCLIQueryFilterEdgeCases: EdgeCases#
  TestCLIQueryFilterEdgeCases.setup_method: EdgeCases#setup_method().
---
# Module: [`tests/integration/cli/test_cli_query_filter_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py)

## Classes
### `TestCLIQueryFilterEdgeCases`
- def: [`tests/integration/cli/test_cli_query_filter_integration.py:217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L217)
- doc: Edge case tests for CLI query filtering
- signature: `class TestCLIQueryFilterEdgeCases:`
- members:
  - `setup_method(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L220) — Set up test fixtures
  - `teardown_method(self)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L257) — Clean up test fixtures
  - `test_filter_generic_methods(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L312) — Test filtering generic methods
  - `test_filter_methods_with_annotations(self)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L289) — Test filtering methods that have annotations
  - `test_filter_overloaded_methods_by_params(self)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L264) — Test filtering overloaded methods by parameter count
  - `edge_case_code` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L223)
  - `temp_file` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L251)
- uses (calls/refs, reference-scoped): [`QueryCommand`](../../../tree_sitter_analyzer/cli/commands/query_command.md#QueryCommand), [`execute_query`](../../../tree_sitter_analyzer/cli/commands/query_command.md#QueryCommand.execute_query)

### `TestCLIQueryFilterIntegration`
- def: [`tests/integration/cli/test_cli_query_filter_integration.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L16)
- doc: Integration tests for CLI query filtering
- signature: `class TestCLIQueryFilterIntegration:`
- members:
  - `setup_method(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L19) — Set up test fixtures
  - `teardown_method(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L66) — Clean up test fixtures
  - `test_cli_custom_query_with_filter(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L179) — Test CLI custom query string with filter
  - `test_cli_query_filter_no_matches(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L164) — Test CLI query filter with no matching results
  - `test_cli_query_with_modifier_filter(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L130) — Test CLI query with modifier filter
  - `test_cli_query_with_multiple_filters(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L147) — Test CLI query with multiple filter conditions
  - `test_cli_query_with_name_filter(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L73) — Test CLI query with exact name filter
  - `test_cli_query_with_parameter_filter(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L107) — Test CLI query with parameter count filter
  - `test_cli_query_with_pattern_filter(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L91) — Test CLI query with pattern name filter
  - `test_cli_query_without_filter(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L197) — Test CLI query without filter (should return all results)
  - `base_args` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L54)
  - `java_code` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L22)
  - `temp_file` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_cli_query_filter_integration.py#L47)
- uses (calls/refs, reference-scoped): [`QueryCommand`](../../../tree_sitter_analyzer/cli/commands/query_command.md#QueryCommand), [`execute_query`](../../../tree_sitter_analyzer/cli/commands/query_command.md#QueryCommand.execute_query)

