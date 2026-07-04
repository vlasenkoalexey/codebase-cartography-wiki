---
title: 'Module: tests/unit/mcp/test_file_health_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_file_health_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_file_health_tool`/
symbols:
  test_low_complexity_smell_reports_largest_function_location: test_low_complexity_smell_reports_largest_function_location().
  test_execute_scores_file_and_returns_agent_signal: test_execute_scores_file_and_returns_agent_signal().
  test_execute_reports_missing_file_with_clear_error: test_execute_reports_missing_file_with_clear_error().
  test_file_health_binary_file: test_file_health_binary_file().
  test_file_health_empty_file: test_file_health_empty_file().
  test_tool_definition_exposes_file_health_contract: test_tool_definition_exposes_file_health_contract().
  test_validate_arguments_requires_non_empty_file_path: test_validate_arguments_requires_non_empty_file_path().
  _run: _run().
  test_file_health_result_marks_healthy_files_as_no_action: test_file_health_result_marks_healthy_files_as_no_action().
  test_file_health_result_includes_direct_agent_commands_for_smells: test_file_health_result_includes_direct_agent_commands_for_smells().
  test_agent_summary_avoids_refactor_when_smell_is_generic_complexity: test_agent_summary_avoids_refactor_when_smell_is_generic_complexity().
  test_agent_summary_surfaces_target_symbol_and_detail: test_agent_summary_surfaces_target_symbol_and_detail().
  test_low_complexity_smell_falls_back_to_control_flow_line: test_low_complexity_smell_falls_back_to_control_flow_line().
  test_low_structure_smell_reports_deepest_line_when_available: test_low_structure_smell_reports_deepest_line_when_available().
  test_high_coupling_smell_reports_import_cluster_line: test_high_coupling_smell_reports_import_cluster_line().
  test_deep_nesting_reports_actionable_line_number: test_deep_nesting_reports_actionable_line_number().
  test_deep_nesting_ignores_multiline_data_literals: test_deep_nesting_ignores_multiline_data_literals().
  test_god_class_requires_exactly_one_oversized_class: test_god_class_requires_exactly_one_oversized_class().
  test_god_class_reports_actionable_symbol_location: test_god_class_reports_actionable_symbol_location().
  test_long_function_smells_report_symbol_and_line: test_long_function_smells_report_symbol_and_line().
  test_heuristic_long_method_smells_report_symbol_and_line: test_heuristic_long_method_smells_report_symbol_and_line().
  test_technical_debt_ignores_marker_strings_in_code: test_technical_debt_ignores_marker_strings_in_code().
  test_technical_debt_reports_first_comment_line: test_technical_debt_reports_first_comment_line().
  test_god_class_reports_single_oversized_class_span: test_god_class_reports_single_oversized_class_span().
---
# Module: [`tests/unit/mcp/test_file_health_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py)

## Functions
- `_run(coro)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L27)
- `test_agent_summary_avoids_refactor_when_smell_is_generic_complexity()` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L194)
- `test_agent_summary_surfaces_target_symbol_and_detail()` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L219)
- `test_deep_nesting_ignores_multiline_data_literals()` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L367)
- `test_deep_nesting_reports_actionable_line_number()` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L342)
- `test_execute_reports_missing_file_with_clear_error(tmp_path)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L81)
- `test_execute_scores_file_and_returns_agent_signal(tmp_path)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L50)
- `test_file_health_binary_file(tmp_path)` — [`L544`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L544) — Bug M6 regression: refuse to analyze binary files cleanly.
- `test_file_health_empty_file(tmp_path)` — [`L560`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L560) — Bug M7 regression: 0-byte file returns an n/a envelope, never grade B.
- `test_file_health_result_includes_direct_agent_commands_for_smells()` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L127)
- `test_file_health_result_marks_healthy_files_as_no_action()` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L88)
- `test_god_class_reports_actionable_symbol_location()` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L409)
- `test_god_class_reports_single_oversized_class_span()` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L512)
- `test_god_class_requires_exactly_one_oversized_class()` — [`L388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L388)
- `test_heuristic_long_method_smells_report_symbol_and_line()` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L453)
- `test_high_coupling_smell_reports_import_cluster_line()` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L322)
- `test_long_function_smells_report_symbol_and_line()` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L430)
- `test_low_complexity_smell_falls_back_to_control_flow_line()` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L276)
- `test_low_complexity_smell_reports_largest_function_location()` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L248)
- `test_low_structure_smell_reports_deepest_line_when_available()` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L297)
- `test_technical_debt_ignores_marker_strings_in_code()` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L471)
- `test_technical_debt_reports_first_comment_line()` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L487)
- `test_tool_definition_exposes_file_health_contract()` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L31)
- `test_validate_arguments_requires_non_empty_file_path()` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_file_health_tool.py#L41)

