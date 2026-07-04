---
title: 'Module: tests/unit/utils/test_text_utils.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_text_utils.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_text_utils`/TestSafePreview#
symbols:
  TestSafePreview.test_text_under_limit: test_text_under_limit().
  TestSafePreview.test_text_over_limit: test_text_over_limit().
  TestSafePreview.test_multiline_flattens: test_multiline_flattens().
  TestSafePreview.test_multiline_with_carriage_return: test_multiline_with_carriage_return().
  TestSafePreview.test_unicode_safe: test_unicode_safe().
  TestSafePreview.test_empty_string: test_empty_string().
  TestSafePreview.test_none_input: test_none_input().
  TestSafePreview.test_custom_max_length: test_custom_max_length().
  TestSafePreview.test_exact_limit: test_exact_limit().
  TestSafePreview: ''
---
# Module: [`tests/unit/utils/test_text_utils.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py)

## Classes
### `TestSafePreview`
- def: [`tests/unit/utils/test_text_utils.py:7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py#L7)
- doc: Tests for safe_preview function.
- signature: `class TestSafePreview:`
- members:
  - `test_custom_max_length(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py#L55) — Should respect custom max_length parameter.
  - `test_empty_string(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py#L46) — Empty string should return empty string.
  - `test_exact_limit(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py#L62) — Text exactly at limit should not be truncated.
  - `test_multiline_flattens(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py#L23) — Multi-line text should be flattened to single line.
  - `test_multiline_with_carriage_return(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py#L30) — Carriage returns should also be removed.
  - `test_none_input(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py#L51) — None input should return empty string (not raise).
  - `test_text_over_limit(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py#L15) — Text over limit should be truncated with ellipsis.
  - `test_text_under_limit(self)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py#L10) — Text under limit should be returned as-is.
  - `test_unicode_safe(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_text_utils.py#L37) — Unicode characters should not be split mid-character.
- uses (calls/refs, reference-scoped): [`safe_preview`](../../../tree_sitter_analyzer/utils/text_utils.md#safe_preview)

