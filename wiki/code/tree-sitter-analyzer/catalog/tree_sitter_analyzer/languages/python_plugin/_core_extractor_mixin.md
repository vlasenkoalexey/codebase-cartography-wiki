---
title: 'Module: tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.python_plugin._core_extractor_mixin`/PythonExtractorCoreMixin#
symbols:
  PythonExtractorCoreMixin._traverse_and_extract_iterative: _traverse_and_extract_iterative().
  PythonExtractorCoreMixin._extract_docstring_for_line: _extract_docstring_for_line().
  PythonExtractorCoreMixin._get_node_text_optimized: _get_node_text_optimized().
  PythonExtractorCoreMixin._logging_hooks: _logging_hooks().
  PythonExtractorCoreMixin._encoding_hooks: _encoding_hooks().
  PythonExtractorCoreMixin: ''
  PythonExtractorCoreMixin.framework_type: framework_type.
  PythonExtractorCoreMixin._extract_parameters_from_node_optimized: _extract_parameters_from_node_optimized().
  PythonExtractorCoreMixin._calculate_complexity_optimized: _calculate_complexity_optimized().
  PythonExtractorCoreMixin._reset_caches: _reset_caches().
  PythonExtractorCoreMixin._detect_file_characteristics: _detect_file_characteristics().
  PythonExtractorCoreMixin.is_module: is_module.
---
# Module: [`tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py)

## Classes
### `PythonExtractorCoreMixin`
- def: [`tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L21)
- signature: `class PythonExtractorCoreMixin:`
- members:
  - `_calculate_complexity_optimized(self, node: Any)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L151) — Calculate cyclomatic complexity via an AST-node walk.
  - `_detect_file_characteristics(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L30) — Detect Python file characteristics.
  - `_encoding_hooks(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L105) — Return encoding helpers from the public extractor module for patchability.
  - `_extract_docstring_for_line(self, target_line: int)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L136) — Extract docstring for the specified line.
  - `_extract_parameters_from_node_optimized(self, params_node: Any)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L126) — Extract function parameters with type hints.
  - `_get_node_text_optimized(self, node: Any)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L64) — Get node text with optimized caching using position-based keys.
  - `_logging_hooks(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L115) — Return log helpers from the public extractor module for patchability.
  - `_reset_caches(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L22) — Reset performance caches.
  - `_traverse_and_extract_iterative(self, root_node: Any | None, extractors: dict[str, Any], results: list[Any], element_type: str)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L42) — Iterative node traversal and extraction with caching.
  - `framework_type` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L33)
  - `is_module` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/python_plugin/_core_extractor_mixin.py#L32)
- uses (calls/refs, reference-scoped): [`log_debug`](../../utils/logging.md#log_debug), [`log_error`](../../utils/logging.md#log_error), [`log_warning`](../../utils/logging.md#log_warning), [`PythonElementExtractor`](extractor.md#PythonElementExtractor), [`safe_encode`](../../encoding_utils.md#safe_encode), [`run_iterative_traversal`](_traversal_helpers.md#run_iterative_traversal), [`extract_text_slice`](../../encoding_utils.md#extract_text_slice), [`_extract_node_text_by_points`](_text_helpers.md#_extract_node_text_by_points), [`find_docstring_after_line`](_docstring_helpers.md#find_docstring_after_line), [`_extract_node_text_by_bytes`](_text_helpers.md#_extract_node_text_by_bytes), [`python_cyclomatic_complexity`](_python_complexity.md#python_cyclomatic_complexity), [`TraversalRuntime`](_traversal_helpers.md#TraversalRuntime), [`_PARAMETER_NODE_TYPES`](_signature_helpers.md#_PARAMETER_NODE_TYPES), [`element_cache`](_traversal_helpers.md#TraversalRuntime.element_cache), [`element_type`](_traversal_helpers.md#TraversalRuntime.element_type), [`extractors`](_traversal_helpers.md#TraversalRuntime.extractors), [`log_debug_fn`](_traversal_helpers.md#TraversalRuntime.log_debug_fn), [`log_warning_fn`](_traversal_helpers.md#TraversalRuntime.log_warning_fn), [`processed_node_ids`](_traversal_helpers.md#TraversalRuntime.processed_node_ids), [`results`](_traversal_helpers.md#TraversalRuntime.results), [`cache_value`](_docstring_helpers.md#DocstringSearchResult.cache_value), [`should_cache`](_docstring_helpers.md#DocstringSearchResult.should_cache), [`value`](_docstring_helpers.md#DocstringSearchResult.value)
- used by: [`PythonElementExtractor`](extractor.md#PythonElementExtractor)

