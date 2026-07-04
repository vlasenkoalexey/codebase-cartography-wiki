---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_element_builders.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_element_builders.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._element_builders`/
symbols:
  build_function_element: build_function_element().
  build_class_element: build_class_element().
  build_detailed_function_element: build_detailed_function_element().
  _build_module_constant: _build_module_constant().
  extract_class_attribute_info: extract_class_attribute_info().
  extract_module_constants: extract_module_constants().
  ClassBuildInput.superclasses: ClassBuildInput#superclasses.
  node_raw_text: node_raw_text().
  ClassBuildInput: ClassBuildInput#
  node_line_range: node_line_range().
  FunctionBuildInput.decorators: FunctionBuildInput#decorators.
  ClassBuildInput.name: ClassBuildInput#name.
  ClassBuildInput.raw_text: ClassBuildInput#raw_text.
  ClassBuildInput.decorators: ClassBuildInput#decorators.
  ClassBuildInput.current_module: ClassBuildInput#current_module.
  FunctionBuildInput: FunctionBuildInput#
  DetailedFunctionBuildInput: DetailedFunctionBuildInput#
  DetailedFunctionBuildInput.decorators: DetailedFunctionBuildInput#decorators.
  ClassBuildInput.start_line: ClassBuildInput#start_line.
  ClassBuildInput.end_line: ClassBuildInput#end_line.
  ClassBuildInput.docstring: ClassBuildInput#docstring.
  ClassBuildInput.framework_type: ClassBuildInput#framework_type.
  function_raw_text: function_raw_text().
  FunctionBuildInput.name: FunctionBuildInput#name.
  FunctionBuildInput.raw_text: FunctionBuildInput#raw_text.
  _function_visibility: _function_visibility().
  DetailedFunctionBuildInput.name: DetailedFunctionBuildInput#name.
  FunctionBuildInput.start_line: FunctionBuildInput#start_line.
  FunctionBuildInput.end_line: FunctionBuildInput#end_line.
  FunctionBuildInput.parameters: FunctionBuildInput#parameters.
  FunctionBuildInput.return_type: FunctionBuildInput#return_type.
  FunctionBuildInput.is_async: FunctionBuildInput#is_async.
  FunctionBuildInput.docstring: FunctionBuildInput#docstring.
  FunctionBuildInput.complexity_score: FunctionBuildInput#complexity_score.
  FunctionBuildInput.framework_type: FunctionBuildInput#framework_type.
  FunctionBuildInput.is_constructor: FunctionBuildInput#is_constructor.
  FunctionBuildInput.is_method: FunctionBuildInput#is_method.
  FunctionBuildInput.parent_class: FunctionBuildInput#parent_class.
  DetailedFunctionBuildInput.start_line: DetailedFunctionBuildInput#start_line.
  DetailedFunctionBuildInput.end_line: DetailedFunctionBuildInput#end_line.
  DetailedFunctionBuildInput.raw_text: DetailedFunctionBuildInput#raw_text.
  DetailedFunctionBuildInput.parameters: DetailedFunctionBuildInput#parameters.
  DetailedFunctionBuildInput.return_type: DetailedFunctionBuildInput#return_type.
  _class_attribute_name_and_type: _class_attribute_name_and_type().
  _class_full_qualified_name: _class_full_qualified_name().
  _is_exception_class: _is_exception_class().
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_element_builders.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py)

## Classes
### `ClassBuildInput`
- def: [`tree_sitter_analyzer/languages/python_plugin/_element_builders.py:198`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L198)
- signature: `class ClassBuildInput:`
- members:
  - `current_module` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L206)
  - `decorators` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L204)
  - `docstring` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L205)
  - `end_line` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L201)
  - `framework_type` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L207)
  - `name` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L199)
  - `raw_text` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L202)
  - `start_line` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L200)
  - `superclasses` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L203)
- used by: [`build_class_element`](_element_builders.md#build_class_element), [`_extract_class_optimized`](_class_extractor_mixin.md#PythonClassExtractionMixin._extract_class_optimized)  (2 test-only)

### `DetailedFunctionBuildInput`
- def: [`tree_sitter_analyzer/languages/python_plugin/_element_builders.py:169`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L169)
- signature: `class DetailedFunctionBuildInput:`
- members:
  - `decorators` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L176)
  - `end_line` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L172)
  - `name` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L170)
  - `parameters` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L174)
  - `raw_text` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L173)
  - `return_type` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L175)
  - `start_line` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L171)
- used by: [`build_detailed_function_element`](_element_builders.md#build_detailed_function_element), [`_extract_detailed_function_info`](_function_extractor_mixin.md#PythonFunctionExtractionMixin._extract_detailed_function_info)

### `FunctionBuildInput`
- def: [`tree_sitter_analyzer/languages/python_plugin/_element_builders.py:112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L112)
- signature: `class FunctionBuildInput:`
- members:
  - `complexity_score` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L122)
  - `decorators` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L120)
  - `docstring` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L121)
  - `end_line` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L115)
  - `framework_type` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L123)
  - `is_async` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L119)
  - `is_constructor` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L124)
  - `is_method` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L125)
  - `name` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L113)
  - `parameters` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L117)
  - `parent_class` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L126)
  - `raw_text` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L116)
  - `return_type` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L118)
  - `start_line` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L114)
- used by: [`build_function_element`](_element_builders.md#build_function_element), [`_extract_function_optimized`](_function_extractor_mixin.md#PythonFunctionExtractionMixin._extract_function_optimized)

## Functions
- `_build_module_constant(node: Any, sym: dict[str, Any], source_code: str)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L93)
- `_class_attribute_name_and_type(left_part: str)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L58)
- `_class_full_qualified_name(current_module: str, class_name: str)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L236)
- `_function_visibility(name: str)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L160)
- `_is_exception_class(superclasses: list[str])` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L242)
- `build_class_element(data: ClassBuildInput)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L210) — documented in [tree_sitter_analyzer-models-base](../../../../concepts/tree_sitter_analyzer-models-base.md)
- `build_detailed_function_element(data: DetailedFunctionBuildInput)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L179) — documented in [tree_sitter_analyzer-models-base](../../../../concepts/tree_sitter_analyzer-models-base.md)
- `build_function_element(data: FunctionBuildInput)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L129) — documented in [tree_sitter_analyzer-models-base](../../../../concepts/tree_sitter_analyzer-models-base.md)
- `extract_class_attribute_info(node: Any, source_code: str)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L36) — Extract class attribute information from an assignment node.
- `extract_module_constants(tree: Any, source_code: str)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L66) — Extract module-level constants as Variable elements (issue #639).
- `function_raw_text(content_lines: list[str], start_line: int, end_line: int)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L30)
- `node_line_range(node: Any)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L13)
- `node_raw_text(node: Any, source_code: str)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_element_builders.py#L17)

