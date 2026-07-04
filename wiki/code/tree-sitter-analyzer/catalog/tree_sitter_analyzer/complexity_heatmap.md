---
title: 'Module: tree_sitter_analyzer/complexity_heatmap.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/complexity_heatmap.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.complexity_heatmap`/
symbols:
  analyze_project_heatmap: analyze_project_heatmap().
  analyze_file_complexity: analyze_file_complexity().
  _extract_functions_via_plugin: _extract_functions_via_plugin().
  analyze_file_complexity_from_cache: analyze_file_complexity_from_cache().
  _extract_functions_from_ast: _extract_functions_from_ast().
  FunctionComplexity.complexity: FunctionComplexity#complexity.
  _risk_band: _risk_band().
  FunctionComplexity.name: FunctionComplexity#name.
  _extractor_complexity_by_line: _extractor_complexity_by_line().
  FunctionComplexity: FunctionComplexity#
  _extract_functions: _extract_functions().
  FunctionComplexity.line: FunctionComplexity#line.
  FunctionComplexity.decision_points: FunctionComplexity#decision_points.
  _name_from_children: _name_from_children().
  _arrow_function_name: _arrow_function_name().
  _get_function_name: _get_function_name().
  logger: logger.
  FileHeatmap.functions: FileHeatmap#functions.
  FunctionComplexity.class_name: FunctionComplexity#class_name.
  FunctionComplexity.file: FunctionComplexity#file.
  FunctionComplexity.language: FunctionComplexity#language.
  _get_nodes_for_language: _get_nodes_for_language().
  _count_complexity_in_node: _count_complexity_in_node().
  _find_class_name: _find_class_name().
  _collect_source_files: _collect_source_files().
  FunctionComplexity.end_line: FunctionComplexity#end_line.
  FileHeatmap.max_complexity: FileHeatmap#max_complexity.
  RISK_BANDS: RISK_BANDS.
  FileHeatmap: FileHeatmap#
  FileHeatmap.file: FileHeatmap#file.
  FileHeatmap.language: FileHeatmap#language.
  FileHeatmap.total_complexity: FileHeatmap#total_complexity.
  FileHeatmap.avg_complexity: FileHeatmap#avg_complexity.
  _node_text: _node_text().
  _NAME_CHILD_TYPES: _NAME_CHILD_TYPES.
  _ARROW_PARENT_TYPES: _ARROW_PARENT_TYPES.
  _COMPLEXITY_NODES._COMPLEXITY_NODES: _COMPLEXITY_NODES._COMPLEXITY_NODES.
  _METHOD_NODES._METHOD_NODES: _METHOD_NODES._METHOD_NODES.
  _CLASS_NODES._CLASS_NODES: _CLASS_NODES._CLASS_NODES.
  _FUNCTION_NODES._FUNCTION_NODES: _FUNCTION_NODES._FUNCTION_NODES.
---
# Module: [`tree_sitter_analyzer/complexity_heatmap.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py)

## Classes
### `FileHeatmap`
- def: [`tree_sitter_analyzer/complexity_heatmap.py:176`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L176)
- signature: `class FileHeatmap:`
- members:
  - `avg_complexity` — [`L181`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L181)
  - `file` — [`L177`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L177)
  - `functions` — [`L179`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L179)
  - `language` — [`L178`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L178)
  - `max_complexity` — [`L182`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L182)
  - `total_complexity` — [`L180`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L180)
- uses (calls/refs, reference-scoped): [`FunctionComplexity`](complexity_heatmap.md#FunctionComplexity)
- used by: [`analyze_project_heatmap`](complexity_heatmap.md#analyze_project_heatmap)

### `FunctionComplexity`
- def: [`tree_sitter_analyzer/complexity_heatmap.py:164`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L164)
- signature: `class FunctionComplexity:`
- members:
  - `class_name` — [`L171`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L171)
  - `complexity` — [`L169`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L169)
  - `decision_points` — [`L172`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L172)
  - `end_line` — [`L168`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L168)
  - `file` — [`L166`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L166)
  - `language` — [`L170`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L170)
  - `line` — [`L167`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L167)
  - `name` — [`L165`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L165)
- used by: [`analyze_project_heatmap`](complexity_heatmap.md#analyze_project_heatmap), [`analyze_file_complexity`](complexity_heatmap.md#analyze_file_complexity), [`_extract_functions_via_plugin`](complexity_heatmap.md#_extract_functions_via_plugin), [`analyze_file_complexity_from_cache`](complexity_heatmap.md#analyze_file_complexity_from_cache), [`_extract_functions_from_ast`](complexity_heatmap.md#_extract_functions_from_ast), [`score_complexity`](health_scorer.md#score_complexity), [`complexity_facet`](mcp/tools/_codegraph_query_facets.md#complexity_facet), [`_extract_functions`](complexity_heatmap.md#_extract_functions), [`functions`](complexity_heatmap.md#FileHeatmap.functions)  (17 test-only)

## Functions
- `_arrow_function_name(node: Any)` — [`L260`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L260) — Return the variable name an arrow function is assigned to, or ``""``.
- `_collect_source_files(project_root: str, language_filter: str | None, directory_filter: str | None, max_files: int)` — [`L566`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L566)
- `_count_complexity_in_node(node: Any, language: str)` — [`L207`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L207)
- `_extract_functions(tree: Any, source: str, language: str, file_path: str)` — [`L278`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L278)
- `_extract_functions_from_ast(tree: Any, source: str, language: str, file_path: str, method_nodes: set[str])` — [`L289`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L289) — AST-walk path for the 8 hardcoded languages.
- `_extract_functions_via_plugin(tree: Any, source: str, language: str, file_path: str)` — [`L356`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L356) — Fallback path for languages not in _METHOD_NODES.
- `_extractor_complexity_by_line(tree: Any, source: str, language: str)` — [`L329`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L329) — Map function start-line → the plugin extractor's ``complexity_score``.
- `_find_class_name(node: Any, language: str)` — [`L222`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L222)
- `_get_function_name(node: Any)` — [`L270`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L270) — Extract the name from any function / method definition node.
- `_get_nodes_for_language(language: str)` — [`L200`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L200)
- `_name_from_children(node: Any)` — [`L252`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L252) — Return the first name-like child's text, or ``""``.
- `_node_text(node: Any)` — [`L246`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L246) — Decode a node's text field to ``str``.
- `_risk_band(score: int)` — [`L193`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L193)
- `analyze_file_complexity(file_path: str, language: str)` — [`L401`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L401)
- `analyze_file_complexity_from_cache(cache: Any, file_path: str)` — [`L410`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L410) — Compute complexity from a pre-indexed AST cache entry (no re-parse).
- `analyze_project_heatmap(project_root: str, language_filter: str | None = None, directory_filter: str | None = None, max_files: int = 500, cache: Any | None = None)` — [`L460`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L460)

## Module values
- `RISK_BANDS` — [`L185`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L185)
- `_ARROW_PARENT_TYPES` — [`L243`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L243)
- `_CLASS_NODES` — [`L151`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L151)
- `_COMPLEXITY_NODES` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L28)
- `_FUNCTION_NODES` — [`L129`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L129)
- `_METHOD_NODES` — [`L140`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L140)
- `_NAME_CHILD_TYPES` — [`L240`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L240)
- `logger` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/complexity_heatmap.py#L26)

