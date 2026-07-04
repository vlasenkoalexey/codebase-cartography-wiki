---
title: 'Module: tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.utils._tree_sitter_compat_helpers`/
symbols:
  execute_query_object: execute_query_object().
  logger: logger.
  get_node_text_compat: get_node_text_compat().
  execute_old_api: execute_old_api().
  execute_query_compat: execute_query_compat().
  get_node_text_by_points: get_node_text_by_points().
  execute_newest_api: execute_newest_api().
  execute_modern_api: execute_modern_api().
  execute_legacy_api: execute_legacy_api().
  old_api_captures_from_result: old_api_captures_from_result().
  old_api_capture_from_item: old_api_capture_from_item().
  get_node_text_by_bytes: get_node_text_by_bytes().
  get_node_text_attribute: get_node_text_attribute().
  get_single_line_text: get_single_line_text().
  get_multi_line_text: get_multi_line_text().
---
# Module: [`tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py)

## Functions
- `execute_legacy_api(query: Any, root_node: Any)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L72)
- `execute_modern_api(query: Any, root_node: Any)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L57)
- `execute_newest_api(query: Any, root_node: Any)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L39)
- `execute_old_api(query: Any, root_node: Any)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L101)
- `execute_query_compat(language: Any, query_string: str, root_node: Any)` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L9)
- `execute_query_object(tree_sitter_module: Any, query: Any, root_node: Any)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L23)
- `get_multi_line_text(lines: list[str], start_point: tuple[int, int], end_point: tuple[int, int])` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L141)
- `get_node_text_attribute(node: Any, encoding: str)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L126)
- `get_node_text_by_bytes(node: Any, source_code: str, encoding: str)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L114)
- `get_node_text_by_points(node: Any, source_code: str)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L158)
- `get_node_text_compat(node: Any, source_code: str, encoding: str)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L172)
- `get_single_line_text(line: str, start_column: int, end_column: int)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L135)
- `old_api_capture_from_item(item: Any)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L82)
- `old_api_captures_from_result(query_result: Any)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L90)

## Module values
- `logger` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/_tree_sitter_compat_helpers.py#L6)

