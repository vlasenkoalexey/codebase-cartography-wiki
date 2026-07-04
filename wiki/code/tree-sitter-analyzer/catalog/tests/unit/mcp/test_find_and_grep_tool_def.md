---
title: 'Module: tests/unit/mcp/test_find_and_grep_tool_def.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_find_and_grep_tool_def.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_find_and_grep_tool_def`/
symbols:
  tool: tool().
  TestFindAndGrepToolInitialization.test_init_multiple_instances: TestFindAndGrepToolInitialization#test_init_multiple_instances().
  sample_project_structure: sample_project_structure().
  TestFindAndGrepToolInitialization: TestFindAndGrepToolInitialization#
  TestFindAndGrepToolInitialization.test_init_creates_tool: TestFindAndGrepToolInitialization#test_init_creates_tool().
  TestSetProjectPath: TestSetProjectPath#
  TestSetProjectPath.test_set_project_path_updates_all_components: TestSetProjectPath#test_set_project_path_updates_all_components().
  TestSetProjectPath.test_set_project_path_recreates_file_manager: TestSetProjectPath#test_set_project_path_recreates_file_manager().
  TestGetToolDefinition: TestGetToolDefinition#
  TestGetToolDefinition.test_tool_definition_description: TestGetToolDefinition#test_tool_definition_description().
  TestGetToolDefinition.test_input_schema_structure: TestGetToolDefinition#test_input_schema_structure().
  TestGetToolDefinition.test_required_fields: TestGetToolDefinition#test_required_fields().
  TestGetToolDefinition.test_file_stage_parameters: TestGetToolDefinition#test_file_stage_parameters().
  TestGetToolDefinition.test_content_stage_parameters: TestGetToolDefinition#test_content_stage_parameters().
  TestGetToolDefinition.test_output_format_parameters: TestGetToolDefinition#test_output_format_parameters().
  TestGetToolDefinition.test_sort_enum_values: TestGetToolDefinition#test_sort_enum_values().
  TestGetToolDefinition.test_case_enum_values: TestGetToolDefinition#test_case_enum_values().
  TestGetToolDefinition.test_output_format_enum_values: TestGetToolDefinition#test_output_format_enum_values().
  TestValidateRoots: TestValidateRoots#
  TestValidateRoots.test_validate_roots_success: TestValidateRoots#test_validate_roots_success().
  TestValidateRoots.test_validate_roots_multiple: TestValidateRoots#test_validate_roots_multiple().
  TestValidateRoots.test_validate_roots_invalid_directory: TestValidateRoots#test_validate_roots_invalid_directory().
  TestValidateArguments: TestValidateArguments#
  TestValidateArguments.test_validate_valid_arguments: TestValidateArguments#test_validate_valid_arguments().
  TestValidateArguments.test_validate_missing_roots: TestValidateArguments#test_validate_missing_roots().
  TestValidateArguments.test_validate_roots_not_array: TestValidateArguments#test_validate_roots_not_array().
  TestValidateArguments.test_validate_missing_query: TestValidateArguments#test_validate_missing_query().
  TestValidateArguments.test_validate_query_not_string: TestValidateArguments#test_validate_query_not_string().
  TestValidateArguments.test_validate_empty_query: TestValidateArguments#test_validate_empty_query().
  TestValidateArguments.test_validate_whitespace_query: TestValidateArguments#test_validate_whitespace_query().
  TestValidateArguments.test_validate_invalid_file_limit_type: TestValidateArguments#test_validate_invalid_file_limit_type().
---
# Module: [`tests/unit/mcp/test_find_and_grep_tool_def.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py)

## Classes
### `TestFindAndGrepToolInitialization`
- def: [`tests/unit/mcp/test_find_and_grep_tool_def.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L37)
- doc: Tests for tool initialization.
- signature: `class TestFindAndGrepToolInitialization:`
- members:
  - `test_init_creates_tool(self, tool)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L40) — Test that initialization creates a tool instance.
  - `test_init_multiple_instances(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L45) — Test that multiple instances are independent.
- uses (calls/refs, reference-scoped): [`FindAndGrepTool`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_tool.md#FindAndGrepTool)

### `TestGetToolDefinition`
- def: [`tests/unit/mcp/test_find_and_grep_tool_def.py:68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L68)
- doc: Tests for get_tool_definition method.
- signature: `class TestGetToolDefinition:`
- members:
  - `test_case_enum_values(self, tool)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L163) — Test that case parameter has correct enum values.
  - `test_content_stage_parameters(self, tool)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L117) — Test that content stage parameters are defined.
  - `test_file_stage_parameters(self, tool)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L94) — Test that file stage parameters are defined.
  - `test_input_schema_structure(self, tool)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L77) — Test that input schema has correct structure.
  - `test_output_format_enum_values(self, tool)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L171) — Test that output_format parameter has correct enum values.
  - `test_output_format_parameters(self, tool)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L141) — Test that output format parameters are defined.
  - `test_required_fields(self, tool)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L85) — Test that required fields are correctly defined.
  - `test_sort_enum_values(self, tool)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L156) — Test that sort parameter has correct enum values.
  - `test_tool_definition_description(self, tool)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L71) — Test that tool definition has description.

### `TestSetProjectPath`
- def: [`tests/unit/mcp/test_find_and_grep_tool_def.py:52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L52)
- doc: Tests for set_project_path method.
- signature: `class TestSetProjectPath:`
- members:
  - `test_set_project_path_recreates_file_manager(self, tool)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L61) — Test that set_project_path recreates file manager.
  - `test_set_project_path_updates_all_components(self, tool)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L55) — Test that set_project_path updates all components.

### `TestValidateArguments`
- def: [`tests/unit/mcp/test_find_and_grep_tool_def.py:206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L206)
- doc: Tests for validate_arguments method.
- signature: `class TestValidateArguments:`
- members:
  - `test_validate_empty_query(self, tool)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L241) — Test validation fails when query is empty.
  - `test_validate_invalid_file_limit_type(self, tool)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L253) — Test validation fails when file_limit is not an integer.
  - `test_validate_missing_query(self, tool)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L229) — Test validation fails when query is missing.
  - `test_validate_missing_roots(self, tool)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L217) — Test validation fails when roots is missing.
  - `test_validate_query_not_string(self, tool)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L235) — Test validation fails when query is not a string.
  - `test_validate_roots_not_array(self, tool)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L223) — Test validation fails when roots is not an array.
  - `test_validate_valid_arguments(self, tool)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L209) — Test validation with valid arguments.
  - `test_validate_whitespace_query(self, tool)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L247) — Test validation fails when query is only whitespace.

### `TestValidateRoots`
- def: [`tests/unit/mcp/test_find_and_grep_tool_def.py:180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L180)
- doc: Tests for _validate_roots method.
- signature: `class TestValidateRoots:`
- members:
  - `test_validate_roots_invalid_directory(self, tool)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L199) — Test validation fails when directory doesn't exist.
  - `test_validate_roots_multiple(self, tool, sample_project_structure)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L190) — Test validation of multiple roots.
  - `test_validate_roots_success(self, tool, sample_project_structure)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L183) — Test successful roots validation.

## Functions
- `sample_project_structure(tmp_path: Path)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L22) — Create a sample project structure for testing.
- `tool()` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_tool_def.py#L16) — Create a fresh tool instance for each test.

