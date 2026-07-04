---
title: 'Module: tests/unit/mcp/test_analyze_code_structure_tool_core.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_analyze_code_structure_tool_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_analyze_code_structure_tool_core`/
symbols:
  TestAnalyzeSurfacesParseErrors.test_wrong_language_file_flags_parse_errors: TestAnalyzeSurfacesParseErrors#test_wrong_language_file_flags_parse_errors().
  TestAnalyzeSurfacesParseErrors.test_valid_file_has_no_parse_errors_flag: TestAnalyzeSurfacesParseErrors#test_valid_file_has_no_parse_errors_flag().
  TestAnalyzeSurfacesParseErrors.test_relative_file_path_with_project_root_still_flags: TestAnalyzeSurfacesParseErrors#test_relative_file_path_with_project_root_still_flags().
  tool: tool().
  tool_with_project_root: tool_with_project_root().
  TestAnalyzeCodeStructureToolInit: TestAnalyzeCodeStructureToolInit#
  TestAnalyzeCodeStructureToolInit.test_init_without_project_root: TestAnalyzeCodeStructureToolInit#test_init_without_project_root().
  TestAnalyzeCodeStructureToolInit.test_init_with_project_root: TestAnalyzeCodeStructureToolInit#test_init_with_project_root().
  TestAnalyzeCodeStructureToolSetProjectPath: TestAnalyzeCodeStructureToolSetProjectPath#
  TestAnalyzeCodeStructureToolSetProjectPath.test_set_project_path_updates_analysis_engine: TestAnalyzeCodeStructureToolSetProjectPath#test_set_project_path_updates_analysis_engine().
  TestAnalyzeCodeStructureToolGetToolDefinition: TestAnalyzeCodeStructureToolGetToolDefinition#
  TestAnalyzeCodeStructureToolGetToolDefinition.test_get_tool_definition_name: TestAnalyzeCodeStructureToolGetToolDefinition#test_get_tool_definition_name().
  TestAnalyzeCodeStructureToolGetToolDefinition.test_get_tool_definition_has_description: TestAnalyzeCodeStructureToolGetToolDefinition#test_get_tool_definition_has_description().
  TestAnalyzeCodeStructureToolGetToolDefinition.test_get_tool_definition_has_input_schema: TestAnalyzeCodeStructureToolGetToolDefinition#test_get_tool_definition_has_input_schema().
  TestAnalyzeCodeStructureToolGetToolDefinition.test_get_tool_definition_schema_has_file_path: TestAnalyzeCodeStructureToolGetToolDefinition#test_get_tool_definition_schema_has_file_path().
  TestAnalyzeCodeStructureToolGetToolDefinition.test_get_tool_definition_schema_has_format_type: TestAnalyzeCodeStructureToolGetToolDefinition#test_get_tool_definition_schema_has_format_type().
  TestAnalyzeCodeStructureToolGetToolDefinition.test_get_tool_definition_schema_has_language: TestAnalyzeCodeStructureToolGetToolDefinition#test_get_tool_definition_schema_has_language().
  TestAnalyzeCodeStructureToolGetToolDefinition.test_get_tool_definition_schema_has_output_file: TestAnalyzeCodeStructureToolGetToolDefinition#test_get_tool_definition_schema_has_output_file().
  TestAnalyzeCodeStructureToolGetToolDefinition.test_get_tool_definition_schema_has_suppress_output: TestAnalyzeCodeStructureToolGetToolDefinition#test_get_tool_definition_schema_has_suppress_output().
  TestAnalyzeCodeStructureToolGetToolDefinition.test_get_tool_definition_schema_has_output_format: TestAnalyzeCodeStructureToolGetToolDefinition#test_get_tool_definition_schema_has_output_format().
  TestAnalyzeCodeStructureToolValidateArguments: TestAnalyzeCodeStructureToolValidateArguments#
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_valid_basic: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_valid_basic().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_with_format_type: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_with_format_type().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_with_language: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_with_language().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_with_output_file: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_with_output_file().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_with_suppress_output: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_with_suppress_output().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_missing_file_path: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_missing_file_path().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_invalid_file_path_type: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_invalid_file_path_type().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_empty_file_path: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_empty_file_path().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_invalid_format_type: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_invalid_format_type().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_unsupported_format_type: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_unsupported_format_type().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_unsupported_format_type_enumerates_valid: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_unsupported_format_type_enumerates_valid().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_invalid_language_type: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_invalid_language_type().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_invalid_output_file_type: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_invalid_output_file_type().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_empty_output_file: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_empty_output_file().
  TestAnalyzeCodeStructureToolValidateArguments.test_validate_arguments_invalid_suppress_output_type: TestAnalyzeCodeStructureToolValidateArguments#test_validate_arguments_invalid_suppress_output_type().
  TestAnalyzeSurfacesParseErrors: TestAnalyzeSurfacesParseErrors#
---
# Module: [`tests/unit/mcp/test_analyze_code_structure_tool_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py)

## Classes
### `TestAnalyzeCodeStructureToolGetToolDefinition`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_core.py:56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L56)
- doc: Tests for get_tool_definition method.
- signature: `class TestAnalyzeCodeStructureToolGetToolDefinition:`
- members:
  - `test_get_tool_definition_has_description(self, tool)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L64) — Test tool definition has description.
  - `test_get_tool_definition_has_input_schema(self, tool)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L71) — Test tool definition has input schema.
  - `test_get_tool_definition_name(self, tool)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L59) — Test tool definition has correct name.
  - `test_get_tool_definition_schema_has_file_path(self, tool)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L77) — Test schema has file_path property.
  - `test_get_tool_definition_schema_has_format_type(self, tool)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L83) — Test schema has format_type property.
  - `test_get_tool_definition_schema_has_language(self, tool)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L94) — Test schema has language property.
  - `test_get_tool_definition_schema_has_output_file(self, tool)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L100) — Test schema has output_file property.
  - `test_get_tool_definition_schema_has_output_format(self, tool)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L112) — Test schema has output_format property.
  - `test_get_tool_definition_schema_has_suppress_output(self, tool)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L106) — Test schema has suppress_output property.

### `TestAnalyzeCodeStructureToolInit`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_core.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L28)
- doc: Tests for AnalyzeCodeStructureTool initialization.
- signature: `class TestAnalyzeCodeStructureToolInit:`
- members:
  - `test_init_with_project_root(self, tool_with_project_root)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L38) — Test initialization with project root.
  - `test_init_without_project_root(self, tool)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L31) — Test initialization without project root.

### `TestAnalyzeCodeStructureToolSetProjectPath`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_core.py:46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L46)
- doc: Tests for set_project_path method.
- signature: `class TestAnalyzeCodeStructureToolSetProjectPath:`
- members:
  - `test_set_project_path_updates_analysis_engine(self, tool)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L49) — Test that setting project path updates analysis engine.

### `TestAnalyzeCodeStructureToolValidateArguments`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_core.py:120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L120)
- doc: Tests for validate_arguments method.
- signature: `class TestAnalyzeCodeStructureToolValidateArguments:`
- members:
  - `test_validate_arguments_empty_file_path(self, tool)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L160) — Test validation fails when file_path is empty.
  - `test_validate_arguments_empty_output_file(self, tool)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L206) — Test validation fails when output_file is empty.
  - `test_validate_arguments_invalid_file_path_type(self, tool)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L154) — Test validation fails when file_path is not a string.
  - `test_validate_arguments_invalid_format_type(self, tool)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L166) — Test validation fails when format_type is invalid.
  - `test_validate_arguments_invalid_language_type(self, tool)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L194) — Test validation fails when language is not a string.
  - `test_validate_arguments_invalid_output_file_type(self, tool)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L200) — Test validation fails when output_file is not a string.
  - `test_validate_arguments_invalid_suppress_output_type(self, tool)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L212) — Test validation fails when suppress_output is not a boolean.
  - `test_validate_arguments_missing_file_path(self, tool)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L148) — Test validation fails when file_path is missing.
  - `test_validate_arguments_unsupported_format_type(self, tool)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L172) — Test validation fails when format_type is not supported.
  - `test_validate_arguments_unsupported_format_type_enumerates_valid(self, tool)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L178) — Error message must enumerate valid format_type values (issue #449).
  - `test_validate_arguments_valid_basic(self, tool)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L123) — Test validation with valid basic arguments.
  - `test_validate_arguments_with_format_type(self, tool)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L128) — Test validation with format_type specified.
  - `test_validate_arguments_with_language(self, tool)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L133) — Test validation with language specified.
  - `test_validate_arguments_with_output_file(self, tool)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L138) — Test validation with output_file specified.
  - `test_validate_arguments_with_suppress_output(self, tool)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L143) — Test validation with suppress_output specified.

### `TestAnalyzeSurfacesParseErrors`
- def: [`tests/unit/mcp/test_analyze_code_structure_tool_core.py:220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L220)
- doc: #572: a wrong-language / corrupt file must not be reported as a clean
- signature: `class TestAnalyzeSurfacesParseErrors:`
- members:
  - `test_relative_file_path_with_project_root_still_flags(self, tmp_path)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L244)
  - `test_valid_file_has_no_parse_errors_flag(self, tmp_path)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L235)
  - `test_wrong_language_file_flags_parse_errors(self, tmp_path)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L225)
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute)

## Functions
- `tool()` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L17) — Create an AnalyzeCodeStructureTool instance for testing.
- `tool_with_project_root()` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_analyze_code_structure_tool_core.py#L23) — Create an AnalyzeCodeStructureTool instance with a project root.

