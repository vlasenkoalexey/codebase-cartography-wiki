---
title: 'Module: tests/unit/test_route_detector_web.py'
type: catalog
provenance: extracted
module: tests/unit/test_route_detector_web.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_route_detector_web`/Test
symbols:
  TestExpressDetection.test_express_framework_label: ExpressDetection#test_express_framework_label().
  TestExpressReceiverFilter.test_es_module_express_import_still_detected: ExpressReceiverFilter#test_es_module_express_import_still_detected().
  TestSpringDetection.test_spring_framework_label: SpringDetection#test_spring_framework_label().
  TestExpressDetection.test_detect_express_routes: ExpressDetection#test_detect_express_routes().
  TestExpressReceiverFilter.test_client_http_call_is_not_a_route: ExpressReceiverFilter#test_client_http_call_is_not_a_route().
  TestExpressReceiverFilter.test_express_routes_still_match_with_router_receiver: ExpressReceiverFilter#test_express_routes_still_match_with_router_receiver().
  TestExpressReceiverFilter.test_app_post_without_express_import_is_skipped: ExpressReceiverFilter#test_app_post_without_express_import_is_skipped().
  TestSpringDetection.test_detect_spring_routes: SpringDetection#test_detect_spring_routes().
  TestExpressDetection: ExpressDetection#
  TestExpressReceiverFilter: ExpressReceiverFilter#
  TestSpringDetection: SpringDetection#
---
# Module: [`tests/unit/test_route_detector_web.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py)

## Classes
### `TestExpressDetection`
- def: [`tests/unit/test_route_detector_web.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L15)
- signature: `class TestExpressDetection:`
- members:
  - `test_detect_express_routes(self, express_project: Path)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L16)
  - `test_express_framework_label(self, express_project: Path)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L22)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`http_method`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.http_method), [`language`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.language)

### `TestExpressReceiverFilter`
- def: [`tests/unit/test_route_detector_web.py:33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L33)
- doc: `X.post('/x', ...)` must not match unless X is an Express receiver.
- signature: `class TestExpressReceiverFilter:`
- members:
  - `test_app_post_without_express_import_is_skipped(self, tmp_path: Path)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L93) — app.post(...) is ignored unless the file imports express.
  - `test_client_http_call_is_not_a_route(self, tmp_path: Path)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L36) — Custom apiClient.post('/save', ...) is a client call, not a route.
  - `test_es_module_express_import_still_detected(self, tmp_path: Path)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L112) — from 'express' should also count as an express import.
  - `test_express_routes_still_match_with_router_receiver(self, tmp_path: Path)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L75) — userRouter.post(...) with require('express') still detected.
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`url_pattern`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.url_pattern)  (1 test-only)

### `TestSpringDetection`
- def: [`tests/unit/test_route_detector_web.py:133`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L133)
- signature: `class TestSpringDetection:`
- members:
  - `test_detect_spring_routes(self, spring_project: Path)` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L134)
  - `test_spring_framework_label(self, spring_project: Path)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_web.py#L141)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`http_method`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.http_method), [`language`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.language)

