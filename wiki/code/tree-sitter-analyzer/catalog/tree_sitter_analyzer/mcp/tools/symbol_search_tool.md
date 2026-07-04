---
title: 'Module: tree_sitter_analyzer/mcp/tools/symbol_search_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/symbol_search_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.symbol_search_tool`/
symbols:
  CodeGraphSymbolSearchTool: CodeGraphSymbolSearchTool#
  CodeGraphSymbolSearchTool.execute: CodeGraphSymbolSearchTool#execute().
  CodeGraphSymbolSearchTool._search: CodeGraphSymbolSearchTool#_search().
  CodeGraphSymbolSearchTool._inline_match_bodies: CodeGraphSymbolSearchTool#_inline_match_bodies().
  SYMBOL_SEARCH_KINDS.SYMBOL_SEARCH_KINDS: SYMBOL_SEARCH_KINDS.SYMBOL_SEARCH_KINDS.
  CodeGraphSymbolSearchTool._get_cache: CodeGraphSymbolSearchTool#_get_cache().
  CodeGraphSymbolSearchTool.validate_arguments: CodeGraphSymbolSearchTool#validate_arguments().
  CodeGraphSymbolSearchTool.get_tool_schema: CodeGraphSymbolSearchTool#get_tool_schema().
  DEFAULT_SYMBOL_SEARCH_LIMIT: DEFAULT_SYMBOL_SEARCH_LIMIT.
  CodeGraphSymbolSearchTool._exact_search: CodeGraphSymbolSearchTool#_exact_search().
  CodeGraphSymbolSearchTool._fuzzy_search: CodeGraphSymbolSearchTool#_fuzzy_search().
  CodeGraphSymbolSearchTool._read_line: CodeGraphSymbolSearchTool#_read_line().
  CodeGraphSymbolSearchTool._cache: CodeGraphSymbolSearchTool#_cache.
  CodeGraphSymbolSearchTool._demote_test_files: CodeGraphSymbolSearchTool#_demote_test_files().
  CodeGraphSymbolSearchTool._fts_to_results: CodeGraphSymbolSearchTool#_fts_to_results().
  CodeGraphSymbolSearchTool._linear_search: CodeGraphSymbolSearchTool#_linear_search().
  CodeGraphSymbolSearchTool._add_source_context: CodeGraphSymbolSearchTool#_add_source_context().
  logger: logger.
  CodeGraphSymbolSearchTool.get_tool_definition: CodeGraphSymbolSearchTool#get_tool_definition().
  CodeGraphSymbolSearchTool._apply_kind_filter: CodeGraphSymbolSearchTool#_apply_kind_filter().
  CodeGraphSymbolSearchTool.__init__: CodeGraphSymbolSearchTool#__init__().
  CodeGraphSymbolSearchTool._on_project_root_changed: CodeGraphSymbolSearchTool#_on_project_root_changed().
  CodeGraphSymbolSearchTool._wildcard_search: CodeGraphSymbolSearchTool#_wildcard_search().
  CodeGraphSymbolSearchTool._fold_and_rank_results: CodeGraphSymbolSearchTool#_fold_and_rank_results().
---
# Module: [`tree_sitter_analyzer/mcp/tools/symbol_search_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py)

## Classes
### `CodeGraphSymbolSearchTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/symbol_search_tool.py:48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L48)
- doc: MCP Tool for FTS5-powered instant symbol search (CodeGraph parity).
- signature: `class CodeGraphSymbolSearchTool(BaseMCPTool):`
- members:
  - `_demote_test_files(self, results: list[dict[str, Any]], query: str)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L428) — Apply test-file demotion as primary sort key.
  - `_fold_and_rank_results(self, results: list[dict[str, Any]])` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L505) — Issue #443: fold duplicate imports, rank definitions first.
  - `_inline_match_bodies(self, cache: Any, results: list[dict[str, Any]])` — [`L455`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L455) — P2: attach a short body summary to the top matches (in place).
  - `execute(self, arguments: dict[str, Any])` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L134)
  - `get_tool_definition(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L67)
  - `get_tool_schema(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L88)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L126)
- protocol/private: `__init__`[`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L51), `_add_source_context`[`L479`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L479), `_apply_kind_filter`[`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L421), `_cache`[`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L52), `_exact_search`[`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L227), `_fts_to_results`[`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L396), `_fuzzy_search`[`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L254), `_get_cache`[`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L58), `_linear_search`[`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L379), `_on_project_root_changed`[`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L55), `_read_line`[`L488`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L488), `_search`[`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L211), `_wildcard_search`[`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L336)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`_validate_positive_int`](_validators.md#_validate_positive_int), [`inline_search_summaries`](symbol_body_inline.md#inline_search_summaries), [`SYMBOL_SEARCH_KINDS`](symbol_search_tool.md#SYMBOL_SEARCH_KINDS.SYMBOL_SEARCH_KINDS), [`DEFAULT_SYMBOL_SEARCH_LIMIT`](symbol_search_tool.md#DEFAULT_SYMBOL_SEARCH_LIMIT), [`_normalize_bm25`](../../_ast_cache_query.md#_normalize_bm25), [`logger`](symbol_search_tool.md#logger), [`SEARCH_DETERRENT`](symbol_body_inline.md#SEARCH_DETERRENT)  (2 test-only)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_search_facade`](search_facade.md#build_search_facade)  (46 test-only)

## Module values
- `DEFAULT_SYMBOL_SEARCH_LIMIT` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L28)
- `SYMBOL_SEARCH_KINDS` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L36)
- `logger` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_search_tool.py#L23)

