---
title: 'Module: tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.sql_plugin._procedure_extractor_helpers`/
symbols:
  _append_fallback_procedure: _append_fallback_procedure().
  _append_source_procedure: _append_source_procedure().
  append_source_procedures: append_source_procedures().
  append_tree_sitter_procedures: append_tree_sitter_procedures().
  PROCEDURE_PATTERN: PROCEDURE_PATTERN.
  _is_create_procedure_line: _is_create_procedure_line().
  _find_procedure_end_line: _find_procedure_end_line().
  _has_create_procedure: _has_create_procedure().
  _already_extracted: _already_extracted().
---
# Module: [`tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py)

## Functions
- `_already_extracted(proc_name: str, sql_elements: list[Any])` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py#L158)
- `_append_fallback_procedure(node: Any, node_text: str, match: re.Match[str], sql_elements: list[Any], traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], extract_parameters: Callable[[str, list[SQLParameter]], None], extract_dependencies: Callable[..., None])` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py#L122)
- `_append_source_procedure(proc_name: str, start_line: int, end_line: int, lines: list[str], sql_elements: list[Any], extract_parameters: Callable[[str, list[SQLParameter]], None])` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py#L89)
- `_find_procedure_end_line(lines: list[str], start_index: int)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py#L80)
- `_has_create_procedure(node: Any, node_text: str)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py#L117)
- `_is_create_procedure_line(line: str)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py#L75)
- `append_source_procedures(source_code: str, sql_elements: list[Any], extract_parameters: Callable[[str, list[SQLParameter]], None])` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py#L16) — Append procedures found by scanning source lines.
- `append_tree_sitter_procedures(root_node: Any, traverse_nodes: Callable[..., Iterator[Any]], get_node_text: Callable[..., str], sql_elements: list[Any], extract_parameters: Callable[[str, list[SQLParameter]], None], extract_dependencies: Callable[..., None])` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py#L41) — Append procedures found in tree-sitter ERROR fallback nodes.

## Module values
- `PROCEDURE_PATTERN` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/sql_plugin/_procedure_extractor_helpers.py#L10)

