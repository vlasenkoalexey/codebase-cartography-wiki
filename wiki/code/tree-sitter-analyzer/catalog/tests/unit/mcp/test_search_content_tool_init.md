---
title: 'Module: tests/unit/mcp/test_search_content_tool_init.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_search_content_tool_init.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_search_content_tool_init`/
symbols:
  TestSearchContentToolInitialization.test_init_with_cache_disabled: TestSearchContentToolInitialization#test_init_with_cache_disabled().
  tool: tool().
  TestSearchContentToolInitialization.test_init_multiple_instances: TestSearchContentToolInitialization#test_init_multiple_instances().
  sample_project_structure: sample_project_structure().
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
  TestValidateRoots: TestValidateRoots#
  TestValidateRoots.test_validate_roots_success: TestValidateRoots#test_validate_roots_success().
  TestValidateRoots.test_validate_roots_invalid_directory: TestValidateRoots#test_validate_roots_invalid_directory().
  TestValidateFiles: TestValidateFiles#
  TestValidateFiles.test_validate_files_success: TestValidateFiles#test_validate_files_success().
  TestValidateFiles.test_validate_files_empty_string: TestValidateFiles#test_validate_files_empty_string().
  TestValidateFiles.test_validate_files_not_found: TestValidateFiles#test_validate_files_not_found().
  TestValidateArguments: TestValidateArguments#
  TestValidateArguments.test_validate_valid_arguments_with_roots: TestValidateArguments#test_validate_valid_arguments_with_roots().
  TestValidateArguments.test_validate_valid_arguments_with_files: TestValidateArguments#test_validate_valid_arguments_with_files().
  TestValidateArguments.test_validate_missing_query: TestValidateArguments#test_validate_missing_query().
  TestValidateArguments.test_validate_empty_query: TestValidateArguments#test_validate_empty_query().
  TestValidateArguments.test_validate_whitespace_query: TestValidateArguments#test_validate_whitespace_query().
  TestValidateArguments.test_validate_missing_both_roots_and_files: TestValidateArguments#test_validate_missing_both_roots_and_files().
  TestValidateArguments.test_validate_invalid_case_type: TestValidateArguments#test_validate_invalid_case_type().
  TestValidateArguments.test_validate_invalid_encoding_type: TestValidateArguments#test_validate_invalid_encoding_type().
  TestValidateArguments.test_validate_invalid_max_filesize_type: TestValidateArguments#test_validate_invalid_max_filesize_type().
  TestValidateArguments.test_validate_invalid_fixed_strings_type: TestValidateArguments#test_validate_invalid_fixed_strings_type().
  TestValidateArguments.test_validate_invalid_word_type: TestValidateArguments#test_validate_invalid_word_type().
  TestValidateArguments.test_validate_invalid_multiline_type: TestValidateArguments#test_validate_invalid_multiline_type().
  TestValidateArguments.test_validate_invalid_include_globs_type: TestValidateArguments#test_validate_invalid_include_globs_type().
  TestDetermineRequestedFormat: TestDetermineRequestedFormat#
  TestDetermineRequestedFormat.test_determine_total_only_format: TestDetermineRequestedFormat#test_determine_total_only_format().
  TestDetermineRequestedFormat.test_determine_count_only_format: TestDetermineRequestedFormat#test_determine_count_only_format().
  TestDetermineRequestedFormat.test_determine_summary_format: TestDetermineRequestedFormat#test_determine_summary_format().
  TestDetermineRequestedFormat.test_determine_group_by_file_format: TestDetermineRequestedFormat#test_determine_group_by_file_format().
  TestDetermineRequestedFormat.test_determine_normal_format: TestDetermineRequestedFormat#test_determine_normal_format().
---
# Module: [`tests/unit/mcp/test_search_content_tool_init.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py)

## Classes
### `TestDetermineRequestedFormat`
- def: [`tests/unit/mcp/test_search_content_tool_init.py:314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L314)
- doc: Tests for _determine_requested_format method.
- signature: `class TestDetermineRequestedFormat:`
- members:
  - `test_determine_count_only_format(self, tool)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L323) — Test format determination for count_only_matches.
  - `test_determine_group_by_file_format(self, tool)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L335) — Test format determination for group_by_file.
  - `test_determine_normal_format(self, tool)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L341) — Test format determination for normal mode.
  - `test_determine_summary_format(self, tool)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L329) — Test format determination for summary_only.
  - `test_determine_total_only_format(self, tool)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L317) — Test format determination for total_only.

### `TestGetToolDefinition`
- def: [`tests/unit/mcp/test_search_content_tool_init.py:77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L77)
- doc: Tests for get_tool_definition method.
- signature: `class TestGetToolDefinition:`
- members:
  - `test_case_property(self, tool)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L112) — Test that case property is correctly defined.
  - `test_count_only_matches_property(self, tool)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L130) — Test that count_only_matches property is correctly defined.
  - `test_files_property(self, tool)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L96) — Test that files property is correctly defined.
  - `test_group_by_file_property(self, tool)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L148) — Test that group_by_file property is correctly defined.
  - `test_optimize_paths_property(self, tool)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L157) — Test that optimize_paths property is correctly defined.
  - `test_query_property(self, tool)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L104) — Test that query property is correctly defined.
  - `test_required_fields(self, tool)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L80) — Test that required fields are correctly defined.
  - `test_roots_property(self, tool)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L88) — Test that roots property is correctly defined.
  - `test_summary_only_property(self, tool)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L139) — Test that summary_only property is correctly defined.
  - `test_total_only_property(self, tool)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L121) — Test that total_only property is correctly defined.

### `TestSearchContentToolInitialization`
- def: [`tests/unit/mcp/test_search_content_tool_init.py:40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L40)
- doc: Tests for tool initialization.
- signature: `class TestSearchContentToolInitialization:`
- members:
  - `test_init_creates_tool(self, tool)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L43) — Test that initialization creates a tool instance.
  - `test_init_multiple_instances(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L54) — Test that multiple instances are independent.
  - `test_init_with_cache_disabled(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L49) — Test initialization with cache disabled.
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`cache`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.cache)

### `TestSetProjectPath`
- def: [`tests/unit/mcp/test_search_content_tool_init.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L61)
- doc: Tests for set_project_path method.
- signature: `class TestSetProjectPath:`
- members:
  - `test_set_project_path_recreates_file_manager(self, tool)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L70) — Test that set_project_path recreates file manager.
  - `test_set_project_path_updates_all_components(self, tool)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L64) — Test that set_project_path updates all components.

### `TestValidateArguments`
- def: [`tests/unit/mcp/test_search_content_tool_init.py:206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L206)
- doc: Tests for validate_arguments method.
- signature: `class TestValidateArguments:`
- members:
  - `test_validate_empty_query(self, tool)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L231) — Test validation fails when query is empty.
  - `test_validate_invalid_case_type(self, tool)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L249) — Test validation fails when case is not a string.
  - `test_validate_invalid_encoding_type(self, tool)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L255) — Test validation fails when encoding is not a string.
  - `test_validate_invalid_fixed_strings_type(self, tool)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L275) — Test validation fails when fixed_strings is not a boolean.
  - `test_validate_invalid_include_globs_type(self, tool)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L301) — Test validation fails when include_globs is not an array.
  - `test_validate_invalid_max_filesize_type(self, tool)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L265) — Test validation fails when max_filesize is not a string.
  - `test_validate_invalid_multiline_type(self, tool)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L291) — Test validation fails when multiline is not a boolean.
  - `test_validate_invalid_word_type(self, tool)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L285) — Test validation fails when word is not a boolean.
  - `test_validate_missing_both_roots_and_files(self, tool)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L243) — Test validation fails when both roots and files are missing.
  - `test_validate_missing_query(self, tool)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L225) — Test validation fails when query is missing.
  - `test_validate_valid_arguments_with_files(self, tool, sample_project_structure)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L217) — Test validation with valid arguments using files.
  - `test_validate_valid_arguments_with_roots(self, tool, sample_project_structure)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L209) — Test validation with valid arguments using roots.
  - `test_validate_whitespace_query(self, tool)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L237) — Test validation fails when query is only whitespace.

### `TestValidateFiles`
- def: [`tests/unit/mcp/test_search_content_tool_init.py:184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L184)
- doc: Tests for _validate_files method.
- signature: `class TestValidateFiles:`
- members:
  - `test_validate_files_empty_string(self, tool)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L193) — Test validation fails when file is empty string.
  - `test_validate_files_not_found(self, tool)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L199) — Test validation fails when file doesn't exist.
  - `test_validate_files_success(self, tool, sample_project_structure)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L187) — Test successful files validation.

### `TestValidateRoots`
- def: [`tests/unit/mcp/test_search_content_tool_init.py:167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L167)
- doc: Tests for _validate_roots method.
- signature: `class TestValidateRoots:`
- members:
  - `test_validate_roots_invalid_directory(self, tool)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L177) — Test validation fails when directory doesn't exist.
  - `test_validate_roots_success(self, tool, sample_project_structure)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L170) — Test successful roots validation.

## Functions
- `sample_project_structure(tmp_path: Path)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L25) — Create a sample project structure for testing.
- `tool()` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_search_content_tool_init.py#L19) — Create a fresh tool instance for each test.

