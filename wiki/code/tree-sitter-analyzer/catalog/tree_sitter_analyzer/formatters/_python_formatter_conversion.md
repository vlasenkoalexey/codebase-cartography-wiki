---
title: 'Module: tree_sitter_analyzer/formatters/_python_formatter_conversion.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_python_formatter_conversion.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._python_formatter_conversion`/
symbols:
  _append_converted_element: _append_converted_element().
  process_python_parameters: process_python_parameters().
  convert_analysis_result_to_python_format: convert_analysis_result_to_python_format().
  convert_class_element_for_python: convert_class_element_for_python().
  convert_function_element_for_python: convert_function_element_for_python().
  convert_variable_element_for_python: convert_variable_element_for_python().
  convert_import_element_for_python: convert_import_element_for_python().
  _process_parameter_item: _process_parameter_item().
  _element_line_range: _element_line_range().
  _new_conversion: _new_conversion().
  _conversion_result: _conversion_result().
  _process_parameter_string: _process_parameter_string().
  _process_parameter_text: _process_parameter_text().
---
# Module: [`tree_sitter_analyzer/formatters/_python_formatter_conversion.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py)

## Functions
- `_append_converted_element(conversion: dict[str, Any], formatter: Any, element: Any)` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L35)
- `_conversion_result(analysis_result: Any, conversion: dict[str, Any])` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L59)
- `_element_line_range(element: Any)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L147)
- `_new_conversion()` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L25)
- `_process_parameter_item(param: Any)` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L171)
- `_process_parameter_string(params: str)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L163)
- `_process_parameter_text(param: str)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L179)
- `convert_analysis_result_to_python_format(formatter: Any, analysis_result: Any)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L15) — Convert AnalysisResult to Python formatter's expected format
- `convert_class_element_for_python(element: Any)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L84) — Convert class element for Python formatter
- `convert_function_element_for_python(formatter: Any, element: Any)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L97) — Convert function element for Python formatter
- `convert_import_element_for_python(element: Any)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L131) — Convert import element for Python formatter
- `convert_variable_element_for_python(element: Any)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L118) — Convert variable element for Python formatter
- `process_python_parameters(params: Any)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_python_formatter_conversion.py#L154) — Process parameters for Python formatter

