---
title: 'Module: tests/unit/test_call_graph_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_call_graph_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_call_graph_tool`/
symbols:
  TestCodeGraphCallToolInit.test_init_with_project_root: TestCodeGraphCallToolInit#test_init_with_project_root().
  PY_PROJECT: PY_PROJECT.
  TestCodeGraphCallToolInit.test_init_without_project_root: TestCodeGraphCallToolInit#test_init_without_project_root().
  tool: tool().
  TestCodeGraphCallToolInit.test_get_call_graph_raises_without_root: TestCodeGraphCallToolInit#test_get_call_graph_raises_without_root().
  TestCodeGraphCallToolCallers.test_callers_qualified_zero_hits_with_hint: TestCodeGraphCallToolCallers#test_callers_qualified_zero_hits_with_hint().
  TestCodeGraphCallToolInit.test_set_project_path_resets_graph: TestCodeGraphCallToolInit#test_set_project_path_resets_graph().
  TestCodeGraphCallToolInit.test_get_call_graph_creates_instance: TestCodeGraphCallToolInit#test_get_call_graph_creates_instance().
  TestCodeGraphCallToolCallees.test_callees_of_main: TestCodeGraphCallToolCallees#test_callees_of_main().
  _WINDOWS_SKIP_PY_FIXTURE: _WINDOWS_SKIP_PY_FIXTURE.
  FIXTURES_DIR: FIXTURES_DIR.
  TestCodeGraphCallToolInit: TestCodeGraphCallToolInit#
  TestCodeGraphCallToolInit.test_get_call_graph_caches: TestCodeGraphCallToolInit#test_get_call_graph_caches().
  TestCodeGraphCallToolDefinition: TestCodeGraphCallToolDefinition#
  TestCodeGraphCallToolDefinition.test_get_tool_definition: TestCodeGraphCallToolDefinition#test_get_tool_definition().
  TestCodeGraphCallToolDefinition.test_get_tool_schema_modes: TestCodeGraphCallToolDefinition#test_get_tool_schema_modes().
  TestCodeGraphCallToolDefinition.test_get_tool_schema_defaults: TestCodeGraphCallToolDefinition#test_get_tool_schema_defaults().
  TestCodeGraphCallToolDefinition.test_get_tool_schema_no_additional_props: TestCodeGraphCallToolDefinition#test_get_tool_schema_no_additional_props().
  TestCodeGraphCallToolValidation: TestCodeGraphCallToolValidation#
  TestCodeGraphCallToolValidation.test_validate_summary_no_func_name: TestCodeGraphCallToolValidation#test_validate_summary_no_func_name().
  TestCodeGraphCallToolValidation.test_validate_all_functions_no_func_name: TestCodeGraphCallToolValidation#test_validate_all_functions_no_func_name().
  TestCodeGraphCallToolValidation.test_validate_callers_requires_func_name: TestCodeGraphCallToolValidation#test_validate_callers_requires_func_name().
  TestCodeGraphCallToolValidation.test_validate_callees_requires_func_name: TestCodeGraphCallToolValidation#test_validate_callees_requires_func_name().
  TestCodeGraphCallToolValidation.test_validate_chain_requires_func_name: TestCodeGraphCallToolValidation#test_validate_chain_requires_func_name().
  TestCodeGraphCallToolValidation.test_validate_callers_with_func_name: TestCodeGraphCallToolValidation#test_validate_callers_with_func_name().
  TestCodeGraphCallToolValidation.test_validate_default_mode: TestCodeGraphCallToolValidation#test_validate_default_mode().
  TestCodeGraphCallToolValidation.test_validate_invalid_mode_lists_valid_modes: TestCodeGraphCallToolValidation#test_validate_invalid_mode_lists_valid_modes().
  TestCodeGraphCallToolValidation.test_validate_invalid_mode_without_function_name: TestCodeGraphCallToolValidation#test_validate_invalid_mode_without_function_name().
  TestCodeGraphCallToolValidation.test_execute_invalid_mode_fails_before_graph_build: TestCodeGraphCallToolValidation#test_execute_invalid_mode_fails_before_graph_build().
  TestCodeGraphCallToolSummary: TestCodeGraphCallToolSummary#
  TestCodeGraphCallToolSummary.test_summary_mode: TestCodeGraphCallToolSummary#test_summary_mode().
  TestCodeGraphCallToolSummary.test_default_mode_is_summary: TestCodeGraphCallToolSummary#test_default_mode_is_summary().
  TestCodeGraphCallToolAllFunctions: TestCodeGraphCallToolAllFunctions#
  TestCodeGraphCallToolAllFunctions.test_all_functions: TestCodeGraphCallToolAllFunctions#test_all_functions().
  TestCodeGraphCallToolCallers: TestCodeGraphCallToolCallers#
  TestCodeGraphCallToolCallers.test_callers_of_existing_function: TestCodeGraphCallToolCallers#test_callers_of_existing_function().
  TestCodeGraphCallToolCallers.test_callers_of_nonexistent: TestCodeGraphCallToolCallers#test_callers_of_nonexistent().
  TestCodeGraphCallToolCallers.test_callers_with_file_path: TestCodeGraphCallToolCallers#test_callers_with_file_path().
  TestCodeGraphCallToolCallers.test_callers_qualified_class_method_resolves: TestCodeGraphCallToolCallers#test_callers_qualified_class_method_resolves().
  TestCodeGraphCallToolCallees: TestCodeGraphCallToolCallees#
  TestCodeGraphCallToolCallees.test_callees_leaf_function: TestCodeGraphCallToolCallees#test_callees_leaf_function().
  TestCodeGraphCallToolChain: TestCodeGraphCallToolChain#
  TestCodeGraphCallToolChain.test_chain_from_main: TestCodeGraphCallToolChain#test_chain_from_main().
  TestCodeGraphCallToolChain.test_chain_custom_depth: TestCodeGraphCallToolChain#test_chain_custom_depth().
  TestCodeGraphCallToolChain.test_chain_nonexistent: TestCodeGraphCallToolChain#test_chain_nonexistent().
  TestCodeGraphCallToolUnknownMode: TestCodeGraphCallToolUnknownMode#
  TestCodeGraphCallToolUnknownMode.test_unknown_mode_raises: TestCodeGraphCallToolUnknownMode#test_unknown_mode_raises().
  TestCodeGraphCallToolToonFormat: TestCodeGraphCallToolToonFormat#
  TestCodeGraphCallToolToonFormat.test_toon_format_summary: TestCodeGraphCallToolToonFormat#test_toon_format_summary().
  TestCodeGraphCallToolFileImpact: TestCodeGraphCallToolFileImpact#
  TestCodeGraphCallToolFileImpact.test_validate_file_impact_requires_file_path: TestCodeGraphCallToolFileImpact#test_validate_file_impact_requires_file_path().
  TestCodeGraphCallToolFileImpact.test_validate_file_impact_with_file_path: TestCodeGraphCallToolFileImpact#test_validate_file_impact_with_file_path().
  TestCodeGraphCallToolFileImpact.test_file_impact_mode: TestCodeGraphCallToolFileImpact#test_file_impact_mode().
  TestCodeGraphCallToolFileImpact.test_file_impact_nonexistent: TestCodeGraphCallToolFileImpact#test_file_impact_nonexistent().
  TestCodeGraphCallToolFileImpact.test_validate_functions_in_file_requires_file_path: TestCodeGraphCallToolFileImpact#test_validate_functions_in_file_requires_file_path().
  TestCodeGraphCallToolFileImpact.test_functions_in_file_mode: TestCodeGraphCallToolFileImpact#test_functions_in_file_mode().
---
# Module: [`tests/unit/test_call_graph_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py)

## Classes
### `TestCodeGraphCallToolAllFunctions`
- def: [`tests/unit/test_call_graph_tool.py:180`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L180)
- signature: `class TestCodeGraphCallToolAllFunctions:`
- members:
  - `test_all_functions(self, tool)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L182)

### `TestCodeGraphCallToolCallees`
- def: [`tests/unit/test_call_graph_tool.py:313`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L313)
- signature: `class TestCodeGraphCallToolCallees:`
- members:
  - `test_callees_leaf_function(self, tool)` — [`L331`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L331)
  - `test_callees_of_main(self, tool)` — [`L316`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L316)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestCodeGraphCallToolCallers`
- def: [`tests/unit/test_call_graph_tool.py:196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L196)
- signature: `class TestCodeGraphCallToolCallers:`
- members:
  - `test_callers_of_existing_function(self, tool)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L198)
  - `test_callers_of_nonexistent(self, tool)` — [`L212`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L212)
  - `test_callers_qualified_class_method_resolves(self, tool)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L236) — Qualified ``Class.method`` form should resolve, not silently return 0.
  - `test_callers_qualified_zero_hits_with_hint(self, tmp_path)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L260) — When a qualified ``Class.method`` lookup resolves but yields 0
  - `test_callers_with_file_path(self, tool)` — [`L224`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L224)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/call_graph_tool.md#CodeGraphCallTool.execute), [`CodeGraphCallTool`](../../tree_sitter_analyzer/mcp/tools/call_graph_tool.md#CodeGraphCallTool)

### `TestCodeGraphCallToolChain`
- def: [`tests/unit/test_call_graph_tool.py:348`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L348)
- signature: `class TestCodeGraphCallToolChain:`
- members:
  - `test_chain_custom_depth(self, tool)` — [`L364`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L364)
  - `test_chain_from_main(self, tool)` — [`L350`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L350)
  - `test_chain_nonexistent(self, tool)` — [`L377`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L377)

### `TestCodeGraphCallToolDefinition`
- def: [`tests/unit/test_call_graph_tool.py:69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L69)
- signature: `class TestCodeGraphCallToolDefinition:`
- members:
  - `test_get_tool_definition(self, tool)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L70)
  - `test_get_tool_schema_defaults(self, tool)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L85)
  - `test_get_tool_schema_modes(self, tool)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L76)
  - `test_get_tool_schema_no_additional_props(self, tool)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L91)

### `TestCodeGraphCallToolFileImpact`
- def: [`tests/unit/test_call_graph_tool.py:417`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L417)
- signature: `class TestCodeGraphCallToolFileImpact:`
- members:
  - `test_file_impact_mode(self, tool)` — [`L426`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L426)
  - `test_file_impact_nonexistent(self, tool)` — [`L441`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L441)
  - `test_functions_in_file_mode(self, tool)` — [`L457`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L457)
  - `test_validate_file_impact_requires_file_path(self, tool)` — [`L418`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L418)
  - `test_validate_file_impact_with_file_path(self, tool)` — [`L422`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L422)
  - `test_validate_functions_in_file_requires_file_path(self, tool)` — [`L452`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L452)

### `TestCodeGraphCallToolInit`
- def: [`tests/unit/test_call_graph_tool.py:31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L31)
- signature: `class TestCodeGraphCallToolInit:`
- members:
  - `test_get_call_graph_caches(self, tool)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L53)
  - `test_get_call_graph_creates_instance(self, tool)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L48)
  - `test_get_call_graph_raises_without_root(self)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L58)
  - `test_init_with_project_root(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L32)
  - `test_init_without_project_root(self)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L37)
  - `test_set_project_path_resets_graph(self, tool)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L42)
- uses (calls/refs, reference-scoped): [`project_root`](../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.project_root), [`CodeGraphCallTool`](../../tree_sitter_analyzer/mcp/tools/call_graph_tool.md#CodeGraphCallTool), [`get_call_graph`](../../tree_sitter_analyzer/mcp/tools/call_graph_tool.md#CodeGraphCallTool.get_call_graph), [`call_graph_initialized`](../../tree_sitter_analyzer/mcp/tools/call_graph_tool.md#CodeGraphCallTool.call_graph_initialized)  (1 test-only)

### `TestCodeGraphCallToolSummary`
- def: [`tests/unit/test_call_graph_tool.py:159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L159)
- signature: `class TestCodeGraphCallToolSummary:`
- members:
  - `test_default_mode_is_summary(self, tool)` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L170)
  - `test_summary_mode(self, tool)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L161)

### `TestCodeGraphCallToolToonFormat`
- def: [`tests/unit/test_call_graph_tool.py:410`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L410)
- signature: `class TestCodeGraphCallToolToonFormat:`
- members:
  - `test_toon_format_summary(self, tool)` — [`L412`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L412)

### `TestCodeGraphCallToolUnknownMode`
- def: [`tests/unit/test_call_graph_tool.py:394`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L394)
- signature: `class TestCodeGraphCallToolUnknownMode:`
- members:
  - `test_unknown_mode_raises(self, tool)` — [`L396`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L396)

### `TestCodeGraphCallToolValidation`
- def: [`tests/unit/test_call_graph_tool.py:101`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L101)
- signature: `class TestCodeGraphCallToolValidation:`
- members:
  - `test_execute_invalid_mode_fails_before_graph_build(self, tool)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L145)
  - `test_validate_all_functions_no_func_name(self, tool)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L105)
  - `test_validate_callees_requires_func_name(self, tool)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L112)
  - `test_validate_callers_requires_func_name(self, tool)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L108)
  - `test_validate_callers_with_func_name(self, tool)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L120)
  - `test_validate_chain_requires_func_name(self, tool)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L116)
  - `test_validate_default_mode(self, tool)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L123)
  - `test_validate_invalid_mode_lists_valid_modes(self, tool)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L130)
  - `test_validate_invalid_mode_without_function_name(self, tool)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L139)
  - `test_validate_summary_no_func_name(self, tool)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L102)

## Functions
- `tool()` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L21)

## Module values
- `FIXTURES_DIR` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L16)
- `PY_PROJECT` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L17)
- `_WINDOWS_SKIP_PY_FIXTURE` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_graph_tool.py#L12)

