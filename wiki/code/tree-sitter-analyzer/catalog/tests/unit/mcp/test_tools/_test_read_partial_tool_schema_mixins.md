---
title: 'Module: tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools._test_read_partial_tool_schema_mixins`/ReadPartialTool
symbols:
  ReadPartialToolInitMixin.test_init_without_project_root: InitMixin#test_init_without_project_root().
  ReadPartialToolInitMixin.test_init_with_project_root: InitMixin#test_init_with_project_root().
  ReadPartialToolGetToolSchemaMixin.test_get_tool_schema_structure: GetToolSchemaMixin#test_get_tool_schema_structure().
  ReadPartialToolGetToolSchemaMixin.test_get_tool_schema_has_required: GetToolSchemaMixin#test_get_tool_schema_has_required().
  ReadPartialToolGetToolSchemaMixin.test_get_tool_schema_has_requests_property: GetToolSchemaMixin#test_get_tool_schema_has_requests_property().
  ReadPartialToolGetToolSchemaMixin.test_get_tool_schema_has_file_path_property: GetToolSchemaMixin#test_get_tool_schema_has_file_path_property().
  ReadPartialToolGetToolDefinitionMixin.test_get_tool_definition_name: GetToolDefinitionMixin#test_get_tool_definition_name().
  ReadPartialToolGetToolDefinitionMixin.test_get_tool_definition_has_description: GetToolDefinitionMixin#test_get_tool_definition_has_description().
  ReadPartialToolGetToolDefinitionMixin.test_get_tool_definition_has_input_schema: GetToolDefinitionMixin#test_get_tool_definition_has_input_schema().
  ReadPartialToolGetToolDefinitionMixin.test_get_tool_definition_schema_has_properties: GetToolDefinitionMixin#test_get_tool_definition_schema_has_properties().
  ReadPartialToolGetToolDefinitionMixin.test_get_tool_definition_name_correct: GetToolDefinitionMixin#test_get_tool_definition_name_correct().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_missing_file_path: ValidateArgumentsMixin#test_validate_arguments_missing_file_path().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_missing_start_line: ValidateArgumentsMixin#test_validate_arguments_missing_start_line().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_invalid_file_path_type: ValidateArgumentsMixin#test_validate_arguments_invalid_file_path_type().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_empty_file_path: ValidateArgumentsMixin#test_validate_arguments_empty_file_path().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_invalid_start_line_type: ValidateArgumentsMixin#test_validate_arguments_invalid_start_line_type().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_start_line_below_minimum: ValidateArgumentsMixin#test_validate_arguments_start_line_below_minimum().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_invalid_end_line_type: ValidateArgumentsMixin#test_validate_arguments_invalid_end_line_type().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_end_line_below_start_line: ValidateArgumentsMixin#test_validate_arguments_end_line_below_start_line().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_invalid_start_column_type: ValidateArgumentsMixin#test_validate_arguments_invalid_start_column_type().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_start_column_below_zero: ValidateArgumentsMixin#test_validate_arguments_start_column_below_zero().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_invalid_format: ValidateArgumentsMixin#test_validate_arguments_invalid_format().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_valid_single_mode: ValidateArgumentsMixin#test_validate_arguments_valid_single_mode().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_valid_batch_mode: ValidateArgumentsMixin#test_validate_arguments_valid_batch_mode().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_batch_empty_requests: ValidateArgumentsMixin#test_validate_arguments_batch_empty_requests().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_batch_single_request: ValidateArgumentsMixin#test_validate_arguments_batch_single_request().
  ReadPartialToolValidateArgumentsMixin.test_validate_arguments_mutually_exclusive: ValidateArgumentsMixin#test_validate_arguments_mutually_exclusive().
  ReadPartialToolValidateExtraMixin.test_validate_end_column_below_zero: ValidateExtraMixin#test_validate_end_column_below_zero().
  ReadPartialToolValidateExtraMixin.test_validate_format_not_string: ValidateExtraMixin#test_validate_format_not_string().
  ReadPartialToolValidateExtraMixin.test_validate_output_file_not_string: ValidateExtraMixin#test_validate_output_file_not_string().
  ReadPartialToolValidateExtraMixin.test_validate_output_file_empty: ValidateExtraMixin#test_validate_output_file_empty().
  ReadPartialToolValidateExtraMixin.test_validate_suppress_output_not_bool: ValidateExtraMixin#test_validate_suppress_output_not_bool().
  ReadPartialToolValidateExtraMixin.test_validate_end_line_below_one: ValidateExtraMixin#test_validate_end_line_below_one().
  ReadPartialToolValidateExtraMixin.test_validate_requests_not_list: ValidateExtraMixin#test_validate_requests_not_list().
  ReadPartialToolValidateExtraMixin.test_validate_valid_with_all_optional_fields: ValidateExtraMixin#test_validate_valid_with_all_optional_fields().
  ReadPartialToolInitMixin: InitMixin#
  ReadPartialToolGetToolSchemaMixin: GetToolSchemaMixin#
  ReadPartialToolGetToolDefinitionMixin: GetToolDefinitionMixin#
  ReadPartialToolValidateArgumentsMixin: ValidateArgumentsMixin#
  ReadPartialToolValidateExtraMixin: ValidateExtraMixin#
  ReadPartialToolInitMixin.test_init_without_project_root_attributes: InitMixin#test_init_without_project_root_attributes().
---
# Module: [`tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py)

## Classes
### `ReadPartialToolGetToolDefinitionMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py:68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L68)
- doc: Tests for get_tool_definition method.
- signature: `class ReadPartialToolGetToolDefinitionMixin:`
- members:
  - `test_get_tool_definition_has_description(self)` — [`L77`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L77) — Test that tool definition has description.
  - `test_get_tool_definition_has_input_schema(self)` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L84) — Test that tool definition has inputSchema.
  - `test_get_tool_definition_name(self)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L71) — Test that tool definition has correct name.
  - `test_get_tool_definition_name_correct(self)` — [`L98`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L98)
  - `test_get_tool_definition_schema_has_properties(self)` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L91)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.get_tool_definition)  (1 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolGetToolSchemaMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py:34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L34)
- doc: Tests for get_tool_schema method.
- signature: `class ReadPartialToolGetToolSchemaMixin:`
- members:
  - `test_get_tool_schema_has_file_path_property(self)` — [`L60`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L60) — Test that schema has file_path property.
  - `test_get_tool_schema_has_requests_property(self)` — [`L52`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L52) — Test that schema has requests property for batch mode.
  - `test_get_tool_schema_has_required(self)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L46)
  - `test_get_tool_schema_structure(self)` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L37) — Test that schema has correct structure.
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.get_tool_schema)  (1 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolInitMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py:11`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L11)
- doc: Tests for ReadPartialTool initialization.
- signature: `class ReadPartialToolInitMixin:`
- members:
  - `test_init_with_project_root(self)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L26) — Test initialization with project root.
  - `test_init_without_project_root(self)` — [`L14`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L14) — Test initialization without project root.
  - `test_init_without_project_root_attributes(self)` — [`L21`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L21)
- uses (calls/refs, reference-scoped): [`project_root`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.project_root), [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`file_output_manager`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.file_output_manager)  (1 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolValidateArgumentsMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py:105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L105)
- doc: Tests for validate_arguments method.
- signature: `class ReadPartialToolValidateArgumentsMixin:`
- members:
  - `test_validate_arguments_batch_empty_requests(self)` — [`L202`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L202)
  - `test_validate_arguments_batch_single_request(self)` — [`L207`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L207)
  - `test_validate_arguments_empty_file_path(self)` — [`L129`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L129) — Test that validation fails when file_path is empty.
  - `test_validate_arguments_end_line_below_start_line(self)` — [`L157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L157) — Test that validation fails when end_line < start_line.
  - `test_validate_arguments_invalid_end_line_type(self)` — [`L150`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L150) — Test that validation fails when end_line is not an integer.
  - `test_validate_arguments_invalid_file_path_type(self)` — [`L122`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L122) — Test that validation fails when file_path is not a string.
  - `test_validate_arguments_invalid_format(self)` — [`L178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L178) — Test that validation fails when format is invalid.
  - `test_validate_arguments_invalid_start_column_type(self)` — [`L164`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L164) — Test that validation fails when start_column is not an integer.
  - `test_validate_arguments_invalid_start_line_type(self)` — [`L136`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L136) — Test that validation fails when start_line is not an integer.
  - `test_validate_arguments_missing_file_path(self)` — [`L108`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L108) — Test that validation fails when file_path is missing.
  - `test_validate_arguments_missing_start_line(self)` — [`L115`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L115) — Test that validation fails when start_line is missing.
  - `test_validate_arguments_mutually_exclusive(self)` — [`L212`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L212) — Test that validation fails when both batch and single mode args are present.
  - `test_validate_arguments_start_column_below_zero(self)` — [`L171`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L171) — Test that validation fails when start_column < 0.
  - `test_validate_arguments_start_line_below_minimum(self)` — [`L143`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L143) — Test that validation fails when start_line < 1.
  - `test_validate_arguments_valid_batch_mode(self)` — [`L196`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L196) — Test that validation passes for valid batch mode arguments.
  - `test_validate_arguments_valid_single_mode(self)` — [`L185`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L185) — Test that validation passes for valid single mode arguments.
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.validate_arguments)  (1 test-only)
- used by: (1 test-only callers)

### `ReadPartialToolValidateExtraMixin`
- def: [`tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py:224`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L224)
- doc: Additional tests for uncovered validate_arguments paths.
- signature: `class ReadPartialToolValidateExtraMixin:`
- members:
  - `test_validate_end_column_below_zero(self)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L227)
  - `test_validate_end_line_below_one(self)` — [`L262`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L262)
  - `test_validate_format_not_string(self)` — [`L234`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L234)
  - `test_validate_output_file_empty(self)` — [`L248`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L248)
  - `test_validate_output_file_not_string(self)` — [`L241`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L241)
  - `test_validate_requests_not_list(self)` — [`L269`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L269)
  - `test_validate_suppress_output_not_bool(self)` — [`L255`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L255)
  - `test_validate_valid_with_all_optional_fields(self)` — [`L274`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/_test_read_partial_tool_schema_mixins.py#L274)
- uses (calls/refs, reference-scoped): [`ReadPartialTool`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.validate_arguments)  (1 test-only)
- used by: (1 test-only callers)

