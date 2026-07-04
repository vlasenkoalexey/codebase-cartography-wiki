---
title: 'Module: tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools.test_analyze_scale_tool_cli_compat_unit`/
symbols:
  tool: tool().
  TestInit: TestInit#
  TestInit.test_initializes: TestInit#test_initializes().
  TestGetToolSchema: TestGetToolSchema#
  TestGetToolSchema.test_schema_structure: TestGetToolSchema#test_schema_structure().
  TestGetToolSchema.test_schema_optional_fields: TestGetToolSchema#test_schema_optional_fields().
  TestGetToolSchema.test_schema_no_additional_properties: TestGetToolSchema#test_schema_no_additional_properties().
  TestGetToolDefinition: TestGetToolDefinition#
  TestGetToolDefinition.test_returns_definition_with_mcp: TestGetToolDefinition#test_returns_definition_with_mcp().
  TestGetToolDefinition.test_returns_definition_as_dict_without_mcp: TestGetToolDefinition#test_returns_definition_as_dict_without_mcp().
  TestValidateArguments: TestValidateArguments#
  TestValidateArguments.test_valid_arguments: TestValidateArguments#test_valid_arguments().
  TestValidateArguments.test_valid_with_all_fields: TestValidateArguments#test_valid_with_all_fields().
  TestValidateArguments.test_missing_required_field: TestValidateArguments#test_missing_required_field().
  TestValidateArguments.test_file_path_not_string: TestValidateArguments#test_file_path_not_string().
  TestValidateArguments.test_file_path_empty: TestValidateArguments#test_file_path_empty().
  TestValidateArguments.test_language_not_string: TestValidateArguments#test_language_not_string().
  TestValidateArguments.test_include_complexity_not_bool: TestValidateArguments#test_include_complexity_not_bool().
  TestValidateArguments.test_include_details_not_bool: TestValidateArguments#test_include_details_not_bool().
  TestExecute: TestExecute#
  TestExecute.test_missing_file_path: TestExecute#test_missing_file_path().
  TestExecute.test_file_not_found: TestExecute#test_file_not_found().
  TestExecute.test_unknown_language: TestExecute#test_unknown_language().
  TestExecute.test_success_with_elements: TestExecute#test_success_with_elements().
  TestExecute.test_success_no_package: TestExecute#test_success_no_package().
  TestExecute.test_analysis_failure_with_error_message: TestExecute#test_analysis_failure_with_error_message().
  TestExecute.test_analysis_failure_without_error_message: TestExecute#test_analysis_failure_without_error_message().
  TestExecute.test_exception_returns_error_format: TestExecute#test_exception_returns_error_format().
  TestExecute.test_explicit_language: TestExecute#test_explicit_language().
  TestExecute.test_method_count_includes_method_type: TestExecute#test_method_count_includes_method_type().
---
# Module: [`tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py)

## Classes
### `TestExecute`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py:97`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L97)
- signature: `class TestExecute:`
- members:
  - `test_analysis_failure_with_error_message(self, tool)` — [`L204`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L204)
  - `test_analysis_failure_without_error_message(self, tool)` — [`L234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L234)
  - `test_exception_returns_error_format(self, tool)` — [`L264`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L264)
  - `test_explicit_language(self, tool)` — [`L290`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L290)
  - `test_file_not_found(self, tool)` — [`L104`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L104)
  - `test_method_count_includes_method_type(self, tool)` — [`L315`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L315)
  - `test_missing_file_path(self, tool)` — [`L99`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L99)
  - `test_success_no_package(self, tool)` — [`L173`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L173)
  - `test_success_with_elements(self, tool)` — [`L122`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L122)
  - `test_unknown_language(self, tool)` — [`L110`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L110)

### `TestGetToolDefinition`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py:43`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L43)
- signature: `class TestGetToolDefinition:`
- members:
  - `test_returns_definition_as_dict_without_mcp(self, tool)` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L50)
  - `test_returns_definition_with_mcp(self, tool)` — [`L44`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L44)

### `TestGetToolSchema`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py:24`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L24)
- signature: `class TestGetToolSchema:`
- members:
  - `test_schema_no_additional_properties(self, tool)` — [`L38`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L38)
  - `test_schema_optional_fields(self, tool)` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L32)
  - `test_schema_structure(self, tool)` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L25)

### `TestInit`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py:18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L18)
- signature: `class TestInit:`
- members:
  - `test_initializes(self, tool)` — [`L19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L19)

### `TestValidateArguments`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py:57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L57)
- signature: `class TestValidateArguments:`
- members:
  - `test_file_path_empty(self, tool)` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L78)
  - `test_file_path_not_string(self, tool)` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L74)
  - `test_include_complexity_not_bool(self, tool)` — [`L86`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L86)
  - `test_include_details_not_bool(self, tool)` — [`L92`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L92)
  - `test_language_not_string(self, tool)` — [`L82`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L82)
  - `test_missing_required_field(self, tool)` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L70)
  - `test_valid_arguments(self, tool)` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L58)
  - `test_valid_with_all_fields(self, tool)` — [`L61`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L61)

## Functions
- `tool()` — [`L11`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_tool_cli_compat_unit.py#L11)

