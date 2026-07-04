---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._function_mixin`/JavaScriptFunctionExtractionMixin#
symbols:
  JavaScriptFunctionExtractionMixin: ''
  JavaScriptFunctionExtractionMixin._extract_function_optimized: _extract_function_optimized().
  JavaScriptFunctionExtractionMixin._extract_arrow_function_optimized: _extract_arrow_function_optimized().
  JavaScriptFunctionExtractionMixin._extract_method_optimized: _extract_method_optimized().
  JavaScriptFunctionExtractionMixin._extract_generator_function_optimized: _extract_generator_function_optimized().
  JavaScriptFunctionExtractionMixin._extract_prototype_method_optimized: _extract_prototype_method_optimized().
  JavaScriptFunctionExtractionMixin._extract_parameters: _extract_parameters().
  JavaScriptFunctionExtractionMixin._parse_function_signature_optimized: _parse_function_signature_optimized().
  JavaScriptFunctionExtractionMixin._parse_method_signature_optimized: _parse_method_signature_optimized().
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py)

## Classes
### `JavaScriptFunctionExtractionMixin`
- def: [`tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py#L18)
- doc: Function-oriented extraction methods shared by JavaScript extractors.
- signature: `class JavaScriptFunctionExtractionMixin:`
- members:
  - `_extract_arrow_function_optimized(self, node: tree_sitter.Node)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py#L32) — Extract arrow function information.
  - `_extract_function_optimized(self, node: tree_sitter.Node)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py#L21) — Extract regular function information with detailed metadata.
  - `_extract_generator_function_optimized(self, node: tree_sitter.Node)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py#L56) — Extract generator function information.
  - `_extract_method_optimized(self, node: tree_sitter.Node)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py#L45) — Extract method information from class.
  - `_extract_parameters(self, params_node: tree_sitter.Node)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py#L153) — Extract function parameters.
  - `_extract_prototype_method_optimized(self, node: tree_sitter.Node)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py#L69) — Extract a prototype-assignment method: ``X.prototype.m = function(){}``.
  - `_parse_function_signature_optimized(self, node: tree_sitter.Node)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py#L82) — Parse function signature for regular functions.
  - `_parse_method_signature_optimized(self, node: tree_sitter.Node)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.py#L104) — Parse method signature for class methods.
- uses (calls/refs, reference-scoped): [`Function`](../../models/base.md#Function), [`extract_arrow_function`](_function_helpers.md#extract_arrow_function), [`extract_prototype_method`](_function_helpers.md#extract_prototype_method), [`extract_method`](_function_helpers.md#extract_method), [`extract_function`](_function_helpers.md#extract_function), [`extract_generator_function`](_function_helpers.md#extract_generator_function), [`JavaScriptElementExtractor`](extractor.md#JavaScriptElementExtractor)  (3 test-only)
- used by: [`JavaScriptElementExtractor`](extractor.md#JavaScriptElementExtractor), [`TREE_SITTER_AVAILABLE`](extractor.md#TREE_SITTER_AVAILABLE)  (6 test-only)

