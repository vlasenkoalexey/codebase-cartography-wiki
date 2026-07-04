---
title: 'Module: tree_sitter_analyzer/languages/_go_import_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/_go_import_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages._go_import_helpers`/
symbols:
  _build_go_import: _build_go_import().
  extract_import_spec: extract_import_spec().
  _extract_import_declaration: _extract_import_declaration().
  extract_imports_from_tree: extract_imports_from_tree().
  _extract_import_parts: _extract_import_parts().
  _iter_import_specs: _iter_import_specs().
---
# Module: [`tree_sitter_analyzer/languages/_go_import_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_import_helpers.py)

## Functions
- `_build_go_import(node: Any, get_node_text: Callable[..., str], alias: str | None, path: str)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_import_helpers.py#L43)
- `_extract_import_declaration(node: Any, get_node_text: Callable[..., str])` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_import_helpers.py#L86) — Extract import declaration (may contain multiple imports).
- `_extract_import_parts(node: Any, get_node_text: Callable[..., str])` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_import_helpers.py#L63)
- `_iter_import_specs(node: Any)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_import_helpers.py#L102)
- `extract_import_spec(node: Any, get_node_text: Callable[..., str])` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_import_helpers.py#L27) — Extract single import spec.
- `extract_imports_from_tree(tree: Any, source_code: str, get_node_text: Callable[..., str])` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/_go_import_helpers.py#L10) — Extract Go import declarations.

