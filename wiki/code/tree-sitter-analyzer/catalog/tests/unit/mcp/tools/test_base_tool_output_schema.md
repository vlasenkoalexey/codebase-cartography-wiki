---
title: 'Module: tests/unit/mcp/tools/test_base_tool_output_schema.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_base_tool_output_schema.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_base_tool_output_schema`/
symbols:
  test_output_schema_has_required_envelope_fields: test_output_schema_has_required_envelope_fields().
  test_output_schema_agent_summary_mirrors_verdict_enum: test_output_schema_agent_summary_mirrors_verdict_enum().
  _StubTool: _StubTool#
  test_output_schema_allows_payload_extension: test_output_schema_allows_payload_extension().
  _StubTool.get_tool_definition: _StubTool#get_tool_definition().
  _StubTool.get_tool_schema: _StubTool#get_tool_schema().
  _StubTool.execute: _StubTool#execute().
  _StubTool.validate_arguments: _StubTool#validate_arguments().
---
# Module: [`tests/unit/mcp/tools/test_base_tool_output_schema.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_base_tool_output_schema.py)

## Classes
### `_StubTool`  ·  implements/extends BaseMCPTool
- def: [`tests/unit/mcp/tools/test_base_tool_output_schema.py:25`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_base_tool_output_schema.py#L25)
- doc: Minimal concrete subclass for instantiation.
- signature: `class _StubTool(BaseMCPTool):`
- members:
  - `execute(self, arguments: dict[str, Any])` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_base_tool_output_schema.py#L40)
  - `get_tool_definition(self)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_base_tool_output_schema.py#L34)
  - `get_tool_schema(self)` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_base_tool_output_schema.py#L37)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L43`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_base_tool_output_schema.py#L43)
- uses (calls/refs, reference-scoped): [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool)
- used by: [`BaseMCPTool`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.validate_arguments)  (3 test-only)

## Functions
- `test_output_schema_agent_summary_mirrors_verdict_enum()` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_base_tool_output_schema.py#L72) — Nested agent_summary.verdict must also use the canonical vocabulary.
- `test_output_schema_allows_payload_extension()` — [`L61`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_base_tool_output_schema.py#L61) — ``additionalProperties=True`` so tools can attach arbitrary payloads.
- `test_output_schema_has_required_envelope_fields()` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_base_tool_output_schema.py#L47) — Top-level shape: object with success+verdict required, enum tied to canon.

