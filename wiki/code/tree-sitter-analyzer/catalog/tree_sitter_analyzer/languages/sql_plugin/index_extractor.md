---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/index_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/index_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin.index_extractor`/
symbols:
  _append_legacy_index: _append_legacy_index().
  _append_sql_index: _append_sql_index().
  _extract_index_metadata: _extract_index_metadata().
  extract_sql_indexes: extract_sql_indexes().
  extract_indexes_with_regex: extract_indexes_with_regex().
  extract_legacy_indexes: extract_legacy_indexes().
  _append_regex_index: _append_regex_index().
  _sql_index_name: _sql_index_name().
  _legacy_index_name: _legacy_index_name().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/index_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/index_extractor.py)

## Functions
- `_append_legacy_index(node: tree_sitter.Node, variables: list[Variable], get_node_text: Callable[..., str])` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/index_extractor.py#L110) — Append one legacy Variable index when an index name is present.
- `_append_regex_index(match: re.Match[str], line: str, line_num: int, sql_elements: list, processed_indexes: set[str], index_factory: Callable[..., SQLIndex])` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/index_extractor.py#L205) — Append one regex-extracted SQLIndex when its name is not duplicated.
- `_append_sql_index(node: tree_sitter.Node, sql_elements: list[Any], processed_indexes: set[str], get_node_text: Callable[..., str], index_factory: Callable[..., SQLIndex])` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/index_extractor.py#L45) — Append one enhanced SQLIndex when the AST node yields a new valid name.
- `_extract_index_metadata(index_node: tree_sitter.Node, index: SQLIndex, get_node_text: Callable[..., str])` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/index_extractor.py#L148) — Extract index metadata including target table and columns.
- `_legacy_index_name(node: tree_sitter.Node, get_node_text: Callable[..., str])` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/index_extractor.py#L134) — Return the first identifier child text used by legacy extraction.
- `_sql_index_name(node: tree_sitter.Node, get_node_text: Callable[..., str])` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/index_extractor.py#L80) — Return a validated CREATE INDEX name from node text.
- `extract_indexes_with_regex(sql_elements: list, processed_indexes: set[str], source_code: str, index_factory: Callable[..., SQLIndex] = SQLIndex)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/index_extractor.py#L172) — Extract CREATE INDEX statements using regex as fallback.
- `extract_legacy_indexes(root_node: tree_sitter.Node, variables: list[Variable], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str])` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/index_extractor.py#L97) — Extract CREATE INDEX statements as generic Variable elements.
- `extract_sql_indexes(root_node: tree_sitter.Node, traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], source_code: str, sql_elements: list[Any], index_factory: Callable[..., SQLIndex] = SQLIndex)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/index_extractor.py#L15) — Extract CREATE INDEX statements with enhanced metadata.

