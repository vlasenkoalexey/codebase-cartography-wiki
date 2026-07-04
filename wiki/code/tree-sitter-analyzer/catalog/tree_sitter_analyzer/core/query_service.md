---
title: 'Module: tree_sitter_analyzer/core/query_service.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/query_service.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.query_service`/
symbols:
  QueryService: QueryService#
  QueryService.execute_query: QueryService#execute_query().
  QueryService._execute_plugin_query: QueryService#_execute_plugin_query().
  QueryService.plugin_manager: QueryService#plugin_manager.
  QueryService._fallback_query_execution: QueryService#_fallback_query_execution().
  QueryService.parser: QueryService#parser.
  QueryService.get_available_queries: QueryService#get_available_queries().
  QueryService._create_result_dict: QueryService#_create_result_dict().
  QueryService._extract_parent_context: QueryService#_extract_parent_context().
  QueryService._extract_name_node_text: QueryService#_extract_name_node_text().
  QueryService.get_query_description: QueryService#get_query_description().
  QueryService._read_file_async: QueryService#_read_file_async().
  QueryService._extract_nested_declarator_name: QueryService#_extract_nested_declarator_name().
  QueryService._is_node_like: QueryService#_is_node_like().
  QueryService.project_root: QueryService#project_root.
  QueryService._extract_node_name: QueryService#_extract_node_name().
  QueryService._extract_container_name: QueryService#_extract_container_name().
  logger: logger.
  QueryService._is_point: QueryService#_is_point().
  QueryService._MAX_PARENT_CONTEXT_DEPTH: QueryService#_MAX_PARENT_CONTEXT_DEPTH.
  QueryService._CONTAINER_TYPES: QueryService#_CONTAINER_TYPES.
  QueryService.__init__: QueryService#__init__().
---
# Module: [`tree_sitter_analyzer/core/query_service.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py)

## Classes
### `QueryService`
- def: [`tree_sitter_analyzer/core/query_service.py:29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L29)
- doc: Unified query service providing tree-sitter query functionality
- signature: `class QueryService:`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L34) — Initialize the query service
  - `_create_result_dict(self, node: Any, capture_name: str, source_code: str = "")` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L87) — Create result dictionary from tree-sitter node
  - `_execute_plugin_query(self, root_node: Any, query_key: str | None, language: str, source_code: str)` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L293) — Execute query using plugin-based dynamic dispatch
  - `_extract_node_name(self, node: Any)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L131) — Extract a human-readable name from a tree-sitter node.
  - `_extract_parent_context(self, node: Any)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L198) — Walk up the tree to find the enclosing class/struct/module name.
  - `_fallback_query_execution(self, root_node: Any, query_key: str | None)` — [`L325`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L325) — Basic fallback query execution for unsupported languages
  - `_is_node_like(self, node: Any)` — [`L242`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L242) — Return True for real tree-sitter nodes or explicitly configured test nodes.
  - `_is_point(value: Any)` — [`L257`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L257) — Return True for tree-sitter point tuples.
  - `_read_file_async(self, file_path: str)` — [`L340`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L340) — 非同期ファイル読み込み
  - `execute_query(self, file_path: str, language: str, query_key: str | None = None, query_string: str | None = None, filter_expression: str | None = None)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L42) — Execute a query against a file. — documented in [tree_sitter_analyzer-core-parser](../../../concepts/tree_sitter_analyzer-core-parser.md)
  - `get_available_queries(self, language: str)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L265) — Get available query keys for specified language
  - `get_query_description(self, language: str, query_key: str)` — [`L277`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L277) — Get description for query key
  - `parser` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L37)
  - `plugin_manager` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L39)
  - `project_root` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L36)
- protocol/private: `_CONTAINER_TYPES`[`L173`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L173), `_MAX_PARENT_CONTEXT_DEPTH`[`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L32), `_extract_container_name`[`L228`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L228), `_extract_name_node_text`[`L145`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L145), `_extract_nested_declarator_name`[`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L156)
- uses (calls/refs, reference-scoped): [`Parser`](parser.md#Parser), [`PluginManager`](../plugins/manager.md#PluginManager), [`tree`](parser.md#ParseResult.tree), [`get_plugin`](../plugins/manager.md#PluginManager.get_plugin), [`parse_code`](parser.md#Parser.parse_code), [`QueryFilter`](query_filter.md#QueryFilter), [`get_node_text_safe`](../utils/tree_sitter_compat.md#get_node_text_safe), [`read_file_safe`](../encoding_utils.md#read_file_safe), [`query_loader`](../query_loader.md#query_loader), [`filter_results`](query_filter.md#QueryFilter.filter_results), [`load_plugins`](../plugins/manager.md#PluginManager.load_plugins), [`get_query_description`](../query_loader.md#QueryLoader.get_query_description), [`fallback_query_captures`](_query_service_helpers.md#fallback_query_captures), [`plugin_category_captures`](_query_service_helpers.md#plugin_category_captures), [`plugin_strategy_captures`](_query_service_helpers.md#plugin_strategy_captures), [`execute_ts_query`](query_executor.md#execute_ts_query), [`list_queries`](../query_loader.md#QueryLoader.list_queries), [`resolve_query_string`](query_executor.md#resolve_query_string), [`logger`](query_service.md#logger), [`process_captures`](query_executor.md#process_captures)
- used by: [`_execute_file_query`](../mcp/tools/query_tool.md#QueryTool._execute_file_query), [`_resolve_query`](../cli/commands/query_command.md#QueryCommand._resolve_query), [`execute_query`](../cli/commands/query_command.md#QueryCommand.execute_query), [`query_service`](../mcp/tools/query_tool.md#QueryTool.query_service), [`_on_project_root_changed`](../mcp/tools/query_tool.md#QueryTool._on_project_root_changed), [`debug_test`](../../debug_async_test.md#debug_test), [`_reject_unknown_query_key`](../mcp/tools/query_tool.md#QueryTool._reject_unknown_query_key), [`get_available_queries`](../mcp/tools/query_tool.md#QueryTool.get_available_queries), [`query_service`](../cli/commands/query_command.md#QueryCommand.query_service)  (74 test-only)

## Module values
- `logger` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/query_service.py#L26)

