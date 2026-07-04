---
title: 'Module: tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.agent_workflow_tool`/
symbols:
  AgentWorkflowTool.execute: AgentWorkflowTool#execute().
  AgentWorkflowTool: AgentWorkflowTool#
  AgentWorkflowTool._validate_target_path: AgentWorkflowTool#_validate_target_path().
  _canonicalize_workflow_verdict: _canonicalize_workflow_verdict().
  AgentWorkflowTool.get_tool_definition: AgentWorkflowTool#get_tool_definition().
  AgentWorkflowTool.get_tool_schema: AgentWorkflowTool#get_tool_schema().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  AgentWorkflowTool.validate_arguments: AgentWorkflowTool#validate_arguments().
  _build_toon_response: _build_toon_response().
---
# Module: [`tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py)

## Classes
### `AgentWorkflowTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py#L32)
- doc: MCP tool that returns a SMART workflow command pack for agents.
- signature: `class AgentWorkflowTool(BaseMCPTool):`
- members:
  - `_validate_target_path(self, target_path: str | None)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py#L109) — Keep optional workflow targets inside the configured project boundary.
  - `execute(self, arguments: dict[str, Any])` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py#L70) — Build a SMART agent workflow pack.
  - `get_tool_definition(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py#L35) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py#L53) — Return the JSON schema for tool input validation.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py#L57) — Validate output format and optional target path.
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`validate_file_path`](../../security/validator.md#SecurityValidator.validate_file_path), [`build_agent_workflow_pack`](../../cli/agent_workflow.md#build_agent_workflow_pack), [`security_validator`](base_tool.md#BaseMCPTool.security_validator), [`_canonicalize_workflow_verdict`](agent_workflow_tool.md#_canonicalize_workflow_verdict), [`TOOL_SCHEMA`](agent_workflow_tool.md#TOOL_SCHEMA.TOOL_SCHEMA), [`_build_toon_response`](agent_workflow_tool.md#_build_toon_response)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_project_facade`](project_facade.md#build_project_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases)  (16 test-only)

## Functions
- `_build_toon_response(result: dict[str, Any])` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py#L142) — Return a compact MCP response when callers request TOON output.
- `_canonicalize_workflow_verdict(result: dict[str, Any])` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py#L121) — Rewrite both verdict surfaces in-place to the canonical vocabulary.

## Module values
- `TOOL_SCHEMA` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_workflow_tool.py#L12)

