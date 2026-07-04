---
title: 'Module: tests/unit/test_route_detector_python.py'
type: catalog
provenance: extracted
module: tests/unit/test_route_detector_python.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_route_detector_python`/Test
symbols:
  TestRouteInfo.test_to_dict_includes_extra: RouteInfo#test_to_dict_includes_extra().
  TestRouteInfo.test_to_dict_round_trip: RouteInfo#test_to_dict_round_trip().
  TestK1FrameworkDisambiguation.test_flask_2x_app_get_post_labels_as_flask: K1FrameworkDisambiguation#test_flask_2x_app_get_post_labels_as_flask().
  TestK1FrameworkDisambiguation.test_flask_legacy_route_decorator_still_works: K1FrameworkDisambiguation#test_flask_legacy_route_decorator_still_works().
  TestFlaskDetection.test_flask_methods: FlaskDetection#test_flask_methods().
  TestFlaskDetection.test_flask_framework_label: FlaskDetection#test_flask_framework_label().
  TestK1FrameworkDisambiguation.test_fastapi_app_get_post_still_labels_as_fastapi: K1FrameworkDisambiguation#test_fastapi_app_get_post_still_labels_as_fastapi().
  TestK1FrameworkDisambiguation.test_express_app_get_unaffected_by_k1: K1FrameworkDisambiguation#test_express_app_get_unaffected_by_k1().
  TestK1FrameworkDisambiguation.test_dual_import_uses_constructor_tiebreak: K1FrameworkDisambiguation#test_dual_import_uses_constructor_tiebreak().
  TestFlaskDetection.test_detect_flask_routes: FlaskDetection#test_detect_flask_routes().
  TestFlaskDetection.test_flask_handler_names: FlaskDetection#test_flask_handler_names().
  TestFastAPIDetection.test_detect_fastapi_routes: FastAPIDetection#test_detect_fastapi_routes().
  TestFastAPIDetection.test_fastapi_framework_label: FastAPIDetection#test_fastapi_framework_label().
  TestK1FrameworkDisambiguation.test_no_framework_imports_returns_nothing: K1FrameworkDisambiguation#test_no_framework_imports_returns_nothing().
  TestRouteInfo: RouteInfo#
  TestFlaskDetection: FlaskDetection#
  TestFastAPIDetection: FastAPIDetection#
  TestK1FrameworkDisambiguation: K1FrameworkDisambiguation#
---
# Module: [`tests/unit/test_route_detector_python.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py)

## Classes
### `TestFastAPIDetection`
- def: [`tests/unit/test_route_detector_python.py:81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L81)
- signature: `class TestFastAPIDetection:`
- members:
  - `test_detect_fastapi_routes(self, fastapi_project: Path)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L82)
  - `test_fastapi_framework_label(self, fastapi_project: Path)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L88)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`http_method`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.http_method)

### `TestFlaskDetection`
- def: [`tests/unit/test_route_detector_python.py:51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L51)
- signature: `class TestFlaskDetection:`
- members:
  - `test_detect_flask_routes(self, flask_project: Path)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L52)
  - `test_flask_framework_label(self, flask_project: Path)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L70)
  - `test_flask_handler_names(self, flask_project: Path)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L65)
  - `test_flask_methods(self, flask_project: Path)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L58)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`url_pattern`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.url_pattern), [`http_method`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.http_method), [`language`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.language), [`handler_name`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.handler_name)

### `TestK1FrameworkDisambiguation`
- def: [`tests/unit/test_route_detector_python.py:98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L98)
- doc: `@app.get('/x')` is identical between Flask 2.x and FastAPI — the
- signature: `class TestK1FrameworkDisambiguation:`
- members:
  - `test_dual_import_uses_constructor_tiebreak(self, tmp_path: Path)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L204) — K1: unusual case where both flask and fastapi are imported —
  - `test_express_app_get_unaffected_by_k1(self, tmp_path: Path)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L148) — K1 must not touch Express detection — receiver-shape + express
  - `test_fastapi_app_get_post_still_labels_as_fastapi(self, tmp_path: Path)` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L128) — K1 baseline: FastAPI imports must keep ``framework='fastapi'``.
  - `test_flask_2x_app_get_post_labels_as_flask(self, tmp_path: Path)` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L103) — K1 reproducer: Flask 2.0+ shortcut decorators with ``from flask``
  - `test_flask_legacy_route_decorator_still_works(self, tmp_path: Path)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L184) — ``@app.route(...)`` is Flask-only and stays unconditional —
  - `test_no_framework_imports_returns_nothing(self, tmp_path: Path)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L164) — K1: when neither flask nor fastapi is imported, fall through to
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`http_method`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.http_method)  (1 test-only)

### `TestRouteInfo`
- def: [`tests/unit/test_route_detector_python.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L15)
- signature: `class TestRouteInfo:`
- members:
  - `test_to_dict_includes_extra(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L32)
  - `test_to_dict_round_trip(self)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_python.py#L16)
- uses (calls/refs, reference-scoped): [`RouteInfo`](../../tree_sitter_analyzer/route_detector.md#RouteInfo), [`to_dict`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.to_dict), [`framework`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.framework), [`url_pattern`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.url_pattern), [`http_method`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.http_method), [`language`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.language), [`file_path`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.file_path), [`handler_name`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.handler_name), [`line_number`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.line_number), [`extra`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.extra)

