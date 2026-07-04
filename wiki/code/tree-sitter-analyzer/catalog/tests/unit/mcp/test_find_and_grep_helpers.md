---
title: 'Module: tests/unit/mcp/test_find_and_grep_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_find_and_grep_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_find_and_grep_helpers`/Test
symbols:
  TestBuildCountOnlyResponseEdgeCases.test_empty_count_data: BuildCountOnlyResponseEdgeCases#test_empty_count_data().
  TestBuildCountOnlyResponseEdgeCases.test_only_total_no_file_counts: BuildCountOnlyResponseEdgeCases#test_only_total_no_file_counts().
  TestBuildCountOnlyResponseEdgeCases.test_truncated_true: BuildCountOnlyResponseEdgeCases#test_truncated_true().
  TestFindAndGrepFullMatchContext.test_creation: FindAndGrepFullMatchContext#test_creation().
  TestFindAndGrepFullMatchContext.test_frozen: FindAndGrepFullMatchContext#test_frozen().
  TestFindAndGrepCountOnlyContext.test_creation: FindAndGrepCountOnlyContext#test_creation().
  TestFindAndGrepCountOnlyContext.test_frozen: FindAndGrepCountOnlyContext#test_frozen().
  TestFindAndGrepRgModeContext.test_creation: FindAndGrepRgModeContext#test_creation().
  TestFindAndGrepRgModeContext.test_frozen: FindAndGrepRgModeContext#test_frozen().
  TestBuildCountOnlyResponse._make_context: BuildCountOnlyResponse#_make_context().
  TestBuildCountOnlyResponse.test_basic_count_only_response: BuildCountOnlyResponse#test_basic_count_only_response().
  TestBuildCountOnlyResponse.test_count_only_extracts_total: BuildCountOnlyResponse#test_count_only_extracts_total().
  TestBuildCountOnlyResponse.test_count_only_file_counts_without_total: BuildCountOnlyResponse#test_count_only_file_counts_without_total().
  TestBuildCountOnlyResponse.test_count_only_missing_total_defaults_zero: BuildCountOnlyResponse#test_count_only_missing_total_defaults_zero().
  TestBuildCountOnlyResponse.test_count_only_has_meta: BuildCountOnlyResponse#test_count_only_has_meta().
  TestBuildCountOnlyResponse.test_count_only_has_agent_summary: BuildCountOnlyResponse#test_count_only_has_agent_summary().
  TestBuildCountOnlyResponse.test_count_only_toon_format: BuildCountOnlyResponse#test_count_only_toon_format().
  TestBuildCountOnlyResponse.test_count_only_json_format_no_toon: BuildCountOnlyResponse#test_count_only_json_format_no_toon().
  TestToolSchema.test_schema_is_dict: ToolSchema#test_schema_is_dict().
  TestToolSchema.test_schema_type_is_object: ToolSchema#test_schema_type_is_object().
  TestToolSchema.test_schema_has_required_fields: ToolSchema#test_schema_has_required_fields().
  TestToolSchema.test_schema_has_roots_property: ToolSchema#test_schema_has_roots_property().
  TestToolSchema.test_schema_has_query_property: ToolSchema#test_schema_has_query_property().
  TestToolSchema.test_schema_has_pattern_property: ToolSchema#test_schema_has_pattern_property().
  TestToolSchema.test_schema_has_output_format_with_enum: ToolSchema#test_schema_has_output_format_with_enum().
  TestToolSchema.test_schema_has_sort_with_enum: ToolSchema#test_schema_has_sort_with_enum().
  TestToolSchema.test_schema_has_case_with_enum: ToolSchema#test_schema_has_case_with_enum().
  TestToolSchema.test_schema_additional_properties_false: ToolSchema#test_schema_additional_properties_false().
  TestToolSchema.test_schema_boolean_defaults: ToolSchema#test_schema_boolean_defaults().
  TestToolSchema.test_schema_integer_properties: ToolSchema#test_schema_integer_properties().
  TestFindAndGrepFullMatchContext.test_equality: FindAndGrepFullMatchContext#test_equality().
  TestFindAndGrepFullMatchContext.test_unhashable_due_to_dict: FindAndGrepFullMatchContext#test_unhashable_due_to_dict().
  TestBuildMissingCommandsResponse.test_returns_none_when_no_missing: BuildMissingCommandsResponse#test_returns_none_when_no_missing().
  TestBuildMissingCommandsResponse.test_returns_none_when_none_input: BuildMissingCommandsResponse#test_returns_none_when_none_input().
  TestBuildMissingCommandsResponse.test_returns_error_for_missing_fd: BuildMissingCommandsResponse#test_returns_error_for_missing_fd().
  TestBuildMissingCommandsResponse.test_returns_error_for_missing_rg: BuildMissingCommandsResponse#test_returns_error_for_missing_rg().
  TestBuildMissingCommandsResponse.test_returns_error_for_both_missing: BuildMissingCommandsResponse#test_returns_error_for_both_missing().
  TestBuildMissingCommandsResponse.test_error_mentions_install: BuildMissingCommandsResponse#test_error_mentions_install().
  TestBuildSearchMeta.test_basic_meta: BuildSearchMeta#test_basic_meta().
  TestBuildSearchMeta.test_meta_keys: BuildSearchMeta#test_meta_keys().
  TestBuildSearchMeta.test_meta_with_truncated_true: BuildSearchMeta#test_meta_with_truncated_true().
  TestBuildSearchMeta.test_meta_preserves_zero_values: BuildSearchMeta#test_meta_preserves_zero_values().
  TestBuildEmptyResponse.test_basic_empty_response: BuildEmptyResponse#test_basic_empty_response().
  TestBuildEmptyResponse.test_empty_response_has_meta: BuildEmptyResponse#test_empty_response_has_meta().
  TestBuildEmptyResponse.test_empty_response_has_agent_summary: BuildEmptyResponse#test_empty_response_has_agent_summary().
  TestBuildEmptyResponse.test_empty_response_with_truncated: BuildEmptyResponse#test_empty_response_with_truncated().
  TestHandleOutput.test_returns_none_when_no_output_file_and_no_suppress: HandleOutput#test_returns_none_when_no_output_file_and_no_suppress().
  TestHandleOutput.test_suppress_without_output_file: HandleOutput#test_suppress_without_output_file().
  TestHandleOutput.test_suppress_includes_agent_summary: HandleOutput#test_suppress_includes_agent_summary().
  TestHandleOutput.test_output_file_triggers_file_output: HandleOutput#test_output_file_triggers_file_output().
  TestHandleOutput.test_output_file_updates_result: HandleOutput#test_output_file_updates_result().
  TestHandleFileOutput.test_save_with_summary_only: HandleFileOutput#test_save_with_summary_only().
  TestHandleFileOutput.test_save_with_matches: HandleFileOutput#test_save_with_matches().
  TestHandleFileOutput.test_suppress_returns_minimal: HandleFileOutput#test_suppress_returns_minimal().
  TestHandleFileOutput.test_exception_sets_error: HandleFileOutput#test_exception_sets_error().
  TestMakeMinimal.test_basic_minimal: MakeMinimal#test_basic_minimal().
  TestMakeMinimal.test_minimal_without_summary: MakeMinimal#test_minimal_without_summary().
  TestMakeMinimal.test_minimal_with_summary: MakeMinimal#test_minimal_with_summary().
  TestMakeMinimal.test_minimal_includes_agent_summary: MakeMinimal#test_minimal_includes_agent_summary().
  TestMakeMinimal.test_minimal_without_agent_summary: MakeMinimal#test_minimal_without_agent_summary().
  TestMakeMinimal.test_minimal_defaults_success_true: MakeMinimal#test_minimal_defaults_success_true().
  TestMakeMinimal.test_minimal_defaults_count_zero: MakeMinimal#test_minimal_defaults_count_zero().
  TestBuildEmptyResponseIntegration.test_empty_response_meta_fd_elapsed: BuildEmptyResponseIntegration#test_empty_response_meta_fd_elapsed().
  TestBuildEmptyResponseIntegration.test_empty_response_meta_rg_elapsed_zero: BuildEmptyResponseIntegration#test_empty_response_meta_rg_elapsed_zero().
  TestToolSchema: ToolSchema#
  TestFindAndGrepFullMatchContext: FindAndGrepFullMatchContext#
  TestFindAndGrepCountOnlyContext: FindAndGrepCountOnlyContext#
  TestFindAndGrepRgModeContext: FindAndGrepRgModeContext#
  TestBuildMissingCommandsResponse: BuildMissingCommandsResponse#
  TestBuildSearchMeta: BuildSearchMeta#
  TestBuildEmptyResponse: BuildEmptyResponse#
  TestBuildCountOnlyResponse: BuildCountOnlyResponse#
  TestHandleOutput: HandleOutput#
  TestHandleFileOutput: HandleFileOutput#
  TestMakeMinimal: MakeMinimal#
  TestBuildEmptyResponseIntegration: BuildEmptyResponseIntegration#
  TestBuildCountOnlyResponseEdgeCases: BuildCountOnlyResponseEdgeCases#
---
# Module: [`tests/unit/mcp/test_find_and_grep_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py)

## Classes
### `TestBuildCountOnlyResponse`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L335)
- signature: `class TestBuildCountOnlyResponse:`
- members:
  - `test_basic_count_only_response(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L349)
  - `test_count_only_extracts_total(self)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L356)
  - `test_count_only_file_counts_without_total(self)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L361)
  - `test_count_only_has_agent_summary(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L378)
  - `test_count_only_has_meta(self)` — [`L372`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L372)
  - `test_count_only_json_format_no_toon(self)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L389)
  - `test_count_only_missing_total_defaults_zero(self)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L367)
  - `test_count_only_toon_format(self)` — [`L384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L384)
- protocol/private: `_make_context`[`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L336)
- uses (calls/refs, reference-scoped): [`build_count_only_response`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#build_count_only_response), [`FindAndGrepCountOnlyContext`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext)

### `TestBuildCountOnlyResponseEdgeCases`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:593`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L593)
- signature: `class TestBuildCountOnlyResponseEdgeCases:`
- members:
  - `test_empty_count_data(self)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L594)
  - `test_only_total_no_file_counts(self)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L608)
  - `test_truncated_true(self)` — [`L622`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L622)
- uses (calls/refs, reference-scoped): [`build_count_only_response`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#build_count_only_response), [`FindAndGrepCountOnlyContext`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext), [`output_format`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.output_format), [`arguments`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.arguments), [`count_data`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.count_data), [`fd_elapsed_ms`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.fd_elapsed_ms), [`rg_elapsed_ms`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.rg_elapsed_ms), [`searched_file_count`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.searched_file_count), [`truncated`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.truncated)

### `TestBuildEmptyResponse`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L296)
- signature: `class TestBuildEmptyResponse:`
- members:
  - `test_basic_empty_response(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L297)
  - `test_empty_response_has_agent_summary(self)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L317)
  - `test_empty_response_has_meta(self)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L307)
  - `test_empty_response_with_truncated(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L326)
- uses (calls/refs, reference-scoped): [`build_empty_response`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#build_empty_response)

### `TestBuildEmptyResponseIntegration`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:575`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L575)
- signature: `class TestBuildEmptyResponseIntegration:`
- members:
  - `test_empty_response_meta_fd_elapsed(self)` — [`L576`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L576)
  - `test_empty_response_meta_rg_elapsed_zero(self)` — [`L584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L584)
- uses (calls/refs, reference-scoped): [`build_empty_response`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#build_empty_response)

### `TestBuildMissingCommandsResponse`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L208)
- signature: `class TestBuildMissingCommandsResponse:`
- members:
  - `test_error_mentions_install(self)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L234)
  - `test_returns_error_for_both_missing(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L228)
  - `test_returns_error_for_missing_fd(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L215)
  - `test_returns_error_for_missing_rg(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L223)
  - `test_returns_none_when_no_missing(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L209)
  - `test_returns_none_when_none_input(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L212)
- uses (calls/refs, reference-scoped): [`build_missing_commands_response`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#build_missing_commands_response)

### `TestBuildSearchMeta`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L239)
- signature: `class TestBuildSearchMeta:`
- members:
  - `test_basic_meta(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L240)
  - `test_meta_keys(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L252)
  - `test_meta_preserves_zero_values(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L285)
  - `test_meta_with_truncated_true(self)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L275)
- uses (calls/refs, reference-scoped): [`build_search_meta`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#build_search_meta)

### `TestFindAndGrepCountOnlyContext`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L156)
- signature: `class TestFindAndGrepCountOnlyContext:`
- members:
  - `test_creation(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L157)
  - `test_frozen(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L170)
- uses (calls/refs, reference-scoped): [`FindAndGrepCountOnlyContext`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext), [`output_format`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.output_format), [`arguments`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.arguments), [`count_data`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.count_data), [`fd_elapsed_ms`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.fd_elapsed_ms), [`rg_elapsed_ms`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.rg_elapsed_ms), [`searched_file_count`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.searched_file_count), [`truncated`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepCountOnlyContext.truncated)

### `TestFindAndGrepFullMatchContext`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L95)
- signature: `class TestFindAndGrepFullMatchContext:`
- members:
  - `test_creation(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L96)
  - `test_equality(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L127)
  - `test_frozen(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L114)
  - `test_unhashable_due_to_dict(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L141)
- uses (calls/refs, reference-scoped): [`FindAndGrepFullMatchContext`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepFullMatchContext), [`fd_elapsed_ms`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepFullMatchContext.fd_elapsed_ms), [`arguments`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepFullMatchContext.arguments), [`output_format`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepFullMatchContext.output_format), [`rg_elapsed_ms`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepFullMatchContext.rg_elapsed_ms), [`rg_out`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepFullMatchContext.rg_out), [`searched_file_count`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepFullMatchContext.searched_file_count), [`truncated_fd`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepFullMatchContext.truncated_fd)

### `TestFindAndGrepRgModeContext`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L184)
- signature: `class TestFindAndGrepRgModeContext:`
- members:
  - `test_creation(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L185)
  - `test_frozen(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L196)
- uses (calls/refs, reference-scoped): [`files`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepRgModeContext.files), [`FindAndGrepRgModeContext`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepRgModeContext), [`fd_elapsed_ms`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepRgModeContext.fd_elapsed_ms), [`output_format`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepRgModeContext.output_format), [`truncated_fd`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepRgModeContext.truncated_fd), [`arguments`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#FindAndGrepRgModeContext.arguments)

### `TestHandleFileOutput`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L439)
- signature: `class TestHandleFileOutput:`
- members:
  - `test_exception_sets_error(self)` — [`L495`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L495)
  - `test_save_with_matches(self)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L459)
  - `test_save_with_summary_only(self)` — [`L440`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L440)
  - `test_suppress_returns_minimal(self)` — [`L475`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L475)
- uses (calls/refs, reference-scoped): [`_handle_file_output`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#_handle_file_output)

### `TestHandleOutput`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L395)
- signature: `class TestHandleOutput:`
- members:
  - `test_output_file_triggers_file_output(self)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L418)
  - `test_output_file_updates_result(self)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L430)
  - `test_returns_none_when_no_output_file_and_no_suppress(self)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L396)
  - `test_suppress_includes_agent_summary(self)` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L408)
  - `test_suppress_without_output_file(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L401)
- uses (calls/refs, reference-scoped): [`handle_output`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#handle_output)

### `TestMakeMinimal`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L511)
- signature: `class TestMakeMinimal:`
- members:
  - `test_basic_minimal(self)` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L512)
  - `test_minimal_defaults_count_zero(self)` — [`L569`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L569)
  - `test_minimal_defaults_success_true(self)` — [`L564`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L564)
  - `test_minimal_includes_agent_summary(self)` — [`L545`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L545)
  - `test_minimal_with_summary(self)` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L535)
  - `test_minimal_without_agent_summary(self)` — [`L555`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L555)
  - `test_minimal_without_summary(self)` — [`L525`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L525)
- uses (calls/refs, reference-scoped): [`_make_minimal`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#_make_minimal)

### `TestToolSchema`
- def: [`tests/unit/mcp/test_find_and_grep_helpers.py:26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L26)
- signature: `class TestToolSchema:`
- members:
  - `test_schema_additional_properties_false(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L59)
  - `test_schema_boolean_defaults(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L62)
  - `test_schema_has_case_with_enum(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L55)
  - `test_schema_has_output_format_with_enum(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L47)
  - `test_schema_has_pattern_property(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L44)
  - `test_schema_has_query_property(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L40)
  - `test_schema_has_required_fields(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L33)
  - `test_schema_has_roots_property(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L36)
  - `test_schema_has_sort_with_enum(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L51)
  - `test_schema_integer_properties(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L82)
  - `test_schema_is_dict(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L27)
  - `test_schema_type_is_object(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_find_and_grep_helpers.py#L30)
- uses (calls/refs, reference-scoped): [`TOOL_SCHEMA`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA)

