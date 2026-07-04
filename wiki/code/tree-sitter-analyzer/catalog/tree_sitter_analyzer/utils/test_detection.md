---
title: 'Module: tree_sitter_analyzer/utils/test_detection.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/utils/test_detection.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.utils.test_detection`/
symbols:
  is_test_file: is_test_file().
  query_wants_tests: query_wants_tests().
  rank_tier: rank_tier().
  _TEST_INTENT_RE: _TEST_INTENT_RE.
  _TEST_DIR_SEGMENTS._TEST_DIR_SEGMENTS: _TEST_DIR_SEGMENTS._TEST_DIR_SEGMENTS.
  _TEST_DIR_PREFIXES._TEST_DIR_PREFIXES: _TEST_DIR_PREFIXES._TEST_DIR_PREFIXES.
  _TEST_FILE_SUFFIXES._TEST_FILE_SUFFIXES: _TEST_FILE_SUFFIXES._TEST_FILE_SUFFIXES.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/utils/test_detection.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/test_detection.py)

## Functions
- `is_test_file(path: str | None)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/test_detection.py#L64) — Return True when *path* points at a test/spec/fixture file.
- `query_wants_tests(query: str | None)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/test_detection.py#L113) — True when the query/task explicitly asks about test/spec/benchmark code.
- `rank_tier(path: str | None, *, wants_tests: bool = False)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/test_detection.py#L93) — Ranking tier: 0 (non-test, ranks first) or 1 (test, demoted).

## Module values
- `_TEST_DIR_PREFIXES` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/test_detection.py#L34)
- `_TEST_DIR_SEGMENTS` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/test_detection.py#L21)
- `_TEST_FILE_SUFFIXES` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/test_detection.py#L45)
- `_TEST_INTENT_RE` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/test_detection.py#L106)
- `__all__` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/test_detection.py#L118)

