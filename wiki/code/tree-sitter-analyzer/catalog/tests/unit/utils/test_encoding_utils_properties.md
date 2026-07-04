---
title: 'Module: tests/unit/utils/test_encoding_utils_properties.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_encoding_utils_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_encoding_utils_properties`/Test
symbols:
  TestEncodingCacheProperties.test_clear_cache_resets_size: EncodingCacheProperties#test_clear_cache_resets_size().
  TestEncodingRoundtripProperties.test_utf8_roundtrip: EncodingRoundtripProperties#test_utf8_roundtrip().
  TestEncodingRoundtripProperties.test_ascii_roundtrip: EncodingRoundtripProperties#test_ascii_roundtrip().
  TestEncodingDetectionProperties.test_detect_encoding_consistency: EncodingDetectionProperties#test_detect_encoding_consistency().
  TestEncodingCacheProperties.test_cache_size_bounded: EncodingCacheProperties#test_cache_size_bounded().
  TestStringEncodingProperties.test_empty_and_whitespace_handling: StringEncodingProperties#test_empty_and_whitespace_handling().
  TestStringEncodingProperties.test_unicode_handling: StringEncodingProperties#test_unicode_handling().
  TestEncodingRoundtripProperties.test_decode_never_raises: EncodingRoundtripProperties#test_decode_never_raises().
  TestEncodingDetectionProperties.test_detect_encoding_returns_valid_encoding: EncodingDetectionProperties#test_detect_encoding_returns_valid_encoding().
  TestEncodingDetectionProperties.test_detect_encoding_with_bom: EncodingDetectionProperties#test_detect_encoding_with_bom().
  TestEncodingCacheProperties.setup_method: EncodingCacheProperties#setup_method().
  TestFileReadingProperties.test_read_file_safe_roundtrip: FileReadingProperties#test_read_file_safe_roundtrip().
  TestFileReadingProperties.test_read_various_file_types: FileReadingProperties#test_read_various_file_types().
  TestEncodingRoundtripProperties: EncodingRoundtripProperties#
  TestEncodingDetectionProperties: EncodingDetectionProperties#
  TestEncodingCacheProperties: EncodingCacheProperties#
  TestFileReadingProperties: FileReadingProperties#
  TestStringEncodingProperties: StringEncodingProperties#
---
# Module: [`tests/unit/utils/test_encoding_utils_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py)

## Classes
### `TestEncodingCacheProperties`
- def: [`tests/unit/utils/test_encoding_utils_properties.py:100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L100)
- doc: Property tests for encoding cache behavior.
- signature: `class TestEncodingCacheProperties:`
- members:
  - `setup_method(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L103) — Clear cache before each test.
  - `test_cache_size_bounded(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L107) — Cache size should be bounded after many operations.
  - `test_clear_cache_resets_size(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L119) — Clearing cache should reset size to 0.
- uses (calls/refs, reference-scoped): [`detect_encoding`](../../../tree_sitter_analyzer/encoding_utils.md#detect_encoding), [`get_encoding_cache_size`](../../../tree_sitter_analyzer/encoding_utils.md#get_encoding_cache_size), [`clear_encoding_cache`](../../../tree_sitter_analyzer/encoding_utils.md#clear_encoding_cache)

### `TestEncodingDetectionProperties`
- def: [`tests/unit/utils/test_encoding_utils_properties.py:65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L65)
- doc: Property tests for encoding detection.
- signature: `class TestEncodingDetectionProperties:`
- members:
  - `test_detect_encoding_consistency(self, text: str)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L82) — detect_encoding should return consistent results for same input.
  - `test_detect_encoding_returns_valid_encoding(self, text: str)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L70) — detect_encoding should return a valid encoding name.
  - `test_detect_encoding_with_bom(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L93) — UTF-8 BOM should be detected as UTF-8.
- uses (calls/refs, reference-scoped): [`detect_encoding`](../../../tree_sitter_analyzer/encoding_utils.md#detect_encoding), [`clear_encoding_cache`](../../../tree_sitter_analyzer/encoding_utils.md#clear_encoding_cache)

### `TestEncodingRoundtripProperties`
- def: [`tests/unit/utils/test_encoding_utils_properties.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L23)
- doc: Property tests for encoding/decoding roundtrip consistency.
- signature: `class TestEncodingRoundtripProperties:`
- members:
  - `test_ascii_roundtrip(self, text: str)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L45) — ASCII encode/decode should be lossless for ASCII text.
  - `test_decode_never_raises(self, data: bytes)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L56) — safe_decode should never raise an exception.
  - `test_utf8_roundtrip(self, text: str)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L28) — UTF-8 encode/decode should be lossless for any text.
- uses (calls/refs, reference-scoped): [`safe_encode`](../../../tree_sitter_analyzer/encoding_utils.md#safe_encode), [`safe_decode`](../../../tree_sitter_analyzer/encoding_utils.md#safe_decode)

### `TestFileReadingProperties`
- def: [`tests/unit/utils/test_encoding_utils_properties.py:130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L130)
- doc: Property tests for file reading operations.
- signature: `class TestFileReadingProperties:`
- members:
  - `test_read_file_safe_roundtrip(self, text: str)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L135) — read_file_safe should read back what was written.
  - `test_read_various_file_types(self, content: str, extension: str)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L157) — read_file_safe should handle various file types.
- uses (calls/refs, reference-scoped): [`read_file_safe`](../../../tree_sitter_analyzer/encoding_utils.md#read_file_safe)

### `TestStringEncodingProperties`
- def: [`tests/unit/utils/test_encoding_utils_properties.py:176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L176)
- doc: Property tests for string encoding edge cases.
- signature: `class TestStringEncodingProperties:`
- members:
  - `test_empty_and_whitespace_handling(self, text: str)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L181) — Empty and whitespace strings should be handled correctly.
  - `test_unicode_handling(self, text: str)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_properties.py#L202) — Unicode text should be handled correctly.
- uses (calls/refs, reference-scoped): [`safe_encode`](../../../tree_sitter_analyzer/encoding_utils.md#safe_encode), [`safe_decode`](../../../tree_sitter_analyzer/encoding_utils.md#safe_decode)

