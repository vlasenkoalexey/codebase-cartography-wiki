---
title: 'Module: tree_sitter_analyzer/_encoding_conversion.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_encoding_conversion.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._encoding_conversion`/
symbols:
  safe_decode_bytes: safe_decode_bytes().
  safe_encode_text: safe_encode_text().
  encode_with_fallbacks: encode_with_fallbacks().
  decode_with_fallbacks: decode_with_fallbacks().
---
# Module: [`tree_sitter_analyzer/_encoding_conversion.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_conversion.py)

## Functions
- `decode_with_fallbacks(data: bytes, target_encoding: str, fallback_encodings: Sequence[str])` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_conversion.py#L74) — Try fallback decoders, skipping the encoding that already failed.
- `encode_with_fallbacks(text: str, target_encoding: str, fallback_encodings: Sequence[str])` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_conversion.py#L32) — Try fallback encodings, skipping the encoding that already failed.
- `safe_decode_bytes(data: bytes | None, *, encoding: str | None, default_encoding: str, fallback_encodings: Sequence[str], detect_encoding: Callable[[bytes], str], log_debug: Callable[[str], None], log_warning: Callable[[str], None])` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_conversion.py#L46) — Decode bytes with detected encoding and configured fallbacks.
- `safe_encode_text(text: str | None, *, target_encoding: str, default_encoding: str, fallback_encodings: Sequence[str], log_debug: Callable[[str], None], log_warning: Callable[[str], None])` — [`L6`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_encoding_conversion.py#L6) — Encode text with configured fallbacks.

