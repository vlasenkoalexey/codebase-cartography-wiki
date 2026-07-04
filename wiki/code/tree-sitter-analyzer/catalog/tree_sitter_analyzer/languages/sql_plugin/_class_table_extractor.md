---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/_class_table_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/_class_table_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin._class_table_extractor`/
symbols:
  _append_class_table: _append_class_table().
  extract_class_tables: extract_class_tables().
  _table_name_from_children: _table_name_from_children().
  _last_identifier_from_object_reference: _last_identifier_from_object_reference().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/_class_table_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_table_extractor.py)

## Functions
- `_append_class_table(node: tree_sitter.Node, classes: list[Class], get_node_text: Callable[..., str], is_valid_identifier: Callable[[str], bool])` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_table_extractor.py#L29) — Append one table Class when a valid table name can be extracted.
- `_last_identifier_from_object_reference(node: tree_sitter.Node, get_node_text: Callable[..., str], is_valid_identifier: Callable[[str], bool])` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_table_extractor.py#L76) — Extract the LAST valid identifier from an object_reference node.
- `_table_name_from_children(node: tree_sitter.Node, get_node_text: Callable[..., str], is_valid_identifier: Callable[[str], bool])` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_table_extractor.py#L54) — Extract a table name from object_reference children.
- `extract_class_tables(root_node: tree_sitter.Node, classes: list[Class], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], is_valid_identifier: Callable[[str], bool])` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_table_extractor.py#L15) — Extract CREATE TABLE statements as generic Class elements.

