---
title: 'Module: tests/unit/mcp/test_base_mcp_tool_contract.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_base_mcp_tool_contract.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_base_mcp_tool_contract`/
symbols:
  _make_tools: _make_tools().
  _tool_id: _tool_id().
  TOOLS: TOOLS.
  TestUniversalOutputFormatParam.test_every_contract_tool_accepts_output_format: TestUniversalOutputFormatParam#test_every_contract_tool_accepts_output_format().
  TestBaseMCPToolContract.test_get_tool_definition_returns_required_top_level_keys: TestBaseMCPToolContract#test_get_tool_definition_returns_required_top_level_keys().
  TestBaseMCPToolContract.test_name_is_non_empty_string: TestBaseMCPToolContract#test_name_is_non_empty_string().
  TestBaseMCPToolContract.test_set_project_path_does_not_raise: TestBaseMCPToolContract#test_set_project_path_does_not_raise().
  TestBaseMCPToolContract.test_input_schema_has_properties: TestBaseMCPToolContract#test_input_schema_has_properties().
  TestBaseMCPToolContract.test_tool_name_is_stable_across_calls: TestBaseMCPToolContract#test_tool_name_is_stable_across_calls().
  TestBaseMCPToolContract.test_output_format_defaults_to_toon: TestBaseMCPToolContract#test_output_format_defaults_to_toon().
  TestUniversalOutputFormatParam.test_output_format_accepted_when_schema_omits_it: TestUniversalOutputFormatParam#test_output_format_accepted_when_schema_omits_it().
  TestUniversalOutputFormatParam.test_genuinely_unknown_param_still_rejected: TestUniversalOutputFormatParam#test_genuinely_unknown_param_still_rejected().
  TestBaseMCPToolContract: TestBaseMCPToolContract#
  TestUniversalOutputFormatParam: TestUniversalOutputFormatParam#
---
# Module: [`tests/unit/mcp/test_base_mcp_tool_contract.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py)

## Classes
### `TestBaseMCPToolContract`
- def: [`tests/unit/mcp/test_base_mcp_tool_contract.py:60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L60)
- doc: Parametrized contract suite — one test class, 6 invariants × N tools.
- signature: `class TestBaseMCPToolContract:`
- members:
  - `test_get_tool_definition_returns_required_top_level_keys(self, tool: object)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L64) — Invariant 1: get_tool_definition() returns a dict with name, description, inputSchema.
  - `test_input_schema_has_properties(self, tool: object)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L94) — Invariant 4: inputSchema has 'properties' key; 'required' is optional (valid when all params optional).
  - `test_name_is_non_empty_string(self, tool: object)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L76) — Invariant 2: the 'name' in get_tool_definition() is a non-empty string.
  - `test_output_format_defaults_to_toon(self, tool: object)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L127) — Invariant 6: output_format property defaults to 'toon' (MCP token-efficiency design).
  - `test_set_project_path_does_not_raise(self, tool: object)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L86) — Invariant 3: set_project_path('/tmp') completes without raising.
  - `test_tool_name_is_stable_across_calls(self, tool: object)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L118) — Invariant 5: get_tool_definition()['name'] is identical across two calls.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestUniversalOutputFormatParam`
- def: [`tests/unit/mcp/test_base_mcp_tool_contract.py:146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L146)
- doc: #651: output_format is a universal envelope param. enforce_strict_params
- signature: `class TestUniversalOutputFormatParam:`
- members:
  - `test_every_contract_tool_accepts_output_format(self, tool: object)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L177)
  - `test_genuinely_unknown_param_still_rejected(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L167)
  - `test_output_format_accepted_when_schema_omits_it(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L152)
- uses (calls/refs, reference-scoped): [`enforce_strict_params`](../../../tree_sitter_analyzer/mcp/utils/schema_strictness.md#enforce_strict_params)  (2 test-only)

## Functions
- `_make_tools()` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L34) — Return one instantiated instance of each tool under contract.
- `_tool_id(tool: object)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L53)

## Module values
- `TOOLS` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_base_mcp_tool_contract.py#L57)

