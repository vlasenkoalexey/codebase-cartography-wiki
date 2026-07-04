---
title: 'Module: tree_sitter_analyzer/_encoding_detection.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_encoding_detection.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._encoding_detection`/
symbols:
  detect_data_encoding: detect_data_encoding().
  detect_uncached_encoding: detect_uncached_encoding().
  get_cached_encoding: get_cached_encoding().
  is_utf8: is_utf8().
  detect_bom_encoding: detect_bom_encoding().
  detect_with_chardet: detect_with_chardet().
  cache_detected_encoding: cache_detected_encoding().
---
# Module: [`tree_sitter_analyzer/_encoding_detection.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_detection.py)

## Functions
- `cache_detected_encoding(file_path: str | None, cache: Any, encoding: str)` — [`L119`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_detection.py#L119) — Cache a detected encoding when the caller supplied a file path.
- `detect_bom_encoding(data: bytes)` — [`L79`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_detection.py#L79) — Detect UTF BOM encodings after the UTF-8 fast path.
- `detect_data_encoding(data: bytes, *, default_encoding: str, file_path: str | None, cache: Any, chardet_module: Any | None, log_debug: Callable[[str], None])` — [`L7`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_detection.py#L7) — Detect byte encoding with optional file-path cache support.
- `detect_uncached_encoding(data: bytes, *, default_encoding: str, chardet_module: Any | None, log_debug: Callable[[str], None])` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_detection.py#L47) — Detect encoding without consulting or mutating the file cache.
- `detect_with_chardet(data: bytes, *, default_encoding: str, chardet_module: Any | None, log_debug: Callable[[str], None])` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_detection.py#L90) — Use chardet as the slower fallback detector when available.
- `get_cached_encoding(file_path: str | None, cache: Any, log_debug: Callable[[str], None])` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_detection.py#L34) — Return cached encoding for a file path, when available.
- `is_utf8(data: bytes)` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_detection.py#L70) — Return whether data can be decoded as UTF-8.

