---
title: 'Module: tree_sitter_analyzer/mcp/tools/check_tools_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/check_tools_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.check_tools_tool`/
symbols:
  CheckToolsTool: CheckToolsTool#
  CheckToolsTool._check_command: CheckToolsTool#_check_command().
  _build_recommended_fix: _build_recommended_fix().
  CheckToolsTool.execute: CheckToolsTool#execute().
  CheckToolsTool._failure: CheckToolsTool#_failure().
  _MIN_VERSIONS._MIN_VERSIONS: _MIN_VERSIONS._MIN_VERSIONS.
  CheckToolsTool.get_tool_definition: CheckToolsTool#get_tool_definition().
  CheckToolsTool._build_next_step: CheckToolsTool#_build_next_step().
  FM_UNKNOWN: FM_UNKNOWN.
  FM_PERMISSION_DENIED: FM_PERMISSION_DENIED.
  FM_WRONG_VERSION: FM_WRONG_VERSION.
  FM_NOT_INSTALLED: FM_NOT_INSTALLED.
  FM_TIMEOUT: FM_TIMEOUT.
  _MIN_FD_MAJOR: _MIN_FD_MAJOR.
  _MIN_RG_MAJOR: _MIN_RG_MAJOR.
  _parse_major_version: _parse_major_version().
  CheckToolsTool.get_tool_schema: CheckToolsTool#get_tool_schema().
  _INSTALL_HINTS._INSTALL_HINTS: _INSTALL_HINTS._INSTALL_HINTS.
  _UPGRADE_HINTS._UPGRADE_HINTS: _UPGRADE_HINTS._UPGRADE_HINTS.
  CheckToolsTool.validate_arguments: CheckToolsTool#validate_arguments().
---
# Module: [`tree_sitter_analyzer/mcp/tools/check_tools_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py)

## Classes
### `CheckToolsTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/check_tools_tool.py:104`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L104)
- doc: MCP tool that checks whether fd and ripgrep are available.
- signature: `class CheckToolsTool(BaseMCPTool):`
- members:
  - `_build_next_step(*, missing: list[str], fd_result: dict[str, Any], rg_result: dict[str, Any])` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L317) — Compose ``agent_summary.next_step`` routed by per-tool failure_mode.
  - `_check_command(self, cmd: str)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L165) — Probe ``cmd --version`` and classify the result.
  - `_failure(cmd: str, failure_mode: str, *, detail: str = "")` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L241) — Build the standard failure dict for a probe error.
  - `execute(self, arguments: dict[str, Any])` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L250) — Check fd and rg availability and return version info.
  - `get_tool_definition(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L114)
  - `get_tool_schema(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L107)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L162)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`mirror_summary_line`](base_tool.md#mirror_summary_line), [`_build_recommended_fix`](check_tools_tool.md#_build_recommended_fix), [`_MIN_VERSIONS`](check_tools_tool.md#_MIN_VERSIONS._MIN_VERSIONS), [`FM_UNKNOWN`](check_tools_tool.md#FM_UNKNOWN), [`FM_PERMISSION_DENIED`](check_tools_tool.md#FM_PERMISSION_DENIED), [`FM_WRONG_VERSION`](check_tools_tool.md#FM_WRONG_VERSION), [`FM_NOT_INSTALLED`](check_tools_tool.md#FM_NOT_INSTALLED), [`FM_TIMEOUT`](check_tools_tool.md#FM_TIMEOUT), [`_parse_major_version`](check_tools_tool.md#_parse_major_version)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_project_facade`](project_facade.md#build_project_facade)  (17 test-only)

## Functions
- `_build_recommended_fix(cmd: str, failure_mode: str, detail: str = "")` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L72) — Build a per-(command, failure_mode) actionable fix string.
- `_parse_major_version(version_line: str)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L49) — Extract the leading major version integer from a ``--version`` line.

## Module values
- `FM_NOT_INSTALLED` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L30)
- `FM_PERMISSION_DENIED` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L32)
- `FM_TIMEOUT` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L31)
- `FM_UNKNOWN` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L34)
- `FM_WRONG_VERSION` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L33)
- `_INSTALL_HINTS` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L38)
- `_MIN_FD_MAJOR` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L25)
- `_MIN_RG_MAJOR` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L26)
- `_MIN_VERSIONS` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L46)
- `_UPGRADE_HINTS` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/check_tools_tool.py#L42)

