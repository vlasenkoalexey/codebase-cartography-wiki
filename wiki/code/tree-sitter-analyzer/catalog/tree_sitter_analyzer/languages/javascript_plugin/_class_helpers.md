---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._class_helpers`/
symbols:
  extract_class: extract_class().
  _parse_class_parts: _parse_class_parts().
  _ClassParts.name: _ClassParts#name.
  _ClassParts: _ClassParts#
  _ClassParts.superclass: _ClassParts#superclass.
  TextExtractor.TextExtractor: TextExtractor.TextExtractor.
  _class_superclass: _class_superclass().
  JsdocExtractor.JsdocExtractor: JsdocExtractor.JsdocExtractor.
  ComponentPredicate.ComponentPredicate: ComponentPredicate.ComponentPredicate.
  ExportPredicate.ExportPredicate: ExportPredicate.ExportPredicate.
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py)

## Classes
### `_ClassParts`
- def: [`tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py#L24)
- signature: `class _ClassParts:`
- members:
  - `name` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py#L25)
  - `superclass` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py#L26)
- used by: [`extract_class`](_class_helpers.md#extract_class), [`_parse_class_parts`](_class_helpers.md#_parse_class_parts)

## Functions
- `_class_superclass(heritage_text: str)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py#L76)
- `_parse_class_parts(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py#L63)
- `extract_class(node: tree_sitter.Node, get_node_text: TextExtractor, extract_jsdoc: JsdocExtractor, is_react_component: ComponentPredicate, is_exported_class: ExportPredicate, framework_type: str)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py#L29) — Extract class information with detailed metadata.

## Module values
- `ComponentPredicate` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py#L19)
- `ExportPredicate` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py#L20)
- `JsdocExtractor` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py#L18)
- `TextExtractor` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_class_helpers.py#L17)

