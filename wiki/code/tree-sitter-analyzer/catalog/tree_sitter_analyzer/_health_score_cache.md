---
title: 'Module: tree_sitter_analyzer/_health_score_cache.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_health_score_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._health_score_cache`/
symbols:
  HealthScoreCache.store: HealthScoreCache#store().
  HealthScoreCache.lookup: HealthScoreCache#lookup().
  HealthScoreCache._conn: HealthScoreCache#_conn.
  HealthScoreCache._init_db: HealthScoreCache#_init_db().
  HealthScoreCache.enabled: HealthScoreCache#enabled().
  HealthScoreCache.close: HealthScoreCache#close().
  HealthScoreCache.stats: HealthScoreCache#stats().
  HealthScoreCache: HealthScoreCache#
  HealthScoreCache.invalidate: HealthScoreCache#invalidate().
  HealthScoreCache._db_path: HealthScoreCache#_db_path.
  _Fingerprint.from_path: _Fingerprint#from_path().
  HealthScoreCache._enabled: HealthScoreCache#_enabled.
  _Fingerprint: _Fingerprint#
  logger: logger.
  _Fingerprint.mtime_ns: _Fingerprint#mtime_ns.
  _Fingerprint.size_bytes: _Fingerprint#size_bytes.
  _SCHEMA: _SCHEMA.
  HealthScoreCache._default_db_path: HealthScoreCache#_default_db_path().
  HealthScoreCache.__init__: HealthScoreCache#__init__().
  HealthScoreCache._project_root: HealthScoreCache#_project_root.
---
# Module: [`tree_sitter_analyzer/_health_score_cache.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py)

## Classes
### `HealthScoreCache`
- def: [`tree_sitter_analyzer/_health_score_cache.py:67`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L67)
- doc: Per-file persistent cache for `HealthScore` instances.
- signature: `class HealthScoreCache:`
- members:
  - `close(self)` — [`L107`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L107)
  - `enabled(self)` — [`L104`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L104)
  - `invalidate(self, file_path: str)` — [`L202`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L202) — Remove an explicit entry; returns True iff a row was deleted.
  - `lookup(self, file_path: str)` — [`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L117) — Return cached score dict iff the on-disk fingerprint still matches.
  - `stats(self)` — [`L214`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L214)
  - `store(self, score: Any)` — [`L160`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L160) — Persist a :class:`HealthScore` keyed by current fingerprint.
- protocol/private: `__init__`[`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L75), `_conn`[`L78`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L78), `_db_path`[`L77`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L77), `_default_db_path`[`L82`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L82), `_enabled`[`L79`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L79), `_init_db`[`L86`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L86), `_project_root`[`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L76)
- uses (calls/refs, reference-scoped): [`from_path`](_health_score_cache.md#_Fingerprint.from_path), [`_Fingerprint`](_health_score_cache.md#_Fingerprint), [`logger`](_health_score_cache.md#logger), [`mtime_ns`](_health_score_cache.md#_Fingerprint.mtime_ns), [`size_bytes`](_health_score_cache.md#_Fingerprint.size_bytes), [`_SCHEMA`](_health_score_cache.md#_SCHEMA)
- used by: [`score_project_with_stats`](health_scorer.md#HealthScorer.score_project_with_stats)  (5 test-only)

### `_Fingerprint`
- def: [`tree_sitter_analyzer/_health_score_cache.py:52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L52)
- doc: File-system fingerprint used to detect staleness without re-reading.
- signature: `class _Fingerprint:`
- members:
  - `from_path(cls, path: str)` — [`L59`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L59)
  - `mtime_ns` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L55)
  - `size_bytes` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L56)
- used by: [`store`](_health_score_cache.md#HealthScoreCache.store), [`lookup`](_health_score_cache.md#HealthScoreCache.lookup)

## Module values
- `_SCHEMA` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L37)
- `logger` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_health_score_cache.py#L35)

