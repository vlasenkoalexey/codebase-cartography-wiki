---
title: 'Module: tests/unit/mcp/test_check_tools_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_check_tools_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_check_tools_tool`/
symbols:
  TestCheckToolsToolExecution.test_all_tools_available: TestCheckToolsToolExecution#test_all_tools_available().
  TestCheckToolsToolExecution.test_fd_missing: TestCheckToolsToolExecution#test_fd_missing().
  TestCheckToolsToolExecution.test_rg_missing: TestCheckToolsToolExecution#test_rg_missing().
  TestCheckToolsToolExecution.test_both_missing: TestCheckToolsToolExecution#test_both_missing().
  TestCheckToolsToolExecution.test_version_parsing: TestCheckToolsToolExecution#test_version_parsing().
  TestCheckToolsToolExecution.test_version_from_stderr_when_stdout_empty: TestCheckToolsToolExecution#test_version_from_stderr_when_stdout_empty().
  TestCheckToolsToolExecution.test_timeout_marks_tool_unavailable: TestCheckToolsToolExecution#test_timeout_marks_tool_unavailable().
  TestCheckToolsFailureModes.test_failure_mode_not_installed: TestCheckToolsFailureModes#test_failure_mode_not_installed().
  TestCheckToolsFailureModes.test_failure_mode_timeout: TestCheckToolsFailureModes#test_failure_mode_timeout().
  TestCheckToolsFailureModes.test_failure_mode_permission_denied: TestCheckToolsFailureModes#test_failure_mode_permission_denied().
  TestCheckToolsFailureModes.test_failure_mode_wrong_version: TestCheckToolsFailureModes#test_failure_mode_wrong_version().
  TestCheckToolsToolExecution.fake_subprocess: TestCheckToolsToolExecution#fake_subprocess().
  TestCheckToolsToolDefinition.test_tool_definition_description_contains_when_to_use: TestCheckToolsToolDefinition#test_tool_definition_description_contains_when_to_use().
  TestCheckToolsToolDefinition.test_tool_definition_description_contains_when_not_to_use: TestCheckToolsToolDefinition#test_tool_definition_description_contains_when_not_to_use().
  TestCheckToolsToolDefinition.test_tool_definition_input_schema_empty_properties: TestCheckToolsToolDefinition#test_tool_definition_input_schema_empty_properties().
  TestCheckToolsToolDefinition.test_tool_definition_no_required_fields: TestCheckToolsToolDefinition#test_tool_definition_no_required_fields().
  TestCheckToolsFailureModes.fake_subprocess: TestCheckToolsFailureModes#fake_subprocess().
  tool: tool().
  TestCheckToolsToolInitialization.test_init_creates_tool: TestCheckToolsToolInitialization#test_init_creates_tool().
  TestCheckToolsToolInitialization: TestCheckToolsToolInitialization#
  TestCheckToolsToolDefinition: TestCheckToolsToolDefinition#
  TestCheckToolsToolExecution: TestCheckToolsToolExecution#
  TestCheckToolsFailureModes: TestCheckToolsFailureModes#
---
# Module: [`tests/unit/mcp/test_check_tools_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py)

## Classes
### `TestCheckToolsFailureModes`
- def: [`tests/unit/mcp/test_check_tools_tool.py:249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L249)
- doc: Tests for the per-tool `failure_mode` classification (r37fD).
- signature: `class TestCheckToolsFailureModes:`
- members:
  - `fake_subprocess(*args: object, **kwargs: object)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L261)
  - `test_failure_mode_not_installed(self, tool: CheckToolsTool)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L258) — FileNotFoundError → failure_mode='not_installed' with install hint.
  - `test_failure_mode_permission_denied(self, tool: CheckToolsTool)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L329) — PermissionError on spawn → failure_mode='permission_denied' with chmod hint.
  - `test_failure_mode_timeout(self, tool: CheckToolsTool)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L294) — TimeoutError on communicate() → failure_mode='timeout' with PATH hint.
  - `test_failure_mode_wrong_version(self, tool: CheckToolsTool)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L354) — Old fd version (< MIN_FD_MAJOR=8) → failure_mode='wrong_version'.
- uses (calls/refs, reference-scoped): [`CheckToolsTool`](../../../tree_sitter_analyzer/mcp/tools/check_tools_tool.md#CheckToolsTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/check_tools_tool.md#CheckToolsTool.execute)

### `TestCheckToolsToolDefinition`
- def: [`tests/unit/mcp/test_check_tools_tool.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L33)
- doc: Tests for get_tool_definition().
- signature: `class TestCheckToolsToolDefinition:`
- members:
  - `test_tool_definition_description_contains_when_not_to_use(self, tool: CheckToolsTool)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L43) — Test that the description contains WHEN NOT TO USE section.
  - `test_tool_definition_description_contains_when_to_use(self, tool: CheckToolsTool)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L36) — Test that the description contains WHEN TO USE section.
  - `test_tool_definition_input_schema_empty_properties(self, tool: CheckToolsTool)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L50) — Test that the input schema has no required properties (no arguments needed).
  - `test_tool_definition_no_required_fields(self, tool: CheckToolsTool)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L60) — Test that the schema has no required fields.
- uses (calls/refs, reference-scoped): [`CheckToolsTool`](../../../tree_sitter_analyzer/mcp/tools/check_tools_tool.md#CheckToolsTool), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/check_tools_tool.md#CheckToolsTool.get_tool_definition)

### `TestCheckToolsToolExecution`
- def: [`tests/unit/mcp/test_check_tools_tool.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L67)
- doc: Tests for execute() — core test class.
- signature: `class TestCheckToolsToolExecution:`
- members:
  - `fake_subprocess(*args: object, **kwargs: object)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L81)
  - `test_all_tools_available(self, tool: CheckToolsTool)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L71) — Test that when both fd and rg are present, status is all_tools_available.
  - `test_both_missing(self, tool: CheckToolsTool)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L144) — Test that when both fd and rg are missing, status is missing_tools and recommendation is set.
  - `test_fd_missing(self, tool: CheckToolsTool)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L98) — Test that when fd is missing, fd.available is False.
  - `test_rg_missing(self, tool: CheckToolsTool)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L121) — Test that when rg is missing, rg.available is False.
  - `test_timeout_marks_tool_unavailable(self, tool: CheckToolsTool)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L220) — Test that a timeout when checking a tool marks it as unavailable.
  - `test_version_from_stderr_when_stdout_empty(self, tool: CheckToolsTool)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L193) — Test that stderr is used when stdout is empty.
  - `test_version_parsing(self, tool: CheckToolsTool)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L163) — Test that only the first line of stdout is used as the version string.
- uses (calls/refs, reference-scoped): [`CheckToolsTool`](../../../tree_sitter_analyzer/mcp/tools/check_tools_tool.md#CheckToolsTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/check_tools_tool.md#CheckToolsTool.execute)

### `TestCheckToolsToolInitialization`
- def: [`tests/unit/mcp/test_check_tools_tool.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L25)
- doc: Tests for tool initialization.
- signature: `class TestCheckToolsToolInitialization:`
- members:
  - `test_init_creates_tool(self, tool: CheckToolsTool)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L28) — Test that initialization creates a tool instance.
- uses (calls/refs, reference-scoped): [`CheckToolsTool`](../../../tree_sitter_analyzer/mcp/tools/check_tools_tool.md#CheckToolsTool)

## Functions
- `tool()` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_check_tools_tool.py#L20) — Create a fresh CheckToolsTool instance for each test.

