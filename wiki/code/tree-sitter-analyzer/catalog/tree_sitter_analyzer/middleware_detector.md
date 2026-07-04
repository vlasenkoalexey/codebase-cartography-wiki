---
title: 'Module: tree_sitter_analyzer/middleware_detector.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/middleware_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.middleware_detector`/
symbols:
  MiddlewareInfo: MiddlewareInfo#
  MiddlewareDetector._scan_flask_hooks: MiddlewareDetector#_scan_flask_hooks().
  MiddlewareDetector._scan_fastapi_middleware: MiddlewareDetector#_scan_fastapi_middleware().
  MiddlewareDetector._scan_django_settings: MiddlewareDetector#_scan_django_settings().
  MiddlewareDetector._scan_express_middleware: MiddlewareDetector#_scan_express_middleware().
  MiddlewareDetector._scan_spring_controller_advice: MiddlewareDetector#_scan_spring_controller_advice().
  MiddlewareDetector._scan_spring_filters: MiddlewareDetector#_scan_spring_filters().
  MiddlewareDetector._scan_spring_interceptors: MiddlewareDetector#_scan_spring_interceptors().
  MiddlewareInfo.to_dict: MiddlewareInfo#to_dict().
  MiddlewareDetector.detect_all: MiddlewareDetector#detect_all().
  MiddlewareInfo.middleware_name: MiddlewareInfo#middleware_name.
  MiddlewareInfo.middleware_type: MiddlewareInfo#middleware_type.
  MiddlewareInfo.framework: MiddlewareInfo#framework.
  MiddlewareDetector._detect_python_middleware: MiddlewareDetector#_detect_python_middleware().
  MiddlewareDetector._detect_java_middleware: MiddlewareDetector#_detect_java_middleware().
  MiddlewareDetector: MiddlewareDetector#
  MiddlewareDetector.detect_file: MiddlewareDetector#detect_file().
  MiddlewareDetector._parse_tree: MiddlewareDetector#_parse_tree().
  MiddlewareInfo.url_pattern: MiddlewareInfo#url_pattern.
  MiddlewareDetector.summary: MiddlewareDetector#summary().
  MiddlewareInfo.file_path: MiddlewareInfo#file_path.
  MiddlewareDetector._detect_js_middleware: MiddlewareDetector#_detect_js_middleware().
  MiddlewareInfo.http_method: MiddlewareInfo#http_method.
  MiddlewareInfo.line_number: MiddlewareInfo#line_number.
  MiddlewareInfo.language: MiddlewareInfo#language.
  MiddlewareDetector.lookup_by_url_prefix: MiddlewareDetector#lookup_by_url_prefix().
  MiddlewareDetector._walk_source_files: MiddlewareDetector#_walk_source_files().
  MiddlewareInfo.extra: MiddlewareInfo#extra.
  MiddlewareDetector._middlewares: MiddlewareDetector#_middlewares.
  MiddlewareDetector._java_class_implements: MiddlewareDetector#_java_class_implements().
  MiddlewareDetector.project_root: MiddlewareDetector#project_root.
  MiddlewareDetector._parser: MiddlewareDetector#_parser.
  MiddlewareDetector._extract_js_string: MiddlewareDetector#_extract_js_string().
  MiddlewareDetector._func_name_after_decorator: MiddlewareDetector#_func_name_after_decorator().
  logger: logger.
  _EXCLUDE_DIRS: _EXCLUDE_DIRS.
  _SOURCE_EXTENSIONS: _SOURCE_EXTENSIONS.
  _collect_generic_type_names: _collect_generic_type_names().
  MiddlewareDetector._extract_mw_name: MiddlewareDetector#_extract_mw_name().
  MiddlewareDetector._java_class_containing: MiddlewareDetector#_java_class_containing().
  MiddlewareDetector._java_method_after_annotation: MiddlewareDetector#_java_method_after_annotation().
  _MIDDLEWARE_TYPES: _MIDDLEWARE_TYPES.
  MiddlewareDetector.__init__: MiddlewareDetector#__init__().
---
# Module: [`tree_sitter_analyzer/middleware_detector.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py)

## Classes
### `MiddlewareDetector`
- def: [`tree_sitter_analyzer/middleware_detector.py:112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L112)
- doc: Detect middleware/interceptor declarations across web frameworks.
- signature: `class MiddlewareDetector:`
- members:
  - `detect_all(self)` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L128)
  - `detect_file(self, file_path: str)` — [`L140`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L140)
  - `lookup_by_url_prefix(self, prefix: str)` — [`L166`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L166)
  - `summary(self)` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L152)
  - `project_root` — [`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L124)
- protocol/private: `__init__`[`L123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L123), `_detect_java_middleware`[`L392`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L392), `_detect_js_middleware`[`L332`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L332), `_detect_python_middleware`[`L207`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L207), `_extract_js_string`[`L522`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L522), `_extract_mw_name`[`L530`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L530), `_func_name_after_decorator`[`L510`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L510), `_java_class_containing`[`L539`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L539), `_java_class_implements`[`L562`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L562), `_java_method_after_annotation`[`L550`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L550), `_middlewares`[`L126`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L126), `_parse_tree`[`L201`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L201), `_parser`[`L125`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L125), `_scan_django_settings`[`L294`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L294), `_scan_express_middleware`[`L341`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L341), `_scan_fastapi_middleware`[`L264`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L264), `_scan_flask_hooks`[`L220`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L220), `_scan_spring_controller_advice`[`L404`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L404), `_scan_spring_filters`[`L446`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L446), `_scan_spring_interceptors`[`L477`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L477), `_walk_source_files`[`L172`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L172)
- uses (calls/refs, reference-scoped): [`Parser`](core/parser.md#Parser), [`tree`](core/parser.md#ParseResult.tree), [`success`](core/parser.md#ParseResult.success), [`_language_from_ext`](project_graph.md#_language_from_ext), [`parse_file`](core/parser.md#Parser.parse_file), [`MiddlewareInfo`](middleware_detector.md#MiddlewareInfo), [`walk`](_route_detector_helpers.md#walk), [`middleware_name`](middleware_detector.md#MiddlewareInfo.middleware_name), [`framework`](middleware_detector.md#MiddlewareInfo.framework), [`middleware_type`](middleware_detector.md#MiddlewareInfo.middleware_type), [`unquote`](_route_detector_helpers.md#unquote), [`url_pattern`](middleware_detector.md#MiddlewareInfo.url_pattern), [`file_path`](middleware_detector.md#MiddlewareInfo.file_path), [`http_method`](middleware_detector.md#MiddlewareInfo.http_method), [`language`](middleware_detector.md#MiddlewareInfo.language), [`line_number`](middleware_detector.md#MiddlewareInfo.line_number), [`extra`](middleware_detector.md#MiddlewareInfo.extra), [`_EXCLUDE_DIRS`](middleware_detector.md#_EXCLUDE_DIRS), [`_SOURCE_EXTENSIONS`](middleware_detector.md#_SOURCE_EXTENSIONS), [`_collect_generic_type_names`](middleware_detector.md#_collect_generic_type_names), [`logger`](middleware_detector.md#logger)
- used by: [`execute`](mcp/tools/middleware_detector_tool.md#MiddlewareDetectorTool.execute), [`_get_detector`](mcp/tools/middleware_detector_tool.md#MiddlewareDetectorTool._get_detector), [`__init__`](mcp/tools/middleware_detector_tool.md#MiddlewareDetectorTool.__init__)  (10 test-only)

### `MiddlewareInfo`
- def: [`tree_sitter_analyzer/middleware_detector.py:75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L75)
- signature: `class MiddlewareInfo:`
- members:
  - `to_dict(self)` — [`L86`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L86)
  - `extra` — [`L84`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L84)
  - `file_path` — [`L80`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L80)
  - `framework` — [`L82`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L82)
  - `http_method` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L76)
  - `language` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L83)
  - `line_number` — [`L81`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L81)
  - `middleware_name` — [`L78`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L78)
  - `middleware_type` — [`L79`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L79)
  - `url_pattern` — [`L77`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L77)
- used by: [`_scan_django_settings`](middleware_detector.md#MiddlewareDetector._scan_django_settings), [`_scan_express_middleware`](middleware_detector.md#MiddlewareDetector._scan_express_middleware), [`_scan_fastapi_middleware`](middleware_detector.md#MiddlewareDetector._scan_fastapi_middleware), [`_scan_flask_hooks`](middleware_detector.md#MiddlewareDetector._scan_flask_hooks), [`_scan_spring_controller_advice`](middleware_detector.md#MiddlewareDetector._scan_spring_controller_advice), [`_scan_spring_filters`](middleware_detector.md#MiddlewareDetector._scan_spring_filters), [`_scan_spring_interceptors`](middleware_detector.md#MiddlewareDetector._scan_spring_interceptors), [`detect_all`](middleware_detector.md#MiddlewareDetector.detect_all), [`execute`](mcp/tools/middleware_detector_tool.md#MiddlewareDetectorTool.execute), [`_detect_java_middleware`](middleware_detector.md#MiddlewareDetector._detect_java_middleware), [`_detect_python_middleware`](middleware_detector.md#MiddlewareDetector._detect_python_middleware), [`detect_file`](middleware_detector.md#MiddlewareDetector.detect_file), [`summary`](middleware_detector.md#MiddlewareDetector.summary), [`_detect_js_middleware`](middleware_detector.md#MiddlewareDetector._detect_js_middleware), [`lookup_by_url_prefix`](middleware_detector.md#MiddlewareDetector.lookup_by_url_prefix), [`_middlewares`](middleware_detector.md#MiddlewareDetector._middlewares)  (10 test-only)

## Functions
- `_collect_generic_type_names(child: Any, interfaces: list[str])` — [`L100`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L100) — Append type_identifier names from a generic_type AST node to *interfaces*.

## Module values
- `_EXCLUDE_DIRS` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L29)
- `_MIDDLEWARE_TYPES` — [`L57`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L57)
- `_SOURCE_EXTENSIONS` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L55)
- `logger` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/middleware_detector.py#L27)

