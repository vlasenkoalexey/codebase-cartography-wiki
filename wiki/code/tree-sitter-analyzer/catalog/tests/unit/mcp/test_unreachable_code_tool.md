---
title: 'Module: tests/unit/mcp/test_unreachable_code_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_unreachable_code_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_unreachable_code_tool`/
symbols:
  _make_result: _make_result().
  TestBuildFileResponse.test_toon_format_with_blocks: TestBuildFileResponse#test_toon_format_with_blocks().
  TestFormatFileBlocksToon.test_returns_header_and_block_lines: TestFormatFileBlocksToon#test_returns_header_and_block_lines().
  TestBuildProjectResponse.test_toon_format_with_results: TestBuildProjectResponse#test_toon_format_with_results().
  TestBuildProjectResponse.test_json_format_returns_counts: TestBuildProjectResponse#test_json_format_returns_counts().
  _make_block: _make_block().
  TestFormatBlockLine.test_formats_correctly: TestFormatBlockLine#test_formats_correctly().
  TestBuildFileResponse.test_toon_format_no_blocks: TestBuildFileResponse#test_toon_format_no_blocks().
  TestBuildFileResponse.test_toon_format_with_errors: TestBuildFileResponse#test_toon_format_with_errors().
  TestBuildFileResponse.test_json_format_returns_dict: TestBuildFileResponse#test_json_format_returns_dict().
  TestBuildFileResponse.test_toon_says_no_unreachable_when_empty: TestBuildFileResponse#test_toon_says_no_unreachable_when_empty().
  TestFormatFileBlocksToon.test_returns_empty_for_no_blocks: TestFormatFileBlocksToon#test_returns_empty_for_no_blocks().
  TestExecute.test_file_mode_success_toon: TestExecute#test_file_mode_success_toon().
  TestExecute.test_project_mode_success: TestExecute#test_project_mode_success().
  TestToolDefinition.test_get_tool_name: TestToolDefinition#test_get_tool_name().
  TestToolDefinition.test_get_tool_definition_has_name: TestToolDefinition#test_get_tool_definition_has_name().
  TestToolDefinition.test_get_tool_schema_has_mode: TestToolDefinition#test_get_tool_schema_has_mode().
  TestValidateArguments.test_valid_file_mode_with_path: TestValidateArguments#test_valid_file_mode_with_path().
  TestValidateArguments.test_valid_project_mode: TestValidateArguments#test_valid_project_mode().
  TestValidateArguments.test_file_mode_missing_path_raises: TestValidateArguments#test_file_mode_missing_path_raises().
  TestValidateArguments.test_invalid_mode_raises: TestValidateArguments#test_invalid_mode_raises().
  TestBuildProjectResponse.test_toon_format_empty_results: TestBuildProjectResponse#test_toon_format_empty_results().
  TestResolvePath.test_returns_absolute_path_when_file_exists: TestResolvePath#test_returns_absolute_path_when_file_exists().
  TestResolvePath.test_resolves_relative_to_project_root: TestResolvePath#test_resolves_relative_to_project_root().
  TestResolvePath.test_returns_none_when_not_found: TestResolvePath#test_returns_none_when_not_found().
  TestExecute.test_file_mode_not_found_returns_error: TestExecute#test_file_mode_not_found_returns_error().
  TestExecute.test_file_mode_missing_path_raises: TestExecute#test_file_mode_missing_path_raises().
  TestExecute.test_file_mode_analysis_error_returns_error: TestExecute#test_file_mode_analysis_error_returns_error().
  TestExecute.test_project_mode_no_root_returns_error: TestExecute#test_project_mode_no_root_returns_error().
  TestExecute.test_project_mode_error_returns_error: TestExecute#test_project_mode_error_returns_error().
  tool: tool().
  TestToolDefinition: TestToolDefinition#
  TestValidateArguments: TestValidateArguments#
  TestFormatBlockLine: TestFormatBlockLine#
  TestBuildFileResponse: TestBuildFileResponse#
  TestFormatFileBlocksToon: TestFormatFileBlocksToon#
  TestBuildProjectResponse: TestBuildProjectResponse#
  TestResolvePath: TestResolvePath#
  TestExecute: TestExecute#
---
# Module: [`tests/unit/mcp/test_unreachable_code_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py)

## Classes
### `TestBuildFileResponse`
- def: [`tests/unit/mcp/test_unreachable_code_tool.py:125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L125)
- signature: `class TestBuildFileResponse:`
- members:
  - `test_json_format_returns_dict(self, tool: UnreachableCodeTool)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L144)
  - `test_toon_format_no_blocks(self, tool: UnreachableCodeTool)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L126)
  - `test_toon_format_with_blocks(self, tool: UnreachableCodeTool)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L131)
  - `test_toon_format_with_errors(self, tool: UnreachableCodeTool)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L138)
  - `test_toon_says_no_unreachable_when_empty(self, tool: UnreachableCodeTool)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L150)
- uses (calls/refs, reference-scoped): [`UnreachableCodeTool`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool), [`_build_file_response`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool._build_file_response)  (2 test-only)

### `TestBuildProjectResponse`
- def: [`tests/unit/mcp/test_unreachable_code_tool.py:182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L182)
- signature: `class TestBuildProjectResponse:`
- members:
  - `test_json_format_returns_counts(self, tool: UnreachableCodeTool)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L196)
  - `test_toon_format_empty_results(self, tool: UnreachableCodeTool)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L183)
  - `test_toon_format_with_results(self, tool: UnreachableCodeTool)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L188)
- uses (calls/refs, reference-scoped): [`UnreachableCodeTool`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool), [`_build_project_response`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool._build_project_response)  (2 test-only)

### `TestExecute`
- def: [`tests/unit/mcp/test_unreachable_code_tool.py:234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L234)
- signature: `class TestExecute:`
- members:
  - `test_file_mode_analysis_error_returns_error(self, tmp_path: Any)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L265)
  - `test_file_mode_missing_path_raises(self, tool: UnreachableCodeTool)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L243)
  - `test_file_mode_not_found_returns_error(self, tool: UnreachableCodeTool)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L236)
  - `test_file_mode_success_toon(self, tmp_path: Any)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L250)
  - `test_project_mode_error_returns_error(self, tool: UnreachableCodeTool)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L292)
  - `test_project_mode_no_root_returns_error(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L277)
  - `test_project_mode_success(self, tool: UnreachableCodeTool)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L283)
- uses (calls/refs, reference-scoped): [`UnreachableCodeTool`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool.execute)  (1 test-only)

### `TestFormatBlockLine`
- def: [`tests/unit/mcp/test_unreachable_code_tool.py:108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L108)
- signature: `class TestFormatBlockLine:`
- members:
  - `test_formats_correctly(self, tool: UnreachableCodeTool)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L109)
- uses (calls/refs, reference-scoped): [`UnreachableCodeTool`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool), [`_format_block_line`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool._format_block_line)  (1 test-only)

### `TestFormatFileBlocksToon`
- def: [`tests/unit/mcp/test_unreachable_code_tool.py:164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L164)
- signature: `class TestFormatFileBlocksToon:`
- members:
  - `test_returns_empty_for_no_blocks(self, tool: UnreachableCodeTool)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L165)
  - `test_returns_header_and_block_lines(self, tool: UnreachableCodeTool)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L169)
- uses (calls/refs, reference-scoped): [`UnreachableCodeTool`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool), [`_format_file_blocks_toon`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool._format_file_blocks_toon)  (2 test-only)

### `TestResolvePath`
- def: [`tests/unit/mcp/test_unreachable_code_tool.py:210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L210)
- signature: `class TestResolvePath:`
- members:
  - `test_resolves_relative_to_project_root(self, tmp_path)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L218)
  - `test_returns_absolute_path_when_file_exists(self, tmp_path, tool: UnreachableCodeTool)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L211)
  - `test_returns_none_when_not_found(self, tool: UnreachableCodeTool)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L225)
- uses (calls/refs, reference-scoped): [`UnreachableCodeTool`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool), [`_resolve_path`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool._resolve_path)

### `TestToolDefinition`
- def: [`tests/unit/mcp/test_unreachable_code_tool.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L67)
- signature: `class TestToolDefinition:`
- members:
  - `test_get_tool_definition_has_name(self, tool: UnreachableCodeTool)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L71)
  - `test_get_tool_name(self, tool: UnreachableCodeTool)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L68)
  - `test_get_tool_schema_has_mode(self, tool: UnreachableCodeTool)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L76)
- uses (calls/refs, reference-scoped): [`UnreachableCodeTool`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool.get_tool_definition), [`get_tool_schema`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool.get_tool_schema), [`get_tool_name`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool.get_tool_name)

### `TestValidateArguments`
- def: [`tests/unit/mcp/test_unreachable_code_tool.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L87)
- signature: `class TestValidateArguments:`
- members:
  - `test_file_mode_missing_path_raises(self, tool: UnreachableCodeTool)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L94)
  - `test_invalid_mode_raises(self, tool: UnreachableCodeTool)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L98)
  - `test_valid_file_mode_with_path(self, tool: UnreachableCodeTool)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L88)
  - `test_valid_project_mode(self, tool: UnreachableCodeTool)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L91)
- uses (calls/refs, reference-scoped): [`UnreachableCodeTool`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/unreachable_code_tool.md#UnreachableCodeTool.validate_arguments)

## Functions
- `_make_block(start: int = 10, end: int = 12, fn: str = "my_func", reason: str = "after return", severity: str = "warning")` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L21)
- `_make_result(file_path: str = "src/foo.py", language: str = "python", blocks: list[Any] | None = None, functions_analyzed: int = 5, errors: list[str] | None = None)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L37)
- `tool()` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_unreachable_code_tool.py#L58)

