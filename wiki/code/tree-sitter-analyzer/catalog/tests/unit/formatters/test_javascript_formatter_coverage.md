---
title: 'Module: tests/unit/formatters/test_javascript_formatter_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_javascript_formatter_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_javascript_formatter_coverage`/
symbols:
  fmt: fmt().
  sample_data: sample_data().
  TestFormatNonDictInput: TestFormatNonDictInput#
  TestFormatNonDictInput.test_format_raises_typeerror_for_list: TestFormatNonDictInput#test_format_raises_typeerror_for_list().
  TestFormatNonDictInput.test_format_raises_typeerror_for_string: TestFormatNonDictInput#test_format_raises_typeerror_for_string().
  TestFormatNonDictInput.test_format_raises_typeerror_for_int: TestFormatNonDictInput#test_format_raises_typeerror_for_int().
  TestFormatNonDictInput.test_format_raises_typeerror_for_tuple: TestFormatNonDictInput#test_format_raises_typeerror_for_tuple().
  TestFormatEmptyFormatType: TestFormatEmptyFormatType#
  TestFormatEmptyFormatType.test_empty_string_calls_format_structure: TestFormatEmptyFormatType#test_empty_string_calls_format_structure().
  TestFormatEmptyFormatType.test_none_format_type_calls_format_structure: TestFormatEmptyFormatType#test_none_format_type_calls_format_structure().
  TestFormatTable: TestFormatTable#
  TestFormatTable.test_format_table_restores_format_type: TestFormatTable#test_format_table_restores_format_type().
  TestFormatTable.test_format_table_json_unsupported: TestFormatTable#test_format_table_json_unsupported().
  TestFormatTable.test_format_table_default_type: TestFormatTable#test_format_table_default_type().
  TestFormatAdvanced: TestFormatAdvanced#
  TestFormatAdvanced.test_format_advanced_json: TestFormatAdvanced#test_format_advanced_json().
  TestFormatAdvanced.test_format_advanced_csv: TestFormatAdvanced#test_format_advanced_csv().
  TestFormatAdvanced.test_format_advanced_default_fallback: TestFormatAdvanced#test_format_advanced_default_fallback().
  TestFormatAdvanced.test_format_advanced_default_output_format: TestFormatAdvanced#test_format_advanced_default_output_format().
  TestFormatAdvanced.test_format_advanced_non_json_non_csv: TestFormatAdvanced#test_format_advanced_non_json_non_csv().
  TestJavaScriptModuleLevelFunctions: TestJavaScriptModuleLevelFunctions#
  TestJavaScriptModuleLevelFunctions.test_flat_module_functions_render: TestJavaScriptModuleLevelFunctions#test_flat_module_functions_render().
  TestJavaScriptModuleLevelFunctions.test_top_level_function_alongside_class: TestJavaScriptModuleLevelFunctions#test_top_level_function_alongside_class().
  TestJavaScriptModuleLevelFunctions.test_plugin_shaped_functions_key_render: TestJavaScriptModuleLevelFunctions#test_plugin_shaped_functions_key_render().
---
# Module: [`tests/unit/formatters/test_javascript_formatter_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py)

## Classes
### `TestFormatAdvanced`
- def: [`tests/unit/formatters/test_javascript_formatter_coverage.py:81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L81)
- signature: `class TestFormatAdvanced:`
- members:
  - `test_format_advanced_csv(self, fmt, sample_data)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L87)
  - `test_format_advanced_default_fallback(self, fmt, sample_data)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L91)
  - `test_format_advanced_default_output_format(self, fmt, sample_data)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L95)
  - `test_format_advanced_json(self, fmt, sample_data)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L82)
  - `test_format_advanced_non_json_non_csv(self, fmt, sample_data)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L100)

### `TestFormatEmptyFormatType`
- def: [`tests/unit/formatters/test_javascript_formatter_coverage.py:54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L54)
- signature: `class TestFormatEmptyFormatType:`
- members:
  - `test_empty_string_calls_format_structure(self, fmt, sample_data)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L55)
  - `test_none_format_type_calls_format_structure(self, fmt, sample_data)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L60)

### `TestFormatNonDictInput`
- def: [`tests/unit/formatters/test_javascript_formatter_coverage.py:36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L36)
- signature: `class TestFormatNonDictInput:`
- members:
  - `test_format_raises_typeerror_for_int(self, fmt)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L45)
  - `test_format_raises_typeerror_for_list(self, fmt)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L37)
  - `test_format_raises_typeerror_for_string(self, fmt)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L41)
  - `test_format_raises_typeerror_for_tuple(self, fmt)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L49)

### `TestFormatTable`
- def: [`tests/unit/formatters/test_javascript_formatter_coverage.py:65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L65)
- signature: `class TestFormatTable:`
- members:
  - `test_format_table_default_type(self, fmt, sample_data)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L75)
  - `test_format_table_json_unsupported(self, fmt, sample_data)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L71)
  - `test_format_table_restores_format_type(self, fmt, sample_data)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L66)

### `TestJavaScriptModuleLevelFunctions`
- def: [`tests/unit/formatters/test_javascript_formatter_coverage.py:105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L105)
- doc: Module-level (non-class) functions must render in the full table.
- signature: `class TestJavaScriptModuleLevelFunctions:`
- members:
  - `test_flat_module_functions_render(self, fmt)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L112)
  - `test_plugin_shaped_functions_key_render(self, fmt)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L169) — Top-level functions arrive under 'functions' (JS plugin shape),
  - `test_top_level_function_alongside_class(self, fmt)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L138)

## Functions
- `fmt()` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L19)
- `sample_data()` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_javascript_formatter_coverage.py#L24)

