---
title: 'Module: tests/unit/mcp/test_search_content_init_and_def.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_search_content_init_and_def.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_search_content_init_and_def`/
symbols:
  TestSearchContentToolInitialization.test_init_with_cache_disabled: TestSearchContentToolInitialization#test_init_with_cache_disabled().
  tool: tool().
  TestSearchContentToolInitialization.test_init_multiple_instances: TestSearchContentToolInitialization#test_init_multiple_instances().
  TestSearchContentToolInitialization: TestSearchContentToolInitialization#
  TestSearchContentToolInitialization.test_init_creates_tool: TestSearchContentToolInitialization#test_init_creates_tool().
  TestSetProjectPath: TestSetProjectPath#
  TestSetProjectPath.test_set_project_path_updates_all_components: TestSetProjectPath#test_set_project_path_updates_all_components().
  TestSetProjectPath.test_set_project_path_recreates_file_manager: TestSetProjectPath#test_set_project_path_recreates_file_manager().
  TestGetToolDefinition: TestGetToolDefinition#
  TestGetToolDefinition.test_required_fields: TestGetToolDefinition#test_required_fields().
  TestGetToolDefinition.test_roots_property: TestGetToolDefinition#test_roots_property().
  TestGetToolDefinition.test_files_property: TestGetToolDefinition#test_files_property().
  TestGetToolDefinition.test_query_property: TestGetToolDefinition#test_query_property().
  TestGetToolDefinition.test_case_property: TestGetToolDefinition#test_case_property().
  TestGetToolDefinition.test_total_only_property: TestGetToolDefinition#test_total_only_property().
  TestGetToolDefinition.test_count_only_matches_property: TestGetToolDefinition#test_count_only_matches_property().
  TestGetToolDefinition.test_summary_only_property: TestGetToolDefinition#test_summary_only_property().
  TestGetToolDefinition.test_group_by_file_property: TestGetToolDefinition#test_group_by_file_property().
  TestGetToolDefinition.test_optimize_paths_property: TestGetToolDefinition#test_optimize_paths_property().
  TestDetermineRequestedFormat: TestDetermineRequestedFormat#
  TestDetermineRequestedFormat.test_determine_total_only_format: TestDetermineRequestedFormat#test_determine_total_only_format().
  TestDetermineRequestedFormat.test_determine_count_only_format: TestDetermineRequestedFormat#test_determine_count_only_format().
  TestDetermineRequestedFormat.test_determine_summary_format: TestDetermineRequestedFormat#test_determine_summary_format().
  TestDetermineRequestedFormat.test_determine_group_by_file_format: TestDetermineRequestedFormat#test_determine_group_by_file_format().
  TestDetermineRequestedFormat.test_determine_normal_format: TestDetermineRequestedFormat#test_determine_normal_format().
---
# Module: [`tests/unit/mcp/test_search_content_init_and_def.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py)

## Classes
### `TestDetermineRequestedFormat`
- def: [`tests/unit/mcp/test_search_content_init_and_def.py:128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L128)
- doc: Tests for _determine_requested_format method.
- signature: `class TestDetermineRequestedFormat:`
- members:
  - `test_determine_count_only_format(self, tool)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L136)
  - `test_determine_group_by_file_format(self, tool)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L146)
  - `test_determine_normal_format(self, tool)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L151)
  - `test_determine_summary_format(self, tool)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L141)
  - `test_determine_total_only_format(self, tool)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L131)

### `TestGetToolDefinition`
- def: [`tests/unit/mcp/test_search_content_init_and_def.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L48)
- doc: Tests for get_tool_definition method.
- signature: `class TestGetToolDefinition:`
- members:
  - `test_case_property(self, tool)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L79)
  - `test_count_only_matches_property(self, tool)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L95)
  - `test_files_property(self, tool)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L65)
  - `test_group_by_file_property(self, tool)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L111)
  - `test_optimize_paths_property(self, tool)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L119)
  - `test_query_property(self, tool)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L72)
  - `test_required_fields(self, tool)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L51)
  - `test_roots_property(self, tool)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L58)
  - `test_summary_only_property(self, tool)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L103)
  - `test_total_only_property(self, tool)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L87)

### `TestSearchContentToolInitialization`
- def: [`tests/unit/mcp/test_search_content_init_and_def.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L16)
- doc: Tests for tool initialization.
- signature: `class TestSearchContentToolInitialization:`
- members:
  - `test_init_creates_tool(self, tool)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L19)
  - `test_init_multiple_instances(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L28)
  - `test_init_with_cache_disabled(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L24)
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`cache`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.cache)

### `TestSetProjectPath`
- def: [`tests/unit/mcp/test_search_content_init_and_def.py:34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L34)
- doc: Tests for set_project_path method.
- signature: `class TestSetProjectPath:`
- members:
  - `test_set_project_path_recreates_file_manager(self, tool)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L42)
  - `test_set_project_path_updates_all_components(self, tool)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L37)

## Functions
- `tool()` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_init_and_def.py#L12)

