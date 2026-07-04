---
title: 'Module: tests/unit/test_codegraph_callees_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_codegraph_callees_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_codegraph_callees_tool`/
symbols:
  indexed_call_project: indexed_call_project().
  TestCodeGraphCalleesResolutionFields.test_callees_tool_response_includes_resolution_fields: TestCodeGraphCalleesResolutionFields#test_callees_tool_response_includes_resolution_fields().
  callees_tool: callees_tool().
  TestCodeGraphCalleesResolutionFields: TestCodeGraphCalleesResolutionFields#
---
# Module: [`tests/unit/test_codegraph_callees_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_callees_tool.py)

## Classes
### `TestCodeGraphCalleesResolutionFields`
- def: [`tests/unit/test_codegraph_callees_tool.py:44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_callees_tool.py#L44)
- doc: Once Synapse lands, every callee entry exposes the resolution columns.
- signature: `class TestCodeGraphCalleesResolutionFields:`
- members:
  - `test_callees_tool_response_includes_resolution_fields(self, callees_tool: CodeGraphCalleesTool)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_callees_tool.py#L48) — Each callees[*] entry must have callee_resolution + resolved_file.
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool.execute), [`CodeGraphCalleesTool`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool)

## Functions
- `callees_tool(indexed_call_project: str)` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_callees_tool.py#L40)
- `indexed_call_project(tmp_path: Path)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_codegraph_callees_tool.py#L22)

