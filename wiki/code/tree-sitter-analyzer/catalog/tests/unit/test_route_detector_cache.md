---
title: 'Module: tests/unit/test_route_detector_cache.py'
type: catalog
provenance: extracted
module: tests/unit/test_route_detector_cache.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_route_detector_cache`/Test
symbols:
  TestHandlerNameQuality._handlers_by_url: HandlerNameQuality#_handlers_by_url().
  TestRouteCachePersistence.test_route_cache_round_trip: RouteCachePersistence#test_route_cache_round_trip().
  TestRouteCachePersistence.trial: RouteCachePersistence#trial().
  TestRouteCachePersistence.test_warm_pass_uses_cache: RouteCachePersistence#test_warm_pass_uses_cache().
  TestRouteCachePersistence.test_cache_invalidates_on_content_change: RouteCachePersistence#test_cache_invalidates_on_content_change().
  TestRouteCachePersistence.test_warm_pass_is_meaningfully_faster_than_cold: RouteCachePersistence#test_warm_pass_is_meaningfully_faster_than_cold().
  TestRouteCacheVersionInvalidation.test_version_mismatch_clears_cache: RouteCacheVersionInvalidation#test_version_mismatch_clears_cache().
  TestRouteEnvelopeConsistency._run: RouteEnvelopeConsistency#_run().
  TestRouteCachePersistence.test_cache_disabled_flag: RouteCachePersistence#test_cache_disabled_flag().
  TestRouteCachePersistence.test_results_identical_with_and_without_cache: RouteCachePersistence#test_results_identical_with_and_without_cache().
  TestRouteCacheVersionInvalidation.test_version_match_preserves_cache: RouteCacheVersionInvalidation#test_version_match_preserves_cache().
  TestRouteCachePersistence.test_route_cache_creates_db_file: RouteCachePersistence#test_route_cache_creates_db_file().
  TestHandlerNameQuality.test_inline_arrow_function_returns_inline: HandlerNameQuality#test_inline_arrow_function_returns_inline().
  TestHandlerNameQuality.test_named_function_reference_returns_identifier: HandlerNameQuality#test_named_function_reference_returns_identifier().
  TestHandlerNameQuality.test_object_literal_handler_returns_object_marker: HandlerNameQuality#test_object_literal_handler_returns_object_marker().
  TestHandlerNameQuality.test_middleware_array_skipped_real_handler_wins: HandlerNameQuality#test_middleware_array_skipped_real_handler_wins().
  TestHandlerNameQuality.test_handler_never_starts_with_slash: HandlerNameQuality#test_handler_never_starts_with_slash().
  TestRouteEnvelopeConsistency.test_summary_envelope_is_internally_consistent_on_empty_project: RouteEnvelopeConsistency#test_summary_envelope_is_internally_consistent_on_empty_project().
  TestRouteEnvelopeConsistency.test_summary_envelope_routes_match_total_on_populated_project: RouteEnvelopeConsistency#test_summary_envelope_routes_match_total_on_populated_project().
  TestRouteEnvelopeConsistency.test_tree_sitter_analyzer_project_reports_zero_routes: RouteEnvelopeConsistency#test_tree_sitter_analyzer_project_reports_zero_routes().
  TestRouteCachePersistence.key: RouteCachePersistence#key().
  TestRouteCachePersistence: RouteCachePersistence#
  TestHandlerNameQuality: HandlerNameQuality#
  TestRouteEnvelopeConsistency: RouteEnvelopeConsistency#
  TestRouteCacheVersionInvalidation: RouteCacheVersionInvalidation#
---
# Module: [`tests/unit/test_route_detector_cache.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py)

## Classes
### `TestHandlerNameQuality`
- def: [`tests/unit/test_route_detector_cache.py:183`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L183)
- doc: `handler_name` must never silently be the URL pattern or a junk
- signature: `class TestHandlerNameQuality:`
- members:
  - `test_handler_never_starts_with_slash(self, tmp_path: Path)` — [`L292`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L292) — Whatever the callback slot looks like, the handler name must
  - `test_inline_arrow_function_returns_inline(self, tmp_path: Path)` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L201)
  - `test_middleware_array_skipped_real_handler_wins(self, tmp_path: Path)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L270) — ``app.get('/x', [mw1, mw2], realHandler)`` — handler must be the
  - `test_named_function_reference_returns_identifier(self, tmp_path: Path)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L221)
  - `test_object_literal_handler_returns_object_marker(self, tmp_path: Path)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L244) — The big bug: an object literal callback slot must NOT surface
- protocol/private: `_handlers_by_url`[`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L195)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`url_pattern`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.url_pattern), [`handler_name`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.handler_name)  (1 test-only)

### `TestRouteCachePersistence`
- def: [`tests/unit/test_route_detector_cache.py:20`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L20)
- doc: The content-hash cache must survive across RouteDetector instances
- signature: `class TestRouteCachePersistence:`
- members:
  - `key(rs: list)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L75)
  - `test_cache_disabled_flag(self, flask_project: Path)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L61)
  - `test_cache_invalidates_on_content_change(self, multi_framework_project: Path)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L41)
  - `test_results_identical_with_and_without_cache(self, flask_project: Path)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L69)
  - `test_route_cache_creates_db_file(self, flask_project: Path, tmp_path: Path)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L145)
  - `test_route_cache_round_trip(self, tmp_path: Path)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L152)
  - `test_warm_pass_is_meaningfully_faster_than_cold(self, tmp_path: Path)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L83) — PERF-1 regression guard: the cache must produce a >=3x speedup on
  - `test_warm_pass_uses_cache(self, flask_project: Path)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L24)
  - `trial()` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L118)
- uses (calls/refs, reference-scoped): [`Parser`](../../tree_sitter_analyzer/core/parser.md#Parser), [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`url_pattern`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.url_pattern), [`cache_clear`](../../tree_sitter_analyzer/core/parser.md#Parser.cache_clear), [`cache_stats`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.cache_stats), [`RouteCache`](../../tree_sitter_analyzer/_route_cache.md#RouteCache), [`get`](../../tree_sitter_analyzer/_route_cache.md#RouteCache.get), [`put`](../../tree_sitter_analyzer/_route_cache.md#RouteCache.put), [`bulk_get_by_stat`](../../tree_sitter_analyzer/_route_cache.md#RouteCache.bulk_get_by_stat), [`get_by_stat`](../../tree_sitter_analyzer/_route_cache.md#RouteCache.get_by_stat), [`stats`](../../tree_sitter_analyzer/_route_cache.md#RouteCache.stats)

### `TestRouteCacheVersionInvalidation`
- def: [`tests/unit/test_route_detector_cache.py:410`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L410)
- doc: r37f7-F4: bumping `_SCANNER_VERSION` must wipe stale rows so a
- signature: `class TestRouteCacheVersionInvalidation:`
- members:
  - `test_version_match_preserves_cache(self, tmp_path: Path)` — [`L462`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L462)
  - `test_version_mismatch_clears_cache(self, tmp_path: Path)` — [`L421`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L421)
- uses (calls/refs, reference-scoped): [`RouteCache`](../../tree_sitter_analyzer/_route_cache.md#RouteCache), [`get`](../../tree_sitter_analyzer/_route_cache.md#RouteCache.get), [`put`](../../tree_sitter_analyzer/_route_cache.md#RouteCache.put), [`_SCANNER_VERSION`](../../tree_sitter_analyzer/_route_cache.md#_SCANNER_VERSION)

### `TestRouteEnvelopeConsistency`
- def: [`tests/unit/test_route_detector_cache.py:322`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L322)
- doc: r37f7-F4: `mode=summary` used to return `total_routes=N` next to
- signature: `class TestRouteEnvelopeConsistency:`
- members:
  - `test_summary_envelope_is_internally_consistent_on_empty_project(self, tmp_path: Path)` — [`L334`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L334) — A project with no web-framework code must produce a fully
  - `test_summary_envelope_routes_match_total_on_populated_project(self, flask_project: Path)` — [`L357`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L357) — When ``total_routes > 0`` the ``routes`` list must contain the
  - `test_tree_sitter_analyzer_project_reports_zero_routes(self)` — [`L374`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L374) — Regression guard for the original F4 reproducer: running the
- protocol/private: `_run`[`L331`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_cache.py#L331)
- uses (calls/refs, reference-scoped): [`RouteDetectorTool`](../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool.execute)

