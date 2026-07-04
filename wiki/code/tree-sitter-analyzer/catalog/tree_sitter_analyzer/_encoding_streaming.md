---
title: 'Module: tree_sitter_analyzer/_encoding_streaming.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_encoding_streaming.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._encoding_streaming`/
symbols:
  read_file_safe_streaming_context: read_file_safe_streaming_context().
  detect_streaming_encoding: detect_streaming_encoding().
  read_encoding_sample: read_encoding_sample().
  open_streaming_context: open_streaming_context().
---
# Module: [`tree_sitter_analyzer/_encoding_streaming.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_streaming.py)

## Functions
- `detect_streaming_encoding(file_path: Path, *, default_encoding: str, detect_encoding: Callable[[bytes, str | None], str], log_warning: Callable[[str], None])` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_streaming.py#L27) — Detect encoding for streaming reads using a small file sample.
- `open_streaming_context(file_path: Path, detected_encoding: str, log_warning: Callable[[str], None])` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_streaming.py#L53) — Open a detected-encoding file handle for line-by-line reading.
- `read_encoding_sample(file_path: Path)` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_streaming.py#L46) — Read the leading bytes used for streaming encoding detection.
- `read_file_safe_streaming_context(file_path: str | Path, *, default_encoding: str, detect_encoding: Callable[[bytes, str | None], str], log_warning: Callable[[str], None])` — [`L9`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_streaming.py#L9) — Return a context manager that streams a file with detected encoding.

