---
title: 'Module: tree_sitter_analyzer/mcp/tools/query_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/query_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.query_tool`/
symbols:
  QueryTool: QueryTool#
  QueryTool.execute: QueryTool#execute().
  QueryTool._execute_file_query: QueryTool#_execute_file_query().
  _categorize_queries: _categorize_queries.
  QueryTool.query_service: QueryTool#query_service.
  QueryTool._on_project_root_changed: QueryTool#_on_project_root_changed().
  QueryTool._find_productive_queries: QueryTool#_find_productive_queries().
  QueryTool._dispatch: QueryTool#_dispatch().
  QueryTool._check_query_language_mismatch: QueryTool#_check_query_language_mismatch().
  QueryTool._reject_unknown_query_key: QueryTool#_reject_unknown_query_key().
  QueryTool._empty_result: QueryTool#_empty_result().
  _attach_query_envelope_extras: _attach_query_envelope_extras().
  QueryTool.get_tool_definition: QueryTool#get_tool_definition().
  QueryTool.file_output_manager: QueryTool#file_output_manager.
  QueryTool.get_available_queries: QueryTool#get_available_queries().
  QueryTool._execute_cross_file: QueryTool#_execute_cross_file().
  QueryTool._detect_language: QueryTool#_detect_language().
  QueryTool._handle_output: QueryTool#_handle_output().
  QueryTool._execute_symbol_search: QueryTool#_execute_symbol_search().
  QueryTool._execute_find_references: QueryTool#_execute_find_references().
  _analysis_error: _analysis_error().
  QueryTool._extract_name_from_content: QueryTool#_extract_name_from_content().
  QueryTool.validate_arguments: QueryTool#validate_arguments().
  QueryTool.get_tool_schema: QueryTool#get_tool_schema().
  QueryTool._validate_query_arguments: QueryTool#_validate_query_arguments().
  QueryTool._format_summary: QueryTool#_format_summary().
  _build_query_error_response: _build_query_error_response().
  _format_query_results: _format_query_results().
  logger: logger.
  QueryTool._build_next_steps: QueryTool#_build_next_steps().
  _apply_max_count_cap: _apply_max_count_cap().
  _probe_query_keys: _probe_query_keys().
  _PROBE_QUERY_KEYS._PROBE_QUERY_KEYS: _PROBE_QUERY_KEYS._PROBE_QUERY_KEYS.
  QueryTool.__init__: QueryTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/query_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py)

## Classes
### `QueryTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/query_tool.py:40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L40) — documented in [tree_sitter_analyzer-mcp-server](../../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: MCP query tool providing tree-sitter query functionality
- signature: `class QueryTool(BaseMCPTool):`
- members:
  - `_check_query_language_mismatch(self, resolved: str, file_path: str, arguments: dict[str, Any])` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L220) — O3 (round-30): refuse ``--language java`` on a ``.py`` file.
  - `_detect_language(self, resolved: str, arguments: dict[str, Any])` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L264) — Detect language from file or argument.
  - `_dispatch(self, arguments: dict[str, Any])` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L108) — Route to cross-file search or single-file query.
  - `_empty_result(self, file_path: str, language: str, query_key: str | None, query_string: str | None, resolved: str, *, elapsed_ms: float | None = None, output_format: str = "json")` — [`L273`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L273) — Build helpful response for empty query results.
  - `_execute_cross_file(self, arguments: dict[str, Any])` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L118) — Dispatch cross-file query: symbol search or find-references.
  - `_execute_file_query(self, arguments: dict[str, Any])` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L124) — Execute a single-file query.
  - `_execute_find_references(self, arguments: dict[str, Any])` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L367) — Delegate cross-file reference search to helper.
  - `_execute_symbol_search(self, arguments: dict[str, Any])` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L363) — Delegate cross-file symbol search to helper.
  - `_find_productive_queries(self, resolved: str, language: str)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L315) — Find which common queries produce results for a file.
  - `_handle_output(self, formatted: dict[str, Any], arguments: dict[str, Any], file_path: str, language: str, query: str | None)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L326) — Handle file output and suppress logic.
  - `_reject_unknown_query_key(self, query_key: str | None, language: str)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L245) — Return an error envelope when ``query_key`` isn't registered for ``language``.
  - `_validate_query_arguments(arguments: dict[str, Any])` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L203) — Reject missing / mutually-exclusive ``query_key`` + ``query_string``.
  - `execute(self, arguments: dict[str, Any])` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L96) — Execute a single-file query or cross-file symbol search. — documented in [tree_sitter_analyzer-mcp-utils-error_handler](../../../../concepts/tree_sitter_analyzer-mcp-utils-error_handler.md)
  - `get_available_queries(self, language: str)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L358) — Return available query keys for a language.
  - `get_tool_definition(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L60) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L56)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L374) — Validate file_path/symbol, query_key/query_string, and options.
  - `file_output_manager` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L49)
  - `query_service` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L48)
- protocol/private: `__init__`[`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L43), `_build_next_steps`[`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L352), `_extract_name_from_content`[`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L346), `_format_summary`[`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L340), `_on_project_root_changed`[`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L52)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`detect_language_from_file`](../../language_detector.md#detect_language_from_file), [`FileOutputManager`](../utils/file_output_manager.md#FileOutputManager), [`AnalysisError`](../utils/error_handler.md#AnalysisError), [`QueryService`](../../core/query_service.md#QueryService), [`execute_query`](../../core/query_service.md#QueryService.execute_query), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`execute_symbol_search`](query_symbol_search.md#execute_symbol_search), [`normalize_envelope`](search_envelope.md#normalize_envelope), [`get_managed_instance`](../utils/file_output_manager.md#FileOutputManager.get_managed_instance), [`execute_find_references`](query_symbol_search.md#execute_find_references), [`detect_language_mismatch`](base_tool.md#detect_language_mismatch), [`language_mismatch_error_response`](base_tool.md#language_mismatch_error_response), [`get_available_queries`](../../core/query_service.md#QueryService.get_available_queries), [`handle_query_output`](query_helpers.md#handle_query_output), [`_attach_query_envelope_extras`](query_tool.md#_attach_query_envelope_extras), [`build_query_agent_summary`](query_helpers.md#build_query_agent_summary), [`TOOL_SCHEMA`](query_helpers.md#TOOL_SCHEMA.TOOL_SCHEMA), [`_analysis_error`](query_tool.md#_analysis_error), [`extract_name_from_content`](query_helpers.md#extract_name_from_content), [`format_summary`](query_helpers.md#format_summary), [`validate_query_arguments`](query_helpers.md#validate_query_arguments), [`_build_query_error_response`](query_tool.md#_build_query_error_response), [`_format_query_results`](query_tool.md#_format_query_results), [`build_next_steps`](query_helpers.md#build_next_steps), [`categorize_queries`](query_symbol_search.md#categorize_queries), [`logger`](query_tool.md#logger), [`_PROBE_QUERY_KEYS`](query_tool.md#_PROBE_QUERY_KEYS._PROBE_QUERY_KEYS), [`_apply_max_count_cap`](query_tool.md#_apply_max_count_cap), [`_probe_query_keys`](query_tool.md#_probe_query_keys)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_search_facade`](search_facade.md#build_search_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases), [`_load_mcp_tool_class`](../../../compatibility_test/scripts/run_compatibility_test.md#_load_mcp_tool_class)  (84 test-only)

## Functions
- `_analysis_error(msg: str)` — [`L482`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L482)
- `_apply_max_count_cap(results: list[Any], max_count: Any)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L401) — Return (capped_results, truncated, total) — caps if ``max_count`` set.
- `_attach_query_envelope_extras(formatted: dict[str, Any], *, arguments: dict[str, Any], file_path: str, language: str, query_used: str, results: list[Any], elapsed_ms: float, truncated: bool, total_results: int)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L411) — Attach elapsed/truncated/output_format/agent_summary + next_steps in place.
- `_build_query_error_response(exc: Exception, project_root: str | None, arguments: dict[str, Any])` — [`L388`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L388) — Build a standardised error response dict for a query execution failure.
- `_format_query_results(results: list[Any], arguments: dict[str, Any], file_path: str, language: str, query_used: str)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L456) — Pick the result envelope shape based on ``result_format``.
- `_probe_query_keys(query_service: Any, resolved: str, language: str, keys: tuple[str, ...])` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L441) — Return which query keys produce non-empty results for a file.

## Module values
- `_PROBE_QUERY_KEYS` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L379)
- `_categorize_queries` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L489)
- `logger` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/query_tool.py#L37)

