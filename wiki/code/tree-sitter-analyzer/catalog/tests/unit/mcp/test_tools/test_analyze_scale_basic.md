---
title: 'Module: tests/unit/mcp/test_tools/test_analyze_scale_basic.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/test_analyze_scale_basic.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools.test_analyze_scale_basic`/
symbols:
  tool: tool().
  tool_with_project_root: tool_with_project_root().
  TestAnalyzeScaleToolInit: TestAnalyzeScaleToolInit#
  TestAnalyzeScaleToolInit.test_init_without_project_root: TestAnalyzeScaleToolInit#test_init_without_project_root().
  TestAnalyzeScaleToolInit.test_init_with_project_root: TestAnalyzeScaleToolInit#test_init_with_project_root().
  TestAnalyzeScaleToolGetToolSchema: TestAnalyzeScaleToolGetToolSchema#
  TestAnalyzeScaleToolGetToolSchema.test_get_tool_schema_structure: TestAnalyzeScaleToolGetToolSchema#test_get_tool_schema_structure().
  TestAnalyzeScaleToolGetToolSchema.test_get_tool_schema_has_file_path_property: TestAnalyzeScaleToolGetToolSchema#test_get_tool_schema_has_file_path_property().
  TestAnalyzeScaleToolGetToolSchema.test_get_tool_schema_has_file_paths_property: TestAnalyzeScaleToolGetToolSchema#test_get_tool_schema_has_file_paths_property().
  TestAnalyzeScaleToolGetToolSchema.test_get_tool_schema_has_metrics_only_property: TestAnalyzeScaleToolGetToolSchema#test_get_tool_schema_has_metrics_only_property().
  TestAnalyzeScaleToolGetToolSchema.test_get_tool_schema_has_language_property: TestAnalyzeScaleToolGetToolSchema#test_get_tool_schema_has_language_property().
  TestAnalyzeScaleToolGetToolSchema.test_get_tool_schema_has_include_complexity_property: TestAnalyzeScaleToolGetToolSchema#test_get_tool_schema_has_include_complexity_property().
  TestAnalyzeScaleToolGetToolSchema.test_get_tool_schema_has_include_details_property: TestAnalyzeScaleToolGetToolSchema#test_get_tool_schema_has_include_details_property().
  TestAnalyzeScaleToolGetToolSchema.test_get_tool_schema_has_include_guidance_property: TestAnalyzeScaleToolGetToolSchema#test_get_tool_schema_has_include_guidance_property().
  TestAnalyzeScaleToolGetToolSchema.test_get_tool_schema_has_output_format_property: TestAnalyzeScaleToolGetToolSchema#test_get_tool_schema_has_output_format_property().
  TestAnalyzeScaleToolGetToolDefinition: TestAnalyzeScaleToolGetToolDefinition#
  TestAnalyzeScaleToolGetToolDefinition.test_get_tool_definition_has_description: TestAnalyzeScaleToolGetToolDefinition#test_get_tool_definition_has_description().
  TestAnalyzeScaleToolGetToolDefinition.test_get_tool_definition_has_input_schema: TestAnalyzeScaleToolGetToolDefinition#test_get_tool_definition_has_input_schema().
  TestAnalyzeScaleToolValidateArguments: TestAnalyzeScaleToolValidateArguments#
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_valid_single_mode: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_valid_single_mode().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_valid_batch_mode: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_valid_batch_mode().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_missing_file_path: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_missing_file_path().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_empty_file_path: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_empty_file_path().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_invalid_file_path_type: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_invalid_file_path_type().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_invalid_language_type: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_invalid_language_type().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_invalid_include_complexity_type: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_invalid_include_complexity_type().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_invalid_include_details_type: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_invalid_include_details_type().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_invalid_include_guidance_type: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_invalid_include_guidance_type().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_mutually_exclusive: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_mutually_exclusive().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_empty_file_paths: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_empty_file_paths().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_invalid_file_paths_type: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_invalid_file_paths_type().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_invalid_metrics_only_type: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_invalid_metrics_only_type().
  TestAnalyzeScaleToolValidateArguments.test_validate_arguments_metrics_only_required_for_batch: TestAnalyzeScaleToolValidateArguments#test_validate_arguments_metrics_only_required_for_batch().
---
# Module: [`tests/unit/mcp/test_tools/test_analyze_scale_basic.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py)

## Classes
### `TestAnalyzeScaleToolGetToolDefinition`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_basic.py:104`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L104)
- doc: Tests for get_tool_definition method.
- signature: `class TestAnalyzeScaleToolGetToolDefinition:`
- members:
  - `test_get_tool_definition_has_description(self, tool)` — [`L107`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L107) — Test tool definition has description.
  - `test_get_tool_definition_has_input_schema(self, tool)` — [`L114`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L114) — Test tool definition has input schema.

### `TestAnalyzeScaleToolGetToolSchema`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_basic.py:41`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L41)
- doc: Tests for get_tool_schema method.
- signature: `class TestAnalyzeScaleToolGetToolSchema:`
- members:
  - `test_get_tool_schema_has_file_path_property(self, tool)` — [`L52`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L52) — Test schema has file_path property.
  - `test_get_tool_schema_has_file_paths_property(self, tool)` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L58) — Test schema has file_paths property for batch mode.
  - `test_get_tool_schema_has_include_complexity_property(self, tool)` — [`L76`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L76) — Test schema has include_complexity property.
  - `test_get_tool_schema_has_include_details_property(self, tool)` — [`L82`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L82) — Test schema has include_details property.
  - `test_get_tool_schema_has_include_guidance_property(self, tool)` — [`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L88) — Test schema has include_guidance property.
  - `test_get_tool_schema_has_language_property(self, tool)` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L70) — Test schema has language property.
  - `test_get_tool_schema_has_metrics_only_property(self, tool)` — [`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L64) — Test schema has metrics_only property.
  - `test_get_tool_schema_has_output_format_property(self, tool)` — [`L94`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L94) — Test schema has output_format property.
  - `test_get_tool_schema_structure(self, tool)` — [`L44`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L44) — Test tool schema has correct structure.

### `TestAnalyzeScaleToolInit`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_basic.py:25`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L25)
- doc: Tests for AnalyzeScaleTool initialization.
- signature: `class TestAnalyzeScaleToolInit:`
- members:
  - `test_init_with_project_root(self, tool_with_project_root)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L34) — Test initialization with project root.
  - `test_init_without_project_root(self, tool)` — [`L28`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L28) — Test initialization without project root.

### `TestAnalyzeScaleToolValidateArguments`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_basic.py:121`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L121)
- doc: Tests for validate_arguments method.
- signature: `class TestAnalyzeScaleToolValidateArguments:`
- members:
  - `test_validate_arguments_empty_file_path(self, tool)` — [`L149`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L149) — Test validation fails when file_path is empty.
  - `test_validate_arguments_empty_file_paths(self, tool)` — [`L193`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L193) — Test validation fails when file_paths is empty.
  - `test_validate_arguments_invalid_file_path_type(self, tool)` — [`L155`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L155) — Test validation fails when file_path is not a string.
  - `test_validate_arguments_invalid_file_paths_type(self, tool)` — [`L199`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L199) — Test validation fails when file_paths is not a list.
  - `test_validate_arguments_invalid_include_complexity_type(self, tool)` — [`L167`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L167) — Test validation fails when include_complexity is not a boolean.
  - `test_validate_arguments_invalid_include_details_type(self, tool)` — [`L173`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L173) — Test validation fails when include_details is not a boolean.
  - `test_validate_arguments_invalid_include_guidance_type(self, tool)` — [`L179`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L179) — Test validation fails when include_guidance is not a boolean.
  - `test_validate_arguments_invalid_language_type(self, tool)` — [`L161`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L161) — Test validation fails when language is not a string.
  - `test_validate_arguments_invalid_metrics_only_type(self, tool)` — [`L205`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L205) — Test validation fails when metrics_only is not a boolean.
  - `test_validate_arguments_metrics_only_required_for_batch(self, tool)` — [`L211`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L211) — Test validation fails when metrics_only is False in batch mode.
  - `test_validate_arguments_missing_file_path(self, tool)` — [`L143`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L143) — Test validation fails when file_path is missing.
  - `test_validate_arguments_mutually_exclusive(self, tool)` — [`L185`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L185) — Test validation fails when both file_path and file_paths are provided.
  - `test_validate_arguments_valid_batch_mode(self, tool)` — [`L135`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L135) — Test validation with valid batch mode arguments.
  - `test_validate_arguments_valid_single_mode(self, tool)` — [`L124`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L124) — Test validation with valid single mode arguments.

## Functions
- `tool()` — [`L14`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L14) — Create an AnalyzeScaleTool instance for testing.
- `tool_with_project_root()` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_basic.py#L20) — Create an AnalyzeScaleTool instance with a project root.

