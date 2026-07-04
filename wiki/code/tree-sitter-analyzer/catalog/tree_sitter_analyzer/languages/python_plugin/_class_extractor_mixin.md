---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._class_extractor_mixin`/PythonClassExtractionMixin#
symbols:
  PythonClassExtractionMixin._extract_class_optimized: _extract_class_optimized().
  PythonClassExtractionMixin._extract_detailed_class_info: _extract_detailed_class_info().
  PythonClassExtractionMixin.extract_variables: extract_variables().
  PythonClassExtractionMixin.content_lines: content_lines.
  PythonClassExtractionMixin._extract_class_attributes: _extract_class_attributes().
  PythonClassExtractionMixin.source_code: source_code.
  PythonClassExtractionMixin: ''
  PythonClassExtractionMixin.extract_classes: extract_classes().
  PythonClassExtractionMixin._is_framework_class: _is_framework_class().
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py)

## Classes
### `PythonClassExtractionMixin`
- def: [`tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py#L23)
- signature: `class PythonClassExtractionMixin:`
- members:
  - `_extract_class_attributes(self, class_body_node: Any, source_code: str)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py#L131) — Extract class-level attribute assignments.
  - `_extract_class_optimized(self, node: Any)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py#L84) — Extract class information with detailed metadata.
  - `_extract_detailed_class_info(self, node: Any, source_code: str)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py#L151) — Extract comprehensive class information from AST node.
  - `_is_framework_class(self, node: Any, class_name: str)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py#L117) — Check if class is a framework-specific class.
  - `extract_classes(self, tree: Any, source_code: str)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py#L24) — Extract Python class definitions with detailed information.
  - `extract_variables(self, tree: Any, source_code: str)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py#L47) — Extract Python variables: class attributes + module constants (#639).
  - `content_lines` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py#L27)
  - `source_code` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_class_extractor_mixin.py#L26)
- uses (calls/refs, reference-scoped): [`name`](../../models/base.md#CodeElement.name), [`start_line`](../../models/base.md#CodeElement.start_line), [`end_line`](../../models/base.md#CodeElement.end_line), [`log_debug`](../../utils/logging.md#log_debug), [`language`](../../models/base.md#CodeElement.language), [`raw_text`](../../models/base.md#CodeElement.raw_text), [`Class`](../../models/base.md#Class), [`Variable`](../../models/base.md#Variable), [`log_warning`](../../utils/logging.md#log_warning), [`class_type`](../../models/base.md#Class.class_type), [`build_class_element`](_element_builders.md#build_class_element), [`PythonElementExtractor`](extractor.md#PythonElementExtractor), [`get_node_text_safe`](../../utils/tree_sitter_compat.md#get_node_text_safe), [`interfaces`](../../models/base.md#Class.interfaces), [`superclass`](../../models/base.md#Class.superclass), [`full_qualified_name`](../../models/base.md#Class.full_qualified_name), [`modifiers`](../../models/base.md#Class.modifiers), [`query_class_body_nodes`](_import_helpers.md#query_class_body_nodes), [`extract_module_constants`](_element_builders.md#extract_module_constants), [`package_name`](../../models/base.md#Class.package_name), [`superclasses`](_element_builders.md#ClassBuildInput.superclasses), [`ClassBodyQueryRuntime`](_import_helpers.md#ClassBodyQueryRuntime), [`ClassBuildInput`](_element_builders.md#ClassBuildInput), [`_extract_class_name_and_superclasses`](_signature_helpers.md#_extract_class_name_and_superclasses), [`node_line_range`](_element_builders.md#node_line_range), [`tree`](_import_helpers.md#ClassBodyQueryRuntime.tree), [`_extract_class_decorators`](_signature_helpers.md#_extract_class_decorators), [`current_module`](_element_builders.md#ClassBuildInput.current_module), [`decorators`](_element_builders.md#ClassBuildInput.decorators), [`name`](_element_builders.md#ClassBuildInput.name), [`raw_text`](_element_builders.md#ClassBuildInput.raw_text), [`class_query`](_import_helpers.md#ClassBodyQueryRuntime.class_query), [`docstring`](_element_builders.md#ClassBuildInput.docstring), [`end_line`](_element_builders.md#ClassBuildInput.end_line), [`framework_type`](_element_builders.md#ClassBuildInput.framework_type), [`log_debug_fn`](_import_helpers.md#ClassBodyQueryRuntime.log_debug_fn), [`log_warning_fn`](_import_helpers.md#ClassBodyQueryRuntime.log_warning_fn), [`start_line`](_element_builders.md#ClassBuildInput.start_line), [`_class_body_assignment_node`](_signature_helpers.md#_class_body_assignment_node)
- used by: [`PythonElementExtractor`](extractor.md#PythonElementExtractor)  (7 test-only)

