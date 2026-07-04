---
title: 'Module: tree_sitter_analyzer/_route_detector_scanners.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_route_detector_scanners.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._route_detector_scanners`/
symbols:
  scan_express_routes: scan_express_routes().
  scan_flask_decorators: scan_flask_decorators().
  scan_django_urls: scan_django_urls().
  scan_spring_annotations: scan_spring_annotations().
  _python_app_framework: _python_app_framework().
  scan_fastapi_decorators: scan_fastapi_decorators().
  _flask_route_from_match: _flask_route_from_match().
  _scan_handler_args: _scan_handler_args().
  parse_request_mapping: parse_request_mapping().
  _extract_express_url: _extract_express_url().
  _is_express_receiver: _is_express_receiver().
  _extract_express_handler_name: _extract_express_handler_name().
  _resolve_handler_text: _resolve_handler_text().
  _file_imports_express: _file_imports_express().
  _url_from_paren_child: _url_from_paren_child().
  _resolve_method_keyword: _resolve_method_keyword().
  _INLINE_HANDLER_TYPES: _INLINE_HANDLER_TYPES.
  _python_source_text: _python_source_text().
  _OBJECT_HANDLER_TYPES: _OBJECT_HANDLER_TYPES.
  _REFERENCE_HANDLER_TYPES: _REFERENCE_HANDLER_TYPES.
  _EXPRESS_HTTP_METHODS: _EXPRESS_HTTP_METHODS.
  _PY_FLASK_IMPORT_RE: _PY_FLASK_IMPORT_RE.
  _PY_FASTAPI_IMPORT_RE: _PY_FASTAPI_IMPORT_RE.
  _PY_FLASK_CONSTRUCTOR_RE: _PY_FLASK_CONSTRUCTOR_RE.
  _PY_FASTAPI_CONSTRUCTOR_RE: _PY_FASTAPI_CONSTRUCTOR_RE.
  _append_flask_routes: _append_flask_routes().
  _EXPRESS_RECEIVER_WHITELIST: _EXPRESS_RECEIVER_WHITELIST.
  _EXPRESS_RECEIVER_SUFFIX: _EXPRESS_RECEIVER_SUFFIX.
  _EXPRESS_IMPORT_RE: _EXPRESS_IMPORT_RE.
  _SPRING_ANNOTATION_MAP: _SPRING_ANNOTATION_MAP.
---
# Module: [`tree_sitter_analyzer/_route_detector_scanners.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py)

## Functions
- `_append_flask_routes(routes: list[Any], route_info_cls: type, *, methods: list[str], url_pattern: str, handler: str, file_path: str, line_number: int)` — [`L149`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L149) — Append one ``route_info_cls`` entry per HTTP method for a Flask route.
- `_extract_express_handler_name(args_node: Any)` — [`L453`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L453) — Resolve the handler name for an Express ``app.<verb>(...)`` call.
- `_extract_express_url(args_node: Any)` — [`L234`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L234) — Return the URL pattern from the first string/template_string arg, or None.
- `_file_imports_express(root: Any)` — [`L429`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L429) — Return True when the parsed file imports ``express`` in any form.
- `_flask_route_from_match(m: re.Match, node: Any, route_info_cls: type, file_path: str, routes: list[Any])` — [`L183`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L183) — Append Flask @app.route(...) entries extracted from *m* to *routes*.
- `_is_express_receiver(receiver: str)` — [`L438`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L438) — Decide whether ``receiver`` (the text before ``.get``/``.post``/...)
- `_python_app_framework(source: str)` — [`L106`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L106) — Return ``"flask"`` / ``"fastapi"`` / ``"unknown"`` for a Python source.
- `_python_source_text(root: Any)` — [`L141`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L141) — Decode the root node's source. Returns an empty string on failure.
- `_resolve_handler_text(last_callable: Any)` — [`L224`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L224) — Convert a callable AST node to a handler name string.
- `_resolve_method_keyword(args_node: Any)` — [`L659`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L659) — Return the HTTP method named in a ``method=RequestMethod.<X>`` kw arg.
- `_scan_handler_args(rest: list[Any])` — [`L206`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L206) — Scan *rest* positional args; return (last_callable_node, saw_object).
- `_url_from_paren_child(node: Any)` — [`L639`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L639) — Find the first ``string_literal`` after a bare ``(`` in ``node.children``.
- `parse_request_mapping(node: Any)` — [`L608`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L608) — Extract (http_method, url_pattern) from a Spring @RequestMapping.
- `scan_django_urls(root: Any, file_path: str, _source: str, route_info_cls: type)` — [`L335`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L335)
- `scan_express_routes(root: Any, file_path: str, language: str, route_info_cls: type)` — [`L499`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L499)
- `scan_fastapi_decorators(root: Any, file_path: str, _source: str, route_info_cls: type)` — [`L292`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L292)
- `scan_flask_decorators(root: Any, file_path: str, _source: str, route_info_cls: type)` — [`L244`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L244)
- `scan_spring_annotations(root: Any, file_path: str, route_info_cls: type)` — [`L561`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L561)

## Module values
- `_EXPRESS_HTTP_METHODS` — [`L60`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L60)
- `_EXPRESS_IMPORT_RE` — [`L418`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L418)
- `_EXPRESS_RECEIVER_SUFFIX` — [`L417`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L417)
- `_EXPRESS_RECEIVER_WHITELIST` — [`L411`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L411)
- `_INLINE_HANDLER_TYPES` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L42)
- `_OBJECT_HANDLER_TYPES` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L36)
- `_PY_FASTAPI_CONSTRUCTOR_RE` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L103)
- `_PY_FASTAPI_IMPORT_RE` — [`L93`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L93)
- `_PY_FLASK_CONSTRUCTOR_RE` — [`L102`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L102)
- `_PY_FLASK_IMPORT_RE` — [`L84`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L84)
- `_REFERENCE_HANDLER_TYPES` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L49)
- `_SPRING_ANNOTATION_MAP` — [`L552`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_scanners.py#L552)

