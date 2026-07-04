---
title: 'Module: tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.middleware_detector_tool`/
symbols:
  MiddlewareDetectorTool.execute: MiddlewareDetectorTool#execute().
  MiddlewareDetectorTool._get_detector: MiddlewareDetectorTool#_get_detector().
  MiddlewareDetectorTool: MiddlewareDetectorTool#
  MiddlewareDetectorTool.__init__: MiddlewareDetectorTool#__init__().
  MiddlewareDetectorTool._detector: MiddlewareDetectorTool#_detector.
  logger: logger.
  MiddlewareDetectorTool._on_project_root_changed: MiddlewareDetectorTool#_on_project_root_changed().
  MiddlewareDetectorTool.get_tool_definition: MiddlewareDetectorTool#get_tool_definition().
  MiddlewareDetectorTool.get_tool_schema: MiddlewareDetectorTool#get_tool_schema().
  MiddlewareDetectorTool.validate_arguments: MiddlewareDetectorTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py)

## Classes
### `MiddlewareDetectorTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py#L18)
- doc: MCP Tool for detecting framework middleware and interceptors.
- signature: `class MiddlewareDetectorTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py#L85)
  - `get_tool_definition(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py#L35)
  - `get_tool_schema(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py#L48)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py#L82)
- protocol/private: `__init__`[`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py#L21), `_detector`[`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py#L22), `_get_detector`[`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py#L28), `_on_project_root_changed`[`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py#L25)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`to_dict`](../../middleware_detector.md#MiddlewareInfo.to_dict), [`detect_all`](../../middleware_detector.md#MiddlewareDetector.detect_all), [`framework`](../../middleware_detector.md#MiddlewareInfo.framework), [`MiddlewareDetector`](../../middleware_detector.md#MiddlewareDetector), [`summary`](../../middleware_detector.md#MiddlewareDetector.summary), [`lookup_by_url_prefix`](../../middleware_detector.md#MiddlewareDetector.lookup_by_url_prefix)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed)  (2 test-only)

## Module values
- `logger` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/middleware_detector_tool.py#L15)

