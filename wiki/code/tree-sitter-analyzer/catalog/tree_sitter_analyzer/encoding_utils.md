---
title: 'Module: tree_sitter_analyzer/encoding_utils.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/encoding_utils.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.encoding_utils`/
symbols:
  EncodingManager: EncodingManager#
  read_file_safe: read_file_safe().
  safe_encode: safe_encode().
  extract_text_slice: extract_text_slice().
  read_file_safe_streaming: read_file_safe_streaming().
  detect_encoding: detect_encoding().
  EncodingManager.safe_decode: EncodingManager#safe_decode().
  EncodingManager.detect_encoding: EncodingManager#detect_encoding().
  EncodingManager.safe_encode: EncodingManager#safe_encode().
  EncodingManager.read_file_safe: EncodingManager#read_file_safe().
  get_encoding_cache_size: get_encoding_cache_size().
  safe_decode: safe_decode().
  read_file_safe_async: read_file_safe_async().
  clear_encoding_cache: clear_encoding_cache().
  EncodingManager.read_file_safe_async: EncodingManager#read_file_safe_async().
  EncodingCache._cache: EncodingCache#_cache.
  EncodingCache.get: EncodingCache#get().
  EncodingManager.write_file_safe: EncodingManager#write_file_safe().
  EncodingCache: EncodingCache#
  write_file_safe: write_file_safe().
  EncodingCache.set: EncodingCache#set().
  EncodingCache.size: EncodingCache#size().
  EncodingManager.normalize_line_endings: EncodingManager#normalize_line_endings().
  CHARDET_AVAILABLE: CHARDET_AVAILABLE.
  _encoding_cache: _encoding_cache.
  EncodingManager.DEFAULT_ENCODING: EncodingManager#DEFAULT_ENCODING.
  EncodingManager.extract_text_slice: EncodingManager#extract_text_slice().
  EncodingCache._cleanup_expired: EncodingCache#_cleanup_expired().
  EncodingCache.clear: EncodingCache#clear().
  EncodingCache._lock: EncodingCache#_lock.
  EncodingCache._max_size: EncodingCache#_max_size.
  EncodingCache._ttl_seconds: EncodingCache#_ttl_seconds.
  EncodingManager.FALLBACK_ENCODINGS: EncodingManager#FALLBACK_ENCODINGS.
  ANYIO_AVAILABLE: ANYIO_AVAILABLE.
  _setup_encoding_environment: _setup_encoding_environment().
  EncodingCache.__init__: EncodingCache#__init__().
---
# Module: [`tree_sitter_analyzer/encoding_utils.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py)

## Classes
### `EncodingCache`
- def: [`tree_sitter_analyzer/encoding_utils.py:71`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L71)
- doc: Thread-safe encoding cache for file-based encoding detection optimization
- signature: `class EncodingCache:`
- members:
  - `__init__(self, max_size: int = 1000, ttl_seconds: int = 3600)` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L74) — Initialize encoding cache
  - `_cleanup_expired(self)` — [`L135`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L135) — Remove expired entries from cache
  - `clear(self)` — [`L146`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L146) — Clear all cached entries
  - `get(self, file_path: str)` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L89) — Get cached encoding for file path
  - `set(self, file_path: str, encoding: str)` — [`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L113) — Cache encoding for file path
  - `size(self)` — [`L151`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L151) — Get current cache size
- protocol/private: `_cache`[`L82`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L82), `_lock`[`L85`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L85), `_max_size`[`L86`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L86), `_ttl_seconds`[`L87`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L87)
- used by: [`get_encoding_cache_size`](encoding_utils.md#get_encoding_cache_size), [`clear_encoding_cache`](encoding_utils.md#clear_encoding_cache), [`_encoding_cache`](encoding_utils.md#_encoding_cache)  (8 test-only)

### `EncodingManager`
- def: [`tree_sitter_analyzer/encoding_utils.py:161`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L161) — documented in [tree_sitter_analyzer-languages-scala_plugin](../../concepts/tree_sitter_analyzer-languages-scala_plugin.md)
- members:
  - `detect_encoding(cls, data: bytes, file_path: str | None = None)` — [`L211`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L211) — Detect encoding of byte data with optional file-based caching.
  - `extract_text_slice(cls, content_bytes: bytes, start_byte: int, end_byte: int, encoding: str | None = None)` — [`L353`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L353) — Extract a slice of text from bytes with proper encoding handling
  - `normalize_line_endings(cls, text: str)` — [`L336`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L336) — Normalize line endings to Unix style (
  - `read_file_safe(cls, file_path: str | Path)` — [`L233`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L233) — Safely read a file with automatic encoding detection and caching
  - `read_file_safe_async(cls, file_path: str | Path)` — [`L267`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L267) — Safely read a file asynchronously with automatic encoding detection.
  - `safe_decode(cls, data: bytes, encoding: str | None = None)` — [`L189`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L189) — Safely decode bytes to text with fallback handling
  - `safe_encode(cls, text: str | None, encoding: str | None = None)` — [`L168`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L168) — Safely encode text to bytes with fallback handling — documented in [tree_sitter_analyzer-core-parser](../../concepts/tree_sitter_analyzer-core-parser.md)
  - `write_file_safe(cls, file_path: str | Path, content: str, encoding: str | None = None)` — [`L306`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L306) — Safely write content to a file
  - `DEFAULT_ENCODING` — [`L164`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L164)
  - `FALLBACK_ENCODINGS` — [`L165`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L165)
- uses (calls/refs, reference-scoped): [`log_debug`](utils/logging.md#log_debug), [`log_warning`](utils/logging.md#log_warning), [`safe_decode_bytes`](_encoding_conversion.md#safe_decode_bytes), [`CHARDET_AVAILABLE`](encoding_utils.md#CHARDET_AVAILABLE), [`_encoding_cache`](encoding_utils.md#_encoding_cache), [`detect_data_encoding`](_encoding_detection.md#detect_data_encoding), [`safe_encode_text`](_encoding_conversion.md#safe_encode_text), [`ANYIO_AVAILABLE`](encoding_utils.md#ANYIO_AVAILABLE)
- used by: [`parse_code`](core/parser.md#Parser.parse_code), [`read_file_safe`](encoding_utils.md#read_file_safe), [`safe_encode`](encoding_utils.md#safe_encode), [`extract_text_slice`](encoding_utils.md#extract_text_slice), [`read_file_safe_streaming`](encoding_utils.md#read_file_safe_streaming), [`detect_encoding`](encoding_utils.md#detect_encoding), [`read_file_safe_async`](encoding_utils.md#read_file_safe_async), [`safe_decode`](encoding_utils.md#safe_decode), [`_file_byte_diagnostics`](mcp/tools/utils/parse_validity.md#_file_byte_diagnostics), [`_read_source_code`](core/parser.md#Parser._read_source_code), [`write_file_safe`](encoding_utils.md#write_file_safe), [`_encoding_manager`](core/parser.md#Parser._encoding_manager), [`_decode_replacement_used`](mcp/tools/utils/parse_validity.md#_decode_replacement_used)  (44 test-only)

## Functions
- `_setup_encoding_environment()` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L26) — Set up proper encoding environment
- `clear_encoding_cache()` — [`L463`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L463) — Clear the global encoding cache
- `detect_encoding(data: bytes, file_path: str | None = None)` — [`L400`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L400) — Convenience function for encoding detection with optional caching
- `extract_text_slice(content_bytes: bytes, start_byte: int, end_byte: int, encoding: str | None = None)` — [`L422`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L422) — Convenience function for text slice extraction
- `get_encoding_cache_size()` — [`L468`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L468) — Get the current size of the encoding cache
- `read_file_safe(file_path: str | Path)` — [`L405`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L405) — Convenience function for safe file reading
- `read_file_safe_async(file_path: str | Path)` — [`L410`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L410) — Convenience function for safe file reading (async)
- `read_file_safe_streaming(file_path: str | Path)` — [`L431`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L431) — Context manager for streaming file reading with automatic encoding detection.
- `safe_decode(data: bytes, encoding: str | None = None)` — [`L395`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L395) — Convenience function for safe decoding
- `safe_encode(text: str, encoding: str | None = None)` — [`L390`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L390) — Convenience function for safe encoding
- `write_file_safe(file_path: str | Path, content: str, encoding: str | None = None)` — [`L415`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L415) — Convenience function for safe file writing

## Module values
- `ANYIO_AVAILABLE` — [`L22`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L22)
- `CHARDET_AVAILABLE` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L55)
- `_encoding_cache` — [`L158`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/encoding_utils.py#L158)

