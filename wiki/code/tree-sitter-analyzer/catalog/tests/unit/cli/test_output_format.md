---
title: 'Module: tests/unit/cli/test_output_format.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_output_format.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_output_format`/Test
symbols:
  TestWantsJsonOutput.test_format_json_explicit: WantsJsonOutput#test_format_json_explicit().
  TestWantsJsonOutput.test_output_format_json_fallback: WantsJsonOutput#test_output_format_json_fallback().
  TestWantsJsonOutput.test_format_takes_precedence_over_output_format: WantsJsonOutput#test_format_takes_precedence_over_output_format().
  TestWantsJsonOutput.test_format_text_explicit: WantsJsonOutput#test_format_text_explicit().
  TestWantsJsonOutput.test_output_format_text: WantsJsonOutput#test_output_format_text().
  TestWantsJsonOutput.test_neither_attribute_set: WantsJsonOutput#test_neither_attribute_set().
  TestWantsJsonOutput.test_format_toon: WantsJsonOutput#test_format_toon().
  TestWantsJsonOutput.test_non_json_values_return_false: WantsJsonOutput#test_non_json_values_return_false().
  TestWantsJsonOutput: WantsJsonOutput#
  TestSingleSourceOfTruth: SingleSourceOfTruth#
  TestSingleSourceOfTruth.test_no_duplicate_wants_json_helper: SingleSourceOfTruth#test_no_duplicate_wants_json_helper().
  TestSingleSourceOfTruth.test_no_inline_format_getattr_duplication: SingleSourceOfTruth#test_no_inline_format_getattr_duplication().
---
# Module: [`tests/unit/cli/test_output_format.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py)

## Classes
### `TestSingleSourceOfTruth`
- def: [`tests/unit/cli/test_output_format.py:66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L66)
- doc: r37am: anti-duplication guard — only one definition allowed.
- signature: `class TestSingleSourceOfTruth:`
- members:
  - `test_no_duplicate_wants_json_helper(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L69) — Only ``cli/output_format.py`` may define ``_wants_json*`` helpers.
  - `test_no_inline_format_getattr_duplication(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L100) — r37an: catch the INLINE pattern that r37am's guard missed.

### `TestWantsJsonOutput`
- def: [`tests/unit/cli/test_output_format.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L24)
- doc: Pin behaviour of `wants_json_output` across input shapes.
- signature: `class TestWantsJsonOutput:`
- members:
  - `test_format_json_explicit(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L27)
  - `test_format_takes_precedence_over_output_format(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L35) — ``--format`` should win over ``--output-format`` when both set.
  - `test_format_text_explicit(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L40)
  - `test_format_toon(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L52) — ``--format=toon`` is not JSON — return False.
  - `test_neither_attribute_set(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L48)
  - `test_non_json_values_return_false(self, value)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L60) — Only the exact lowercase string ``"json"`` triggers JSON path.
  - `test_output_format_json_fallback(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L31)
  - `test_output_format_text(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_output_format.py#L44)
- uses (calls/refs, reference-scoped): [`wants_json_output`](../../../tree_sitter_analyzer/cli/output_format.md#wants_json_output)

