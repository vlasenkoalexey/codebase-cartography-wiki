---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/function_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/function_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin.function_extractor`/
symbols:
  _append_source_function: _append_source_function().
  _append_ast_function: _append_ast_function().
  _append_legacy_function: _append_legacy_function().
  _extract_function_metadata: _extract_function_metadata().
  _extract_functions_from_source: _extract_functions_from_source().
  extract_legacy_functions: extract_legacy_functions().
  _extract_functions_from_ast: _extract_functions_from_ast().
  extract_sql_functions_enhanced: extract_sql_functions_enhanced().
  _scan_function_end: _scan_function_end().
  _legacy_function_name: _legacy_function_name().
  _traverse_nodes_default: _traverse_nodes_default().
  _function_name_from_ast: _function_name_from_ast().
  _function_name_from_object_reference: _function_name_from_object_reference().
  _FUNCTION_PATTERN: _FUNCTION_PATTERN.
  _is_sql_comment_line: _is_sql_comment_line().
  _is_function_end_line: _is_function_end_line().
  _extract_return_type: _extract_return_type().
  _function_already_extracted: _function_already_extracted().
  _legacy_function_name_from_children: _legacy_function_name_from_children().
  _legacy_function_name_from_text: _legacy_function_name_from_text().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/function_extractor.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py)

## Functions
- `_append_ast_function(node: tree_sitter.Node, func_name: str, get_node_text: Callable[..., str], sql_elements: list[Any])` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L199)
- `_append_legacy_function(node: tree_sitter.Node, functions: list[Function], get_node_text: Callable[..., str], is_valid_identifier_fn: Callable[[str], bool])` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L278) — Append one legacy Function element when a valid name can be found.
- `_append_source_function(sql_elements: list[Any], func_name: str, start_line: int, end_line: int, raw_text: str)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L106)
- `_extract_function_metadata(func_node: tree_sitter.Node, parameters: list[SQLParameter], return_type: str | None, dependencies: list[str], get_node_text: Callable[..., str])` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L234) — Extract function metadata including parameters and return type.
- `_extract_functions_from_ast(root_node: tree_sitter.Node, traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], sql_elements: list[Any])` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L143)
- `_extract_functions_from_source(lines: list[str], sql_elements: list[Any])` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L35)
- `_extract_return_type(raw_text: str)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L136)
- `_function_already_extracted(sql_elements: list[Any], func_name: str)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L190)
- `_function_name_from_ast(node: tree_sitter.Node, get_node_text: Callable[..., str])` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L160)
- `_function_name_from_object_reference(node: tree_sitter.Node, get_node_text: Callable[..., str])` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L172) — Return the function name from an object_reference node.
- `_is_function_end_line(line_stripped: str)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L102)
- `_is_sql_comment_line(line_stripped: str)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L98)
- `_legacy_function_name(node: tree_sitter.Node, get_node_text: Callable[..., str], is_valid_identifier_fn: Callable[[str], bool])` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L303) — Return a legacy function name from AST children or SQL text.
- `_legacy_function_name_from_children(node: tree_sitter.Node, get_node_text: Callable[..., str], is_valid_identifier_fn: Callable[[str], bool])` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L319) — Extract a function name from object_reference children.
- `_legacy_function_name_from_text(raw_text: str, is_valid_identifier_fn: Callable[[str], bool])` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L338) — Extract a function name with regex fallback.
- `_scan_function_end(lines: list[str], search_start: int, default_end_line: int)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L73)
- `_traverse_nodes_default(node: Any)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L356) — Default traverse implementation.
- `extract_legacy_functions(root_node: tree_sitter.Node, functions: list[Function], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], is_valid_identifier_fn: Callable[[str], bool] = is_valid_identifier)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L259) — Extract CREATE FUNCTION statements as generic Function elements.
- `extract_sql_functions_enhanced(root_node: tree_sitter.Node, traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], source_code: str, sql_elements: list[Any])` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L22) — Extract CREATE FUNCTION statements with enhanced metadata.

## Module values
- `_FUNCTION_PATTERN` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/function_extractor.py#L15)

