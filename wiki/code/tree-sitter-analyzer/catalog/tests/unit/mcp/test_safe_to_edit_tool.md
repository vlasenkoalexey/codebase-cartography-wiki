---
title: 'Module: tests/unit/mcp/test_safe_to_edit_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_safe_to_edit_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_safe_to_edit_tool`/
symbols:
  _run: _run().
  TARGET_FILE: TARGET_FILE.
  tool: tool().
  TestChecklistSequentialNumbering._checklist: TestChecklistSequentialNumbering#_checklist().
  TestSafeToEditTool.test_execute_returns_risk_level: TestSafeToEditTool#test_execute_returns_risk_level().
  TestSafeToEditTool.test_execute_includes_health_grade: TestSafeToEditTool#test_execute_includes_health_grade().
  TestSafeToEditTool.test_execute_includes_pre_edit_checklist: TestSafeToEditTool#test_execute_includes_pre_edit_checklist().
  TestSafeToEditTool.test_execute_includes_structured_agent_workflow: TestSafeToEditTool#test_execute_includes_structured_agent_workflow().
  TestSafeToEditTool.test_execute_includes_compact_agent_summary: TestSafeToEditTool#test_execute_includes_compact_agent_summary().
  TestSafeToEditTool.test_pre_edit_checklist_uses_uv_pytest_contract: TestSafeToEditTool#test_pre_edit_checklist_uses_uv_pytest_contract().
  TestSafeToEditTool.test_execute_includes_risk_factors: TestSafeToEditTool#test_execute_includes_risk_factors().
  TestSafeToEditTool.test_execute_includes_dependency_info: TestSafeToEditTool#test_execute_includes_dependency_info().
  TestSafeToEditTool.test_execute_includes_test_files: TestSafeToEditTool#test_execute_includes_test_files().
  TestSafeToEditTool.test_edit_type_rename_higher_risk: TestSafeToEditTool#test_edit_type_rename_higher_risk().
  TestSafeToEditTool.test_toon_format: TestSafeToEditTool#test_toon_format().
  TestSafeToEditTool.test_json_format: TestSafeToEditTool#test_json_format().
  TestSafeToEditTool.test_well_connected_file_has_downstream: TestSafeToEditTool#test_well_connected_file_has_downstream().
  TestHelperFunctions.test_find_test_files_for_known_file: TestHelperFunctions#test_find_test_files_for_known_file().
  TestSafeToEditTool.test_file_not_found: TestSafeToEditTool#test_file_not_found().
  TestRiskComputation.test_safe_with_no_risk_factors: TestRiskComputation#test_safe_with_no_risk_factors().
  TestRiskComputation.test_caution_with_moderate_downstream: TestRiskComputation#test_caution_with_moderate_downstream().
  TestRiskComputation.test_dangerous_with_high_downstream_no_tests: TestRiskComputation#test_dangerous_with_high_downstream_no_tests().
  TestRiskComputation.test_rename_adds_risk_factor: TestRiskComputation#test_rename_adds_risk_factor().
  TestRiskComputation.test_init_file_flagged: TestRiskComputation#test_init_file_flagged().
  TestHelperFunctions.test_is_init_file_true: TestHelperFunctions#test_is_init_file_true().
  TestHelperFunctions.test_is_init_file_false: TestHelperFunctions#test_is_init_file_false().
  TestChecklistSequentialNumbering.test_rename_no_downstream_sequential: TestChecklistSequentialNumbering#test_rename_no_downstream_sequential().
  TestChecklistSequentialNumbering.test_refactor_no_downstream_sequential: TestChecklistSequentialNumbering#test_refactor_no_downstream_sequential().
  TestChecklistSequentialNumbering.test_rename_with_downstream_sequential: TestChecklistSequentialNumbering#test_rename_with_downstream_sequential().
  TestChecklistSequentialNumbering.test_health_grade_no_downstream_sequential: TestChecklistSequentialNumbering#test_health_grade_no_downstream_sequential().
  TestChecklistSequentialNumbering.test_rename_downstream_and_health_sequential: TestChecklistSequentialNumbering#test_rename_downstream_and_health_sequential().
  PROJECT_ROOT: PROJECT_ROOT.
  SERVER_FILE: SERVER_FILE.
  TestSafeToEditTool: TestSafeToEditTool#
  TestSafeToEditTool.test_tool_definition: TestSafeToEditTool#test_tool_definition().
  TestSafeToEditTool.test_validate_arguments_missing_path: TestSafeToEditTool#test_validate_arguments_missing_path().
  TestSafeToEditTool.test_validate_arguments_empty_path: TestSafeToEditTool#test_validate_arguments_empty_path().
  TestSafeToEditTool.test_validate_arguments_valid: TestSafeToEditTool#test_validate_arguments_valid().
  TestRiskComputation: TestRiskComputation#
  TestHelperFunctions: TestHelperFunctions#
  TestChecklistSequentialNumbering: TestChecklistSequentialNumbering#
---
# Module: [`tests/unit/mcp/test_safe_to_edit_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py)

## Classes
### `TestChecklistSequentialNumbering`
- def: [`tests/unit/mcp/test_safe_to_edit_tool.py:309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L309)
- doc: build_checklist must emit 1, 2, 3, 4, ... without skipping any number.
- signature: `class TestChecklistSequentialNumbering:`
- members:
  - `test_health_grade_no_downstream_sequential(self)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L360) — poor health (D) + 0 downstream + no edit_type addon: [1, 2, 3, 4].
  - `test_refactor_no_downstream_sequential(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L336) — refactor + 0 downstream: must be [1, 2, 3, 4], not [1, 2, 3, 5].
  - `test_rename_downstream_and_health_sequential(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L374) — rename + downstream + poor health: [1, 2, 3, 4, 5, 6].
  - `test_rename_no_downstream_sequential(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L324) — rename + 0 downstream: must be [1, 2, 3, 4], not [1, 2, 3, 5].
  - `test_rename_with_downstream_sequential(self)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L348) — rename + 2 downstream: must be [1, 2, 3, 4, 5].
- protocol/private: `_checklist`[`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L317)
- uses (calls/refs, reference-scoped): [`build_checklist`](../../../tree_sitter_analyzer/mcp/tools/utils/safe_to_edit_risk.md#build_checklist)

### `TestHelperFunctions`
- def: [`tests/unit/mcp/test_safe_to_edit_tool.py:289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L289)
- signature: `class TestHelperFunctions:`
- members:
  - `test_find_test_files_for_known_file(self)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L296)
  - `test_is_init_file_false(self)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L293)
  - `test_is_init_file_true(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L290)
- uses (calls/refs, reference-scoped): [`_is_init_file`](../../../tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.md#_is_init_file)  (2 test-only)

### `TestRiskComputation`
- def: [`tests/unit/mcp/test_safe_to_edit_tool.py:218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L218)
- signature: `class TestRiskComputation:`
- members:
  - `test_caution_with_moderate_downstream(self)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L232)
  - `test_dangerous_with_high_downstream_no_tests(self)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L243)
  - `test_init_file_flagged(self)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L276)
  - `test_rename_adds_risk_factor(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L254)
  - `test_safe_with_no_risk_factors(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L219)
- uses (calls/refs, reference-scoped): [`_compute_risk`](../../../tree_sitter_analyzer/mcp/tools/safe_to_edit_tool.md#_compute_risk)

### `TestSafeToEditTool`
- def: [`tests/unit/mcp/test_safe_to_edit_tool.py:58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L58)
- signature: `class TestSafeToEditTool:`
- members:
  - `test_edit_type_rename_higher_risk(self, tool)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L158)
  - `test_execute_includes_compact_agent_summary(self, tool)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L118)
  - `test_execute_includes_dependency_info(self, tool)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L149)
  - `test_execute_includes_health_grade(self, tool)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L81)
  - `test_execute_includes_pre_edit_checklist(self, tool)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L86)
  - `test_execute_includes_risk_factors(self, tool)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L144)
  - `test_execute_includes_structured_agent_workflow(self, tool)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L94)
  - `test_execute_includes_test_files(self, tool)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L154)
  - `test_execute_returns_risk_level(self, tool)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L76)
  - `test_file_not_found(self, tool)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L205)
  - `test_json_format(self, tool)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L193)
  - `test_pre_edit_checklist_uses_uv_pytest_contract(self, tool)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L137)
  - `test_tool_definition(self, tool)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L59)
  - `test_toon_format(self, tool)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L182)
  - `test_validate_arguments_empty_path(self, tool)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L69)
  - `test_validate_arguments_missing_path(self, tool)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L65)
  - `test_validate_arguments_valid(self, tool)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L73)
  - `test_well_connected_file_has_downstream(self, tool)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L209)
- uses (calls/refs, reference-scoped): (3 test-only callers)

## Functions
- `_run(coro)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L54)
- `tool(tmp_path)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L21)

## Module values
- `PROJECT_ROOT` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L15)
- `SERVER_FILE` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L17)
- `TARGET_FILE` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_safe_to_edit_tool.py#L16)

