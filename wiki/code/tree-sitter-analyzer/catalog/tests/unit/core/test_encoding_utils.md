---
title: 'Module: tests/unit/core/test_encoding_utils.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_encoding_utils.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_encoding_utils`/Test
symbols:
  TestEncodingManager.test_detect_encoding_empty: EncodingManager#test_detect_encoding_empty().
  TestFileOperations.test_write_file_safe_basic: FileOperations#test_write_file_safe_basic().
  TestFileOperations.test_write_file_safe_unicode: FileOperations#test_write_file_safe_unicode().
  TestFileOperations.test_read_write_roundtrip: FileOperations#test_read_write_roundtrip().
  TestEncodingManager.test_safe_encode_basic: EncodingManager#test_safe_encode_basic().
  TestEncodingManager.test_safe_encode_unicode: EncodingManager#test_safe_encode_unicode().
  TestEncodingManager.test_safe_encode_none: EncodingManager#test_safe_encode_none().
  TestEncodingManager.test_safe_encode_empty_string: EncodingManager#test_safe_encode_empty_string().
  TestEncodingManager.test_safe_decode_basic: EncodingManager#test_safe_decode_basic().
  TestEncodingManager.test_safe_decode_unicode: EncodingManager#test_safe_decode_unicode().
  TestEncodingManager.test_safe_decode_none: EncodingManager#test_safe_decode_none().
  TestEncodingManager.test_safe_decode_empty_bytes: EncodingManager#test_safe_decode_empty_bytes().
  TestEncodingManager.test_detect_encoding_utf8: EncodingManager#test_detect_encoding_utf8().
  TestEncodingManager.test_normalize_line_endings: EncodingManager#test_normalize_line_endings().
  TestEncodingManager.test_extract_text_slice: EncodingManager#test_extract_text_slice().
  TestEncodingManager.test_extract_text_slice_unicode: EncodingManager#test_extract_text_slice_unicode().
  TestEncodingManager.test_extract_text_slice_invalid_bounds: EncodingManager#test_extract_text_slice_invalid_bounds().
  TestFileOperations.test_read_file_safe_basic: FileOperations#test_read_file_safe_basic().
  TestFileOperations.test_read_file_safe_unicode: FileOperations#test_read_file_safe_unicode().
  TestFileOperations.test_read_file_safe_nonexistent: FileOperations#test_read_file_safe_nonexistent().
  TestErrorHandling.test_encoding_with_invalid_characters: ErrorHandling#test_encoding_with_invalid_characters().
  TestErrorHandling.test_large_content_handling: ErrorHandling#test_large_content_handling().
  TestConvenienceFunctions.test_safe_encode_function: ConvenienceFunctions#test_safe_encode_function().
  TestConvenienceFunctions.test_safe_decode_function: ConvenienceFunctions#test_safe_decode_function().
  TestConvenienceFunctions.test_detect_encoding_function: ConvenienceFunctions#test_detect_encoding_function().
  TestConvenienceFunctions.test_read_file_safe_function: ConvenienceFunctions#test_read_file_safe_function().
  TestConvenienceFunctions.test_write_file_safe_function: ConvenienceFunctions#test_write_file_safe_function().
  TestConvenienceFunctions.test_extract_text_slice_function: ConvenienceFunctions#test_extract_text_slice_function().
  TestErrorHandling.test_mixed_encoding_content: ErrorHandling#test_mixed_encoding_content().
  TestEncodingManager: EncodingManager#
  TestFileOperations: FileOperations#
  TestConvenienceFunctions: ConvenienceFunctions#
  TestErrorHandling: ErrorHandling#
---
# Module: [`tests/unit/core/test_encoding_utils.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py)

## Classes
### `TestConvenienceFunctions`
- def: [`tests/unit/core/test_encoding_utils.py:287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L287)
- doc: Test module-level convenience functions
- signature: `class TestConvenienceFunctions:`
- members:
  - `test_detect_encoding_function(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L302) — Test detect_encoding convenience function
  - `test_extract_text_slice_function(self)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L342) — Test extract_text_slice convenience function
  - `test_read_file_safe_function(self)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L308) — Test read_file_safe convenience function
  - `test_safe_decode_function(self)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L296) — Test safe_decode convenience function
  - `test_safe_encode_function(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L290) — Test safe_encode convenience function
  - `test_write_file_safe_function(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L326) — Test write_file_safe convenience function
- uses (calls/refs, reference-scoped): [`read_file_safe`](../../../tree_sitter_analyzer/encoding_utils.md#read_file_safe), [`safe_encode`](../../../tree_sitter_analyzer/encoding_utils.md#safe_encode), [`extract_text_slice`](../../../tree_sitter_analyzer/encoding_utils.md#extract_text_slice), [`detect_encoding`](../../../tree_sitter_analyzer/encoding_utils.md#detect_encoding), [`safe_decode`](../../../tree_sitter_analyzer/encoding_utils.md#safe_decode), [`write_file_safe`](../../../tree_sitter_analyzer/encoding_utils.md#write_file_safe)

### `TestEncodingManager`
- def: [`tests/unit/core/test_encoding_utils.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L25)
- doc: Test cases for EncodingManager class
- signature: `class TestEncodingManager:`
- members:
  - `test_detect_encoding_empty(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L87) — Test encoding detection with empty data
  - `test_detect_encoding_utf8(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L78) — Test encoding detection for UTF-8
  - `test_extract_text_slice(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L114) — Test text slice extraction
  - `test_extract_text_slice_invalid_bounds(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L142) — Test text slice extraction with invalid bounds
  - `test_extract_text_slice_unicode(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L128) — Test text slice extraction with unicode
  - `test_normalize_line_endings(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L92) — Test line ending normalization
  - `test_safe_decode_basic(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L54) — Test basic decoding functionality
  - `test_safe_decode_empty_bytes(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L73) — Test decoding with empty bytes
  - `test_safe_decode_none(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L68) — Test decoding with None input
  - `test_safe_decode_unicode(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L61) — Test decoding with unicode bytes
  - `test_safe_encode_basic(self)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L28) — Test basic encoding functionality
  - `test_safe_encode_empty_string(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L49) — Test encoding with empty string
  - `test_safe_encode_none(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L44) — Test encoding with None input
  - `test_safe_encode_unicode(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L35) — Test encoding with unicode characters
- uses (calls/refs, reference-scoped): [`EncodingManager`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager), [`safe_decode`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.safe_decode), [`detect_encoding`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.detect_encoding), [`safe_encode`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.safe_encode), [`normalize_line_endings`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.normalize_line_endings), [`DEFAULT_ENCODING`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.DEFAULT_ENCODING), [`extract_text_slice`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.extract_text_slice)

### `TestErrorHandling`
- def: [`tests/unit/core/test_encoding_utils.py:350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L350)
- doc: Test error handling and edge cases
- signature: `class TestErrorHandling:`
- members:
  - `test_encoding_with_invalid_characters(self, test_string)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L361) — Test encoding with potentially problematic characters
  - `test_large_content_handling(self)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L370) — Test handling of large content
  - `test_mixed_encoding_content(self)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L382) — Test content that might have mixed encoding issues
- uses (calls/refs, reference-scoped): [`safe_encode`](../../../tree_sitter_analyzer/encoding_utils.md#safe_encode), [`safe_decode`](../../../tree_sitter_analyzer/encoding_utils.md#safe_decode)

### `TestFileOperations`
- def: [`tests/unit/core/test_encoding_utils.py:159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L159)
- doc: Test file reading/writing operations
- signature: `class TestFileOperations:`
- members:
  - `test_read_file_safe_basic(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L162) — Test safe file reading
  - `test_read_file_safe_nonexistent(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L203) — Test safe file reading with nonexistent file
  - `test_read_file_safe_unicode(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L183) — Test safe file reading with unicode content
  - `test_read_write_roundtrip(self)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L248) — Test read-write roundtrip consistency
  - `test_write_file_safe_basic(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L208) — Test safe file writing
  - `test_write_file_safe_unicode(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_utils.py#L228) — Test safe file writing with unicode
- uses (calls/refs, reference-scoped): [`EncodingManager`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager), [`read_file_safe`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.read_file_safe), [`write_file_safe`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.write_file_safe)

