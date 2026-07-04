---
title: 'Module: tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.typescript_plugin._class_helpers`/
symbols:
  extract_class: extract_class().
  extract_interface: extract_interface().
  extract_namespace: extract_namespace().
  extract_type_alias: extract_type_alias().
  extract_enum: extract_enum().
  _parse_class_parts: _parse_class_parts().
  _parse_interface_parts: _parse_interface_parts().
  TextExtractor.TextExtractor: TextExtractor.TextExtractor.
  _ClassParts.name: _ClassParts#name.
  GenericsExtractor.GenericsExtractor: GenericsExtractor.GenericsExtractor.
  TsdocExtractor.TsdocExtractor: TsdocExtractor.TsdocExtractor.
  ExportPredicate.ExportPredicate: ExportPredicate.ExportPredicate.
  _InterfaceParts.name: _InterfaceParts#name.
  _ClassParts.is_abstract: _ClassParts#is_abstract.
  _ClassParts: _ClassParts#
  _ClassParts.superclass: _ClassParts#superclass.
  _ClassParts.interfaces: _ClassParts#interfaces.
  _InterfaceParts: _InterfaceParts#
  _InterfaceParts.interfaces: _InterfaceParts#interfaces.
  _extract_preceding_decorator_names: _extract_preceding_decorator_names().
  _extract_decorator_names: _extract_decorator_names().
  _parse_class_heritage: _parse_class_heritage().
  _parse_extends_clause: _parse_extends_clause().
  ComponentPredicate.ComponentPredicate: ComponentPredicate.ComponentPredicate.
---
# Module: [`tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py)

## Classes
### `_ClassParts`
- def: [`tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L25)
- signature: `class _ClassParts:`
- members:
  - `interfaces` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L28)
  - `is_abstract` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L29)
  - `name` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L26)
  - `superclass` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L27)
- used by: [`extract_class`](_class_helpers.md#extract_class), [`_parse_class_parts`](_class_helpers.md#_parse_class_parts)

### `_InterfaceParts`
- def: [`tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L33)
- signature: `class _InterfaceParts:`
- members:
  - `interfaces` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L35)
  - `name` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L34)
- used by: [`extract_interface`](_class_helpers.md#extract_interface), [`_parse_interface_parts`](_class_helpers.md#_parse_interface_parts)

## Functions
- `_extract_decorator_names(node: tree_sitter.Node)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L38) — Return decorator names (without '@') from direct decorator children of *node*.
- `_extract_preceding_decorator_names(node: tree_sitter.Node)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L71) — Return decorator names that appear as siblings immediately before *node*.
- `_parse_class_heritage(heritage_text: str)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L348)
- `_parse_class_parts(node: tree_sitter.Node, get_node_text: TextExtractor, extract_generics: GenericsExtractor)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L310)
- `_parse_extends_clause(extends_text: str)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L362)
- `_parse_interface_parts(node: tree_sitter.Node, get_node_text: TextExtractor, extract_generics: GenericsExtractor)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L330)
- `extract_class(node: tree_sitter.Node, get_node_text: TextExtractor, extract_generics: GenericsExtractor, extract_tsdoc: TsdocExtractor, is_framework_component: ComponentPredicate, is_exported_class: ExportPredicate, framework_type: str)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L118) — Extract class information with detailed metadata. — documented in [tree_sitter_analyzer-utils-logging](../../../../concepts/tree_sitter_analyzer-utils-logging.md)
- `extract_enum(node: tree_sitter.Node, get_node_text: TextExtractor, extract_tsdoc: TsdocExtractor, is_exported_class: ExportPredicate, framework_type: str)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L230) — Extract enum information.
- `extract_interface(node: tree_sitter.Node, get_node_text: TextExtractor, extract_generics: GenericsExtractor, extract_tsdoc: TsdocExtractor, is_exported_class: ExportPredicate, framework_type: str)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L157) — Extract interface information. — documented in [tree_sitter_analyzer-utils-logging](../../../../concepts/tree_sitter_analyzer-utils-logging.md)
- `extract_namespace(node: tree_sitter.Node, get_node_text: TextExtractor, extract_tsdoc: TsdocExtractor, is_exported_class: ExportPredicate, framework_type: str)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L266) — Extract a ``namespace X { ... }`` / ``module Y { ... }`` container.
- `extract_type_alias(node: tree_sitter.Node, get_node_text: TextExtractor, extract_generics: GenericsExtractor, extract_tsdoc: TsdocExtractor, is_exported_class: ExportPredicate, framework_type: str)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L191) — Extract type alias information.

## Module values
- `ComponentPredicate` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L20)
- `ExportPredicate` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L21)
- `GenericsExtractor` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L18)
- `TextExtractor` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L17)
- `TsdocExtractor` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_class_helpers.py#L19)

