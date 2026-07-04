---
title: 'Module: tests/unit/core/test_streaming_file_reading.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_streaming_file_reading.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_streaming_file_reading`/TestStreamingFileReading#
symbols:
  TestStreamingFileReading.test_streaming_basic_reading: test_streaming_basic_reading().
  TestStreamingFileReading.test_streaming_line_by_line: test_streaming_line_by_line().
  TestStreamingFileReading.test_streaming_with_start_line: test_streaming_with_start_line().
  TestStreamingFileReading.test_streaming_empty_file: test_streaming_empty_file().
  TestStreamingFileReading.test_streaming_unicode_content: test_streaming_unicode_content().
  TestStreamingFileReading.test_streaming_large_file_memory_efficiency: test_streaming_large_file_memory_efficiency().
  TestStreamingFileReading.test_streaming_nonexistent_file: test_streaming_nonexistent_file().
  TestStreamingFileReading.test_streaming_encoding_detection: test_streaming_encoding_detection().
  TestStreamingFileReading.test_streaming_different_line_endings: test_streaming_different_line_endings().
  TestStreamingFileReading.test_streaming_pathlib_path: test_streaming_pathlib_path().
  TestStreamingFileReading: ''
---
# Module: [`tests/unit/core/test_streaming_file_reading.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py)

## Classes
### `TestStreamingFileReading`
- def: [`tests/unit/core/test_streaming_file_reading.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L16)
- doc: Test cases for streaming file reading
- signature: `class TestStreamingFileReading:`
- members:
  - `test_streaming_basic_reading(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L19) — Test basic streaming file reading
  - `test_streaming_different_line_endings(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L154) — Test streaming with different line ending styles
  - `test_streaming_empty_file(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L77) — Test streaming with empty file
  - `test_streaming_encoding_detection(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L139) — Test automatic encoding detection in streaming mode
  - `test_streaming_large_file_memory_efficiency(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L111) — Test that streaming doesn't load entire file into memory
  - `test_streaming_line_by_line(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L39) — Test streaming with line-by-line iteration
  - `test_streaming_nonexistent_file(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L133) — Test streaming with nonexistent file
  - `test_streaming_pathlib_path(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L170) — Test streaming accepts pathlib.Path
  - `test_streaming_unicode_content(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L91) — Test streaming with Unicode content
  - `test_streaming_with_start_line(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_streaming_file_reading.py#L58) — Test streaming starting from specific line
- uses (calls/refs, reference-scoped): [`read_file_safe_streaming`](../../../tree_sitter_analyzer/encoding_utils.md#read_file_safe_streaming)

