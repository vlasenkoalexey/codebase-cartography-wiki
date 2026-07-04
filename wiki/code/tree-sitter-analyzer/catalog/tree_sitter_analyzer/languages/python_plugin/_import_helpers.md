---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_import_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_import_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._import_helpers`/
symbols:
  parse_simple_import: parse_simple_import().
  parse_from_import: parse_from_import().
  _query_imports: _query_imports().
  extract_imports_from_tree: extract_imports_from_tree().
  import_node_context: import_node_context().
  query_class_body_nodes: query_class_body_nodes().
  _query_class_body_nodes: _query_class_body_nodes().
  ImportNodeContext: ImportNodeContext#
  _extend_imports_from_captures: _extend_imports_from_captures().
  _node_source_text: _node_source_text().
  ImportExtractionRuntime: ImportExtractionRuntime#
  ImportExtractionRuntime.tree: ImportExtractionRuntime#tree.
  ImportExtractionRuntime.extract_imports_manual: ImportExtractionRuntime#extract_imports_manual.
  _split_from_import_with_keyword: _split_from_import_with_keyword().
  _split_from_import_without_keyword: _split_from_import_without_keyword().
  ClassBodyQueryRuntime: ClassBodyQueryRuntime#
  ImportExtractionRuntime.source_code: ImportExtractionRuntime#source_code.
  _parse_from_import_parts: _parse_from_import_parts().
  _collect_import_list_items: _collect_import_list_items().
  ImportExtractionRuntime.extract_import_info: ImportExtractionRuntime#extract_import_info.
  ClassBodyQueryRuntime.tree: ClassBodyQueryRuntime#tree.
  parse_from_import_parts: parse_from_import_parts().
  _bound_name_from_aliased_import: _bound_name_from_aliased_import().
  ImportNodeContext.raw_text: ImportNodeContext#raw_text.
  ImportExtractionRuntime.import_query: ImportExtractionRuntime#import_query.
  ImportExtractionRuntime.log_debug_fn: ImportExtractionRuntime#log_debug_fn.
  ImportExtractionRuntime.log_warning_fn: ImportExtractionRuntime#log_warning_fn.
  ClassBodyQueryRuntime.class_query: ClassBodyQueryRuntime#class_query.
  ClassBodyQueryRuntime.log_debug_fn: ClassBodyQueryRuntime#log_debug_fn.
  ClassBodyQueryRuntime.log_warning_fn: ClassBodyQueryRuntime#log_warning_fn.
  ImportNodeContext.start_line: ImportNodeContext#start_line.
  ImportNodeContext.end_line: ImportNodeContext#end_line.
  ImportNodeContext.source_code: ImportNodeContext#source_code.
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_import_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py)

## Classes
### `ClassBodyQueryRuntime`
- def: [`tree_sitter_analyzer/languages/python_plugin/_import_helpers.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L25)
- signature: `class ClassBodyQueryRuntime:`
- members:
  - `class_query` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L27)
  - `log_debug_fn` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L28)
  - `log_warning_fn` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L29)
  - `tree` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L26)
- used by: [`extract_variables`](_class_extractor_mixin.md#PythonClassExtractionMixin.extract_variables), [`_query_class_body_nodes`](_import_helpers.md#_query_class_body_nodes), [`query_class_body_nodes`](_import_helpers.md#query_class_body_nodes)  (2 test-only)

### `ImportExtractionRuntime`
- def: [`tree_sitter_analyzer/languages/python_plugin/_import_helpers.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L14)
- signature: `class ImportExtractionRuntime:`
- members:
  - `extract_import_info` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L18)
  - `extract_imports_manual` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L19)
  - `import_query` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L17)
  - `log_debug_fn` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L20)
  - `log_warning_fn` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L21)
  - `source_code` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L16)
  - `tree` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L15)
- uses (calls/refs, reference-scoped): [`Import`](../../models/base.md#Import)
- used by: [`extract_imports`](_import_package_mixin.md#PythonImportPackageMixin.extract_imports), [`_query_imports`](_import_helpers.md#_query_imports), [`extract_imports_from_tree`](_import_helpers.md#extract_imports_from_tree), [`_extend_imports_from_captures`](_import_helpers.md#_extend_imports_from_captures)  (2 test-only)

### `ImportNodeContext`
- def: [`tree_sitter_analyzer/languages/python_plugin/_import_helpers.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L33)
- signature: `class ImportNodeContext:`
- members:
  - `end_line` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L36)
  - `raw_text` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L37)
  - `source_code` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L34)
  - `start_line` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L35)
- used by: [`parse_simple_import`](_import_helpers.md#parse_simple_import), [`parse_from_import`](_import_helpers.md#parse_from_import), [`import_node_context`](_import_helpers.md#import_node_context)  (10 test-only)

## Functions
- `_bound_name_from_aliased_import(node: Any, source_code: str)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L195) — Return the locally bound identifier for an ``aliased_import`` node.
- `_collect_import_list_items(import_list_node: Any, source_code: str)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L217)
- `_extend_imports_from_captures(runtime: ImportExtractionRuntime, captures: Any, imports: list[Import])` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L312)
- `_node_source_text(node: Any, source_code: str)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L233)
- `_parse_from_import_parts(node: Any, source_code: str)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L114) — Pick apart a ``from X import (A, B as b, C)`` statement node.
- `_query_class_body_nodes(runtime: ClassBodyQueryRuntime, language: Any)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L252)
- `_query_imports(runtime: ImportExtractionRuntime, language: Any)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L284)
- `_split_from_import_with_keyword(children: list[Any], source_code: str)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L136)
- `_split_from_import_without_keyword(children: list[Any], source_code: str)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L169) — Legacy heuristic: first ``dotted_name`` is the module, rest are imports.
- `extract_imports_from_tree(runtime: ImportExtractionRuntime)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L268)
- `import_node_context(node: Any, source_code: str)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L40)
- `parse_from_import(node: Any, context: ImportNodeContext, imports: list[Import])` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L78) — Handle: from abc import ABC, abstractmethod.
- `parse_from_import_parts(node: Any, source_code: str)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L103) — Public alias for :func:`_parse_from_import_parts` (J6).
- `parse_simple_import(node: Any, context: ImportNodeContext, imports: list[Import])` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L56) — Handle: import os, sys, json.
- `query_class_body_nodes(runtime: ClassBodyQueryRuntime)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_helpers.py#L241)

