---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin._class_view_extractor`/
symbols:
  _append_class_view: _append_class_view().
  _is_valid_view_identifier: _is_valid_view_identifier().
  extract_class_views: extract_class_views().
  _recover_single_line_view_span: _recover_single_line_view_span().
  _view_name: _view_name().
  _view_name_from_children: _view_name_from_children().
  _view_name_from_text: _view_name_from_text().
  _find_view_statement_end: _find_view_statement_end().
  _RESERVED_VIEW_NAMES: _RESERVED_VIEW_NAMES.
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py)

## Functions
- `_append_class_view(node: tree_sitter.Node, classes: list[Class], get_node_text: Callable[..., str], is_valid_identifier: Callable[[str], bool], source_code: str, content_lines: list[str])` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py#L53) — Append one view Class when a valid view name can be extracted.
- `_find_view_statement_end(current_line_idx: int, content_lines: list[str])` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py#L175) — Find the inclusive SQL view statement end line number.
- `_is_valid_view_identifier(potential_name: str, is_valid_identifier: Callable[[str], bool])` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py#L140) — Return whether an AST identifier is a plausible view name.
- `_recover_single_line_view_span(raw_text: str, start_line: int, end_line: int, view_name: str, source_code: str, content_lines: list[str])` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py#L152) — Recover full multiline view text when tree-sitter reports one line.
- `_view_name(raw_text: str, node: tree_sitter.Node, get_node_text: Callable[..., str], is_valid_identifier: Callable[[str], bool])` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py#L91) — Return a valid view name from text first, then AST children.
- `_view_name_from_children(node: tree_sitter.Node, get_node_text: Callable[..., str], is_valid_identifier: Callable[[str], bool])` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py#L122) — Extract a view name from object_reference children.
- `_view_name_from_text(raw_text: str, is_valid_identifier: Callable[[str], bool])` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py#L104) — Extract a view name using SQL text.
- `extract_class_views(root_node: tree_sitter.Node, classes: list[Class], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], is_valid_identifier: Callable[[str], bool], source_code: str, content_lines: list[str])` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py#L30) — Extract CREATE VIEW statements as generic Class elements.

## Module values
- `_RESERVED_VIEW_NAMES` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_class_view_extractor.py#L15)

