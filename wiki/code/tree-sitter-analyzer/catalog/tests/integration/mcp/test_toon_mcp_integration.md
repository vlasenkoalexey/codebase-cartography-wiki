---
title: 'Module: tests/integration/mcp/test_toon_mcp_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_toon_mcp_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_toon_mcp_integration`/Test
symbols:
  TestFileOutputManagerToonSupport.test_detect_toon_format: FileOutputManagerToonSupport#test_detect_toon_format().
  TestFileOutputManagerToonSupport.test_detect_toon_array_table: FileOutputManagerToonSupport#test_detect_toon_array_table().
  TestFileOutputManagerToonSupport.test_toon_extension_mapping: FileOutputManagerToonSupport#test_toon_extension_mapping().
  TestFileOutputManagerToonSupport.test_detect_json_not_toon: FileOutputManagerToonSupport#test_detect_json_not_toon().
  TestFileOutputManagerToonSupport.test_detect_simple_kv_as_toon: FileOutputManagerToonSupport#test_detect_simple_kv_as_toon().
  TestMCPToolSchemaValidation.test_list_files_tool_schema: MCPToolSchemaValidation#test_list_files_tool_schema().
  TestMCPToolSchemaValidation.test_search_content_tool_schema: MCPToolSchemaValidation#test_search_content_tool_schema().
  TestMCPToolSchemaValidation.test_find_and_grep_tool_schema: MCPToolSchemaValidation#test_find_and_grep_tool_schema().
  TestMCPToolSchemaValidation.test_query_tool_schema: MCPToolSchemaValidation#test_query_tool_schema().
  TestMCPToolSchemaValidation.test_read_partial_tool_schema: MCPToolSchemaValidation#test_read_partial_tool_schema().
  TestMCPToolSchemaValidation.test_table_format_tool_schema: MCPToolSchemaValidation#test_table_format_tool_schema().
  TestMCPToolSchemaValidation.test_analyze_scale_tool_schema: MCPToolSchemaValidation#test_analyze_scale_tool_schema().
  TestMCPToolSchemaValidation.test_universal_analyze_tool_schema: MCPToolSchemaValidation#test_universal_analyze_tool_schema().
  TestToonFormatTokenReduction.test_simple_dict_token_reduction: ToonFormatTokenReduction#test_simple_dict_token_reduction().
  TestToonFormatTokenReduction.test_nested_dict_token_reduction: ToonFormatTokenReduction#test_nested_dict_token_reduction().
  TestToonFormatTokenReduction.test_array_table_token_reduction: ToonFormatTokenReduction#test_array_table_token_reduction().
  TestFormatHelper.test_format_output_json: FormatHelper#test_format_output_json().
  TestFormatHelper.test_format_output_toon: FormatHelper#test_format_output_toon().
  TestFormatHelper.test_format_as_json: FormatHelper#test_format_as_json().
  TestFormatHelper.test_format_as_toon: FormatHelper#test_format_as_toon().
  TestFormatHelper.test_format_for_file_output_json: FormatHelper#test_format_for_file_output_json().
  TestFormatHelper.test_format_for_file_output_toon: FormatHelper#test_format_for_file_output_toon().
  TestFormatHelper.test_get_formatter_json: FormatHelper#test_get_formatter_json().
  TestFormatHelper.test_get_formatter_toon: FormatHelper#test_get_formatter_toon().
  TestApplyToonFormatToResponse.test_json_format_returns_original: ApplyToonFormatToResponse#test_json_format_returns_original().
  TestApplyToonFormatToResponse.test_toon_format_removes_redundant_fields: ApplyToonFormatToResponse#test_toon_format_removes_redundant_fields().
  TestApplyToonFormatToResponse.test_toon_format_removes_all_redundant_fields: ApplyToonFormatToResponse#test_toon_format_removes_all_redundant_fields().
  TestApplyToonFormatToResponse.test_toon_content_contains_full_data: ApplyToonFormatToResponse#test_toon_content_contains_full_data().
  TestFormatHelper: FormatHelper#
  TestFileOutputManagerToonSupport: FileOutputManagerToonSupport#
  TestMCPToolSchemaValidation: MCPToolSchemaValidation#
  TestApplyToonFormatToResponse: ApplyToonFormatToResponse#
  TestToonFormatTokenReduction: ToonFormatTokenReduction#
---
# Module: [`tests/integration/mcp/test_toon_mcp_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py)

## Classes
### `TestApplyToonFormatToResponse`
- def: [`tests/integration/mcp/test_toon_mcp_integration.py:262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L262)
- doc: Test apply_toon_format_to_response function behavior.
- signature: `class TestApplyToonFormatToResponse:`
- members:
  - `test_json_format_returns_original(self)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L265) — Test that JSON format returns the original result unchanged.
  - `test_toon_content_contains_full_data(self)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L340) — Test that toon_content contains all original data in TOON format.
  - `test_toon_format_removes_all_redundant_fields(self)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L309) — Test that all redundant field types are removed.
  - `test_toon_format_removes_redundant_fields(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L282) — Test that TOON format strips bulk data but keeps metadata.
- uses (calls/refs, reference-scoped): [`apply_toon_format_to_response`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#apply_toon_format_to_response)

### `TestFileOutputManagerToonSupport`
- def: [`tests/integration/mcp/test_toon_mcp_integration.py:95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L95)
- doc: Test FileOutputManager TOON format support.
- signature: `class TestFileOutputManagerToonSupport:`
- members:
  - `test_detect_json_not_toon(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L138) — Test that JSON is not misdetected as TOON.
  - `test_detect_simple_kv_as_toon(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L146) — Test simple key-value content is detected as TOON.
  - `test_detect_toon_array_table(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L115) — Test TOON array table format detection.
  - `test_detect_toon_format(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L98) — Test TOON format detection.
  - `test_toon_extension_mapping(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L131) — Test .toon extension is returned for TOON content type.
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`detect_content_type`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.detect_content_type), [`get_file_extension`](../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_file_extension)

### `TestFormatHelper`
- def: [`tests/integration/mcp/test_toon_mcp_integration.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L22)
- doc: Test format helper functions.
- signature: `class TestFormatHelper:`
- members:
  - `test_format_as_json(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L43) — Test format_as_json function.
  - `test_format_as_toon(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L52) — Test format_as_toon function.
  - `test_format_for_file_output_json(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L60) — Test format_for_file_output with JSON format.
  - `test_format_for_file_output_toon(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L69) — Test format_for_file_output with TOON format.
  - `test_format_output_json(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L25) — Test format_output with JSON format.
  - `test_format_output_toon(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L34) — Test format_output with TOON format.
  - `test_get_formatter_json(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L78) — Test get_formatter returns JSON formatter by default.
  - `test_get_formatter_toon(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L86) — Test get_formatter returns TOON formatter.
- uses (calls/refs, reference-scoped): [`format_for_file_output`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_for_file_output), [`format_as_toon`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_as_toon), [`format_output`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_output), [`get_formatter`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#get_formatter), [`format_as_json`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_as_json)

### `TestMCPToolSchemaValidation`
- def: [`tests/integration/mcp/test_toon_mcp_integration.py:159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L159)
- doc: Test that MCP tools have output_format parameter in their schemas.
- signature: `class TestMCPToolSchemaValidation:`
- members:
  - `test_analyze_scale_tool_schema(self)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L236) — Test check_code_scale tool has output_format parameter.
  - `test_find_and_grep_tool_schema(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L186) — Test find_and_grep tool has output_format parameter.
  - `test_list_files_tool_schema(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L162) — Test list_files tool has output_format parameter.
  - `test_query_tool_schema(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L198) — Test query_code tool has output_format parameter.
  - `test_read_partial_tool_schema(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L210) — Test extract_code_section tool has output_format parameter.
  - `test_search_content_tool_schema(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L174) — Test search_content tool has output_format parameter.
  - `test_table_format_tool_schema(self)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L222) — Test analyze_code_structure tool has output_format parameter.
  - `test_universal_analyze_tool_schema(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L247) — Test analyze_code_universal tool has output_format parameter.
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`ReadPartialTool`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool), [`ListFilesTool`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool), [`AnalyzeCodeStructureTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`FindAndGrepTool`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_tool.md#FindAndGrepTool), [`QueryTool`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool), [`AnalyzeScaleTool`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool), [`UniversalAnalyzeTool`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/read_partial_tool.md#ReadPartialTool.get_tool_definition), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.get_tool_definition), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.get_tool_definition), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/query_tool.md#QueryTool.get_tool_definition), [`get_tool_schema`](../../../tree_sitter_analyzer/mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool.get_tool_schema), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_tool.md#FindAndGrepTool.get_tool_definition), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/list_files_tool.md#ListFilesTool.get_tool_definition), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.get_tool_definition)

### `TestToonFormatTokenReduction`
- def: [`tests/integration/mcp/test_toon_mcp_integration.py:361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L361)
- doc: Test that TOON format achieves token reduction compared to JSON.
- signature: `class TestToonFormatTokenReduction:`
- members:
  - `test_array_table_token_reduction(self)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L405) — Test TOON array table format reduces tokens significantly.
  - `test_nested_dict_token_reduction(self)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L381) — Test TOON produces shorter output for nested structures.
  - `test_simple_dict_token_reduction(self)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_toon_mcp_integration.py#L364) — Test TOON produces shorter output than JSON for simple dict.
- uses (calls/refs, reference-scoped): [`format_as_toon`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_as_toon), [`format_as_json`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#format_as_json)

