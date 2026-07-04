---
title: 'Module: tests/unit/formatters/test_python_formatter_comprehensive_basic.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_python_formatter_comprehensive_basic.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_python_formatter_comprehensive_basic`/TestPythonTableFormatter
symbols:
  TestPythonTableFormatterBasic.formatter: Basic#formatter().
  TestPythonTableFormatterFullFormat.formatter: FullFormat#formatter().
  TestPythonTableFormatterCompactFormat.formatter: CompactFormat#formatter().
  TestPythonTableFormatterMethodFormatting.formatter: MethodFormatting#formatter().
  TestPythonTableFormatterBasic: Basic#
  TestPythonTableFormatterBasic.sample_python_data: Basic#sample_python_data().
  TestPythonTableFormatterBasic.test_format_method_delegates_to_format_structure: Basic#test_format_method_delegates_to_format_structure().
  TestPythonTableFormatterBasic.test_format_with_empty_data: Basic#test_format_with_empty_data().
  TestPythonTableFormatterFullFormat: FullFormat#
  TestPythonTableFormatterFullFormat.test_full_format_module_header: FullFormat#test_full_format_module_header().
  TestPythonTableFormatterFullFormat.test_full_format_package_header: FullFormat#test_full_format_package_header().
  TestPythonTableFormatterFullFormat.test_full_format_script_header: FullFormat#test_full_format_script_header().
  TestPythonTableFormatterFullFormat.test_full_format_module_docstring: FullFormat#test_full_format_module_docstring().
  TestPythonTableFormatterFullFormat.test_full_format_imports_section: FullFormat#test_full_format_imports_section().
  TestPythonTableFormatterFullFormat.test_full_format_multiple_classes: FullFormat#test_full_format_multiple_classes().
  TestPythonTableFormatterFullFormat.test_full_format_single_class: FullFormat#test_full_format_single_class().
  TestPythonTableFormatterFullFormat.test_full_format_fields_section: FullFormat#test_full_format_fields_section().
  TestPythonTableFormatterFullFormat.test_full_format_methods_section: FullFormat#test_full_format_methods_section().
  TestPythonTableFormatterCompactFormat: CompactFormat#
  TestPythonTableFormatterCompactFormat.test_compact_format_multiple_classes_header: CompactFormat#test_compact_format_multiple_classes_header().
  TestPythonTableFormatterCompactFormat.test_compact_format_single_class_header: CompactFormat#test_compact_format_single_class_header().
  TestPythonTableFormatterCompactFormat.test_compact_format_info_section: CompactFormat#test_compact_format_info_section().
  TestPythonTableFormatterCompactFormat.test_compact_format_methods_section: CompactFormat#test_compact_format_methods_section().
  TestPythonTableFormatterMethodFormatting: MethodFormatting#
  TestPythonTableFormatterMethodFormatting.test_format_method_row_basic: MethodFormatting#test_format_method_row_basic().
  TestPythonTableFormatterMethodFormatting.test_format_method_row_async: MethodFormatting#test_format_method_row_async().
  TestPythonTableFormatterMethodFormatting.test_format_method_row_private: MethodFormatting#test_format_method_row_private().
  TestPythonTableFormatterMethodFormatting.test_format_method_row_magic: MethodFormatting#test_format_method_row_magic().
  TestPythonTableFormatterMethodFormatting.test_format_method_row_with_decorators: MethodFormatting#test_format_method_row_with_decorators().
  TestPythonTableFormatterMethodFormatting.test_format_method_row_fallback_line_numbers: MethodFormatting#test_format_method_row_fallback_line_numbers().
---
# Module: [`tests/unit/formatters/test_python_formatter_comprehensive_basic.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py)

## Classes
### `TestPythonTableFormatterBasic`
- def: [`tests/unit/formatters/test_python_formatter_comprehensive_basic.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L11)
- doc: Test basic Python table formatter functionality.
- signature: `class TestPythonTableFormatterBasic:`
- members:
  - `formatter(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L15) — Create a Python table formatter instance.
  - `sample_python_data(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L20) — Sample Python analysis data.
  - `test_format_method_delegates_to_format_structure(self, formatter, sample_python_data)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L105) — Test that format method delegates to format_structure.
  - `test_format_with_empty_data(self, formatter)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L115) — Test formatting with empty data.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonTableFormatterCompactFormat`
- def: [`tests/unit/formatters/test_python_formatter_comprehensive_basic.py:343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L343)
- doc: Test Python table formatter compact format functionality.
- signature: `class TestPythonTableFormatterCompactFormat:`
- members:
  - `formatter(self)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L347) — Create a Python table formatter instance.
  - `test_compact_format_info_section(self, formatter)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L375) — Test compact format info section.
  - `test_compact_format_methods_section(self, formatter)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L390) — Test compact format methods section.
  - `test_compact_format_multiple_classes_header(self, formatter)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L351) — Test compact format header with multiple classes.
  - `test_compact_format_single_class_header(self, formatter)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L363) — Test compact format header with single class.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonTableFormatterFullFormat`
- def: [`tests/unit/formatters/test_python_formatter_comprehensive_basic.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L123)
- doc: Test Python table formatter full format functionality.
- signature: `class TestPythonTableFormatterFullFormat:`
- members:
  - `formatter(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L127) — Create a Python table formatter instance.
  - `test_full_format_fields_section(self, formatter)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L270) — Test full format fields section.
  - `test_full_format_imports_section(self, formatter)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L187) — Test full format imports section.
  - `test_full_format_methods_section(self, formatter)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L307) — Test full format methods section.
  - `test_full_format_module_docstring(self, formatter)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L172) — Test full format module docstring extraction.
  - `test_full_format_module_header(self, formatter)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L131) — Test full format module header generation.
  - `test_full_format_multiple_classes(self, formatter)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L208) — Test full format with multiple classes.
  - `test_full_format_package_header(self, formatter)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L144) — Test full format package header generation.
  - `test_full_format_script_header(self, formatter)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L157) — Test full format script header generation.
  - `test_full_format_single_class(self, formatter)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L242) — Test full format with single class.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonTableFormatterMethodFormatting`
- def: [`tests/unit/formatters/test_python_formatter_comprehensive_basic.py:420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L420)
- doc: Test Python table formatter method formatting functionality.
- signature: `class TestPythonTableFormatterMethodFormatting:`
- members:
  - `formatter(self)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L424) — Create a Python table formatter instance.
  - `test_format_method_row_async(self, formatter)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L452) — Test async method row formatting.
  - `test_format_method_row_basic(self, formatter)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L428) — Test basic method row formatting.
  - `test_format_method_row_fallback_line_numbers(self, formatter)` — [`L529`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L529) — Test method row formatting with fallback line numbers.
  - `test_format_method_row_magic(self, formatter)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L489) — Test magic method row formatting.
  - `test_format_method_row_private(self, formatter)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L470) — Test private method row formatting.
  - `test_format_method_row_with_decorators(self, formatter)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_comprehensive_basic.py#L511) — Test method row formatting with decorators.
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

