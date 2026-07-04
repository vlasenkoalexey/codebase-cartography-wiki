---
title: 'Module: tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._codegraph_query_symbols`/
symbols:
  build_file_entries: build_file_entries().
  source_preference_key: source_preference_key().
  dedupe_symbols: dedupe_symbols().
  symbol_key_tuple: symbol_key_tuple().
  drop_test_shadow_symbols: drop_test_shadow_symbols().
  symbol_key: symbol_key().
  absolute_path: absolute_path().
  unique_symbol_files: unique_symbol_files().
  source_first_symbols: source_first_symbols().
  _MAX_SNIPPET_LINES: _MAX_SNIPPET_LINES.
  _MAX_FILE_BYTES: _MAX_FILE_BYTES.
  row_symbol: row_symbol().
---
# Module: [`tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py)

## Functions
- `absolute_path(project_root: str, file_path: str)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L161)
- `build_file_entries(*, project_root: str, symbols: list[dict[str, Any]], max_files: int, include_code: bool)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L37)
- `dedupe_symbols(symbols: list[dict[str, Any]])` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L102)
- `drop_test_shadow_symbols(symbols: list[dict[str, Any]])` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L118)
- `row_symbol(row: dict[str, Any], name_key: str, file_key: str, line_key: str)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L20)
- `source_first_symbols(symbols: Any)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L114)
- `source_preference_key(symbol: dict[str, Any])` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L137)
- `symbol_key(symbol: dict[str, Any])` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L167)
- `symbol_key_tuple(symbol: dict[str, Any])` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L171)
- `unique_symbol_files(symbols: list[dict[str, Any]])` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L149)

## Module values
- `_MAX_FILE_BYTES` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L17)
- `_MAX_SNIPPET_LINES` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_codegraph_query_symbols.py#L16)

