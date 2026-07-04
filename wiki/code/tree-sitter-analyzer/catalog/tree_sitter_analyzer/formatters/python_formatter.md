---
title: 'Module: tree_sitter_analyzer/formatters/python_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/python_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.python_formatter`/PythonTableFormatter#
symbols:
  PythonTableFormatter: ''
  PythonTableFormatter.format_structure: format_structure().
  PythonTableFormatter.format_type: format_type.
  PythonTableFormatter.format_advanced: format_advanced().
  PythonTableFormatter.format_analysis_result: format_analysis_result().
  PythonTableFormatter.format_table: format_table().
  PythonTableFormatter._convert_analysis_result_to_python_format: _convert_analysis_result_to_python_format().
  PythonTableFormatter._convert_class_element_for_python: _convert_class_element_for_python().
  PythonTableFormatter._convert_function_element_for_python: _convert_function_element_for_python().
  PythonTableFormatter._convert_variable_element_for_python: _convert_variable_element_for_python().
  PythonTableFormatter._convert_import_element_for_python: _convert_import_element_for_python().
  PythonTableFormatter._process_python_parameters: _process_python_parameters().
  PythonTableFormatter._format_full_table: _format_full_table().
  PythonTableFormatter._format_compact_table: _format_compact_table().
  PythonTableFormatter._create_compact_signature: _create_compact_signature().
  PythonTableFormatter._extract_module_docstring: _extract_module_docstring().
  PythonTableFormatter._format_python_signature: _format_python_signature().
  PythonTableFormatter._get_python_visibility_symbol: _get_python_visibility_symbol().
  PythonTableFormatter._format_decorators: _format_decorators().
  PythonTableFormatter._format_class_method_row: _format_class_method_row().
  PythonTableFormatter._format_python_signature_compact: _format_python_signature_compact().
  PythonTableFormatter.format: format().
  PythonTableFormatter.format_summary: format_summary().
  PythonTableFormatter.convert_class_element_for_python: convert_class_element_for_python.
  PythonTableFormatter.convert_function_element_for_python: convert_function_element_for_python.
  PythonTableFormatter.convert_variable_element_for_python: convert_variable_element_for_python.
  PythonTableFormatter.convert_import_element_for_python: convert_import_element_for_python.
  PythonTableFormatter.process_python_parameters: process_python_parameters.
  PythonTableFormatter._format_signatures_table: _format_signatures_table().
  PythonTableFormatter._format_method_row: _format_method_row().
  PythonTableFormatter._shorten_type: _shorten_type().
  PythonTableFormatter.create_compact_signature: create_compact_signature.
  PythonTableFormatter.extract_module_docstring: extract_module_docstring.
  PythonTableFormatter.format_python_signature: format_python_signature.
  PythonTableFormatter.get_python_visibility_symbol: get_python_visibility_symbol.
  PythonTableFormatter.format_decorators: format_decorators.
  PythonTableFormatter.format_class_method_row: format_class_method_row.
  PythonTableFormatter._format_json: _format_json().
  PythonTableFormatter.format_python_signature_compact: format_python_signature_compact.
---
# Module: [`tree_sitter_analyzer/formatters/python_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py)

## Classes
### `PythonTableFormatter`  ·  implements/extends BaseTableFormatter
- def: [`tree_sitter_analyzer/formatters/python_formatter.py:37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L37)
- doc: Table formatter specialized for Python
- signature: `class PythonTableFormatter(BaseTableFormatter):`
- members:
  - `_convert_analysis_result_to_python_format(self, analysis_result: Any)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L95) — Convert AnalysisResult to Python formatter's expected format
  - `_convert_class_element_for_python(self, element: Any)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L101) — Convert class element for Python formatter
  - `_convert_function_element_for_python(self, element: Any)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L105) — Convert function element for Python formatter
  - `_convert_import_element_for_python(self, element: Any)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L113) — Convert import element for Python formatter
  - `_convert_variable_element_for_python(self, element: Any)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L109) — Convert variable element for Python formatter
  - `_create_compact_signature(self, method: dict[str, Any])` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L148) — Create compact method signature for Python
  - `_extract_module_docstring(self, data: dict[str, Any])` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L156) — Extract module-level docstring
  - `_format_class_method_row(self, method: dict[str, Any])` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L172) — Format a method table row for class-specific sections
  - `_format_compact_table(self, data: dict[str, Any])` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L132) — Compact table format for Python
  - `_format_decorators(self, decorators: list[str])` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L168) — Format Python decorators
  - `_format_full_table(self, data: dict[str, Any])` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L128) — Full table format for Python
  - `_format_json(self, data: dict[str, Any])` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L79) — Format data as JSON
  - `_format_method_row(self, method: dict[str, Any])` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L144) — Format a method table row for Python
  - `_format_python_signature(self, method: dict[str, Any])` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L160) — Create Python method signature
  - `_format_python_signature_compact(self, method: dict[str, Any])` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L176) — Create compact Python method signature for class sections
  - `_format_signatures_table(self, data: dict[str, Any])` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L136) — Signatures (lightweight method-directory) format for Python.
  - `_get_python_visibility_symbol(self, visibility: str)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L164) — Get Python visibility symbol
  - `_process_python_parameters(self, params: Any)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L117) — Process parameters for Python formatter
  - `_shorten_type(self, type_name: Any)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L152) — Shorten type name for Python tables
  - `format(self, data: dict[str, Any])` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L40) — Format data using the configured format type
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L68) — Format advanced analysis output for Python
  - `format_analysis_result(self, analysis_result: Any, table_type: str = "full")` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L88) — Format AnalysisResult directly for Python files - prevents degradation
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L64) — Format structure analysis output for Python
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L60) — Format summary output for Python
  - `format_table(self, data: dict[str, Any], table_type: str = "full")` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L50) — Format table output for Python files
  - `convert_class_element_for_python` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L122)
  - `convert_function_element_for_python` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L123)
  - `convert_import_element_for_python` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L125)
  - `convert_variable_element_for_python` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L124)
  - `create_compact_signature` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L181)
  - `extract_module_docstring` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L182)
  - `format_class_method_row` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L186)
  - `format_decorators` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L185)
  - `format_python_signature` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L183)
  - `format_python_signature_compact` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L187)
  - `format_type` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L53)
  - `get_python_visibility_symbol` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L184)
  - `process_python_parameters` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/python_formatter.py#L126)
- uses (calls/refs, reference-scoped): [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_format_csv`](base_formatter.md#BaseTableFormatter._format_csv), [`format_python_signatures_table`](_python_formatter_signatures_table.md#format_python_signatures_table), [`format_python_full_table`](_python_formatter_full.md#format_python_full_table), [`format_python_compact_table`](_python_formatter_compact.md#format_python_compact_table), [`process_python_parameters`](_python_formatter_conversion.md#process_python_parameters), [`format_python_class_method_row`](_python_formatter_rows.md#format_python_class_method_row), [`convert_analysis_result_to_python_format`](_python_formatter_conversion.md#convert_analysis_result_to_python_format), [`convert_class_element_for_python`](_python_formatter_conversion.md#convert_class_element_for_python), [`convert_function_element_for_python`](_python_formatter_conversion.md#convert_function_element_for_python), [`convert_variable_element_for_python`](_python_formatter_conversion.md#convert_variable_element_for_python), [`create_compact_signature`](_python_formatter_signatures.md#create_compact_signature), [`extract_module_docstring`](_python_formatter_docstrings.md#extract_module_docstring), [`format_python_method_row`](_python_formatter_rows.md#format_python_method_row), [`format_python_signature`](_python_formatter_signatures.md#format_python_signature), [`format_python_signature_compact`](_python_formatter_signatures.md#format_python_signature_compact), [`shorten_type`](_python_formatter_signatures.md#shorten_type), [`convert_import_element_for_python`](_python_formatter_conversion.md#convert_import_element_for_python), [`format_decorators`](_python_formatter_docstrings.md#format_decorators), [`get_python_visibility_symbol`](_python_formatter_rows.md#get_python_visibility_symbol)
- used by: [`format_structure`](base_formatter.md#BaseTableFormatter.format_structure), [`BaseTableFormatter`](base_formatter.md#BaseTableFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`_format_compact_table`](base_formatter.md#BaseTableFormatter._format_compact_table), [`_format_full_table`](base_formatter.md#BaseTableFormatter._format_full_table), [`format_table`](base_formatter.md#BaseTableFormatter.format_table), [`format_summary`](base_formatter.md#BaseTableFormatter.format_summary), [`format`](base_formatter.md#BaseFormatter.format), [`format_advanced`](base_formatter.md#BaseTableFormatter.format_advanced)  (61 test-only)

