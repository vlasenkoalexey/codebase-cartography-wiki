---
title: 'Module: tree_sitter_analyzer/mcp/tools/agent_skills_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/agent_skills_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.agent_skills_tool`/
symbols:
  AgentSkillsTool.execute: AgentSkillsTool#execute().
  AgentSkillsTool: AgentSkillsTool#
  AgentSkillsTool._validate_skills_root: AgentSkillsTool#_validate_skills_root().
  AgentSkillsTool.get_tool_definition: AgentSkillsTool#get_tool_definition().
  AgentSkillsTool.get_tool_schema: AgentSkillsTool#get_tool_schema().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  AgentSkillsTool.validate_arguments: AgentSkillsTool#validate_arguments().
  _build_toon_response: _build_toon_response().
---
# Module: [`tree_sitter_analyzer/mcp/tools/agent_skills_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_skills_tool.py)

## Classes
### `AgentSkillsTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/agent_skills_tool.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_skills_tool.py#L32)
- doc: MCP tool that lists project-local agent skills and usability gaps.
- signature: `class AgentSkillsTool(BaseMCPTool):`
- members:
  - `_validate_skills_root(self, skills_root: str | None)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_skills_tool.py#L114) — Keep custom skills roots inside the configured project boundary.
  - `execute(self, arguments: dict[str, Any])` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_skills_tool.py#L89) — Build a project-local agent skill inventory.
  - `get_tool_definition(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_skills_tool.py#L35) — Return the MCP tool name, description, and input schema.
  - `get_tool_schema(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_skills_tool.py#L72) — Return the JSON schema for tool input validation.
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_skills_tool.py#L76) — Validate output format and optional skills root.
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`build_agent_skills_inventory`](../../cli/agent_skills.md#build_agent_skills_inventory), [`security_validator`](base_tool.md#BaseMCPTool.security_validator), [`validate_directory_path`](../../security/validator.md#SecurityValidator.validate_directory_path), [`TOOL_SCHEMA`](agent_skills_tool.md#TOOL_SCHEMA.TOOL_SCHEMA), [`_build_toon_response`](agent_skills_tool.md#_build_toon_response)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_project_facade`](project_facade.md#build_project_facade), [`attach_tool_aliases`](../_server_helpers.md#attach_tool_aliases)  (11 test-only)

## Functions
- `_build_toon_response(result: dict[str, Any])` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_skills_tool.py#L129) — Return a compact MCP response when callers request TOON output.

## Module values
- `TOOL_SCHEMA` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/agent_skills_tool.py#L12)

