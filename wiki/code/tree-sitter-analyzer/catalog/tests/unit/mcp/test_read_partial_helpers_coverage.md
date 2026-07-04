---
title: 'Module: tests/unit/mcp/test_read_partial_helpers_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_read_partial_helpers_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_read_partial_helpers_coverage`/Test
symbols:
  TestToolSchema.test_schema_has_required_properties: ToolSchema#test_schema_has_required_properties().
  TestToolSchema.test_schema_type_is_object: ToolSchema#test_schema_type_is_object().
  TestBuildReadResponse.test_basic_response: BuildReadResponse#test_basic_response().
  TestBuildReadResponse.test_with_columns: BuildReadResponse#test_with_columns().
  TestBuildReadResponse.test_end_line_defaults_to_start: BuildReadResponse#test_end_line_defaults_to_start().
  TestValidateLineRange.test_valid_range: ValidateLineRange#test_valid_range().
  TestValidateLineRange.test_invalid_start_line_zero: ValidateLineRange#test_invalid_start_line_zero().
  TestValidateLineRange.test_invalid_start_line_type: ValidateLineRange#test_invalid_start_line_type().
  TestValidateLineRange.test_invalid_end_line: ValidateLineRange#test_invalid_end_line().
  TestValidateLineRange.test_end_before_start: ValidateLineRange#test_end_before_start().
  TestValidateLineRange.test_invalid_start_column: ValidateLineRange#test_invalid_start_column().
  TestValidateLineRange.test_invalid_end_column: ValidateLineRange#test_invalid_end_column().
  TestValidateLineRange.test_end_column_before_start_column: ValidateLineRange#test_end_column_before_start_column().
  TestValidateLineRange.test_valid_with_columns: ValidateLineRange#test_valid_with_columns().
  TestValidateLineRange.test_none_end_line_ok: ValidateLineRange#test_none_end_line_ok().
  TestValidateLineRange.test_none_columns_ok: ValidateLineRange#test_none_columns_ok().
  TestBuildValidationError.test_structure: BuildValidationError#test_structure().
  TestBuildAgentSummary.test_low_risk: BuildAgentSummary#test_low_risk().
  TestBuildAgentSummary.test_medium_risk_lines: BuildAgentSummary#test_medium_risk_lines().
  TestBuildAgentSummary.test_high_risk_content_length: BuildAgentSummary#test_high_risk_content_length().
  TestBuildAgentSummary.test_with_output_file: BuildAgentSummary#test_with_output_file().
  TestBuildAgentSummary.test_with_columns_next_step: BuildAgentSummary#test_with_columns_next_step().
  TestBuildAgentSummaryForResult.test_from_result_dict: BuildAgentSummaryForResult#test_from_result_dict().
  TestBuildBatchAgentSummary.test_low_risk: BuildBatchAgentSummary#test_low_risk().
  TestBuildBatchAgentSummary.test_high_risk_truncated: BuildBatchAgentSummary#test_high_risk_truncated().
  TestBuildBatchAgentSummary.test_high_risk_errors: BuildBatchAgentSummary#test_high_risk_errors().
  TestBuildBatchAgentSummary.test_medium_risk_many_sections: BuildBatchAgentSummary#test_medium_risk_many_sections().
  TestToolSchema: ToolSchema#
  TestBuildReadResponse: BuildReadResponse#
  TestValidateLineRange: ValidateLineRange#
  TestBuildValidationError: BuildValidationError#
  TestBuildAgentSummary: BuildAgentSummary#
  TestBuildAgentSummaryForResult: BuildAgentSummaryForResult#
  TestBuildBatchAgentSummary: BuildBatchAgentSummary#
---
# Module: [`tests/unit/mcp/test_read_partial_helpers_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py)

## Classes
### `TestBuildAgentSummary`
- def: [`tests/unit/mcp/test_read_partial_helpers_coverage.py:95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L95)
- signature: `class TestBuildAgentSummary:`
- members:
  - `test_high_risk_content_length(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L123)
  - `test_low_risk(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L96)
  - `test_medium_risk_lines(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L110)
  - `test_with_columns_next_step(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L150)
  - `test_with_output_file(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L136)
- uses (calls/refs, reference-scoped): [`build_agent_summary`](../../../tree_sitter_analyzer/mcp/tools/read_partial_helpers.md#build_agent_summary)

### `TestBuildAgentSummaryForResult`
- def: [`tests/unit/mcp/test_read_partial_helpers_coverage.py:164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L164)
- signature: `class TestBuildAgentSummaryForResult:`
- members:
  - `test_from_result_dict(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L165)
- uses (calls/refs, reference-scoped): [`build_agent_summary_for_result`](../../../tree_sitter_analyzer/mcp/tools/read_partial_helpers.md#build_agent_summary_for_result)

### `TestBuildBatchAgentSummary`
- def: [`tests/unit/mcp/test_read_partial_helpers_coverage.py:177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L177)
- signature: `class TestBuildBatchAgentSummary:`
- members:
  - `test_high_risk_errors(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L192)
  - `test_high_risk_truncated(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L185)
  - `test_low_risk(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L178)
  - `test_medium_risk_many_sections(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L199)
- uses (calls/refs, reference-scoped): [`build_batch_agent_summary`](../../../tree_sitter_analyzer/mcp/tools/read_partial_helpers.md#build_batch_agent_summary)

### `TestBuildReadResponse`
- def: [`tests/unit/mcp/test_read_partial_helpers_coverage.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L25)
- signature: `class TestBuildReadResponse:`
- members:
  - `test_basic_response(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L26)
  - `test_end_line_defaults_to_start(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L45)
  - `test_with_columns(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L38)
- uses (calls/refs, reference-scoped): [`build_read_response`](../../../tree_sitter_analyzer/mcp/tools/read_partial_helpers.md#build_read_response)

### `TestBuildValidationError`
- def: [`tests/unit/mcp/test_read_partial_helpers_coverage.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L87)
- signature: `class TestBuildValidationError:`
- members:
  - `test_structure(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L88)
- uses (calls/refs, reference-scoped): [`build_validation_error`](../../../tree_sitter_analyzer/mcp/tools/read_partial_helpers.md#build_validation_error)

### `TestToolSchema`
- def: [`tests/unit/mcp/test_read_partial_helpers_coverage.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L15)
- signature: `class TestToolSchema:`
- members:
  - `test_schema_has_required_properties(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L16)
  - `test_schema_type_is_object(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L21)
- uses (calls/refs, reference-scoped): [`TOOL_SCHEMA`](../../../tree_sitter_analyzer/mcp/tools/read_partial_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA)

### `TestValidateLineRange`
- def: [`tests/unit/mcp/test_read_partial_helpers_coverage.py:52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L52)
- signature: `class TestValidateLineRange:`
- members:
  - `test_end_before_start(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L65)
  - `test_end_column_before_start_column(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L74)
  - `test_invalid_end_column(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L71)
  - `test_invalid_end_line(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L62)
  - `test_invalid_start_column(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L68)
  - `test_invalid_start_line_type(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L59)
  - `test_invalid_start_line_zero(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L56)
  - `test_none_columns_ok(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L83)
  - `test_none_end_line_ok(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L80)
  - `test_valid_range(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L53)
  - `test_valid_with_columns(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_read_partial_helpers_coverage.py#L77)
- uses (calls/refs, reference-scoped): [`validate_line_range`](../../../tree_sitter_analyzer/mcp/tools/read_partial_helpers.md#validate_line_range)

