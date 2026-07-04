---
title: 'Module: tests/unit/utils/test_encoding_utils_edge_cases.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_encoding_utils_edge_cases.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_encoding_utils_edge_cases`/Test
symbols:
  TestEncodingManagerEdge.test_clear_cache: EncodingManagerEdge#test_clear_cache().
  TestEncodingManagerEdge.test_get_encoding_cache_size: EncodingManagerEdge#test_get_encoding_cache_size().
  TestEncodingCache.test_get_miss: EncodingCache#test_get_miss().
  TestEncodingCache.test_set_and_get: EncodingCache#test_set_and_get().
  TestEncodingCache.test_ttl_expiry: EncodingCache#test_ttl_expiry().
  TestEncodingCache.test_max_size_eviction: EncodingCache#test_max_size_eviction().
  TestEncodingCache.test_cleanup_expired_removes_stale: EncodingCache#test_cleanup_expired_removes_stale().
  TestEncodingCache.test_size: EncodingCache#test_size().
  TestEncodingManagerEdge.test_safe_decode_empty_data: EncodingManagerEdge#test_safe_decode_empty_data().
  TestEncodingManagerEdge.test_safe_decode_with_errors: EncodingManagerEdge#test_safe_decode_with_errors().
  TestEncodingManagerEdge.test_detect_encoding_utf8_bom: EncodingManagerEdge#test_detect_encoding_utf8_bom().
  TestEncodingManagerEdge.test_detect_encoding_ascii: EncodingManagerEdge#test_detect_encoding_ascii().
  TestEncodingManagerEdge.test_detect_encoding_chardet_none_result: EncodingManagerEdge#test_detect_encoding_chardet_none_result().
  TestEncodingManagerEdge.test_cleanup_expired_on_eviction: EncodingManagerEdge#test_cleanup_expired_on_eviction().
  TestDetectEncodingBOM.test_utf16_be_bom: DetectEncodingBOM#test_utf16_be_bom().
  TestDetectEncodingBOM.test_utf16_le_bom: DetectEncodingBOM#test_utf16_le_bom().
  TestDetectEncodingBOM.test_chardet_high_confidence: DetectEncodingBOM#test_chardet_high_confidence().
  TestDetectEncodingBOM.test_chardet_exception_falls_back: DetectEncodingBOM#test_chardet_exception_falls_back().
  TestNormalizeLineEndings.test_empty_string: NormalizeLineEndings#test_empty_string().
  TestNormalizeLineEndings.test_none_like_empty: NormalizeLineEndings#test_none_like_empty().
  TestNormalizeLineEndings.test_windows_line_endings: NormalizeLineEndings#test_windows_line_endings().
  TestNormalizeLineEndings.test_mac_line_endings: NormalizeLineEndings#test_mac_line_endings().
  TestWriteFileSafeOSError.test_write_to_readonly_dir: WriteFileSafeOSError#test_write_to_readonly_dir().
  TestSafeDecodeFallbacks.test_safe_decode_with_invalid_utf8: SafeDecodeFallbacks#test_safe_decode_with_invalid_utf8().
  TestSafeDecodeFallbacks.test_safe_decode_wrong_encoding_label: SafeDecodeFallbacks#test_safe_decode_wrong_encoding_label().
  TestSafeDecodeFallbacks.test_safe_decode_no_match_uses_replace: SafeDecodeFallbacks#test_safe_decode_no_match_uses_replace().
  TestSafeEncodeFallbacks.test_safe_encode_none: SafeEncodeFallbacks#test_safe_encode_none().
  TestEncodingManagerEdge.test_read_file_safe_permission_error: EncodingManagerEdge#test_read_file_safe_permission_error().
  TestEncodingManagerEdge.test_extract_text_slice_basic: EncodingManagerEdge#test_extract_text_slice_basic().
  TestEncodingManagerEdge.test_extract_text_slice_oob: EncodingManagerEdge#test_extract_text_slice_oob().
  TestReadFileSafeEmpty.test_read_empty_file: ReadFileSafeEmpty#test_read_empty_file().
  TestAsyncReadFileSafe.test_read_async_basic: AsyncReadFileSafe#test_read_async_basic().
  TestAsyncReadFileSafe.test_read_async_empty_file: AsyncReadFileSafe#test_read_async_empty_file().
  TestAsyncReadFileSafe.test_read_async_nonexistent: AsyncReadFileSafe#test_read_async_nonexistent().
  TestStreamingRead.test_streaming_read_basic: StreamingRead#test_streaming_read_basic().
  TestStreamingRead.test_streaming_read_empty_file: StreamingRead#test_streaming_read_empty_file().
  TestStreamingRead.test_streaming_read_nonexistent: StreamingRead#test_streaming_read_nonexistent().
  TestEncodingCache: EncodingCache#
  TestEncodingManagerEdge: EncodingManagerEdge#
  TestDetectEncodingBOM: DetectEncodingBOM#
  TestNormalizeLineEndings: NormalizeLineEndings#
  TestReadFileSafeEmpty: ReadFileSafeEmpty#
  TestWriteFileSafeOSError: WriteFileSafeOSError#
  TestAsyncReadFileSafe: AsyncReadFileSafe#
  TestStreamingRead: StreamingRead#
  TestSafeDecodeFallbacks: SafeDecodeFallbacks#
  TestSafeEncodeFallbacks: SafeEncodeFallbacks#
---
# Module: [`tests/unit/utils/test_encoding_utils_edge_cases.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py)

## Classes
### `TestAsyncReadFileSafe`
- def: [`tests/unit/utils/test_encoding_utils_edge_cases.py:200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L200)
- signature: `class TestAsyncReadFileSafe:`
- members:
  - `test_read_async_basic(self, tmp_path)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L202)
  - `test_read_async_empty_file(self, tmp_path)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L212)
  - `test_read_async_nonexistent(self, tmp_path)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L222)
- uses (calls/refs, reference-scoped): [`read_file_safe_async`](../../../tree_sitter_analyzer/encoding_utils.md#read_file_safe_async)

### `TestDetectEncodingBOM`
- def: [`tests/unit/utils/test_encoding_utils_edge_cases.py:132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L132)
- signature: `class TestDetectEncodingBOM:`
- members:
  - `test_chardet_exception_falls_back(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L155)
  - `test_chardet_high_confidence(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L144)
  - `test_utf16_be_bom(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L133)
  - `test_utf16_le_bom(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L138)
- uses (calls/refs, reference-scoped): [`EncodingManager`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager), [`detect_encoding`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.detect_encoding)

### `TestEncodingCache`
- def: [`tests/unit/utils/test_encoding_utils_edge_cases.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L21)
- signature: `class TestEncodingCache:`
- members:
  - `test_cleanup_expired_removes_stale(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L43)
  - `test_get_miss(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L22)
  - `test_max_size_eviction(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L37)
  - `test_set_and_get(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L26)
  - `test_size(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L51)
  - `test_ttl_expiry(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L31)
- uses (calls/refs, reference-scoped): [`get`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingCache.get), [`EncodingCache`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingCache), [`size`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingCache.size)

### `TestEncodingManagerEdge`
- def: [`tests/unit/utils/test_encoding_utils_edge_cases.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L58)
- signature: `class TestEncodingManagerEdge:`
- members:
  - `test_cleanup_expired_on_eviction(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L123)
  - `test_clear_cache(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L108)
  - `test_detect_encoding_ascii(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L73)
  - `test_detect_encoding_chardet_none_result(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L78)
  - `test_detect_encoding_utf8_bom(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L68)
  - `test_extract_text_slice_basic(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L99)
  - `test_extract_text_slice_oob(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L103)
  - `test_get_encoding_cache_size(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L115)
  - `test_read_file_safe_permission_error(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L87)
  - `test_safe_decode_empty_data(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L59)
  - `test_safe_decode_with_errors(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L63)
- uses (calls/refs, reference-scoped): [`EncodingManager`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager), [`read_file_safe`](../../../tree_sitter_analyzer/encoding_utils.md#read_file_safe), [`extract_text_slice`](../../../tree_sitter_analyzer/encoding_utils.md#extract_text_slice), [`safe_decode`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.safe_decode), [`detect_encoding`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.detect_encoding), [`get_encoding_cache_size`](../../../tree_sitter_analyzer/encoding_utils.md#get_encoding_cache_size), [`clear_encoding_cache`](../../../tree_sitter_analyzer/encoding_utils.md#clear_encoding_cache), [`EncodingCache`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingCache), [`size`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingCache.size), [`_encoding_cache`](../../../tree_sitter_analyzer/encoding_utils.md#_encoding_cache)

### `TestNormalizeLineEndings`
- def: [`tests/unit/utils/test_encoding_utils_edge_cases.py:163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L163)
- signature: `class TestNormalizeLineEndings:`
- members:
  - `test_empty_string(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L164)
  - `test_mac_line_endings(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L173)
  - `test_none_like_empty(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L167)
  - `test_windows_line_endings(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L170)
- uses (calls/refs, reference-scoped): [`EncodingManager`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager), [`normalize_line_endings`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.normalize_line_endings)

### `TestReadFileSafeEmpty`
- def: [`tests/unit/utils/test_encoding_utils_edge_cases.py:177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L177)
- signature: `class TestReadFileSafeEmpty:`
- members:
  - `test_read_empty_file(self, tmp_path)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L178)
- uses (calls/refs, reference-scoped): [`read_file_safe`](../../../tree_sitter_analyzer/encoding_utils.md#read_file_safe)

### `TestSafeDecodeFallbacks`
- def: [`tests/unit/utils/test_encoding_utils_edge_cases.py:257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L257)
- signature: `class TestSafeDecodeFallbacks:`
- members:
  - `test_safe_decode_no_match_uses_replace(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L267)
  - `test_safe_decode_with_invalid_utf8(self)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L258)
  - `test_safe_decode_wrong_encoding_label(self)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L262)
- uses (calls/refs, reference-scoped): [`EncodingManager`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager), [`safe_decode`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.safe_decode)

### `TestSafeEncodeFallbacks`
- def: [`tests/unit/utils/test_encoding_utils_edge_cases.py:273`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L273)
- signature: `class TestSafeEncodeFallbacks:`
- members:
  - `test_safe_encode_none(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L274)
- uses (calls/refs, reference-scoped): [`EncodingManager`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager), [`safe_encode`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.safe_encode)

### `TestStreamingRead`
- def: [`tests/unit/utils/test_encoding_utils_edge_cases.py:229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L229)
- signature: `class TestStreamingRead:`
- members:
  - `test_streaming_read_basic(self, tmp_path)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L230)
  - `test_streaming_read_empty_file(self, tmp_path)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L240)
  - `test_streaming_read_nonexistent(self, tmp_path)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L250)
- uses (calls/refs, reference-scoped): [`read_file_safe_streaming`](../../../tree_sitter_analyzer/encoding_utils.md#read_file_safe_streaming)

### `TestWriteFileSafeOSError`
- def: [`tests/unit/utils/test_encoding_utils_edge_cases.py:186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L186)
- signature: `class TestWriteFileSafeOSError:`
- members:
  - `test_write_to_readonly_dir(self, tmp_path)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_encoding_utils_edge_cases.py#L187)
- uses (calls/refs, reference-scoped): [`EncodingManager`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager), [`write_file_safe`](../../../tree_sitter_analyzer/encoding_utils.md#EncodingManager.write_file_safe)

