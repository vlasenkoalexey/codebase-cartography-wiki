---
title: 'Module: tree_sitter_analyzer/route_detector.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/route_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.route_detector`/
symbols:
  RouteDetector: RouteDetector#
  RouteDetector.detect_all: RouteDetector#detect_all().
  RouteDetector._detect_all_cached: RouteDetector#_detect_all_cached().
  RouteInfo: RouteInfo#
  RouteInfo.to_dict: RouteInfo#to_dict().
  RouteDetector.detect_file: RouteDetector#detect_file().
  RouteInfo.framework: RouteInfo#framework.
  RouteDetector._cache: RouteDetector#_cache.
  RouteInfo.url_pattern: RouteInfo#url_pattern.
  RouteInfo.http_method: RouteInfo#http_method.
  RouteDetector.cache_stats: RouteDetector#cache_stats().
  RouteDetector._parse_tree: RouteDetector#_parse_tree().
  RouteDetector._detect_python_routes: RouteDetector#_detect_python_routes().
  RouteDetector.summary: RouteDetector#summary().
  RouteDetector.lookup_url_prefix: RouteDetector#lookup_url_prefix().
  RouteInfo.language: RouteInfo#language.
  RouteDetector.lookup_handler: RouteDetector#lookup_handler().
  RouteDetector._classify_dir_entry: RouteDetector#_classify_dir_entry().
  RouteDetector._detect_js_routes: RouteDetector#_detect_js_routes().
  RouteDetector._detect_java_routes: RouteDetector#_detect_java_routes().
  RouteDetector._detect_go_routes: RouteDetector#_detect_go_routes().
  RouteInfo.file_path: RouteInfo#file_path.
  RouteInfo.handler_name: RouteInfo#handler_name.
  RouteDetector._routes: RouteDetector#_routes.
  RouteInfo.from_dict: RouteInfo#from_dict().
  RouteDetector._walk_source_files: RouteDetector#_walk_source_files().
  logger: logger.
  _resolve_symlink_target: _resolve_symlink_target().
  RouteDetector._parser: RouteDetector#_parser.
  RouteInfo.line_number: RouteInfo#line_number.
  _SOURCE_EXTENSIONS: _SOURCE_EXTENSIONS.
  RouteInfo.extra: RouteInfo#extra.
  RouteDetector.project_root: RouteDetector#project_root.
  RouteDetector._cache_hits: RouteDetector#_cache_hits.
  RouteDetector._cache_misses: RouteDetector#_cache_misses.
  _CacheRecord: _CacheRecord.
  _EXCLUDE_DIRS: _EXCLUDE_DIRS.
  _ROUTE_INFO_FIELDS: _ROUTE_INFO_FIELDS.
  _FRAMEWORK_FILES: _FRAMEWORK_FILES.
  RouteDetector.__init__: RouteDetector#__init__().
---
# Module: [`tree_sitter_analyzer/route_detector.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py)

## Classes
### `RouteDetector`
- def: [`tree_sitter_analyzer/route_detector.py:165`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L165)
- doc: Detect HTTP route declarations across web frameworks.
- signature: `class RouteDetector:`
- members:
  - `_classify_dir_entry(entry: Any, root: Path, stack: list[str], files: list[Path])` — [`L348`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L348) — Sort a single scandir entry into ``stack`` (recurse) or ``files``.
  - `_detect_all_cached(self, files: list[str])` — [`L227`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L227) — Cache-aware bulk path used when ``self._cache`` is enabled.
  - `_walk_source_files(self)` — [`L317`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L317) — Manual ``os.scandir`` walk: prune excluded directories at the
  - `cache_stats(self)` — [`L204`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L204)
  - `detect_all(self)` — [`L212`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L212)
  - `detect_file(self, file_path: str)` — [`L278`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L278)
  - `lookup_handler(self, url_pattern: str)` — [`L307`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L307)
  - `lookup_url_prefix(self, prefix: str)` — [`L311`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L311)
  - `summary(self)` — [`L293`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L293)
  - `project_root` — [`L183`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L183)
- protocol/private: `__init__`[`L176`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L176), `_cache`[`L186`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L186), `_cache_hits`[`L201`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L201), `_cache_misses`[`L202`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L202), `_detect_go_routes`[`L415`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L415), `_detect_java_routes`[`L409`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L409), `_detect_js_routes`[`L403`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L403), `_detect_python_routes`[`L391`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L391), `_parse_tree`[`L381`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L381), `_parser`[`L184`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L184), `_routes`[`L185`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L185)
- uses (calls/refs, reference-scoped): [`Parser`](core/parser.md#Parser), [`tree`](core/parser.md#ParseResult.tree), [`success`](core/parser.md#ParseResult.success), [`_language_from_ext`](project_graph.md#_language_from_ext), [`parse_file`](core/parser.md#Parser.parse_file), [`RouteInfo`](route_detector.md#RouteInfo), [`to_dict`](route_detector.md#RouteInfo.to_dict), [`framework`](route_detector.md#RouteInfo.framework), [`url_pattern`](route_detector.md#RouteInfo.url_pattern), [`scan_express_routes`](_route_detector_scanners.md#scan_express_routes), [`http_method`](route_detector.md#RouteInfo.http_method), [`scan_django_urls`](_route_detector_scanners.md#scan_django_urls), [`scan_flask_decorators`](_route_detector_scanners.md#scan_flask_decorators), [`scan_spring_annotations`](_route_detector_scanners.md#scan_spring_annotations), [`scan_fastapi_decorators`](_route_detector_scanners.md#scan_fastapi_decorators), [`scan_go_routes`](_route_detector_go.md#scan_go_routes), [`RouteCache`](_route_cache.md#RouteCache), [`file_path`](route_detector.md#RouteInfo.file_path), [`from_dict`](route_detector.md#RouteInfo.from_dict), [`bulk_get_by_stat`](_route_cache.md#RouteCache.bulk_get_by_stat), [`stats`](_route_cache.md#RouteCache.stats), [`logger`](route_detector.md#logger), [`_resolve_symlink_target`](route_detector.md#_resolve_symlink_target), [`bulk_put`](_route_cache.md#RouteCache.bulk_put), [`freshness_key`](_route_cache.md#RouteCache.freshness_key), [`_SOURCE_EXTENSIONS`](route_detector.md#_SOURCE_EXTENSIONS), [`_CacheRecord`](route_detector.md#_CacheRecord), [`_EXCLUDE_DIRS`](route_detector.md#_EXCLUDE_DIRS), [`stat_mtime`](_route_cache.md#RouteCache.stat_mtime)
- used by: [`_collect_route_metrics`](mcp/tools/codegraph_metrics_tool.md#CodeGraphMetricsTool._collect_route_metrics), [`_get_detector`](mcp/tools/route_detector_tool.md#RouteDetectorTool._get_detector), [`__init__`](mcp/tools/route_detector_tool.md#RouteDetectorTool.__init__)  (53 test-only)

### `RouteInfo`
- def: [`tree_sitter_analyzer/route_detector.py:108`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L108)
- doc: A detected HTTP route mapping.
- signature: `class RouteInfo:`
- members:
  - `from_dict(cls, data: dict[str, Any])` — [`L133`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L133) — Rebuild a RouteInfo from a cached to_dict() output.
  - `to_dict(self)` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L120)
  - `extra` — [`L118`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L118)
  - `file_path` — [`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L114)
  - `framework` — [`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L116)
  - `handler_name` — [`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L113)
  - `http_method` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L111)
  - `language` — [`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L117)
  - `line_number` — [`L115`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L115)
  - `url_pattern` — [`L112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L112)
- uses (calls/refs, reference-scoped): [`_ROUTE_INFO_FIELDS`](route_detector.md#_ROUTE_INFO_FIELDS)
- used by: [`detect_all`](route_detector.md#RouteDetector.detect_all), [`_detect_all_cached`](route_detector.md#RouteDetector._detect_all_cached), [`detect_file`](route_detector.md#RouteDetector.detect_file), [`_detect_python_routes`](route_detector.md#RouteDetector._detect_python_routes), [`summary`](route_detector.md#RouteDetector.summary), [`lookup_url_prefix`](route_detector.md#RouteDetector.lookup_url_prefix), [`lookup_handler`](route_detector.md#RouteDetector.lookup_handler), [`_detect_go_routes`](route_detector.md#RouteDetector._detect_go_routes), [`_detect_java_routes`](route_detector.md#RouteDetector._detect_java_routes), [`_detect_js_routes`](route_detector.md#RouteDetector._detect_js_routes), [`_routes`](route_detector.md#RouteDetector._routes)  (39 test-only)

## Functions
- `_resolve_symlink_target(symlink_path: str, root: Path)` — [`L148`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L148) — Resolve a file-symlink, returning its target if it lives under ``root``.

## Module values
- `_CacheRecord` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L37)
- `_EXCLUDE_DIRS` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L39)
- `_FRAMEWORK_FILES` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L75)
- `_ROUTE_INFO_FIELDS` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L94)
- `_SOURCE_EXTENSIONS` — [`L65`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L65)
- `logger` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/route_detector.py#L34)

