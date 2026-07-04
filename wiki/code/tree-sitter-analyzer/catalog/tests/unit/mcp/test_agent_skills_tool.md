---
title: 'Module: tests/unit/mcp/test_agent_skills_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_agent_skills_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_agent_skills_tool`/
symbols:
  test_agent_skills_tool_permission_denied_skill_is_still_listed: test_agent_skills_tool_permission_denied_skill_is_still_listed().
  test_agent_skills_tool_handles_large_inventory: test_agent_skills_tool_handles_large_inventory().
  test_agent_skills_tool_missing_skills_root_returns_blocked: test_agent_skills_tool_missing_skills_root_returns_blocked().
  test_agent_skills_tool_empty_skills_dir_pins_actual_status: test_agent_skills_tool_empty_skills_dir_pins_actual_status().
  test_agent_skills_tool_handles_malformed_yaml_front_matter: test_agent_skills_tool_handles_malformed_yaml_front_matter().
  test_agent_skills_tool_envelope_contract_holds: test_agent_skills_tool_envelope_contract_holds().
  _LEGAL_VERDICTS: _LEGAL_VERDICTS.
  test_agent_skills_tool_lists_project_skills: test_agent_skills_tool_lists_project_skills().
  test_agent_skills_tool_supports_custom_relative_root: test_agent_skills_tool_supports_custom_relative_root().
  test_agent_skills_tool_rejects_external_absolute_root: test_agent_skills_tool_rejects_external_absolute_root().
  test_agent_skills_tool_concurrent_calls_are_safe: test_agent_skills_tool_concurrent_calls_are_safe().
  _create_large_skill_fixture: _create_large_skill_fixture().
  _probe_chmod_enforcement: _probe_chmod_enforcement().
---
# Module: [`tests/unit/mcp/test_agent_skills_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py)

## Functions
- `_create_large_skill_fixture(skills_root, index: int)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L41) — Create one skill directory + SKILL.md for the large-inventory stress test.
- `_probe_chmod_enforcement(skill_path)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L67) — Skip the test if the OS did not honour chmod 0 (e.g., running as root).
- `test_agent_skills_tool_concurrent_calls_are_safe(tmp_path)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L370) — Re-entrant concurrent calls must each return an independent result.
- `test_agent_skills_tool_empty_skills_dir_pins_actual_status(tmp_path)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L196) — Pin the behaviour of an existing-but-empty skills directory.
- `test_agent_skills_tool_envelope_contract_holds(tmp_path)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L410) — Both output formats must honour the canonical envelope.
- `test_agent_skills_tool_handles_large_inventory(tmp_path)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L334) — A 50-skill inventory must build quickly and stay sorted.
- `test_agent_skills_tool_handles_malformed_yaml_front_matter(tmp_path)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L235) — A skill whose SKILL.md has broken front matter must not crash.
- `test_agent_skills_tool_lists_project_skills(tmp_path)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L82) — MCP output should mirror the CLI inventory shape.
- `test_agent_skills_tool_missing_skills_root_returns_blocked(tmp_path)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L164) — A project with no ``.agents/skills`` directory must still answer.
- `test_agent_skills_tool_permission_denied_skill_is_still_listed(tmp_path)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L280) — One unreadable SKILL.md must not crash the whole inventory build.
- `test_agent_skills_tool_rejects_external_absolute_root(tmp_path)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L150) — MCP callers cannot inspect skills outside the configured project root.
- `test_agent_skills_tool_supports_custom_relative_root(tmp_path)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L117) — Custom skills_root should be validated and passed to the shared builder.

## Module values
- `_LEGAL_VERDICTS` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_agent_skills_tool.py#L36)

