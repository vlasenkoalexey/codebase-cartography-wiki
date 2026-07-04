---
title: 'Module: tests/integration/test_encoding_pipeline.py'
type: catalog
provenance: extracted
module: tests/integration/test_encoding_pipeline.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_encoding_pipeline`/TestEncodingPipeline#
symbols:
  TestEncodingPipeline.test_utf8_file: test_utf8_file().
  TestEncodingPipeline.test_latin1_file: test_latin1_file().
  TestEncodingPipeline.test_shift_jis_file: test_shift_jis_file().
  TestEncodingPipeline.test_empty_file: test_empty_file().
  TestEncodingPipeline.test_binary_file: test_binary_file().
  TestEncodingPipeline: ''
---
# Module: [`tests/integration/test_encoding_pipeline.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_encoding_pipeline.py)

## Classes
### `TestEncodingPipeline`
- def: [`tests/integration/test_encoding_pipeline.py:10`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_encoding_pipeline.py#L10)
- signature: `class TestEncodingPipeline:`
- members:
  - `test_binary_file(self, tmp_path: Path)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_encoding_pipeline.py#L36)
  - `test_empty_file(self, tmp_path: Path)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_encoding_pipeline.py#L30)
  - `test_latin1_file(self, tmp_path: Path)` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_encoding_pipeline.py#L17)
  - `test_shift_jis_file(self, tmp_path: Path)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_encoding_pipeline.py#L23)
  - `test_utf8_file(self, tmp_path: Path)` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_encoding_pipeline.py#L11)
- uses (calls/refs, reference-scoped): [`detect_encoding`](../../tree_sitter_analyzer/encoding_utils.md#detect_encoding)

