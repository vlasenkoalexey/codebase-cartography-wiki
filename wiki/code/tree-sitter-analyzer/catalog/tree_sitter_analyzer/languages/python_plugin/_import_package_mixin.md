---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._import_package_mixin`/
symbols:
  PythonImportPackageMixin.extract_imports: PythonImportPackageMixin#extract_imports().
  PythonImportPackageMixin._extract_import_info: PythonImportPackageMixin#_extract_import_info().
  PythonImportPackageMixin._extract_variable_info: PythonImportPackageMixin#_extract_variable_info().
  PythonImportPackageMixin.current_module: PythonImportPackageMixin#current_module.
  PythonImportPackageMixin._walk_import_nodes: PythonImportPackageMixin#_walk_import_nodes().
  PythonImportPackageMixin._extract_imports_manual: PythonImportPackageMixin#_extract_imports_manual().
  PythonImportPackageMixin._parse_import_node: PythonImportPackageMixin#_parse_import_node().
  PythonImportPackageMixin: PythonImportPackageMixin#
  _clean_import_name_fallback: _clean_import_name_fallback().
  PythonImportPackageMixin.extract_packages: PythonImportPackageMixin#extract_packages().
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py)

## Classes
### `PythonImportPackageMixin`
- def: [`tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py#L20)
- signature: `class PythonImportPackageMixin:`
- members:
  - `_extract_import_info(self, node: Any, source_code: str, import_type: str)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py#L147) — Extract detailed import information from AST node.
  - `_extract_imports_manual(self, root_node: Any, source_code: str)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py#L45) — Manual import extraction for tree-sitter 0.25.x compatibility.
  - `_extract_variable_info(self, node: Any, source_code: str, assignment_type: str)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py#L112) — Extract detailed variable information from AST node.
  - `_parse_import_node(self, node: Any, source_code: str, imports: list[Import])` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py#L64) — Parse a single import_statement or import_from_statement node.
  - `_walk_import_nodes(self, node: Any, source_code: str, imports: list[Import])` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py#L51) — Recursively walk AST to extract import nodes.
  - `extract_imports(self, tree: Any, source_code: str)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py#L21) — Extract Python import statements.
  - `extract_packages(self, tree: Any, source_code: str)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py#L75) — Extract Python package information from file path.
  - `current_module` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py#L99)
- uses (calls/refs, reference-scoped): [`name`](../../models/base.md#CodeElement.name), [`start_line`](../../models/base.md#CodeElement.start_line), [`end_line`](../../models/base.md#CodeElement.end_line), [`log_debug`](../../utils/logging.md#log_debug), [`language`](../../models/base.md#CodeElement.language), [`raw_text`](../../models/base.md#CodeElement.raw_text), [`Variable`](../../models/base.md#Variable), [`Import`](../../models/base.md#Import), [`log_warning`](../../utils/logging.md#log_warning), [`PythonElementExtractor`](extractor.md#PythonElementExtractor), [`get_node_text_safe`](../../utils/tree_sitter_compat.md#get_node_text_safe), [`Package`](../../models/base.md#Package), [`variable_type`](../../models/base.md#Variable.variable_type), [`module_name`](../../models/base.md#Import.module_name), [`extract_imports_from_tree`](_import_helpers.md#extract_imports_from_tree), [`import_node_context`](_import_helpers.md#import_node_context), [`imported_names`](../../models/base.md#Import.imported_names), [`ImportExtractionRuntime`](_import_helpers.md#ImportExtractionRuntime), [`tree`](_import_helpers.md#ImportExtractionRuntime.tree), [`extract_imports_manual`](_import_helpers.md#ImportExtractionRuntime.extract_imports_manual), [`node_raw_text`](_element_builders.md#node_raw_text), [`source_code`](_import_helpers.md#ImportExtractionRuntime.source_code), [`extract_import_info`](_import_helpers.md#ImportExtractionRuntime.extract_import_info), [`parse_from_import_parts`](_import_helpers.md#parse_from_import_parts), [`import_query`](_import_helpers.md#ImportExtractionRuntime.import_query), [`log_debug_fn`](_import_helpers.md#ImportExtractionRuntime.log_debug_fn), [`log_warning_fn`](_import_helpers.md#ImportExtractionRuntime.log_warning_fn), [`_clean_import_name_fallback`](_import_package_mixin.md#_clean_import_name_fallback)
- used by: [`PythonElementExtractor`](extractor.md#PythonElementExtractor)  (3 test-only)

## Functions
- `_clean_import_name_fallback(text: str)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_import_package_mixin.py#L212) — Strip parens, newlines, and trailing comments from an import literal.

