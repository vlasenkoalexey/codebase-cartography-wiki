---
title: 'Module: tree_sitter_analyzer/mcp/tools/route_detector_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/route_detector_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.route_detector_tool`/
symbols:
  RouteDetectorTool: RouteDetectorTool#
  RouteDetectorTool.execute: RouteDetectorTool#execute().
  _attach_route_summary: _attach_route_summary().
  RouteDetectorTool._get_detector: RouteDetectorTool#_get_detector().
  RouteDetectorTool._build_file_response: RouteDetectorTool#_build_file_response().
  _validation_error_envelope: _validation_error_envelope().
  RouteDetectorTool.__init__: RouteDetectorTool#__init__().
  RouteDetectorTool.validate_arguments: RouteDetectorTool#validate_arguments().
  RouteDetectorTool._detector: RouteDetectorTool#_detector.
  RouteDetectorTool.get_tool_definition: RouteDetectorTool#get_tool_definition().
  _validate_file_mode_path: _validate_file_mode_path().
  _pluralize: _pluralize().
  logger: logger.
  RouteDetectorTool._on_project_root_changed: RouteDetectorTool#_on_project_root_changed().
  RouteDetectorTool.get_tool_schema: RouteDetectorTool#get_tool_schema().
  RouteDetectorTool._build_summary_response: RouteDetectorTool#_build_summary_response().
  RouteDetectorTool._build_all_response: RouteDetectorTool#_build_all_response().
  RouteDetectorTool._build_lookup_response: RouteDetectorTool#_build_lookup_response().
  RouteDetectorTool._build_prefix_response: RouteDetectorTool#_build_prefix_response().
---
# Module: [`tree_sitter_analyzer/mcp/tools/route_detector_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py)

## Classes
### `RouteDetectorTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/route_detector_tool.py:21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L21)
- doc: MCP Tool for framework route detection.
- signature: `class RouteDetectorTool(BaseMCPTool):`
- members:
  - `_build_all_response(detector: Any, framework_filter: str)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L178) — M6: ``mode=all`` adds full ``routes`` list + recomputed aggregates.
  - `_build_file_response(self, detector: Any, raw_file_path: str, output_format: str)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L231) — ``mode=file`` — validates path (M4) then runs single-file detection.
  - `_build_lookup_response(detector: Any, url: str, framework_filter: str)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L200) — ``mode=lookup`` returns exact URL pattern matches.
  - `_build_prefix_response(detector: Any, prefix: str, framework_filter: str)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L216) — ``mode=prefix`` returns routes whose URL pattern starts with ``prefix``.
  - `_build_summary_response(detector: Any)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L145) — ``mode=summary`` exposes counts derived from the same ``detect_all()``
  - `execute(self, arguments: dict[str, Any])` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L104) — Dispatch route detection by ``mode``.
  - `get_tool_definition(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L40)
  - `get_tool_schema(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L60)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L94)
- protocol/private: `__init__`[`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L24), `_detector`[`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L25), `_get_detector`[`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L33), `_on_project_root_changed`[`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L30)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`RouteDetector`](../../route_detector.md#RouteDetector), [`resolve_and_validate_file_path`](base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`_attach_route_summary`](route_detector_tool.md#_attach_route_summary), [`_validate_file_mode_path`](route_detector_tool.md#_validate_file_mode_path)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed), [`build_health_facade`](health_facade.md#build_health_facade)  (22 test-only)

## Functions
- `_attach_route_summary(result: dict[str, Any], mode: str)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L265) — Attach summary_line + agent_summary to a route_detector result.
- `_pluralize(count: int, singular: str, plural: str | None = None)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L252) — Return ``count + " " + (singular|plural)`` with English plural rules.
- `_validate_file_mode_path(file_path: str, raw_file_path: str, output_format: str)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L343) — M4: reject missing / dir / non-regular paths with a structured envelope.
- `_validation_error_envelope(message: str, *, mode: str, output_format: str, file_path: str | None = None)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L380) — M4 (round-26): canonical validation-error envelope for detect_routes.

## Module values
- `logger` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/route_detector_tool.py#L18)

