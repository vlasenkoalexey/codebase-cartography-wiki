---
title: 'Module: tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.codegraph_explore_tool`/
symbols:
  CodeGraphExploreTool.execute: CodeGraphExploreTool#execute().
  _handle_no_resolved: _handle_no_resolved().
  CodeGraphExploreTool._try_get_cache: CodeGraphExploreTool#_try_get_cache().
  _build_file_list_results: _build_file_list_results().
  CodeGraphExploreTool._init_cg_if_needed: CodeGraphExploreTool#_init_cg_if_needed().
  CodeGraphExploreTool: CodeGraphExploreTool#
  _resolve_error_resp: _resolve_error_resp().
  CodeGraphExploreTool._call_graph: CodeGraphExploreTool#_call_graph.
  CodeGraphExploreTool._relationship_names: CodeGraphExploreTool#_relationship_names().
  logger: logger.
  CodeGraphExploreTool._get_call_graph: CodeGraphExploreTool#_get_call_graph().
  _warn_response: _warn_response().
  _build_rel_map: _build_rel_map().
  _process_defs: _process_defs().
  _init_call_graph: _init_call_graph().
  CodeGraphExploreTool._get_cache: CodeGraphExploreTool#_get_cache().
  CodeGraphExploreTool._on_project_root_changed: CodeGraphExploreTool#_on_project_root_changed().
  CodeGraphExploreTool._cache: CodeGraphExploreTool#_cache.
  CodeGraphExploreTool.get_tool_schema: CodeGraphExploreTool#get_tool_schema().
  CodeGraphExploreTool._source_path: CodeGraphExploreTool#_source_path().
  CodeGraphExploreTool.get_tool_definition: CodeGraphExploreTool#get_tool_definition().
  _HINT_NOT_FOUND: _HINT_NOT_FOUND.
  _empty_stats: _empty_stats().
  _make_stats: _make_stats().
  _collect_names: _collect_names().
  _MAX_REL_PER_SYMBOL: _MAX_REL_PER_SYMBOL.
  _HINT_NO_ROOT: _HINT_NO_ROOT.
  _HINT_NO_CACHE: _HINT_NO_CACHE.
  _sym_callees: _sym_callees().
  _deduped: _deduped().
  _file_matches_tokens: _file_matches_tokens().
  _merge_with_concept: _merge_with_concept().
  _MAX_FILES_CAP: _MAX_FILES_CAP.
  _MAX_SYMBOLS_CAP: _MAX_SYMBOLS_CAP.
  _MAX_SNIPPET_LINES: _MAX_SNIPPET_LINES.
  _MAX_FILE_BYTES: _MAX_FILE_BYTES.
  CodeGraphExploreTool.validate_arguments: CodeGraphExploreTool#validate_arguments().
  _EXPLORE_SCHEMA._EXPLORE_SCHEMA: _EXPLORE_SCHEMA._EXPLORE_SCHEMA.
  CodeGraphExploreTool.__init__: CodeGraphExploreTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py)

## Classes
### `CodeGraphExploreTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py:358`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L358)
- doc: MCP Tool: bulk-fetch N related symbols' source + relationship map.
- signature: `class CodeGraphExploreTool(BaseMCPTool):`
- members:
  - `_relationship_names(self, cache: Any, symbol_name: str, file_path: str)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L608) — Return capped callers/callees via SQL-native cache lookups.
  - `execute(self, arguments: dict[str, Any])` — [`L472`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L472)
  - `get_tool_definition(self)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L377)
  - `get_tool_schema(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L399)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L402)
- protocol/private: `__init__`[`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L361), `_cache`[`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L363), `_call_graph`[`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L364), `_get_cache`[`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L446), `_get_call_graph`[`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L459), `_init_cg_if_needed`[`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L451), `_on_project_root_changed`[`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L367), `_source_path`[`L603`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L603), `_try_get_cache`[`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L425)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`build_response`](_response_builder.md#build_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`get_stats`](../../ast_cache.md#ASTCache.get_stats), [`SymbolResolver`](../../symbol_resolver.md#SymbolResolver), [`concept_search`](_codegraph_explore_helpers.md#concept_search), [`_handle_no_resolved`](codegraph_explore_tool.md#_handle_no_resolved), [`split_query`](_codegraph_explore_helpers.md#split_query), [`_build_file_list_results`](codegraph_explore_tool.md#_build_file_list_results), [`_resolve_error_resp`](codegraph_explore_tool.md#_resolve_error_resp), [`logger`](codegraph_explore_tool.md#logger), [`_warn_response`](codegraph_explore_tool.md#_warn_response), [`_build_rel_map`](codegraph_explore_tool.md#_build_rel_map), [`_init_call_graph`](codegraph_explore_tool.md#_init_call_graph), [`resolve_tokens`](_codegraph_explore_helpers.md#resolve_tokens), [`_MAX_REL_PER_SYMBOL`](codegraph_explore_tool.md#_MAX_REL_PER_SYMBOL), [`_collect_names`](codegraph_explore_tool.md#_collect_names), [`_empty_stats`](codegraph_explore_tool.md#_empty_stats), [`_EXPLORE_SCHEMA`](codegraph_explore_tool.md#_EXPLORE_SCHEMA._EXPLORE_SCHEMA), [`_HINT_NO_CACHE`](codegraph_explore_tool.md#_HINT_NO_CACHE), [`_HINT_NO_ROOT`](codegraph_explore_tool.md#_HINT_NO_ROOT), [`_MAX_FILES_CAP`](codegraph_explore_tool.md#_MAX_FILES_CAP), [`_MAX_FILE_BYTES`](codegraph_explore_tool.md#_MAX_FILE_BYTES), [`_MAX_SNIPPET_LINES`](codegraph_explore_tool.md#_MAX_SNIPPET_LINES), [`_MAX_SYMBOLS_CAP`](codegraph_explore_tool.md#_MAX_SYMBOLS_CAP), [`_file_matches_tokens`](codegraph_explore_tool.md#_file_matches_tokens), [`_merge_with_concept`](codegraph_explore_tool.md#_merge_with_concept)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_structure_facade`](structure_facade.md#build_structure_facade)  (3 test-only)

## Functions
- `_build_file_list_results(ordered_files: list[str], files_map: dict[str, list[Any]], include_code: bool, source_path_fn: Any, rel_fn: Any, max_file_bytes: int, max_snippet_lines: int)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L216)
- `_build_rel_map(file_entries: list[dict[str, Any]], kept_names: set[str])` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L162)
- `_collect_names(rows: list[Any], key: str, cap: int)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L338)
- `_deduped(items: list[str])` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L152)
- `_empty_stats()` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L128)
- `_file_matches_tokens(d: Any, file_tokens: list[str])` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L322)
- `_handle_no_resolved(concept_entries: list[Any], query: str, nterms: int, output_format: str)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L286)
- `_init_call_graph(project_root: str, cache: Any)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L314)
- `_make_stats(nterms: int, nresolved: int, nreturned: int, nfiles: int)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L137)
- `_merge_with_concept(concept_entries: list[Any], file_entries: list[Any], concept_paths: set[str], max_files: int)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L326)
- `_process_defs(defs: list[Any], source_lines: list[str], file_size: int, include_code: bool, rel_fn: Any, max_file_bytes: int, max_snippet_lines: int)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L175)
- `_resolve_error_resp(exc: Exception, nterms: int, query: str, output_format: str)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L269)
- `_sym_callees(sym: dict[str, Any])` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L148)
- `_warn_response(verdict: str, query: str, stats: dict[str, Any], hint: str, output_format: str)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L255)

## Module values
- `_EXPLORE_SCHEMA` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L61)
- `_HINT_NOT_FOUND` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L56)
- `_HINT_NO_CACHE` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L53)
- `_HINT_NO_ROOT` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L49)
- `_MAX_FILES_CAP` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L351)
- `_MAX_FILE_BYTES` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L354)
- `_MAX_REL_PER_SYMBOL` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L355)
- `_MAX_SNIPPET_LINES` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L353)
- `_MAX_SYMBOLS_CAP` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L352)
- `logger` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/codegraph_explore_tool.py#L46)

