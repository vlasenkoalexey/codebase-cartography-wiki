---
title: 'Module: tests/unit/test_middleware_detector.py'
type: catalog
provenance: extracted
module: tests/unit/test_middleware_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_middleware_detector`/
symbols:
  TestMiddlewareInfo.test_to_dict_roundtrip: TestMiddlewareInfo#test_to_dict_roundtrip().
  TestFlaskMiddleware.test_before_request: TestFlaskMiddleware#test_before_request().
  TestFastAPIMiddleware.test_middleware_decorator: TestFastAPIMiddleware#test_middleware_decorator().
  TestFlaskMiddleware.test_errorhandler: TestFlaskMiddleware#test_errorhandler().
  TestDjangoMiddleware.test_settings_middleware: TestDjangoMiddleware#test_settings_middleware().
  TestExpressMiddleware.test_app_use_with_path: TestExpressMiddleware#test_app_use_with_path().
  _write_fixture: _write_fixture().
  TestFlaskMiddleware.test_after_request: TestFlaskMiddleware#test_after_request().
  TestExpressMiddleware.test_router_use: TestExpressMiddleware#test_router_use().
  TestLookup.test_lookup_by_url_prefix: TestLookup#test_lookup_by_url_prefix().
  TestSourceWalk.test_excludes_hidden_work_dirs: TestSourceWalk#test_excludes_hidden_work_dirs().
  TestSummary.test_summary: TestSummary#test_summary().
  tool: tool().
  TestMiddlewareDetectorTool.test_no_project_root_raises: TestMiddlewareDetectorTool#test_no_project_root_raises().
  _setup_fixtures: _setup_fixtures().
  _PROJECT_ROOT: _PROJECT_ROOT.
  _FIXTURES: _FIXTURES.
  TestMiddlewareInfo: TestMiddlewareInfo#
  TestFlaskMiddleware: TestFlaskMiddleware#
  TestDjangoMiddleware: TestDjangoMiddleware#
  TestFastAPIMiddleware: TestFastAPIMiddleware#
  TestExpressMiddleware: TestExpressMiddleware#
  TestSummary: TestSummary#
  TestLookup: TestLookup#
  TestSourceWalk: TestSourceWalk#
  TestMiddlewareDetectorTool: TestMiddlewareDetectorTool#
  TestMiddlewareDetectorTool.test_tool_definition: TestMiddlewareDetectorTool#test_tool_definition().
  TestMiddlewareDetectorTool.test_validate_arguments: TestMiddlewareDetectorTool#test_validate_arguments().
  TestMiddlewareDetectorTool.test_execute_all: TestMiddlewareDetectorTool#test_execute_all().
  TestMiddlewareDetectorTool.test_execute_summary: TestMiddlewareDetectorTool#test_execute_summary().
  TestMiddlewareDetectorTool.test_execute_toon_format: TestMiddlewareDetectorTool#test_execute_toon_format().
  TestMiddlewareDetectorTool.test_project_root_change_resets_cache: TestMiddlewareDetectorTool#test_project_root_change_resets_cache().
---
# Module: [`tests/unit/test_middleware_detector.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py)

## Classes
### `TestDjangoMiddleware`
- def: [`tests/unit/test_middleware_detector.py:116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L116)
- signature: `class TestDjangoMiddleware:`
- members:
  - `test_settings_middleware(self, tmp_path)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L117)
- uses (calls/refs, reference-scoped): [`detect_all`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector.detect_all), [`middleware_name`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.middleware_name), [`framework`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.framework), [`MiddlewareDetector`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector)  (1 test-only)

### `TestExpressMiddleware`
- def: [`tests/unit/test_middleware_detector.py:161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L161)
- signature: `class TestExpressMiddleware:`
- members:
  - `test_app_use_with_path(self, tmp_path)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L162)
  - `test_router_use(self, tmp_path)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L182)
- uses (calls/refs, reference-scoped): [`detect_all`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector.detect_all), [`middleware_name`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.middleware_name), [`MiddlewareDetector`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector), [`url_pattern`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.url_pattern)  (1 test-only)

### `TestFastAPIMiddleware`
- def: [`tests/unit/test_middleware_detector.py:138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L138)
- signature: `class TestFastAPIMiddleware:`
- members:
  - `test_middleware_decorator(self, tmp_path)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L139)
- uses (calls/refs, reference-scoped): [`detect_all`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector.detect_all), [`middleware_name`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.middleware_name), [`framework`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.framework), [`middleware_type`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.middleware_type), [`MiddlewareDetector`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector)  (1 test-only)

### `TestFlaskMiddleware`
- def: [`tests/unit/test_middleware_detector.py:57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L57)
- signature: `class TestFlaskMiddleware:`
- members:
  - `test_after_request(self, tmp_path)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L78)
  - `test_before_request(self, tmp_path)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L58)
  - `test_errorhandler(self, tmp_path)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L96)
- uses (calls/refs, reference-scoped): [`detect_all`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector.detect_all), [`middleware_name`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.middleware_name), [`framework`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.framework), [`middleware_type`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.middleware_type), [`MiddlewareDetector`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector), [`extra`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.extra)  (1 test-only)

### `TestLookup`
- def: [`tests/unit/test_middleware_detector.py:222`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L222)
- signature: `class TestLookup:`
- members:
  - `test_lookup_by_url_prefix(self, tmp_path)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L223)
- uses (calls/refs, reference-scoped): [`middleware_name`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.middleware_name), [`MiddlewareDetector`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector), [`lookup_by_url_prefix`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector.lookup_by_url_prefix)  (1 test-only)

### `TestMiddlewareDetectorTool`
- def: [`tests/unit/test_middleware_detector.py:261`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L261)
- signature: `class TestMiddlewareDetectorTool:`
- members:
  - `test_execute_all(self, tool)` — [`L273`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L273)
  - `test_execute_summary(self, tool)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L282)
  - `test_execute_toon_format(self, tool)` — [`L291`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L291)
  - `test_no_project_root_raises(self)` — [`L296`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L296)
  - `test_project_root_change_resets_cache(self, tool)` — [`L301`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L301)
  - `test_tool_definition(self, tool)` — [`L262`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L262)
  - `test_validate_arguments(self, tool)` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L267)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/middleware_detector_tool.md#MiddlewareDetectorTool.execute), [`MiddlewareDetectorTool`](../../tree_sitter_analyzer/mcp/tools/middleware_detector_tool.md#MiddlewareDetectorTool)

### `TestMiddlewareInfo`
- def: [`tests/unit/test_middleware_detector.py:38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L38)
- signature: `class TestMiddlewareInfo:`
- members:
  - `test_to_dict_roundtrip(self)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L39)
- uses (calls/refs, reference-scoped): [`MiddlewareInfo`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo), [`to_dict`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.to_dict), [`middleware_name`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.middleware_name), [`framework`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.framework), [`middleware_type`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.middleware_type), [`url_pattern`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.url_pattern), [`file_path`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.file_path), [`http_method`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.http_method), [`language`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.language), [`line_number`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.line_number), [`extra`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.extra)

### `TestSourceWalk`
- def: [`tests/unit/test_middleware_detector.py:239`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L239)
- signature: `class TestSourceWalk:`
- members:
  - `test_excludes_hidden_work_dirs(self, tmp_path)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L240)
- uses (calls/refs, reference-scoped): [`detect_all`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector.detect_all), [`middleware_name`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareInfo.middleware_name), [`MiddlewareDetector`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector)  (1 test-only)

### `TestSummary`
- def: [`tests/unit/test_middleware_detector.py:197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L197)
- signature: `class TestSummary:`
- members:
  - `test_summary(self, tmp_path)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L198)
- uses (calls/refs, reference-scoped): [`MiddlewareDetector`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector), [`summary`](../../tree_sitter_analyzer/middleware_detector.md#MiddlewareDetector.summary)  (1 test-only)

## Functions
- `_setup_fixtures(tmp_path)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L22)
- `_write_fixture(tmp_path, rel_path: str, content: str)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L26)
- `tool()` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L34)

## Module values
- `_FIXTURES` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L18)
- `_PROJECT_ROOT` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_middleware_detector.py#L17)

