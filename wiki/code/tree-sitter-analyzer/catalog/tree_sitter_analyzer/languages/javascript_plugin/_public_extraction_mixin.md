---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._public_extraction_mixin`/JavaScriptPublicExtractionMixin#
symbols:
  JavaScriptPublicExtractionMixin.extract_classes: extract_classes().
  JavaScriptPublicExtractionMixin._extract_prototype_classes: _extract_prototype_classes().
  JavaScriptPublicExtractionMixin.extract_elements: extract_elements().
  JavaScriptPublicExtractionMixin.extract_variables: extract_variables().
  JavaScriptPublicExtractionMixin.extract_imports: extract_imports().
  JavaScriptPublicExtractionMixin.content_lines: content_lines.
  JavaScriptPublicExtractionMixin.extract_functions: extract_functions().
  JavaScriptPublicExtractionMixin.extract_exports: extract_exports().
  JavaScriptPublicExtractionMixin: ''
  JavaScriptPublicExtractionMixin.source_code: source_code.
  JavaScriptPublicExtractionMixin._extract_prototype_methods: _extract_prototype_methods().
  JavaScriptPublicExtractionMixin.exports: exports.
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py)

## Classes
### `JavaScriptPublicExtractionMixin`
- def: [`tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L14)
- doc: Public JavaScript extraction entry points.
- signature: `class JavaScriptPublicExtractionMixin:`
- members:
  - `_extract_prototype_classes(self, root_node: tree_sitter.Node)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L110) — Synthesise Class objects from X.prototype.m assignments.
  - `_extract_prototype_methods(self, root_node: tree_sitter.Node)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L54) — Walk top-level expression statements for X.prototype.m = function(){}.
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L79) — Extract JavaScript class definitions with detailed information.
  - `extract_elements(self, tree: tree_sitter.Tree, source_code: str)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L242) — Extract elements from source code using tree-sitter AST.
  - `extract_exports(self, tree: tree_sitter.Tree, source_code: str)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L221) — Extract JavaScript export statements.
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L18) — Extract JavaScript function definitions with comprehensive details.
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L199) — Extract JavaScript import statements with ES6+ support.
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L172) — Extract JavaScript variable definitions with modern syntax support.
  - `content_lines` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L23)
  - `exports` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L237)
  - `source_code` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_public_extraction_mixin.py#L22)
- uses (calls/refs, reference-scoped): [`name`](../../models/base.md#CodeElement.name), [`start_line`](../../models/base.md#CodeElement.start_line), [`end_line`](../../models/base.md#CodeElement.end_line), [`log_debug`](../../utils/logging.md#log_debug), [`language`](../../models/base.md#CodeElement.language), [`Function`](../../models/base.md#Function), [`raw_text`](../../models/base.md#CodeElement.raw_text), [`log_error`](../../utils/logging.md#log_error), [`Class`](../../models/base.md#Class), [`Variable`](../../models/base.md#Variable), [`Import`](../../models/base.md#Import), [`CodeElement`](../../models/base.md#CodeElement), [`class_type`](../../models/base.md#Class.class_type), [`JavaScriptElementExtractor`](extractor.md#JavaScriptElementExtractor)
- used by: [`JavaScriptElementExtractor`](extractor.md#JavaScriptElementExtractor), [`TREE_SITTER_AVAILABLE`](extractor.md#TREE_SITTER_AVAILABLE), [`extract_elements`](plugin.md#JavaScriptPlugin.extract_elements)  (7 test-only)

