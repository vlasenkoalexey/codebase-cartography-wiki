---
title: 'Module: examples/javascript_analysis_demo.py'
type: catalog
provenance: extracted
module: examples/javascript_analysis_demo.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `examples.javascript_analysis_demo`/
symbols:
  _get_field: _get_field().
  analyze_modern_javascript: analyze_modern_javascript().
  _categorize_elements: _categorize_elements().
  _print_function_section: _print_function_section().
  _print_formatted_table: _print_formatted_table().
  _print_class_section: _print_class_section().
  _print_function_group: _print_function_group().
  project_root: project_root.
  _categorize_functions: _categorize_functions().
  _is_function: _is_function().
  _is_class: _is_class().
  _is_variable: _is_variable().
  _is_import: _is_import().
  _print_methods_group: _print_methods_group().
  _print_method_type_tags: _print_method_type_tags().
  _print_import_section: _print_import_section().
  _build_formatter_data: _build_formatter_data().
  demonstrate_query_capabilities: demonstrate_query_capabilities().
  _print_stats: _print_stats().
  _print_element_breakdown: _print_element_breakdown().
  _print_variable_section: _print_variable_section().
  _print_framework_info: _print_framework_info().
---
# Module: [`examples/javascript_analysis_demo.py`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py)

## Functions
- `_build_formatter_data(js_file, functions, classes, variables, imports)` — [`L291`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L291)
- `_categorize_elements(elements)` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L33) — Split a flat elements list into typed groups.
- `_categorize_functions(functions)` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L74) — Split functions into regular / arrow / async / methods.
- `_get_field(obj, attr, default=None)` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L23) — Uniform attribute access for dict or object.
- `_is_class(e)` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L50)
- `_is_function(e)` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L42)
- `_is_import(e)` — [`L66`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L66)
- `_is_variable(e)` — [`L58`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L58)
- `_print_class_section(classes, methods)` — [`L169`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L169)
- `_print_element_breakdown(functions, classes, variables, imports)` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L103)
- `_print_formatted_table(js_file, functions, classes, variables, imports)` — [`L355`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L355)
- `_print_framework_info(result)` — [`L369`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L369)
- `_print_function_group(label, funcs, limit=5)` — [`L112`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L112)
- `_print_function_section(functions)` — [`L142`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L142)
- `_print_import_section(imports)` — [`L198`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L198)
- `_print_method_type_tags(method)` — [`L154`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L154)
- `_print_methods_group(methods, limit=5)` — [`L126`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L126)
- `_print_stats(result, elements)` — [`L92`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L92)
- `_print_variable_section(variables)` — [`L248`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L248)
- `analyze_modern_javascript()` — [`L386`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L386) — Analyze the ModernJavaScript.js example file
- `demonstrate_query_capabilities()` — [`L431`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L431) — Demonstrate the enhanced query capabilities

## Module values
- `project_root` — [`L16`](../../../../../raw/code/tree-sitter-analyzer/examples/javascript_analysis_demo.py#L16)

