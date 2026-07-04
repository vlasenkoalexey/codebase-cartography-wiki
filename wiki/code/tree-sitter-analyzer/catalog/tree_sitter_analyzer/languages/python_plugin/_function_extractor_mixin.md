---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._function_extractor_mixin`/
symbols:
  PythonFunctionExtractionMixin._extract_function_optimized: PythonFunctionExtractionMixin#_extract_function_optimized().
  PythonFunctionExtractionMixin._extract_detailed_function_info: PythonFunctionExtractionMixin#_extract_detailed_function_info().
  PythonFunctionExtractionMixin.content_lines: PythonFunctionExtractionMixin#content_lines.
  PythonFunctionExtractionMixin.extract_functions: PythonFunctionExtractionMixin#extract_functions().
  PythonFunctionExtractionMixin._parse_function_signature_optimized: PythonFunctionExtractionMixin#_parse_function_signature_optimized().
  PythonFunctionExtractionMixin._extract_docstring_from_node: PythonFunctionExtractionMixin#_extract_docstring_from_node().
  PythonFunctionExtractionMixin: PythonFunctionExtractionMixin#
  PythonFunctionExtractionMixin._extract_return_type_from_node: PythonFunctionExtractionMixin#_extract_return_type_from_node().
  _python_parent_class_name: _python_parent_class_name().
  _is_python_constructor: _is_python_constructor().
  _CLASS_BODY_TRAVERSABLE: _CLASS_BODY_TRAVERSABLE.
  PythonFunctionExtractionMixin.source_code: PythonFunctionExtractionMixin#source_code.
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py)

## Classes
### `PythonFunctionExtractionMixin`
- def: [`tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py:91`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L91)
- signature: `class PythonFunctionExtractionMixin:`
- members:
  - `_extract_detailed_function_info(self, node: Any, source_code: str, is_async: bool = False)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L176) — Extract comprehensive function information from AST node.
  - `_extract_docstring_from_node(self, node: Any, source_code: str)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L233) — Extract docstring from function/class node.
  - `_extract_function_optimized(self, node: Any)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L116) — Extract function information with detailed metadata.
  - `_extract_return_type_from_node(self, node: Any, source_code: str)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L206) — Extract return type annotation from function node.
  - `_parse_function_signature_optimized(self, node: Any)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L153) — Parse function signature for Python functions.
  - `extract_functions(self, tree: Any, source_code: str)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L92) — Extract Python function definitions with comprehensive details.
  - `content_lines` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L95)
  - `source_code` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L94)
- uses (calls/refs, reference-scoped): [`log_debug`](../../utils/logging.md#log_debug), [`Function`](../../models/base.md#Function), [`log_error`](../../utils/logging.md#log_error), [`log_warning`](../../utils/logging.md#log_warning), [`build_function_element`](_element_builders.md#build_function_element), [`PythonElementExtractor`](extractor.md#PythonElementExtractor), [`get_node_text_safe`](../../utils/tree_sitter_compat.md#get_node_text_safe), [`build_detailed_function_element`](_element_builders.md#build_detailed_function_element), [`_parse_function_signature_children`](_signature_helpers.md#_parse_function_signature_children), [`node_raw_text`](_element_builders.md#node_raw_text), [`decorators`](_element_builders.md#FunctionBuildInput.decorators), [`node_line_range`](_element_builders.md#node_line_range), [`_extract_decorated_function_decorators`](_signature_helpers.md#_extract_decorated_function_decorators), [`_return_type_from_signature_text`](_signature_helpers.md#_return_type_from_signature_text), [`DetailedFunctionBuildInput`](_element_builders.md#DetailedFunctionBuildInput), [`FunctionBuildInput`](_element_builders.md#FunctionBuildInput), [`decorators`](_element_builders.md#DetailedFunctionBuildInput.decorators), [`_python_parent_class_name`](_function_extractor_mixin.md#_python_parent_class_name), [`_strip_docstring_quotes`](_signature_helpers.md#_strip_docstring_quotes), [`function_raw_text`](_element_builders.md#function_raw_text), [`name`](_element_builders.md#DetailedFunctionBuildInput.name), [`name`](_element_builders.md#FunctionBuildInput.name), [`raw_text`](_element_builders.md#FunctionBuildInput.raw_text), [`complexity_score`](_element_builders.md#FunctionBuildInput.complexity_score), [`docstring`](_element_builders.md#FunctionBuildInput.docstring), [`end_line`](_element_builders.md#DetailedFunctionBuildInput.end_line), [`end_line`](_element_builders.md#FunctionBuildInput.end_line), [`framework_type`](_element_builders.md#FunctionBuildInput.framework_type), [`is_async`](_element_builders.md#FunctionBuildInput.is_async), [`is_constructor`](_element_builders.md#FunctionBuildInput.is_constructor), [`is_method`](_element_builders.md#FunctionBuildInput.is_method), [`parameters`](_element_builders.md#DetailedFunctionBuildInput.parameters), [`parameters`](_element_builders.md#FunctionBuildInput.parameters), [`parent_class`](_element_builders.md#FunctionBuildInput.parent_class), [`raw_text`](_element_builders.md#DetailedFunctionBuildInput.raw_text), [`return_type`](_element_builders.md#DetailedFunctionBuildInput.return_type), [`return_type`](_element_builders.md#FunctionBuildInput.return_type), [`start_line`](_element_builders.md#DetailedFunctionBuildInput.start_line), [`start_line`](_element_builders.md#FunctionBuildInput.start_line), [`_is_python_constructor`](_function_extractor_mixin.md#_is_python_constructor)
- used by: [`PythonElementExtractor`](extractor.md#PythonElementExtractor)  (12 test-only)

## Functions
- `_is_python_constructor(name: str, node: Any)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L26) — Return True when ``name`` is ``__init__`` and the node lives inside a class body.
- `_python_parent_class_name(node: Any)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L63) — Return the enclosing class name when ``node`` is a class method, else None.

## Module values
- `_CLASS_BODY_TRAVERSABLE` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.py#L47)

