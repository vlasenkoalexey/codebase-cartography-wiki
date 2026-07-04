---
title: 'Module: tests/test_vue_extraction.py'
type: catalog
provenance: extracted
module: tests/test_vue_extraction.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_vue_extraction`/
symbols:
  _write: _write().
  test_generic_component_open_tag_with_angle_brackets: test_generic_component_open_tag_with_angle_brackets().
  test_script_setup_ts_static_imports_resolve: test_script_setup_ts_static_imports_resolve().
  test_typed_props_reference_imported_type: test_typed_props_reference_imported_type().
  test_two_script_blocks_both_parsed: test_two_script_blocks_both_parsed().
  test_dynamic_import_recovered: test_dynamic_import_recovered().
  test_plain_js_script_block: test_plain_js_script_block().
  test_whole_file_to_js_grammar_would_extract_nothing: test_whole_file_to_js_grammar_would_extract_nothing().
  _targets: _targets().
  test_template_only_file_does_not_crash: test_template_only_file_does_not_crash().
  test_script_setup_extracts_symbols_with_correct_lines: test_script_setup_extracts_symbols_with_correct_lines().
  test_vue_joins_cross_file_symbol_resolution: test_vue_joins_cross_file_symbol_resolution().
  test_vue_is_in_code_extensions: test_vue_is_in_code_extensions().
  test_mask_preserves_line_numbers_and_blanks_markup: test_mask_preserves_line_numbers_and_blanks_markup().
  _labels: _labels().
---
# Module: [`tests/test_vue_extraction.py`](../../../../../raw/code/graphify/tests/test_vue_extraction.py)

## Functions
- `_labels(result: dict)` — [`L34`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L34)
- `_targets(result: dict, *, relation: str | None = None)` — [`L26`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L26)
- `_write(path: Path, body: str)` — [`L20`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L20)
- `test_dynamic_import_recovered(tmp_path)` — [`L158`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L158)
- `test_generic_component_open_tag_with_angle_brackets(tmp_path)` — [`L247`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L247) — A Vue 3.3+ generic= attribute containing '>' (e.g. Record<string, unknown>)
- `test_mask_preserves_line_numbers_and_blanks_markup()` — [`L42`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L42)
- `test_plain_js_script_block(tmp_path)` — [`L174`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L174)
- `test_script_setup_extracts_symbols_with_correct_lines(tmp_path)` — [`L85`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L85)
- `test_script_setup_ts_static_imports_resolve(tmp_path)` — [`L63`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L63)
- `test_template_only_file_does_not_crash(tmp_path)` — [`L190`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L190)
- `test_two_script_blocks_both_parsed(tmp_path)` — [`L134`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L134) — Vue allows a classic ``<script>`` plus ``<script setup>``; both are TS.
- `test_typed_props_reference_imported_type(tmp_path)` — [`L112`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L112)
- `test_vue_is_in_code_extensions()` — [`L38`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L38)
- `test_vue_joins_cross_file_symbol_resolution(tmp_path)` — [`L221`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L221) — A ``.vue`` calling an imported function wires to the real symbol across files.
- `test_whole_file_to_js_grammar_would_extract_nothing(tmp_path)` — [`L198`](../../../../../raw/code/graphify/tests/test_vue_extraction.py#L198) — The SFC must not be parsed as one JS blob.

