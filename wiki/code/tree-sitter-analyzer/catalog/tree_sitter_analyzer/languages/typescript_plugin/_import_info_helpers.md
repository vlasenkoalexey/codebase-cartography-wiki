---
title: 'Module: tree_sitter_analyzer/languages/typescript_plugin/_import_info_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/typescript_plugin/_import_info_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.typescript_plugin._import_info_helpers`/
symbols:
  extract_import_info_simple: extract_import_info_simple().
  _import_parts: _import_parts().
  _module_path_from_child: _module_path_from_child().
  TextExtractor.TextExtractor: TextExtractor.TextExtractor.
  ImportNameExtractor.ImportNameExtractor: ImportNameExtractor.ImportNameExtractor.
  _line_span: _line_span().
---
# Module: [`tree_sitter_analyzer/languages/typescript_plugin/_import_info_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_import_info_helpers.py)

## Functions
- `_import_parts(node: tree_sitter.Node, get_node_text: TextExtractor, extract_import_names: ImportNameExtractor)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_import_info_helpers.py#L59)
- `_line_span(node: tree_sitter.Node)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_import_info_helpers.py#L51)
- `_module_path_from_child(child: tree_sitter.Node, get_node_text: TextExtractor)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_import_info_helpers.py#L77)
- `extract_import_info_simple(node: tree_sitter.Node, get_node_text: TextExtractor, extract_import_names: ImportNameExtractor)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_import_info_helpers.py#L19) — Extract import information from an import_statement node.

## Module values
- `ImportNameExtractor` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_import_info_helpers.py#L16)
- `TextExtractor` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_import_info_helpers.py#L15)

