---
title: 'Module: examples/file_output_factory_demo.py'
type: catalog
provenance: extracted
module: examples/file_output_factory_demo.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `examples.file_output_factory_demo`/
symbols:
  demo_mcp_tool_simulation: demo_mcp_tool_simulation().
  demo_factory_pattern: demo_factory_pattern().
  main: main().
  demo_convenience_function: demo_convenience_function().
  demo_mcp_tool_simulation.NewMCPTool.save_result: demo_mcp_tool_simulation().NewMCPTool#save_result().
  demo_backward_compatibility: demo_backward_compatibility().
  demo_thread_safety: demo_thread_safety().
  NewMCPTool.file_output_manager: NewMCPTool#file_output_manager.
  demo_mcp_tool_simulation.OldMCPTool.save_result: demo_mcp_tool_simulation().OldMCPTool#save_result().
  demo_thread_safety.get_instance_worker: demo_thread_safety().get_instance_worker().
  OldMCPTool.file_output_manager: OldMCPTool#file_output_manager.
  demo_mcp_tool_simulation.OldMCPTool: demo_mcp_tool_simulation().OldMCPTool#
  demo_mcp_tool_simulation.NewMCPTool: demo_mcp_tool_simulation().NewMCPTool#
  OldMCPTool.name: OldMCPTool#name.
  NewMCPTool.name: NewMCPTool#name.
  demo_mcp_tool_simulation.OldMCPTool.__init__: demo_mcp_tool_simulation().OldMCPTool#__init__().
  OldMCPTool.project_root: OldMCPTool#project_root.
  demo_mcp_tool_simulation.NewMCPTool.__init__: demo_mcp_tool_simulation().NewMCPTool#__init__().
  NewMCPTool.project_root: NewMCPTool#project_root.
---
# Module: [`examples/file_output_factory_demo.py`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py)

## Classes
### `NewMCPTool`
- def: [`examples/file_output_factory_demo.py:131`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L131)
- signature: `class NewMCPTool:`
- members:
  - `save_result(self, content)` — [`L139`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L139)
  - `file_output_manager` — [`L135`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L135)
  - `name` — [`L133`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L133)
  - `project_root` — [`L134`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L134)
- protocol/private: `__init__`[`L132`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L132)
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`get_managed_instance`](../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_managed_instance), [`save_to_file`](../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.save_to_file)
- used by: (1 test-only callers)

### `OldMCPTool`
- def: [`examples/file_output_factory_demo.py:119`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L119)
- signature: `class OldMCPTool:`
- members:
  - `save_result(self, content)` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L125)
  - `file_output_manager` — [`L123`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L123)
  - `name` — [`L121`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L121)
  - `project_root` — [`L122`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L122)
- protocol/private: `__init__`[`L120`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L120)
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`save_to_file`](../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.save_to_file)
- used by: (1 test-only callers)

## Functions
- `demo_backward_compatibility()` — [`L20`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L20) — Demonstrate that existing code continues to work unchanged.
- `demo_convenience_function()` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L88) — Demonstrate the convenience function.
- `demo_factory_pattern()` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L48) — Demonstrate the new factory pattern benefits.
- `demo_mcp_tool_simulation()` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L111) — Simulate multiple MCP tools using FileOutputManager.
- `demo_thread_safety()` — [`L176`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L176) — Demonstrate thread safety of the factory.
- `get_instance_worker()` — [`L189`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L189)
- `main()` — [`L224`](../../../../../raw/code/tree-sitter-analyzer/examples/file_output_factory_demo.py#L224) — Run all demos.

