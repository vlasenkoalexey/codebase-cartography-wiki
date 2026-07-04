---
title: 'Module: tree_sitter_analyzer/languages/c_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/languages/c_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.languages.c_helpers`/
symbols:
  extract_macro_definition: extract_macro_definition().
  extract_c_imports: extract_c_imports().
  _extract_include_info: _extract_include_info().
  _extract_includes_fallback: _extract_includes_fallback().
  extract_macro_function: extract_macro_function().
  calculate_complexity.count_decisions: calculate_complexity().count_decisions().
  extract_field_declaration: extract_field_declaration().
  extract_variable_declaration: extract_variable_declaration().
  extract_struct_definition: extract_struct_definition().
  extract_enum_definition: extract_enum_definition().
  extract_c_function: extract_c_function().
  parse_function_signature: parse_function_signature().
  calculate_complexity: calculate_complexity().
  extract_comment_for_line: extract_comment_for_line().
  c_traverse_and_extract: c_traverse_and_extract().
  extract_parameters: extract_parameters().
---
# Module: [`tree_sitter_analyzer/languages/c_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py)

## Functions
- `_extract_include_info(node: Any, get_node_text: Callable[..., str])` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L214) — Extract include directive information.
- `_extract_includes_fallback(source_code: str)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L223) — Fallback include extraction using regex.
- `c_traverse_and_extract(root_node: Any, extractors: dict[str, Any], results: list[Any], element_type: str, processed_nodes: set[int], element_cache: dict[tuple[int, str], Any])` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L229) — Iterative node traversal and extraction with caching for C.
- `calculate_complexity(node: Any)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L129) — Calculate cyclomatic complexity.
- `count_decisions(n: Any)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L149)
- `extract_c_function(node: Any, get_node_text: Callable[..., str], content_lines: list[str], parse_function_signature: Callable, calculate_complexity: Callable, extract_comment_for_line: Callable)` — [`L249`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L249) — Extract C function definition.
- `extract_c_imports(tree: Any, source_code: str, get_node_text: Callable[..., str])` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L35) — Extract C include directives.
- `extract_comment_for_line(line: int, content_lines: list[str])` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L208) — Extract comment for a specific line.
- `extract_enum_definition(node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L198) — Extract enum definition.
- `extract_field_declaration(node: Any, get_node_text: Callable[..., str])` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L172) — Extract struct/union field declarations.
- `extract_macro_definition(node: Any, get_node_text: Callable[..., str])` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L83) — Extract macro definitions as constants.
- `extract_macro_function(node: Any, get_node_text: Callable[..., str])` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L121) — Extract macro function definition.
- `extract_parameters(params_node: Any, get_node_text: Callable[..., str])` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L58) — Extract function parameters.
- `extract_struct_definition(node: Any, get_node_text: Callable[..., str], content_lines: list[str])` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L188) — Extract struct definition.
- `extract_variable_declaration(node: Any, get_node_text: Callable[..., str])` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L180) — Extract C variable declarations (not struct members).
- `parse_function_signature(node: Any, get_node_text: Callable[..., str], extract_params_fn: Callable[[Any], list[str]])` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/languages/c_helpers.py#L73) — Parse C function signature.

