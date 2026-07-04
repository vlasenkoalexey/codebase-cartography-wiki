---
title: 'Module: tests/unit/test_route_detector_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_route_detector_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_route_detector_tool`/TestRouteDetectorTool
symbols:
  TestRouteDetectorToolExecute._run: Execute#_run().
  TestRouteDetectorToolExecute.test_file_mode_runs_path_through_validator: Execute#test_file_mode_runs_path_through_validator().
  TestRouteDetectorToolExecute.test_walk_skips_symlinks_outside_project: Execute#test_walk_skips_symlinks_outside_project().
  TestRouteDetectorToolExecute.test_set_project_path_resets_detector: Execute#test_set_project_path_resets_detector().
  TestRouteDetectorToolSchema.test_get_tool_definition_name: Schema#test_get_tool_definition_name().
  TestRouteDetectorToolSchema.test_validate_lookup_requires_url_pattern: Schema#test_validate_lookup_requires_url_pattern().
  TestRouteDetectorToolSchema.test_validate_prefix_requires_url_pattern: Schema#test_validate_prefix_requires_url_pattern().
  TestRouteDetectorToolSchema.test_validate_file_requires_file_path: Schema#test_validate_file_requires_file_path().
  TestRouteDetectorToolSchema.test_validate_summary_no_args: Schema#test_validate_summary_no_args().
  TestRouteDetectorToolExecute.test_execute_summary_mode: Execute#test_execute_summary_mode().
  TestRouteDetectorToolExecute.test_execute_all_mode: Execute#test_execute_all_mode().
  TestRouteDetectorToolExecute.test_execute_all_with_framework_filter: Execute#test_execute_all_with_framework_filter().
  TestRouteDetectorToolExecute.test_execute_lookup_mode: Execute#test_execute_lookup_mode().
  TestRouteDetectorToolExecute.test_execute_prefix_mode: Execute#test_execute_prefix_mode().
  TestRouteDetectorToolExecute.test_execute_file_mode: Execute#test_execute_file_mode().
  TestRouteDetectorToolExecute.test_execute_unknown_mode_raises: Execute#test_execute_unknown_mode_raises().
  TestRouteDetectorToolExecute.test_file_mode_rejects_path_traversal: Execute#test_file_mode_rejects_path_traversal().
  TestRouteDetectorToolExecute.spy: Execute#spy().
  TestRouteDetectorToolSchema: Schema#
  TestRouteDetectorToolExecute: Execute#
---
# Module: [`tests/unit/test_route_detector_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py)

## Classes
### `TestRouteDetectorToolExecute`
- def: [`tests/unit/test_route_detector_tool.py:45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L45)
- signature: `class TestRouteDetectorToolExecute:`
- members:
  - `spy(path: str)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L117)
  - `test_execute_all_mode(self, flask_project: Path)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L57)
  - `test_execute_all_with_framework_filter(self, multi_framework_project: Path)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L64)
  - `test_execute_file_mode(self, flask_project: Path)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L89)
  - `test_execute_lookup_mode(self, flask_project: Path)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L72)
  - `test_execute_prefix_mode(self, flask_project: Path)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L81)
  - `test_execute_summary_mode(self, flask_project: Path)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L50)
  - `test_execute_unknown_mode_raises(self, flask_project: Path)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L101)
  - `test_file_mode_rejects_path_traversal(self, flask_project: Path)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L132) — Security regression: file mode must reject ../ escapes.
  - `test_file_mode_runs_path_through_validator(self, flask_project: Path, monkeypatch: pytest.MonkeyPatch)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L108) — Security regression: file mode must route agent-supplied paths
  - `test_set_project_path_resets_detector(self, flask_project: Path, tmp_path: Path)` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L169)
  - `test_walk_skips_symlinks_outside_project(self, tmp_path: Path)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L145) — Security regression: rglob must not follow symlinks that escape project root.
- protocol/private: `_run`[`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L47)
- uses (calls/refs, reference-scoped): [`RouteDetector`](../../tree_sitter_analyzer/route_detector.md#RouteDetector), [`detect_all`](../../tree_sitter_analyzer/route_detector.md#RouteDetector.detect_all), [`resolve_and_validate_file_path`](../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`set_project_path`](../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.set_project_path), [`RouteDetectorTool`](../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool.execute), [`url_pattern`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.url_pattern), [`file_path`](../../tree_sitter_analyzer/route_detector.md#RouteInfo.file_path)

### `TestRouteDetectorToolSchema`
- def: [`tests/unit/test_route_detector_tool.py:18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L18)
- signature: `class TestRouteDetectorToolSchema:`
- members:
  - `test_get_tool_definition_name(self)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L19)
  - `test_validate_file_requires_file_path(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L32)
  - `test_validate_lookup_requires_url_pattern(self)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L24)
  - `test_validate_prefix_requires_url_pattern(self)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L28)
  - `test_validate_summary_no_args(self)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_tool.py#L36)
- uses (calls/refs, reference-scoped): [`RouteDetectorTool`](../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool.validate_arguments), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/route_detector_tool.md#RouteDetectorTool.get_tool_definition)

