---
title: 'Module: tests/unit/formatters/test_java_formatter_signatures.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_java_formatter_signatures.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_java_formatter_signatures`/
symbols:
  _make_simple_data: _make_simple_data().
  TestJavaSignaturesMode.test_header_contains_signatures_marker: TestJavaSignaturesMode#test_header_contains_signatures_marker().
  TestJavaSignaturesMode.test_method_lines_present: TestJavaSignaturesMode#test_method_lines_present().
  TestJavaSignaturesMode.test_param_count_not_types: TestJavaSignaturesMode#test_param_count_not_types().
  TestJavaSignaturesMode.test_class_group_header_present: TestJavaSignaturesMode#test_class_group_header_present().
  TestJavaSignaturesMode.test_line_range_in_method_output: TestJavaSignaturesMode#test_line_range_in_method_output().
  TestJavaSignaturesMode.test_next_step_hint_present: TestJavaSignaturesMode#test_next_step_hint_present().
  TestJavaSignaturesMode.test_fields_shown_when_few: TestJavaSignaturesMode#test_fields_shown_when_few().
  TestJavaSignaturesMode.test_no_full_signatures_bloat: TestJavaSignaturesMode#test_no_full_signatures_bloat().
  TestJavaSignaturesMode.test_multi_class_grouping: TestJavaSignaturesMode#test_multi_class_grouping().
  TestJavaSignaturesMode.test_package_line_in_output: TestJavaSignaturesMode#test_package_line_in_output().
  test_base_formatter_signatures_dispatch_to_mixin: test_base_formatter_signatures_dispatch_to_mixin().
  test_default_formatter_signatures_dispatch: test_default_formatter_signatures_dispatch().
  test_formatter_registry_returns_formatter_for_signatures: test_formatter_registry_returns_formatter_for_signatures().
  test_base_formatter_signatures_raises_for_unsupported: test_base_formatter_signatures_raises_for_unsupported().
  test_method_sig_line_shape: test_method_sig_line_shape().
  test_shorten_return_type: test_shorten_return_type().
  test_validate_format_type_accepts_signatures: test_validate_format_type_accepts_signatures().
  test_validate_format_type_still_rejects_unknown: test_validate_format_type_still_rejects_unknown().
  TestJavaSignaturesMode: TestJavaSignaturesMode#
---
# Module: [`tests/unit/formatters/test_java_formatter_signatures.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py)

## Classes
### `TestJavaSignaturesMode`
- def: [`tests/unit/formatters/test_java_formatter_signatures.py:166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L166)
- signature: `class TestJavaSignaturesMode:`
- members:
  - `test_class_group_header_present(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L191)
  - `test_fields_shown_when_few(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L208)
  - `test_header_contains_signatures_marker(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L167)
  - `test_line_range_in_method_output(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L196)
  - `test_method_lines_present(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L172)
  - `test_multi_class_grouping(self)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L225) — Each top-level class gets its own block (non-overlapping ranges).
  - `test_next_step_hint_present(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L202)
  - `test_no_full_signatures_bloat(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L214) — Ensure signatures output is shorter than full output.
  - `test_package_line_in_output(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L242)
  - `test_param_count_not_types(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L178) — Signatures mode must show Np, not full type lists.
- uses (calls/refs, reference-scoped): [`format_structure`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter.format_structure), [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter)  (1 test-only)

## Functions
- `_make_simple_data(*, package: str = "com.example", class_name: str = "MyClass", n_methods: int = 3, n_fields: int = 2)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L112) — Build minimal structure data for the formatter.
- `test_base_formatter_signatures_dispatch_to_mixin()` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L253) — format_structure("signatures") routes to _format_signatures_table when present.
- `test_base_formatter_signatures_raises_for_unsupported()` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L262) — A formatter without _format_signatures_table raises ValueError.
- `test_default_formatter_signatures_dispatch()` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L277)
- `test_formatter_registry_returns_formatter_for_signatures()` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L290)
- `test_method_sig_line_shape(method: dict, expected_contains: list[str])` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L80)
- `test_shorten_return_type(return_type: str, expected: str)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L103)
- `test_validate_format_type_accepts_signatures()` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L302)
- `test_validate_format_type_still_rejects_unknown()` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_signatures.py#L307)

