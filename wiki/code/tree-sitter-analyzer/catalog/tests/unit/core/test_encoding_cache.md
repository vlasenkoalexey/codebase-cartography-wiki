---
title: 'Module: tests/unit/core/test_encoding_cache.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_encoding_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_encoding_cache`/
symbols:
  encoding_cache: encoding_cache().
  test_encoding_detection_with_caching: test_encoding_detection_with_caching().
  test_encoding_detection_without_caching: test_encoding_detection_without_caching().
  test_multiple_files_caching: test_multiple_files_caching().
  test_repeated_detection_performance: test_repeated_detection_performance().
  temp_files: temp_files().
  performance_test_file: performance_test_file().
  test_cache_basic_operations: test_cache_basic_operations().
  test_cache_expiration: test_cache_expiration().
  test_cache_size_limit: test_cache_size_limit().
  test_cache_clear: test_cache_clear().
---
# Module: [`tests/unit/core/test_encoding_cache.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py)

## Functions
- `encoding_cache()` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L22) — Fixture for EncodingCache instance
- `performance_test_file()` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L56) — Fixture for performance test file
- `temp_files()` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L31) — Fixture for temporary test files
- `test_cache_basic_operations(encoding_cache)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L87) — Test basic cache operations
- `test_cache_clear(encoding_cache)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L135) — Test cache clearing
- `test_cache_expiration(encoding_cache)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L104) — Test cache entry expiration
- `test_cache_size_limit(encoding_cache)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L118) — Test cache size limit enforcement
- `test_encoding_detection_with_caching(temp_files)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L149) — Test encoding detection with file path caching
- `test_encoding_detection_without_caching(temp_files)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L167) — Test encoding detection without file path (no caching)
- `test_multiple_files_caching(temp_files)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L184) — Test caching with multiple files
- `test_repeated_detection_performance(performance_test_file)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_encoding_cache.py#L211) — Test that repeated detections use cache

