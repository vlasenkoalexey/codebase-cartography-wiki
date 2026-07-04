---
title: 'Module: tree_sitter_analyzer/languages/_java_import_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_java_import_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._java_import_helpers`/
symbols:
  _build_import: _build_import().
  _extract_package_element: _extract_package_element().
  extract_java_imports: extract_java_imports().
  _extract_import_info: _extract_import_info().
  extract_java_packages: extract_java_packages().
  _extract_import_from_text: _extract_import_from_text().
  _extract_package_name: _extract_package_name().
  _extract_imports_fallback: _extract_imports_fallback().
  _extract_static_import: _extract_static_import().
  _extract_regular_import: _extract_regular_import().
  extract_java_packages.find_packages: extract_java_packages().find_packages().
  _extract_import_from_line: _extract_import_from_line().
  _normalize_static_import_name: _normalize_static_import_name().
  _normalize_regular_import_name: _normalize_regular_import_name().
---
# Module: [`tree_sitter_analyzer/languages/_java_import_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py)

## Functions
- `_build_import(import_name: str, line_num: int, raw_text: str, import_statement: str, *, is_static: bool)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L192)
- `_extract_import_from_line(line: str, line_num: int)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L131)
- `_extract_import_from_text(import_text: str, line_num: int, raw_text: str)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L139)
- `_extract_import_info(node: Any, get_node_text: Callable[..., str])` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L105) — Extract import information from import declaration node.
- `_extract_imports_fallback(source_code: str)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L119) — Fallback import extraction using regex.
- `_extract_package_element(node: Any, get_node_text: Callable[..., str])` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L82) — Extract package as a Package model element.
- `_extract_package_name(node: Any, get_node_text: Callable[..., str])` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L65) — Extract package name from a package declaration node.
- `_extract_regular_import(import_text: str, line_num: int, raw_text: str)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L161)
- `_extract_static_import(import_text: str, line_num: int, raw_text: str)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L149)
- `_normalize_regular_import_name(import_name: str, import_text: str)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L182)
- `_normalize_static_import_name(import_name: str, import_text: str)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L173)
- `extract_java_imports(tree: Any, source_code: str, get_node_text: Callable[..., str], set_package: Callable[[str], None])` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L11) — Extract Java import statements.
- `extract_java_packages(tree: Any, get_node_text: Callable[..., str])` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L44) — Extract Java package declarations.
- `find_packages(node: Any)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_java_import_helpers.py#L51)

