---
title: 'Module: tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._cpp_import_namespace_helpers`/
symbols:
  _extract_namespace_info: _extract_namespace_info().
  _include_from_line: _include_from_line().
  _declaration_import: _declaration_import().
  extract_cpp_imports: extract_cpp_imports().
  _extract_include_info: _extract_include_info().
  _extract_includes_fallback: _extract_includes_fallback().
  _import_from_top_level_node: _import_from_top_level_node().
  extract_cpp_namespaces: extract_cpp_namespaces().
  _find_namespaces: _find_namespaces().
  _namespace_name: _namespace_name().
---
# Module: [`tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py)

## Functions
- `_declaration_import(node: Any, get_node_text: Callable[..., str])` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py#L44)
- `_extract_include_info(node: Any, source_code: str, get_node_text: Callable[..., str])` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py#L58) — Extract include directive information.
- `_extract_includes_fallback(source_code: str)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py#L73) — Fallback include extraction using regex.
- `_extract_namespace_info(node: Any, get_node_text: Callable[..., str])` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py#L130) — Extract namespace information.
- `_find_namespaces(node: Any, get_node_text: Callable[..., str], packages: list[Any])` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py#L116)
- `_import_from_top_level_node(node: Any, source_code: str, get_node_text: Callable[..., str])` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py#L32)
- `_include_from_line(line_num: int, line: str)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py#L83)
- `_namespace_name(node: Any, get_node_text: Callable[..., str])` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py#L154)
- `extract_cpp_imports(tree: Any, source_code: str, get_node_text: Callable[..., str])` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py#L11) — Extract C++ include directives and using/alias declarations.
- `extract_cpp_namespaces(tree: Any, get_node_text: Callable[..., str])` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_cpp_import_namespace_helpers.py#L105) — Extract C++ namespace declarations.

