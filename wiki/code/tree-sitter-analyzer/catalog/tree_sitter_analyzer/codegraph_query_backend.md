---
title: 'Module: tree_sitter_analyzer/codegraph_query_backend.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/codegraph_query_backend.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.codegraph_query_backend`/
symbols:
  CodeGraphQueryBackend: CodeGraphQueryBackend#
  CodeGraphQueryBackend.resolve_definitions: CodeGraphQueryBackend#resolve_definitions().
  CodeGraphQueryBackend.semantic_symbols: CodeGraphQueryBackend#semantic_symbols().
  CodeGraphQueryBackend.relation_entries: CodeGraphQueryBackend#relation_entries().
  CodeGraphQueryBackend._fts_definitions: CodeGraphQueryBackend#_fts_definitions().
  CodeGraphQueryBackend._symbols_json_definitions: CodeGraphQueryBackend#_symbols_json_definitions().
  CodeGraphQueryBackend.cache: CodeGraphQueryBackend#cache.
  CodeGraphQueryBackend._symbol_row_definitions: CodeGraphQueryBackend#_symbol_row_definitions().
  _definition: _definition().
  _DEFINITION_KINDS: _DEFINITION_KINDS.
  _row_symbol: _row_symbol().
  CodeGraphQueryBackend.__init__: CodeGraphQueryBackend#__init__().
---
# Module: [`tree_sitter_analyzer/codegraph_query_backend.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py)

## Classes
### `CodeGraphQueryBackend`
- def: [`tree_sitter_analyzer/codegraph_query_backend.py:17`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L17)
- doc: Thin facade over AST-cache-backed symbol and relation lookups.
- signature: `class CodeGraphQueryBackend:`
- members:
  - `relation_entries(self, *, direction: str, name: str, file_path: str, depth: int, limit: int)` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L31)
  - `resolve_definitions(self, symbol: str)` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L23)
  - `semantic_symbols(self, query: str, *, limit: int)` — [`L63`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L63)
  - `cache` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L21)
- protocol/private: `__init__`[`L20`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L20), `_fts_definitions`[`L72`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L72), `_symbol_row_definitions`[`L91`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L91), `_symbols_json_definitions`[`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L116)
- uses (calls/refs, reference-scoped): [`search`](semantic_search.md#SemanticSymbolSearch.search), [`SemanticSymbolSearch`](semantic_search.md#SemanticSymbolSearch), [`_definition`](codegraph_query_backend.md#_definition), [`_DEFINITION_KINDS`](codegraph_query_backend.md#_DEFINITION_KINDS), [`_row_symbol`](codegraph_query_backend.md#_row_symbol)
- used by: [`execute`](mcp/tools/codegraph_query_tool.md#CodeGraphQueryTool.execute), [`_resolve_query_with_backend`](mcp/tools/codegraph_query_tool.md#_resolve_query_with_backend), [`_resolve_query`](mcp/tools/codegraph_query_tool.md#_resolve_query), [`_resolve_simple`](symbol_resolver.md#SymbolResolver._resolve_simple), [`_query_relation_entries`](mcp/tools/codegraph_query_tool.md#_query_relation_entries), [`_semantic_queries_with_backend`](mcp/tools/codegraph_query_tool.md#_semantic_queries_with_backend), [`_resolve_queries_with_backend`](mcp/tools/codegraph_query_tool.md#_resolve_queries_with_backend), [`_state_backend`](mcp/tools/codegraph_query_tool.md#_state_backend), [`_resolve_queries`](mcp/tools/codegraph_query_tool.md#_resolve_queries), [`_backend`](xref.md#XRefEngine._backend), [`_definition_backend`](symbol_resolver.md#SymbolResolver._definition_backend), [`__init__`](mcp/tools/_codegraph_query_state.md#_QueryState.__init__)  (9 test-only)

## Functions
- `_definition(*, file_path: str, name: str, kind: str, line: int, end_line: int, language: str, confidence: float)` — [`L160`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L160)
- `_row_symbol(row: dict[str, Any], name_key: str, file_key: str, line_key: str)` — [`L143`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L143)

## Module values
- `_DEFINITION_KINDS` — [`L12`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/codegraph_query_backend.py#L12)

