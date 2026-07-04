---
title: 'Module: tree_sitter_analyzer/mcp/tools/search_content_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/search_content_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.search_content_tool`/
symbols:
  SearchContentTool: SearchContentTool#
  SearchContentTool.execute: SearchContentTool#execute().
  SearchContentTool.validate_arguments: SearchContentTool#validate_arguments().
  SearchContentTool.cache: SearchContentTool#cache.
  SearchContentTool._resolve_no_ignore: SearchContentTool#_resolve_no_ignore().
  SearchContentTool._create_count_only_cache_key: SearchContentTool#_create_count_only_cache_key().
  SearchContentTool._on_project_root_changed: SearchContentTool#_on_project_root_changed().
  SearchContentTool.file_output_manager: SearchContentTool#file_output_manager.
  SearchContentTool._check_file_in_roots: SearchContentTool#_check_file_in_roots().
  SearchContentTool._resolve_inputs: SearchContentTool#_resolve_inputs().
  SearchContentTool._make_cache_key: SearchContentTool#_make_cache_key().
  SearchContentTool._check_cache: SearchContentTool#_check_cache().
  SearchContentTool._run_search: SearchContentTool#_run_search().
  SearchContentTool._validate_roots: SearchContentTool#_validate_roots().
  SearchContentTool._validate_files: SearchContentTool#_validate_files().
  _try_fts5_fast_path: _try_fts5_fast_path().
  SearchContentTool.get_tool_schema: SearchContentTool#get_tool_schema().
  SearchContentTool.get_tool_definition: SearchContentTool#get_tool_definition().
  SearchContentTool._determine_requested_format: SearchContentTool#_determine_requested_format().
  logger: logger.
  SearchContentTool.__init__: SearchContentTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/search_content_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py)

## Classes
### `SearchContentTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/search_content_tool.py:52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L52) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP tool that wraps ripgrep to search content with safety limits.
- signature: `class SearchContentTool(BaseMCPTool):`
- members:
  - `__init__(self, project_root: str | None = None, enable_cache: bool = True)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L59) — Initialize with optional project root and cache toggle.
  - `_check_cache(self, cache_key: str | None, arguments: dict[str, Any])` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L338) — Return cached result if available, None otherwise.
  - `_check_file_in_roots(self, arguments: dict[str, Any])` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L147) — Detect ``roots=['<file>.py']`` and return a canonical error envelope.
  - `_create_count_only_cache_key(self, total_only_cache_key: str, arguments: dict[str, Any])` — [`L398`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L398) — Derive a count_only cache key from a total_only key for cross-mode caching.
  - `_determine_requested_format(self, arguments: dict[str, Any])` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L113) — Determine which response mode based on argument flags.
  - `_make_cache_key(self, arguments: dict[str, Any], roots: list[str] | None)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L321) — Create a cache key from search arguments.
  - `_resolve_inputs(self, arguments: dict[str, Any])` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L289) — Resolve and validate roots/files inputs.
  - `_resolve_no_ignore(self, arguments: dict[str, Any], roots: list[str] | None)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L303) — Determine no_ignore flag with smart gitignore detection.
  - `_run_search(self, arguments: dict[str, Any], rg_args: dict[str, Any], roots: list[str] | None, files: list[str] | None, max_count: int | None, no_ignore: bool)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L377) — Execute the ripgrep search (parallel or single).
  - `_validate_files(self, files: list[str])` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L130) — Resolve and validate each file path in the list.
  - `_validate_roots(self, roots: list[str])` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L118) — Resolve and validate each root directory path.
  - `execute(self, arguments: dict[str, Any])` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L224) — Execute ripgrep search with caching and parallel support. — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
  - `get_tool_definition(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L76) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L72)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L207) — Validate query, roots/files, and all option types.
  - `cache` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L65)
  - `file_output_manager` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L66)
- protocol/private: `_on_project_root_changed`[`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L69)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`FileOutputManager`](../utils/file_output_manager.md#FileOutputManager), [`get`](../utils/search_cache.md#SearchCache.get), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`resolve`](../utils/path_resolver.md#PathResolver.resolve), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`path_resolver`](base_tool.md#BaseMCPTool.path_resolver), [`handle_mcp_errors`](../utils/error_handler.md#handle_mcp_errors), [`get_default_cache`](../utils/search_cache.md#get_default_cache), [`get_managed_instance`](../utils/file_output_manager.md#FileOutputManager.get_managed_instance), [`get_default_detector`](../utils/gitignore_detector.md#get_default_detector), [`format_search_response`](search_content_response.md#format_search_response), [`resolve_and_validate_directory_path`](base_tool.md#BaseMCPTool.resolve_and_validate_directory_path), [`create_cache_key`](../utils/search_cache.md#SearchCache.create_cache_key), [`attach_toon_content_to_response`](../utils/format_helper.md#attach_toon_content_to_response), [`should_use_no_ignore`](../utils/gitignore_detector.md#GitignoreDetector.should_use_no_ignore), [`validate_search_arguments`](search_content_validation.md#validate_search_arguments), [`get_detection_info`](../utils/gitignore_detector.md#GitignoreDetector.get_detection_info), [`run_search`](search_content_helpers.md#run_search), [`check_external_command`](fd_rg_utils.md#check_external_command), [`determine_requested_format`](search_content_response.md#determine_requested_format), [`_try_fts5_fast_path`](search_content_tool.md#_try_fts5_fast_path), [`create_count_only_cache_key`](search_content_response_modes.md#create_count_only_cache_key), [`TOOL_SCHEMA`](search_content_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA), [`build_rg_args`](search_content_response.md#build_rg_args), [`resolve_max_count`](search_content_response.md#resolve_max_count), [`logger`](search_content_tool.md#logger)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_search_facade`](search_facade.md#build_search_facade), [`_run`](../../cli/commands/search_content_cli.md#_run), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases), [`_load_mcp_tool_class`](../../../compatibility_test/scripts/run_compatibility_test.md#_load_mcp_tool_class), [`_content_route`](search_facade.md#build_search_facade._content_route)  (154 test-only)

## Functions
- `_try_fts5_fast_path(arguments: dict[str, Any], project_root: str | None, requested_format: str)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L41)

## Module values
- `logger` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/search_content_tool.py#L38)

