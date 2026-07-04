---
title: 'Module: tests/unit/formatters/test_python_formatter_signatures_table.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_python_formatter_signatures_table.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_python_formatter_signatures_table`/
symbols:
  _three_method_data: _three_method_data().
  test_python_formatter_signatures_not_raises: test_python_formatter_signatures_not_raises().
  _make_method: _make_method().
  test_signatures_mixed_class_and_module_functions: test_signatures_mixed_class_and_module_functions().
  test_signatures_shorter_than_full: test_signatures_shorter_than_full().
  test_signatures_flat_module_no_classes: test_signatures_flat_module_no_classes().
  test_python_formatter_format_structure_signatures: test_python_formatter_format_structure_signatures().
  test_formatter_registry_python_signatures: test_formatter_registry_python_signatures().
  test_method_sig_line_shape: test_method_sig_line_shape().
  test_signatures_header_contains_signatures_marker: test_signatures_header_contains_signatures_marker().
  test_signatures_module_name_in_header: test_signatures_module_name_in_header().
  test_signatures_class_block_header: test_signatures_class_block_header().
  test_signatures_method_lines_exact_count: test_signatures_method_lines_exact_count().
  test_signatures_init_line_exact: test_signatures_init_line_exact().
  test_signatures_add_line_exact: test_signatures_add_line_exact().
  test_signatures_reset_line_exact: test_signatures_reset_line_exact().
  test_signatures_next_step_hint_present: test_signatures_next_step_hint_present().
  test_signatures_methods_count_line: test_signatures_methods_count_line().
  test_auto_detect_language_resolves_python_for_py_extension: test_auto_detect_language_resolves_python_for_py_extension().
  test_nested_class_methods_not_duplicated: test_nested_class_methods_not_duplicated().
  _make_python_data: _make_python_data().
  _make_class: _make_class().
  test_shorten_return_type: test_shorten_return_type().
  test_structure_facade_description_no_default_java: test_structure_facade_description_no_default_java().
  test_structure_facade_description_mentions_auto_detect: test_structure_facade_description_mentions_auto_detect().
  test_module_name_empty_file_path: test_module_name_empty_file_path().
  test_module_name_pyw_extension: test_module_name_pyw_extension().
  test_module_name_pyi_extension: test_module_name_pyi_extension().
  test_methods_in_range_zero_range_returns_empty: test_methods_in_range_zero_range_returns_empty().
  test_trim_trailing_blank_lines_removes_blanks: test_trim_trailing_blank_lines_removes_blanks().
---
# Module: [`tests/unit/formatters/test_python_formatter_signatures_table.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py)

## Functions
- `_make_class(name: str, start: int, end: int)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L48)
- `_make_method(name: str, return_type: str, n_params: int, start: int, end: int)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L32) — Build a minimal method dict.
- `_make_python_data(*, file_path: str = "src/calculator.py", classes: list | None = None, methods: list | None = None, stats: dict | None = None)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L57) — Build minimal Python structure data.
- `_three_method_data()` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L136) — A Python fixture class with 3 methods for exact-assertion tests.
- `test_auto_detect_language_resolves_python_for_py_extension(tmp_path)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L295) — AnalyzeCodeStructureTool._resolve_language auto-detects 'python' for .py files.
- `test_formatter_registry_python_signatures()` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L282)
- `test_method_sig_line_shape(method: dict, expected_fragments: list[str])` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L99)
- `test_methods_in_range_zero_range_returns_empty()` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L365) — A zero line_range (start=0, end=0) returns an empty list.
- `test_module_name_empty_file_path()` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L338) — Empty file_path falls back to 'module'.
- `test_module_name_pyi_extension()` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L356) — '.pyi' stub extension is stripped correctly.
- `test_module_name_pyw_extension()` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L347) — '.pyw' extension is stripped correctly.
- `test_nested_class_methods_not_duplicated()` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L390) — A method in a nested class must appear under the inner class only.
- `test_python_formatter_format_structure_signatures()` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L257) — PythonTableFormatter with format_type='signatures' must not raise.
- `test_python_formatter_signatures_not_raises()` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L265) — Previously raised ValueError — must now succeed.
- `test_shorten_return_type(ret: str, expected: str)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L127)
- `test_signatures_add_line_exact()` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L179)
- `test_signatures_class_block_header()` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L162)
- `test_signatures_flat_module_no_classes()` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L219) — Module with no classes renders a <module functions> block.
- `test_signatures_header_contains_signatures_marker()` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L152)
- `test_signatures_init_line_exact()` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L174)
- `test_signatures_method_lines_exact_count()` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L167) — Exactly 3 method lines should appear (one per method).
- `test_signatures_methods_count_line()` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L195)
- `test_signatures_mixed_class_and_module_functions()` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L237) — Class methods and module-level functions both appear, separated.
- `test_signatures_module_name_in_header()` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L157)
- `test_signatures_next_step_hint_present()` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L189)
- `test_signatures_reset_line_exact()` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L184)
- `test_signatures_shorter_than_full()` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L200) — signatures output should be shorter than full output.
- `test_structure_facade_description_mentions_auto_detect()` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L323) — Description should mention auto-detection for the signatures action.
- `test_structure_facade_description_no_default_java()` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L315) — 'default java' must not appear in the signatures action description.
- `test_trim_trailing_blank_lines_removes_blanks()` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures_table.py#L376) — _trim_trailing_blank_lines removes trailing empty strings.

