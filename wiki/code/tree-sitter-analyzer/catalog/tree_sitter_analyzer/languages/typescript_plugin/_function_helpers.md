---
title: 'Module: tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.typescript_plugin._function_helpers`/
symbols:
  extract_method: extract_method().
  extract_arrow_function: extract_arrow_function().
  extract_abstract_method_signature: extract_abstract_method_signature().
  extract_generator_function: extract_generator_function().
  extract_function: extract_function().
  extract_method_signature: extract_method_signature().
  TextExtractor.TextExtractor: TextExtractor.TextExtractor.
  _arrow_signature_parts: _arrow_signature_parts().
  TsdocExtractor.TsdocExtractor: TsdocExtractor.TsdocExtractor.
  MethodSignatureParser.MethodSignatureParser: MethodSignatureParser.MethodSignatureParser.
  FunctionSignatureParser.FunctionSignatureParser: FunctionSignatureParser.FunctionSignatureParser.
  ComplexityCalculator.ComplexityCalculator: ComplexityCalculator.ComplexityCalculator.
  _arrow_function_name: _arrow_function_name().
  ParameterExtractor.ParameterExtractor: ParameterExtractor.ParameterExtractor.
---
# Module: [`tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py)

## Functions
- `_arrow_function_name(node: tree_sitter.Node, get_node_text: TextExtractor)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L326)
- `_arrow_signature_parts(node: tree_sitter.Node, get_node_text: TextExtractor, extract_parameters: ParameterExtractor)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L337)
- `extract_abstract_method_signature(node: tree_sitter.Node, parse_signature: MethodSignatureParser, extract_tsdoc: TsdocExtractor, get_node_text: TextExtractor, framework_type: str)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L224) — Extract abstract method signature from an abstract class.
- `extract_arrow_function(node: tree_sitter.Node, get_node_text: TextExtractor, extract_parameters: ParameterExtractor, extract_tsdoc: TsdocExtractor, calculate_complexity: ComplexityCalculator, framework_type: str)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L77) — Extract arrow function information. — documented in [tree_sitter_analyzer-models-base](../../../../concepts/tree_sitter_analyzer-models-base.md)
- `extract_function(node: tree_sitter.Node, parse_signature: FunctionSignatureParser, extract_tsdoc: TsdocExtractor, calculate_complexity: ComplexityCalculator, content_lines: list[str], framework_type: str)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L30) — Extract regular function information with detailed metadata.
- `extract_generator_function(node: tree_sitter.Node, parse_signature: FunctionSignatureParser, extract_tsdoc: TsdocExtractor, calculate_complexity: ComplexityCalculator, get_node_text: TextExtractor, framework_type: str)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L284) — Extract generator function information.
- `extract_method(node: tree_sitter.Node, parse_signature: MethodSignatureParser, extract_tsdoc: TsdocExtractor, calculate_complexity: ComplexityCalculator, get_node_text: TextExtractor, framework_type: str)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L116) — Extract method information from a class. — documented in [tree_sitter_analyzer-utils-logging](../../../../concepts/tree_sitter_analyzer-utils-logging.md)
- `extract_method_signature(node: tree_sitter.Node, parse_signature: MethodSignatureParser, extract_tsdoc: TsdocExtractor, get_node_text: TextExtractor, framework_type: str)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L172) — Extract method signature information from an interface.

## Module values
- `ComplexityCalculator` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L27)
- `FunctionSignatureParser` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L20)
- `MethodSignatureParser` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L23)
- `ParameterExtractor` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L19)
- `TextExtractor` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L18)
- `TsdocExtractor` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.py#L26)

