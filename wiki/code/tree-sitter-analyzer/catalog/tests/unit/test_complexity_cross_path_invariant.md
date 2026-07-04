---
title: 'Module: tests/unit/test_complexity_cross_path_invariant.py'
type: catalog
provenance: extracted
module: tests/unit/test_complexity_cross_path_invariant.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_complexity_cross_path_invariant`/
symbols:
  _cache_cx: _cache_cx().
  test_extractor_live_and_cache_all_agree: test_extractor_live_and_cache_all_agree().
  _live_cx: _live_cx().
  _parse: _parse().
  _extractor_cx: _extractor_cx().
  _cache_cx._FakeCache: _cache_cx()._FakeCache#
  _CASES: _CASES.
  _cache_cx._FakeCache.lookup: _cache_cx()._FakeCache#lookup().
---
# Module: [`tests/unit/test_complexity_cross_path_invariant.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_cross_path_invariant.py)

## Classes
### `_FakeCache`
- def: [`tests/unit/test_complexity_cross_path_invariant.py:61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_cross_path_invariant.py#L61)
- signature: `class _FakeCache:`
- members:
  - `lookup(self, _fp)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_cross_path_invariant.py#L62)
- used by: (1 test-only callers)

## Functions
- `_cache_cx(lang: str, src: str, filename: str)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_cross_path_invariant.py#L57)
- `_extractor_cx(lang: str, src: str, mod: str, cls: str)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_cross_path_invariant.py#L43)
- `_live_cx(lang: str, src: str, filename: str)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_cross_path_invariant.py#L49)
- `_parse(lang: str, src: str)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_cross_path_invariant.py#L33)
- `test_extractor_live_and_cache_all_agree(lang, fname, mod, cls, fn, src)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_cross_path_invariant.py#L123)

## Module values
- `_CASES` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_cross_path_invariant.py#L74)

