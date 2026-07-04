---
title: 'Module: tests/unit/test_route_detector_go.py'
type: catalog
provenance: extracted
module: tests/unit/test_route_detector_go.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_route_detector_go`/Test
symbols:
  TestGoNetHTTPDetection.test_nethttp_framework_label: GoNetHTTPDetection#test_nethttp_framework_label().
  TestGoGinDetection.test_gin_framework_label: GoGinDetection#test_gin_framework_label().
  TestGoEchoDetection.test_echo_framework_label: GoEchoDetection#test_echo_framework_label().
  TestGoFiberDetection.test_fiber_framework_label: GoFiberDetection#test_fiber_framework_label().
  TestSourceWalk.test_excludes_node_modules: SourceWalk#test_excludes_node_modules().
  TestSourceWalk.test_excludes_venv: SourceWalk#test_excludes_venv().
  TestSourceWalk.test_excludes_hidden_work_dirs: SourceWalk#test_excludes_hidden_work_dirs().
  TestGoNetHTTPDetection.test_detect_nethttp_routes: GoNetHTTPDetection#test_detect_nethttp_routes().
  TestGoNetHTTPDetection.test_nethttp_handler_names: GoNetHTTPDetection#test_nethttp_handler_names().
  TestGoGinDetection.test_detect_gin_routes: GoGinDetection#test_detect_gin_routes().
  TestGoGinDetection.test_gin_url_patterns: GoGinDetection#test_gin_url_patterns().
  TestGoEchoDetection.test_detect_echo_routes: GoEchoDetection#test_detect_echo_routes().
  TestGoFiberDetection.test_detect_fiber_routes: GoFiberDetection#test_detect_fiber_routes().
  TestGoMultiFramework.test_detect_mixed_go_frameworks: GoMultiFramework#test_detect_mixed_go_frameworks().
  TestSummaryAndLookup.test_lookup_handler_exact_match: SummaryAndLookup#test_lookup_handler_exact_match().
  TestSummaryAndLookup.test_lookup_url_prefix_matches: SummaryAndLookup#test_lookup_url_prefix_matches().
  TestSummaryAndLookup.test_lookup_url_prefix_normalizes_leading_slash: SummaryAndLookup#test_lookup_url_prefix_normalizes_leading_slash().
  TestGoMultiFramework.test_go_file_dispatch: GoMultiFramework#test_go_file_dispatch().
  TestGoMultiFramework.test_go_in_multi_framework_summary: GoMultiFramework#test_go_in_multi_framework_summary().
  TestSummaryAndLookup.test_summary: SummaryAndLookup#test_summary().
  TestSummaryAndLookup.test_lookup_handler_no_match: SummaryAndLookup#test_lookup_handler_no_match().
  TestSummaryAndLookup.test_detect_all_is_cached: SummaryAndLookup#test_detect_all_is_cached().
  TestDetectFileLanguageDispatch.test_python_file_dispatch: DetectFileLanguageDispatch#test_python_file_dispatch().
  TestDetectFileLanguageDispatch.test_javascript_file_dispatch: DetectFileLanguageDispatch#test_javascript_file_dispatch().
  TestDetectFileLanguageDispatch.test_unknown_extension_returns_empty: DetectFileLanguageDispatch#test_unknown_extension_returns_empty().
  TestR37rSummaryLineGrammar.test_single_framework_uses_singular: R37rSummaryLineGrammar#test_single_framework_uses_singular().
  TestR37rSummaryLineGrammar.test_multiple_frameworks_uses_plural: R37rSummaryLineGrammar#test_multiple_frameworks_uses_plural().
  TestR37rSummaryLineGrammar.test_single_route_uses_singular: R37rSummaryLineGrammar#test_single_route_uses_singular().
  TestR37rSummaryLineGrammar.test_zero_routes_uses_plural: R37rSummaryLineGrammar#test_zero_routes_uses_plural().
  TestR37rSummaryLineGrammar.test_mode_all_single_route_uses_singular: R37rSummaryLineGrammar#test_mode_all_single_route_uses_singular().
  TestR37rSummaryLineGrammar.test_mode_all_multiple_routes_uses_plural: R37rSummaryLineGrammar#test_mode_all_multiple_routes_uses_plural().
  TestGoNetHTTPDetection: GoNetHTTPDetection#
  TestGoGinDetection: GoGinDetection#
  TestGoEchoDetection: GoEchoDetection#
  TestGoFiberDetection: GoFiberDetection#
  TestGoMultiFramework: GoMultiFramework#
  TestSummaryAndLookup: SummaryAndLookup#
  TestR37rSummaryLineGrammar: R37rSummaryLineGrammar#
  TestDetectFileLanguageDispatch: DetectFileLanguageDispatch#
  TestSourceWalk: SourceWalk#
---
# Module: [`tests/unit/test_route_detector_go.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py)

## Classes
### `TestDetectFileLanguageDispatch`
- def: [`tests/unit/test_route_detector_go.py:246`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L246)
- doc: Regression: detect_file used to call _language_from_ext(ext) instead of
- signature: `class TestDetectFileLanguageDispatch:`
- members:
  - `test_javascript_file_dispatch(self, express_project: Path)` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L256)
  - `test_python_file_dispatch(self, flask_project: Path)` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L250)
  - `test_unknown_extension_returns_empty(self, tmp_path: Path)` — [`L262`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L262)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_file`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_file)

### `TestGoEchoDetection`
- def: [`tests/unit/test_route_detector_go.py:65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L65)
- signature: `class TestGoEchoDetection:`
- members:
  - `test_detect_echo_routes(self, go_echo_project: Path)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L66)
  - `test_echo_framework_label(self, go_echo_project: Path)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L74)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`http_method`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.http_method), [`language`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.language)

### `TestGoFiberDetection`
- def: [`tests/unit/test_route_detector_go.py:85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L85)
- signature: `class TestGoFiberDetection:`
- members:
  - `test_detect_fiber_routes(self, go_fiber_project: Path)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L86)
  - `test_fiber_framework_label(self, go_fiber_project: Path)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L92)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`http_method`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.http_method), [`language`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.language)

### `TestGoGinDetection`
- def: [`tests/unit/test_route_detector_go.py:41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L41)
- signature: `class TestGoGinDetection:`
- members:
  - `test_detect_gin_routes(self, go_gin_project: Path)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L42)
  - `test_gin_framework_label(self, go_gin_project: Path)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L48)
  - `test_gin_url_patterns(self, go_gin_project: Path)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L53)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`url_pattern`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.url_pattern), [`http_method`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.http_method), [`language`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.language)

### `TestGoMultiFramework`
- def: [`tests/unit/test_route_detector_go.py:103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L103)
- signature: `class TestGoMultiFramework:`
- members:
  - `test_detect_mixed_go_frameworks(self, go_multi_framework_project: Path)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L104)
  - `test_go_file_dispatch(self, go_gin_project: Path)` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L111)
  - `test_go_in_multi_framework_summary(self, go_multi_framework_project: Path)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L117)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`detect_file`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_file), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`summary`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.summary)

### `TestGoNetHTTPDetection`
- def: [`tests/unit/test_route_detector_go.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L15)
- signature: `class TestGoNetHTTPDetection:`
- members:
  - `test_detect_nethttp_routes(self, go_nethttp_project: Path)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L16)
  - `test_nethttp_framework_label(self, go_nethttp_project: Path)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L24)
  - `test_nethttp_handler_names(self, go_nethttp_project: Path)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L29)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`url_pattern`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.url_pattern), [`language`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.language), [`handler_name`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.handler_name)

### `TestR37rSummaryLineGrammar`
- def: [`tests/unit/test_route_detector_go.py:168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L168)
- doc: r37r dogfood: `2 routes across 1 frameworks` is ungrammatical.
- signature: `class TestR37rSummaryLineGrammar:`
- members:
  - `test_mode_all_multiple_routes_uses_plural(self)` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L230) — 'all' mode with 5 routes stays plural.
  - `test_mode_all_single_route_uses_singular(self)` — [`L220`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L220) — 'all' mode also pluralizes by count.
  - `test_multiple_frameworks_uses_plural(self)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L187) — Summary mode with 3 frameworks keeps 'frameworks' (plural).
  - `test_single_framework_uses_singular(self)` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L177) — Summary mode with 1 framework must say 'framework' not 'frameworks'.
  - `test_single_route_uses_singular(self)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L200) — 1 route + 1 framework → both singular.
  - `test_zero_routes_uses_plural(self)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L210) — English convention: '0 routes' (plural) — n != 1 → plural.
- uses (calls/refs, reference-scoped): [`_attach_route_summary`](../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#_attach_route_summary)

### `TestSourceWalk`
- def: [`tests/unit/test_route_detector_go.py:273`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L273)
- signature: `class TestSourceWalk:`
- members:
  - `test_excludes_hidden_work_dirs(self, tmp_path: Path)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L294)
  - `test_excludes_node_modules(self, tmp_path: Path)` — [`L274`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L274)
  - `test_excludes_venv(self, tmp_path: Path)` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L288)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`file_path`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.file_path)  (1 test-only)

### `TestSummaryAndLookup`
- def: [`tests/unit/test_route_detector_go.py:129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L129)
- signature: `class TestSummaryAndLookup:`
- members:
  - `test_detect_all_is_cached(self, flask_project: Path)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L156)
  - `test_lookup_handler_exact_match(self, flask_project: Path)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L138)
  - `test_lookup_handler_no_match(self, flask_project: Path)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L143)
  - `test_lookup_url_prefix_matches(self, flask_project: Path)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L146)
  - `test_lookup_url_prefix_normalizes_leading_slash(self, flask_project: Path)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L151)
  - `test_summary(self, multi_framework_project: Path)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_go.py#L130)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`url_pattern`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.url_pattern), [`summary`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.summary), [`lookup_url_prefix`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.lookup_url_prefix), [`lookup_handler`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.lookup_handler), [`handler_name`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.handler_name)

