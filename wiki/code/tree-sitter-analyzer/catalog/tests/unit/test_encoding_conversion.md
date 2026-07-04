---
title: 'Module: tests/unit/test_encoding_conversion.py'
type: catalog
provenance: extracted
module: tests/unit/test_encoding_conversion.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_encoding_conversion`/Test
symbols:
  TestSafeEncodeText.test_none_input_returns_empty_bytes: SafeEncodeText#test_none_input_returns_empty_bytes().
  TestSafeEncodeText.test_utf8_encoding_succeeds: SafeEncodeText#test_utf8_encoding_succeeds().
  TestSafeEncodeText.test_target_fails_uses_fallback: SafeEncodeText#test_target_fails_uses_fallback().
  TestSafeEncodeText.test_all_encodings_fail_uses_replace: SafeEncodeText#test_all_encodings_fail_uses_replace().
  TestEncodeWithFallbacks.test_skips_target_encoding: EncodeWithFallbacks#test_skips_target_encoding().
  TestEncodeWithFallbacks.test_returns_none_when_all_fail: EncodeWithFallbacks#test_returns_none_when_all_fail().
  TestEncodeWithFallbacks.test_uses_first_working_fallback: EncodeWithFallbacks#test_uses_first_working_fallback().
  TestSafeDecodeBytes.test_none_returns_empty: SafeDecodeBytes#test_none_returns_empty().
  TestSafeDecodeBytes.test_empty_bytes_returns_empty: SafeDecodeBytes#test_empty_bytes_returns_empty().
  TestSafeDecodeBytes.test_utf8_decode_succeeds: SafeDecodeBytes#test_utf8_decode_succeeds().
  TestSafeDecodeBytes.test_uses_detect_encoding_when_none: SafeDecodeBytes#test_uses_detect_encoding_when_none().
  TestSafeDecodeBytes.test_target_fails_uses_fallback: SafeDecodeBytes#test_target_fails_uses_fallback().
  TestSafeDecodeBytes.test_all_fail_uses_replace: SafeDecodeBytes#test_all_fail_uses_replace().
  TestDecodeWithFallbacks.test_skips_target_encoding: DecodeWithFallbacks#test_skips_target_encoding().
  TestDecodeWithFallbacks.test_returns_none_when_all_fail: DecodeWithFallbacks#test_returns_none_when_all_fail().
  TestDecodeWithFallbacks.test_uses_working_fallback: DecodeWithFallbacks#test_uses_working_fallback().
  TestSafeEncodeText: SafeEncodeText#
  TestEncodeWithFallbacks: EncodeWithFallbacks#
  TestSafeDecodeBytes: SafeDecodeBytes#
  TestDecodeWithFallbacks: DecodeWithFallbacks#
---
# Module: [`tests/unit/test_encoding_conversion.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py)

## Classes
### `TestDecodeWithFallbacks`
- def: [`tests/unit/test_encoding_conversion.py:153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L153)
- signature: `class TestDecodeWithFallbacks:`
- members:
  - `test_returns_none_when_all_fail(self)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L159)
  - `test_skips_target_encoding(self)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L154)
  - `test_uses_working_fallback(self)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L163)
- uses (calls/refs, reference-scoped): [`decode_with_fallbacks`](../../tree_sitter_analyzer/_encoding_conversion.md#decode_with_fallbacks)

### `TestEncodeWithFallbacks`
- def: [`tests/unit/test_encoding_conversion.py:61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L61)
- signature: `class TestEncodeWithFallbacks:`
- members:
  - `test_returns_none_when_all_fail(self)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L66)
  - `test_skips_target_encoding(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L62)
  - `test_uses_first_working_fallback(self)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L70)
- uses (calls/refs, reference-scoped): [`encode_with_fallbacks`](../../tree_sitter_analyzer/_encoding_conversion.md#encode_with_fallbacks)

### `TestSafeDecodeBytes`
- def: [`tests/unit/test_encoding_conversion.py:75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L75)
- signature: `class TestSafeDecodeBytes:`
- members:
  - `test_all_fail_uses_replace(self)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L138)
  - `test_empty_bytes_returns_empty(self)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L88)
  - `test_none_returns_empty(self)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L76)
  - `test_target_fails_uses_fallback(self)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L124)
  - `test_uses_detect_encoding_when_none(self)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L112)
  - `test_utf8_decode_succeeds(self)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L100)
- uses (calls/refs, reference-scoped): [`safe_decode_bytes`](../../tree_sitter_analyzer/_encoding_conversion.md#safe_decode_bytes)

### `TestSafeEncodeText`
- def: [`tests/unit/test_encoding_conversion.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L11)
- signature: `class TestSafeEncodeText:`
- members:
  - `test_all_encodings_fail_uses_replace(self)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L47)
  - `test_none_input_returns_empty_bytes(self)` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L12)
  - `test_target_fails_uses_fallback(self)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L34)
  - `test_utf8_encoding_succeeds(self)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_conversion.py#L23)
- uses (calls/refs, reference-scoped): [`safe_encode_text`](../../tree_sitter_analyzer/_encoding_conversion.md#safe_encode_text)

