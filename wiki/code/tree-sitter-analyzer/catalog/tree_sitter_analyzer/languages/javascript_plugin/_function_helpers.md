---
title: 'Module: tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.javascript_plugin._function_helpers`/
symbols:
  extract_arrow_function: extract_arrow_function().
  extract_prototype_method: extract_prototype_method().
  extract_method: extract_method().
  extract_function: extract_function().
  extract_generator_function: extract_generator_function().
  TextExtractor.TextExtractor: TextExtractor.TextExtractor.
  _arrow_parameters: _arrow_parameters().
  JsdocExtractor.JsdocExtractor: JsdocExtractor.JsdocExtractor.
  ComplexityCalculator.ComplexityCalculator: ComplexityCalculator.ComplexityCalculator.
  FunctionSignatureParser.FunctionSignatureParser: FunctionSignatureParser.FunctionSignatureParser.
  _arrow_function_name: _arrow_function_name().
  _arrow_class_field_context: _arrow_class_field_context().
  MethodSignatureParser.MethodSignatureParser: MethodSignatureParser.MethodSignatureParser.
  ParameterExtractor.ParameterExtractor: ParameterExtractor.ParameterExtractor.
  FunctionSignature: FunctionSignature.
  MethodSignature: MethodSignature.
  _raw_text_for_lines: _raw_text_for_lines().
---
# Module: [`tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py)

## Functions
- `_arrow_class_field_context(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L339`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L339) — Return (is_method, parent_class, is_static) for arrow-function class fields.
- `_arrow_function_name(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L313)
- `_arrow_parameters(node: tree_sitter.Node, get_node_text: TextExtractor, extract_parameters: ParameterExtractor)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L376)
- `_raw_text_for_lines(content_lines: list[str], start_line: int, end_line: int)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L303)
- `extract_arrow_function(node: tree_sitter.Node, get_node_text: TextExtractor, extract_parameters: ParameterExtractor, extract_jsdoc: JsdocExtractor, calculate_complexity: ComplexityCalculator, framework_type: str)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L69) — Extract arrow function information.
- `extract_function(node: tree_sitter.Node, parse_signature: FunctionSignatureParser, extract_jsdoc: JsdocExtractor, calculate_complexity: ComplexityCalculator, content_lines: list[str], framework_type: str)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L30) — Extract regular function information with detailed metadata.
- `extract_generator_function(node: tree_sitter.Node, parse_signature: FunctionSignatureParser, extract_jsdoc: JsdocExtractor, calculate_complexity: ComplexityCalculator, get_node_text: TextExtractor, framework_type: str)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L112) — Extract generator function information.
- `extract_method(node: tree_sitter.Node, parse_signature: MethodSignatureParser, extract_jsdoc: JsdocExtractor, calculate_complexity: ComplexityCalculator, get_node_text: TextExtractor, framework_type: str)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L150) — Extract method information from a class.
- `extract_prototype_method(node: tree_sitter.Node, extract_parameters: ParameterExtractor, extract_jsdoc: JsdocExtractor, calculate_complexity: ComplexityCalculator, get_node_text: TextExtractor, framework_type: str)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L198) — Extract a prototype-assignment method: ``X.prototype.m = function(){}``. — documented in [tree_sitter_analyzer-models-base](../../../../concepts/tree_sitter_analyzer-models-base.md)

## Module values
- `ComplexityCalculator` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L19)
- `FunctionSignature` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L20)
- `FunctionSignatureParser` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L21)
- `JsdocExtractor` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L18)
- `MethodSignature` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L24)
- `MethodSignatureParser` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L25)
- `ParameterExtractor` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L17)
- `TextExtractor` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/javascript_plugin/_function_helpers.py#L16)

