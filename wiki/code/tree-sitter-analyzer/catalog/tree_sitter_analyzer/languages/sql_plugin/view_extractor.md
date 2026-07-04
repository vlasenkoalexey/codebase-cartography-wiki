---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/view_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/view_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin.view_extractor`/
symbols:
  _extract_view_from_create_node: _extract_view_from_create_node().
  _extract_views_from_error_node: _extract_views_from_error_node().
  extract_sql_views: extract_sql_views().
  _find_view_name: _find_view_name().
  _first_valid_identifier_in: _first_valid_identifier_in().
  _find_view_name_via_regex: _find_view_name_via_regex().
  _find_view_name_via_object_reference: _find_view_name_via_object_reference().
  _extract_view_sources: _extract_view_sources().
  _SQL_KEYWORDS_TO_REJECT_AS_VIEW_NAME: _SQL_KEYWORDS_TO_REJECT_AS_VIEW_NAME.
  _extract_source_tables_from_text: _extract_source_tables_from_text().
  _record_source_table_if_identifier: _record_source_table_if_identifier().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/view_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py)

## Functions
- `_extract_source_tables_from_text(view_body: str)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L112) — Pull table names from a ``FROM ...``/``JOIN ...`` regex over text.
- `_extract_view_from_create_node(node: tree_sitter.Node, traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], sql_elements: list[Any])` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L129) — Extract a single view from a structured ``create_view`` AST node.
- `_extract_view_sources(view_node: tree_sitter.Node, source_tables: list[str], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str])` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L220) — Extract source tables from view definition.
- `_extract_views_from_error_node(node: tree_sitter.Node, get_node_text: Callable[..., str], sql_elements: list[Any])` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L69) — Recover views when tree-sitter falls back to an ERROR node.
- `_find_view_name(node: tree_sitter.Node, raw_text: str, get_node_text: Callable[..., str])` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L162) — Best-effort: regex on raw text first, then AST object_reference walk.
- `_find_view_name_via_object_reference(node: tree_sitter.Node, get_node_text: Callable[..., str])` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L189) — Walk node.children for the first identifier inside object_reference.
- `_find_view_name_via_regex(raw_text: str)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L174) — Match ``CREATE VIEW <name> AS`` on the raw text of the node.
- `_first_valid_identifier_in(object_reference: tree_sitter.Node, get_node_text: Callable[..., str])` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L203) — First non-keyword, valid-identifier ``identifier`` child.
- `_record_source_table_if_identifier(object_reference: tree_sitter.Node, source_tables: list[str], get_node_text: Callable[..., str])` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L236) — Append the object_reference text to ``source_tables`` if it has an identifier child.
- `extract_sql_views(root_node: tree_sitter.Node, traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], source_code: str, content_lines: list[str], sql_elements: list[Any])` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L45) — Extract CREATE VIEW statements with enhanced metadata.

## Module values
- `_SQL_KEYWORDS_TO_REJECT_AS_VIEW_NAME` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/view_extractor.py#L23)

