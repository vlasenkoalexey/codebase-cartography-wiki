---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._import_export_mixin`/JavaScriptImportExportMixin#
symbols:
  JavaScriptImportExportMixin._extract_import_info_simple: _extract_import_info_simple().
  JavaScriptImportExportMixin._extract_import_info_enhanced: _extract_import_info_enhanced().
  JavaScriptImportExportMixin._extract_dynamic_import: _extract_dynamic_import().
  JavaScriptImportExportMixin._extract_commonjs_requires: _extract_commonjs_requires().
  JavaScriptImportExportMixin._extract_export_info: _extract_export_info().
  JavaScriptImportExportMixin: ''
  JavaScriptImportExportMixin._extract_import_names: _extract_import_names().
  JavaScriptImportExportMixin._parse_import_statement: _parse_import_statement().
  JavaScriptImportExportMixin._parse_export_statement: _parse_export_statement().
  JavaScriptImportExportMixin._extract_commonjs_exports: _extract_commonjs_exports().
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py)

## Classes
### `JavaScriptImportExportMixin`
- def: [`tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py#L21)
- doc: Import/export-specific extraction methods.
- signature: `class JavaScriptImportExportMixin:`
- members:
  - `_extract_commonjs_exports(self, tree: tree_sitter.Tree, source_code: str)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py#L147) — Extract CommonJS module.exports statements.
  - `_extract_commonjs_requires(self, tree: tree_sitter.Tree, source_code: str)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py#L118) — Extract CommonJS require() statements.
  - `_extract_dynamic_import(self, node: tree_sitter.Node)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py#L91) — Extract dynamic import() calls.
  - `_extract_export_info(self, node: tree_sitter.Node)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py#L125) — Extract export information.
  - `_extract_import_info_enhanced(self, node: tree_sitter.Node, source_code: str)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py#L65) — Extract enhanced import information.
  - `_extract_import_info_simple(self, node: tree_sitter.Node)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py#L25) — Extract import information from import_statement node.
  - `_extract_import_names(self, import_clause_node: tree_sitter.Node)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py#L60) — Extract import names from import clause.
  - `_parse_export_statement(self, export_text: str)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py#L161) — Parse export statement to extract details.
  - `_parse_import_statement(self, import_text: str)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_import_export_mixin.py#L154) — Parse import statement to extract details.
- uses (calls/refs, reference-scoped): [`name`](../../models/base.md#CodeElement.name), [`start_line`](../../models/base.md#CodeElement.start_line), [`end_line`](../../models/base.md#CodeElement.end_line), [`log_debug`](../../utils/logging.md#log_debug), [`language`](../../models/base.md#CodeElement.language), [`raw_text`](../../models/base.md#CodeElement.raw_text), [`Import`](../../models/base.md#Import), [`JavaScriptElementExtractor`](extractor.md#JavaScriptElementExtractor), [`module_name`](../../models/base.md#Import.module_name), [`imported_names`](../../models/base.md#Import.imported_names), [`module_path`](../../models/base.md#Import.module_path), [`parse_export_statement`](_export_helpers.md#parse_export_statement), [`parse_import_statement`](_import_helpers.md#parse_import_statement), [`extract_commonjs_requires`](_import_helpers.md#extract_commonjs_requires), [`extract_commonjs_exports`](_export_helpers.md#extract_commonjs_exports), [`extract_import_names`](_import_helpers.md#extract_import_names)
- used by: [`JavaScriptElementExtractor`](extractor.md#JavaScriptElementExtractor), [`TREE_SITTER_AVAILABLE`](extractor.md#TREE_SITTER_AVAILABLE)

