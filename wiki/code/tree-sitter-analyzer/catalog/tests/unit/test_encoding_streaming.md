---
title: 'Module: tests/unit/test_encoding_streaming.py'
type: catalog
provenance: extracted
module: tests/unit/test_encoding_streaming.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_encoding_streaming`/Test
symbols:
  TestReadEncodingSample.test_reads_first_8192_bytes: ReadEncodingSample#test_reads_first_8192_bytes().
  TestReadEncodingSample.test_small_file_returns_all: ReadEncodingSample#test_small_file_returns_all().
  TestReadEncodingSample.test_empty_file_returns_empty: ReadEncodingSample#test_empty_file_returns_empty().
  TestReadEncodingSample.test_nonexistent_file_raises: ReadEncodingSample#test_nonexistent_file_raises().
  TestDetectStreamingEncoding.test_empty_file_returns_default: DetectStreamingEncoding#test_empty_file_returns_default().
  TestDetectStreamingEncoding.test_detects_encoding_from_sample: DetectStreamingEncoding#test_detects_encoding_from_sample().
  TestDetectStreamingEncoding.test_oserror_logs_and_reraises: DetectStreamingEncoding#test_oserror_logs_and_reraises().
  TestOpenStreamingContext.test_reads_file_with_encoding: OpenStreamingContext#test_reads_file_with_encoding().
  TestOpenStreamingContext.test_invalid_encoding_reraises: OpenStreamingContext#test_invalid_encoding_reraises().
  TestOpenStreamingContext.test_errors_replace_mode: OpenStreamingContext#test_errors_replace_mode().
  TestReadFileSafeStreamingContext.test_end_to_end_streaming: ReadFileSafeStreamingContext#test_end_to_end_streaming().
  TestReadFileSafeStreamingContext.test_string_path_accepted: ReadFileSafeStreamingContext#test_string_path_accepted().
  TestReadEncodingSample: ReadEncodingSample#
  TestDetectStreamingEncoding: DetectStreamingEncoding#
  TestOpenStreamingContext: OpenStreamingContext#
  TestReadFileSafeStreamingContext: ReadFileSafeStreamingContext#
---
# Module: [`tests/unit/test_encoding_streaming.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py)

## Classes
### `TestDetectStreamingEncoding`
- def: [`tests/unit/test_encoding_streaming.py:42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L42)
- doc: Tests for detect_streaming_encoding.
- signature: `class TestDetectStreamingEncoding:`
- members:
  - `test_detects_encoding_from_sample(self, tmp_path)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L56)
  - `test_empty_file_returns_default(self, tmp_path)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L45)
  - `test_oserror_logs_and_reraises(self, tmp_path)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L67)
- uses (calls/refs, reference-scoped): [`detect_streaming_encoding`](../../tree_sitter_analyzer/_encoding_streaming.md#detect_streaming_encoding)

### `TestOpenStreamingContext`
- def: [`tests/unit/test_encoding_streaming.py:82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L82)
- doc: Tests for open_streaming_context.
- signature: `class TestOpenStreamingContext:`
- members:
  - `test_errors_replace_mode(self, tmp_path)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L102)
  - `test_invalid_encoding_reraises(self, tmp_path)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L93)
  - `test_reads_file_with_encoding(self, tmp_path)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L85)
- uses (calls/refs, reference-scoped): [`open_streaming_context`](../../tree_sitter_analyzer/_encoding_streaming.md#open_streaming_context)

### `TestReadEncodingSample`
- def: [`tests/unit/test_encoding_streaming.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L15)
- doc: Tests for read_encoding_sample.
- signature: `class TestReadEncodingSample:`
- members:
  - `test_empty_file_returns_empty(self, tmp_path)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L30)
  - `test_nonexistent_file_raises(self, tmp_path)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L36)
  - `test_reads_first_8192_bytes(self, tmp_path)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L18)
  - `test_small_file_returns_all(self, tmp_path)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L24)
- uses (calls/refs, reference-scoped): [`read_encoding_sample`](../../tree_sitter_analyzer/_encoding_streaming.md#read_encoding_sample)

### `TestReadFileSafeStreamingContext`
- def: [`tests/unit/test_encoding_streaming.py:112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L112)
- doc: Tests for read_file_safe_streaming_context.
- signature: `class TestReadFileSafeStreamingContext:`
- members:
  - `test_end_to_end_streaming(self, tmp_path)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L115)
  - `test_string_path_accepted(self, tmp_path)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_encoding_streaming.py#L127)
- uses (calls/refs, reference-scoped): [`read_file_safe_streaming_context`](../../tree_sitter_analyzer/_encoding_streaming.md#read_file_safe_streaming_context)

