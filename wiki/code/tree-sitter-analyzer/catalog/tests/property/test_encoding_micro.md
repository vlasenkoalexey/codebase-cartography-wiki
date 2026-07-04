---
title: 'Module: tests/property/test_encoding_micro.py'
type: catalog
provenance: extracted
module: tests/property/test_encoding_micro.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.property.test_encoding_micro`/TestEncodingProperties#
symbols:
  TestEncodingProperties.test_encode_decode_roundtrip: test_encode_decode_roundtrip().
  TestEncodingProperties.test_decode_never_raises: test_decode_never_raises().
  TestEncodingProperties: ''
---
# Module: [`tests/property/test_encoding_micro.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_encoding_micro.py)

## Classes
### `TestEncodingProperties`
- def: [`tests/property/test_encoding_micro.py:10`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_encoding_micro.py#L10)
- doc: Verify encode/decode round-trip and idempotency for generic inputs.
- signature: `class TestEncodingProperties:`
- members:
  - `test_decode_never_raises(self, text)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_encoding_micro.py#L22)
  - `test_encode_decode_roundtrip(self, text)` — [`L15`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_encoding_micro.py#L15)
- uses (calls/refs, reference-scoped): [`safe_encode`](../../tree_sitter_analyzer/encoding_utils.md#safe_encode), [`safe_decode`](../../tree_sitter_analyzer/encoding_utils.md#safe_decode)

