---
title: 'Module: tree_sitter_analyzer/_route_detector_go.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_route_detector_go.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._route_detector_go`/
symbols:
  scan_go_net_http: scan_go_net_http().
  _scan_go_verb_routes: _scan_go_verb_routes().
  scan_go_routes: scan_go_routes().
  _go_imports: _go_imports().
  scan_go_fiber: scan_go_fiber().
  scan_go_gin: scan_go_gin().
  scan_go_echo: scan_go_echo().
  _go_source: _go_source().
  go_imports: go_imports().
  _NET_HTTP_IMPORT_RE: _NET_HTTP_IMPORT_RE.
  _GIN_IMPORT_RE: _GIN_IMPORT_RE.
  _ECHO_IMPORT_RE: _ECHO_IMPORT_RE.
  _FIBER_IMPORT_RE: _FIBER_IMPORT_RE.
  _go_extract_string_arg: _go_extract_string_arg().
  _go_handler_name: _go_handler_name().
  _selector_field: _selector_field().
  _GO_HTTP_METHODS: _GO_HTTP_METHODS.
  _FIBER_METHOD_MAP: _FIBER_METHOD_MAP.
---
# Module: [`tree_sitter_analyzer/_route_detector_go.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py)

## Functions
- `_go_extract_string_arg(call_node: Any)` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L71) — Extract the first interpreted_string literal from a Go call_expression.
- `_go_handler_name(call_node: Any)` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L90) — Extract the handler argument from a Go route registration.
- `_go_imports(source: str)` — [`L61`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L61) — Return a flat dict of which Go packages the file imports.
- `_go_source(root: Any)` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L53) — Decode the parse-tree root's source. Empty string on failure.
- `_scan_go_verb_routes(root: Any, file_path: str, route_info_cls: type, *, framework: str, verb_map: dict[str, str] | None, accept_uppercase: bool, extra_verbs: dict[str, str] | None = None)` — [`L168`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L168) — Generic verb-based Go route scanner used by Gin/Echo/Fiber.
- `_selector_field(func_node: Any)` — [`L123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L123) — Return the ``field`` text from a selector_expression, or None.
- `go_imports(source: str)` — [`L287`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L287) — Public alias for ``_go_imports`` used by tests.
- `scan_go_echo(root: Any, file_path: str, route_info_cls: type)` — [`L239`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L239) — Scan for Echo routes — ``e.GET(...)``, ``e.Any(...)``, ``e.Match(...)``.
- `scan_go_fiber(root: Any, file_path: str, route_info_cls: type)` — [`L255`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L255) — Scan for Fiber routes — ``app.Get(...)``, ``app.Post(...)``, etc.
- `scan_go_gin(root: Any, file_path: str, route_info_cls: type)` — [`L224`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L224) — Scan for Gin routes — ``r.GET("/x", h)``, ``r.POST(...)``, etc.
- `scan_go_net_http(root: Any, file_path: str, route_info_cls: type)` — [`L133`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L133) — Scan a Go AST for net/http stdlib route registrations.
- `scan_go_routes(root: Any, file_path: str, route_info_cls: type)` — [`L274`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L274) — Run all four Go framework scanners on a parsed Go file.

## Module values
- `_ECHO_IMPORT_RE` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L49)
- `_FIBER_IMPORT_RE` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L50)
- `_FIBER_METHOD_MAP` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L29)
- `_GIN_IMPORT_RE` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L48)
- `_GO_HTTP_METHODS` — [`L25`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L25)
- `_NET_HTTP_IMPORT_RE` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_go.py#L47)

