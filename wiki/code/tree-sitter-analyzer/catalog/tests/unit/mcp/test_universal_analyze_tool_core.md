---
title: 'Module: tests/unit/mcp/test_universal_analyze_tool_core.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_universal_analyze_tool_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_universal_analyze_tool_core`/
symbols:
  tool: tool().
  tool_with_project_root: tool_with_project_root().
  TestUniversalAnalyzeToolInit: TestUniversalAnalyzeToolInit#
  TestUniversalAnalyzeToolInit.test_init_without_project_root: TestUniversalAnalyzeToolInit#test_init_without_project_root().
  TestUniversalAnalyzeToolInit.test_init_with_project_root: TestUniversalAnalyzeToolInit#test_init_with_project_root().
  TestUniversalAnalyzeToolSetProjectPath: TestUniversalAnalyzeToolSetProjectPath#
  TestUniversalAnalyzeToolSetProjectPath.test_set_project_path_updates_analysis_engine: TestUniversalAnalyzeToolSetProjectPath#test_set_project_path_updates_analysis_engine().
  TestUniversalAnalyzeToolGetToolDefinition: TestUniversalAnalyzeToolGetToolDefinition#
  TestUniversalAnalyzeToolGetToolDefinition.test_get_tool_definition_name: TestUniversalAnalyzeToolGetToolDefinition#test_get_tool_definition_name().
  TestUniversalAnalyzeToolGetToolDefinition.test_get_tool_definition_has_description: TestUniversalAnalyzeToolGetToolDefinition#test_get_tool_definition_has_description().
  TestUniversalAnalyzeToolGetToolDefinition.test_get_tool_definition_has_input_schema: TestUniversalAnalyzeToolGetToolDefinition#test_get_tool_definition_has_input_schema().
  TestUniversalAnalyzeToolGetToolDefinition.test_get_tool_definition_schema_has_file_path: TestUniversalAnalyzeToolGetToolDefinition#test_get_tool_definition_schema_has_file_path().
  TestUniversalAnalyzeToolGetToolDefinition.test_get_tool_definition_schema_has_language: TestUniversalAnalyzeToolGetToolDefinition#test_get_tool_definition_schema_has_language().
  TestUniversalAnalyzeToolGetToolDefinition.test_get_tool_definition_schema_has_analysis_type: TestUniversalAnalyzeToolGetToolDefinition#test_get_tool_definition_schema_has_analysis_type().
  TestUniversalAnalyzeToolGetToolDefinition.test_get_tool_definition_schema_has_include_ast: TestUniversalAnalyzeToolGetToolDefinition#test_get_tool_definition_schema_has_include_ast().
  TestUniversalAnalyzeToolGetToolDefinition.test_get_tool_definition_schema_has_include_queries: TestUniversalAnalyzeToolGetToolDefinition#test_get_tool_definition_schema_has_include_queries().
  TestUniversalAnalyzeToolGetToolDefinition.test_get_tool_definition_schema_has_output_format: TestUniversalAnalyzeToolGetToolDefinition#test_get_tool_definition_schema_has_output_format().
  TestUniversalAnalyzeToolValidateArguments: TestUniversalAnalyzeToolValidateArguments#
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_valid_basic: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_valid_basic().
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_with_language: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_with_language().
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_with_analysis_type: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_with_analysis_type().
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_missing_file_path: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_missing_file_path().
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_invalid_file_path_type: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_invalid_file_path_type().
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_empty_file_path: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_empty_file_path().
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_invalid_language_type: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_invalid_language_type().
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_invalid_analysis_type_type: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_invalid_analysis_type_type().
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_invalid_analysis_type_value: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_invalid_analysis_type_value().
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_invalid_include_ast_type: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_invalid_include_ast_type().
  TestUniversalAnalyzeToolValidateArguments.test_validate_arguments_invalid_include_queries_type: TestUniversalAnalyzeToolValidateArguments#test_validate_arguments_invalid_include_queries_type().
---
# Module: [`tests/unit/mcp/test_universal_analyze_tool_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py)

## Classes
### `TestUniversalAnalyzeToolGetToolDefinition`
- def: [`tests/unit/mcp/test_universal_analyze_tool_core.py:51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L51)
- doc: Tests for get_tool_definition method.
- signature: `class TestUniversalAnalyzeToolGetToolDefinition:`
- members:
  - `test_get_tool_definition_has_description(self, tool)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L59) — Test tool definition has description.
  - `test_get_tool_definition_has_input_schema(self, tool)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L66) — Test tool definition has input schema.
  - `test_get_tool_definition_name(self, tool)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L54) — Test tool definition has correct name.
  - `test_get_tool_definition_schema_has_analysis_type(self, tool)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L84) — Test schema has analysis_type property.
  - `test_get_tool_definition_schema_has_file_path(self, tool)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L72) — Test schema has file_path property.
  - `test_get_tool_definition_schema_has_include_ast(self, tool)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L97) — Test schema has include_ast property.
  - `test_get_tool_definition_schema_has_include_queries(self, tool)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L103) — Test schema has include_queries property.
  - `test_get_tool_definition_schema_has_language(self, tool)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L78) — Test schema has language property.
  - `test_get_tool_definition_schema_has_output_format(self, tool)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L109) — Test schema has output_format property.

### `TestUniversalAnalyzeToolInit`
- def: [`tests/unit/mcp/test_universal_analyze_tool_core.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L25)
- doc: Tests for UniversalAnalyzeTool initialization.
- signature: `class TestUniversalAnalyzeToolInit:`
- members:
  - `test_init_with_project_root(self, tool_with_project_root)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L34) — Test initialization with project root.
  - `test_init_without_project_root(self, tool)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L28) — Test initialization without project root.

### `TestUniversalAnalyzeToolSetProjectPath`
- def: [`tests/unit/mcp/test_universal_analyze_tool_core.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L41)
- doc: Tests for set_project_path method.
- signature: `class TestUniversalAnalyzeToolSetProjectPath:`
- members:
  - `test_set_project_path_updates_analysis_engine(self, tool)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L44) — Test that setting project path updates analysis engine.

### `TestUniversalAnalyzeToolValidateArguments`
- def: [`tests/unit/mcp/test_universal_analyze_tool_core.py:118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L118)
- doc: Tests for validate_arguments method.
- signature: `class TestUniversalAnalyzeToolValidateArguments:`
- members:
  - `test_validate_arguments_empty_file_path(self, tool)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L148) — Test validation fails when file_path is empty.
  - `test_validate_arguments_invalid_analysis_type_type(self, tool)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L160) — Test validation fails when analysis_type is not a string.
  - `test_validate_arguments_invalid_analysis_type_value(self, tool)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L166) — Test validation fails when analysis_type is invalid.
  - `test_validate_arguments_invalid_file_path_type(self, tool)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L142) — Test validation fails when file_path is not a string.
  - `test_validate_arguments_invalid_include_ast_type(self, tool)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L172) — Test validation fails when include_ast is not a boolean.
  - `test_validate_arguments_invalid_include_queries_type(self, tool)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L178) — Test validation fails when include_queries is not a boolean.
  - `test_validate_arguments_invalid_language_type(self, tool)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L154) — Test validation fails when language is not a string.
  - `test_validate_arguments_missing_file_path(self, tool)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L136) — Test validation fails when file_path is missing.
  - `test_validate_arguments_valid_basic(self, tool)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L121) — Test validation with valid basic arguments.
  - `test_validate_arguments_with_analysis_type(self, tool)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L131) — Test validation with analysis_type specified.
  - `test_validate_arguments_with_language(self, tool)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L126) — Test validation with language specified.

## Functions
- `tool()` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L14) — Create a UniversalAnalyzeTool instance for testing.
- `tool_with_project_root()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_universal_analyze_tool_core.py#L20) — Create a UniversalAnalyzeTool instance with a project root.

