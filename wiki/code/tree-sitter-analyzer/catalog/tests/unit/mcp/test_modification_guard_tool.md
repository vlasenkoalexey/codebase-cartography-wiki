---
title: 'Module: tests/unit/mcp/test_modification_guard_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_modification_guard_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_modification_guard_tool`/
symbols:
  _trace_result: _trace_result().
  TestModificationGuardToolInitialization.test_set_project_path_propagates: TestModificationGuardToolInitialization#test_set_project_path_propagates().
  TestModificationGuardToolExecution.test_safe_verdict_no_callers: TestModificationGuardToolExecution#test_safe_verdict_no_callers().
  TestModificationGuardToolExecution.test_caution_verdict_few_callers: TestModificationGuardToolExecution#test_caution_verdict_few_callers().
  TestModificationGuardToolExecution.test_review_verdict_many_callers: TestModificationGuardToolExecution#test_review_verdict_many_callers().
  TestModificationGuardToolExecution.test_unsafe_verdict_high_callers: TestModificationGuardToolExecution#test_unsafe_verdict_high_callers().
  TestModificationGuardToolExecution.test_ast_caller_count_surfaced_when_file_path_given: TestModificationGuardToolExecution#test_ast_caller_count_surfaced_when_file_path_given().
  TestModificationGuardToolExecution.test_required_actions_populated_for_unsafe: TestModificationGuardToolExecution#test_required_actions_populated_for_unsafe().
  TestModificationGuardToolExecution.test_callers_by_file: TestModificationGuardToolExecution#test_callers_by_file().
  TestModificationGuardToolExecution.test_symbol_returned_in_result: TestModificationGuardToolExecution#test_symbol_returned_in_result().
  TestModificationGuardToolExecution.test_modification_type_returned_in_result: TestModificationGuardToolExecution#test_modification_type_returned_in_result().
  TestCriticalNodesIntegration.test_critical_node_adds_architecture_warning: TestCriticalNodesIntegration#test_critical_node_adds_architecture_warning().
  TestCriticalNodesIntegration.test_critical_node_boosts_verdict: TestCriticalNodesIntegration#test_critical_node_boosts_verdict().
  TestCriticalNodesIntegration.test_non_critical_node_no_architecture_info: TestCriticalNodesIntegration#test_non_critical_node_no_architecture_info().
  TestCriticalNodesIntegration.test_no_critical_nodes_file_still_works: TestCriticalNodesIntegration#test_no_critical_nodes_file_still_works().
  TestModificationGuardToolExecution.test_unknown_symbol_is_not_found_not_safe: TestModificationGuardToolExecution#test_unknown_symbol_is_not_found_not_safe().
  TestModificationGuardToolExecution.test_known_symbol_zero_callers_is_still_safe_not_notfound: TestModificationGuardToolExecution#test_known_symbol_zero_callers_is_still_safe_not_notfound().
  TestModificationGuardToolExecution.test_try_ast_caller_count_calls_codegraph_tool: TestModificationGuardToolExecution#test_try_ast_caller_count_calls_codegraph_tool().
  TestModificationGuardToolExecution.test_trace_impact_failure_surfaces_error: TestModificationGuardToolExecution#test_trace_impact_failure_surfaces_error().
  TestModificationGuardToolDefinition.test_description_contains_when_to_use: TestModificationGuardToolDefinition#test_description_contains_when_to_use().
  TestModificationGuardToolDefinition.test_description_contains_when_not_to_use: TestModificationGuardToolDefinition#test_description_contains_when_not_to_use().
  TestModificationGuardToolDefinition.test_required_fields: TestModificationGuardToolDefinition#test_required_fields().
  TestModificationGuardToolDefinition.test_modification_type_enum: TestModificationGuardToolDefinition#test_modification_type_enum().
  TestModificationGuardToolValidation.test_missing_symbol_raises: TestModificationGuardToolValidation#test_missing_symbol_raises().
  TestModificationGuardToolValidation.test_empty_symbol_raises: TestModificationGuardToolValidation#test_empty_symbol_raises().
  TestModificationGuardToolValidation.test_invalid_modification_type_raises: TestModificationGuardToolValidation#test_invalid_modification_type_raises().
  TestModificationGuardToolValidation.test_valid_arguments_pass: TestModificationGuardToolValidation#test_valid_arguments_pass().
  TestModificationGuardToolExecution.test_try_ast_caller_count_returns_none_on_tool_error: TestModificationGuardToolExecution#test_try_ast_caller_count_returns_none_on_tool_error().
  TestModificationGuardToolExecution.test_try_ast_caller_count_ignores_non_integer_count: TestModificationGuardToolExecution#test_try_ast_caller_count_ignores_non_integer_count().
  tool: tool().
  TestModificationGuardToolInitialization.test_init_creates_tool: TestModificationGuardToolInitialization#test_init_creates_tool().
  TestModificationGuardToolInitialization.test_init_creates_trace_impact_tool: TestModificationGuardToolInitialization#test_init_creates_trace_impact_tool().
  TestModificationGuardToolInitialization: TestModificationGuardToolInitialization#
  TestModificationGuardToolDefinition: TestModificationGuardToolDefinition#
  TestModificationGuardToolValidation: TestModificationGuardToolValidation#
  TestModificationGuardToolExecution: TestModificationGuardToolExecution#
  TestCriticalNodesIntegration: TestCriticalNodesIntegration#
---
# Module: [`tests/unit/mcp/test_modification_guard_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py)

## Classes
### `TestCriticalNodesIntegration`
- def: [`tests/unit/mcp/test_modification_guard_tool.py:448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L448)
- doc: modification_guard reads critical_nodes.json and boosts warnings.
- signature: `class TestCriticalNodesIntegration:`
- members:
  - `test_critical_node_adds_architecture_warning(self, tmp_path: Path)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L452) — If symbol is in critical_nodes.json, result includes architecture info.
  - `test_critical_node_boosts_verdict(self, tmp_path: Path)` — [`L489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L489) — Top-10 critical node boosts safety verdict by one level.
  - `test_no_critical_nodes_file_still_works(self, tool: ModificationGuardTool)` — [`L545`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L545) — Without critical_nodes.json, tool works normally (no crash).
  - `test_non_critical_node_no_architecture_info(self, tmp_path: Path)` — [`L518`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L518) — Symbols not in critical_nodes.json have no architecture fields.
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool.execute), [`ModificationGuardTool`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool), [`_trace_impact_tool`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool._trace_impact_tool)  (1 test-only)

### `TestModificationGuardToolDefinition`
- def: [`tests/unit/mcp/test_modification_guard_tool.py:57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L57)
- doc: Tests for get_tool_definition().
- signature: `class TestModificationGuardToolDefinition:`
- members:
  - `test_description_contains_when_not_to_use(self, tool: ModificationGuardTool)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L67) — Test that the description contains WHEN NOT TO USE section.
  - `test_description_contains_when_to_use(self, tool: ModificationGuardTool)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L60) — Test that the description contains WHEN TO USE section.
  - `test_modification_type_enum(self, tool: ModificationGuardTool)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L81) — Test that modification_type has correct enum values.
  - `test_required_fields(self, tool: ModificationGuardTool)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L74) — Test that symbol and modification_type are required.
- uses (calls/refs, reference-scoped): [`ModificationGuardTool`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool.get_tool_definition)

### `TestModificationGuardToolExecution`
- def: [`tests/unit/mcp/test_modification_guard_tool.py:118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L118)
- doc: Tests for execute() — core test class.
- signature: `class TestModificationGuardToolExecution:`
- members:
  - `test_ast_caller_count_surfaced_when_file_path_given(self, tool: ModificationGuardTool)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L266) — Guard exposes AST caller count alongside trace-derived occurrences.
  - `test_callers_by_file(self, tool: ModificationGuardTool)` — [`L371`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L371) — Test that callers_by_file groups usages correctly by file.
  - `test_caution_verdict_few_callers(self, tool: ModificationGuardTool)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L202) — Test that 3 callers (low impact) produces safety_verdict=CAUTION.
  - `test_known_symbol_zero_callers_is_still_safe_not_notfound(self, tool: ModificationGuardTool)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L176) — The distinction edit-08 requires: a KNOWN symbol with 0 callers
  - `test_modification_type_returned_in_result(self, tool: ModificationGuardTool)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L426) — Test that modification_type is echoed back in the result.
  - `test_required_actions_populated_for_unsafe(self, tool: ModificationGuardTool)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L352) — Test that UNSAFE verdict includes a non-empty required_actions list.
  - `test_review_verdict_many_callers(self, tool: ModificationGuardTool)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L226) — Test that 10 callers (medium impact) produces safety_verdict=REVIEW.
  - `test_safe_verdict_no_callers(self, tool: ModificationGuardTool)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L122) — Test that 0 callers produces safety_verdict=SAFE.
  - `test_symbol_returned_in_result(self, tool: ModificationGuardTool)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L411) — Test that the result includes the queried symbol.
  - `test_trace_impact_failure_surfaces_error(self, tool: ModificationGuardTool)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L393) — Test that a trace_impact failure surfaces an error in the result.
  - `test_try_ast_caller_count_calls_codegraph_tool(self, tool: ModificationGuardTool)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L298) — AST reconciliation uses callers_tool and returns its integer count.
  - `test_try_ast_caller_count_ignores_non_integer_count(self, tool: ModificationGuardTool)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L336) — Only integer caller_count values are surfaced.
  - `test_try_ast_caller_count_returns_none_on_tool_error(self, tool: ModificationGuardTool)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L323) — AST reconciliation is best-effort and must not fail the guard.
  - `test_unknown_symbol_is_not_found_not_safe(self, tool: ModificationGuardTool)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L139) — Wave 1b (audit edit-08): a symbol that resolves to ZERO occurrences
  - `test_unsafe_verdict_high_callers(self, tool: ModificationGuardTool)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L245) — Test that 25 callers (high impact) produces safety_verdict=UNSAFE.
- uses (calls/refs, reference-scoped): [`project_root`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.project_root), [`execute`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool.execute), [`ModificationGuardTool`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool), [`_trace_impact_tool`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool._trace_impact_tool), [`_try_ast_caller_count`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool._try_ast_caller_count)  (1 test-only)

### `TestModificationGuardToolInitialization`
- def: [`tests/unit/mcp/test_modification_guard_tool.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L38)
- doc: Tests for tool initialization.
- signature: `class TestModificationGuardToolInitialization:`
- members:
  - `test_init_creates_tool(self, tool: ModificationGuardTool)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L41) — Test that initialization creates a tool instance.
  - `test_init_creates_trace_impact_tool(self, tool: ModificationGuardTool)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L45) — Test that initialization also creates an inner TraceImpactTool.
  - `test_set_project_path_propagates(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L49) — Test that set_project_path propagates to the inner trace_impact tool.
- uses (calls/refs, reference-scoped): [`project_root`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.project_root), [`set_project_path`](../../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.set_project_path), [`ModificationGuardTool`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool), [`_trace_impact_tool`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool._trace_impact_tool)

### `TestModificationGuardToolValidation`
- def: [`tests/unit/mcp/test_modification_guard_tool.py:90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L90)
- doc: Tests for validate_arguments().
- signature: `class TestModificationGuardToolValidation:`
- members:
  - `test_empty_symbol_raises(self, tool: ModificationGuardTool)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L98) — Test that empty symbol raises ValueError.
  - `test_invalid_modification_type_raises(self, tool: ModificationGuardTool)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L103) — Test that an invalid modification_type raises ValueError.
  - `test_missing_symbol_raises(self, tool: ModificationGuardTool)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L93) — Test that missing symbol raises ValueError.
  - `test_valid_arguments_pass(self, tool: ModificationGuardTool)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L110) — Test that valid arguments pass validation.
- uses (calls/refs, reference-scoped): [`ModificationGuardTool`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/modification_guard_tool.md#ModificationGuardTool.validate_arguments)

## Functions
- `_trace_result(total_count: int, usages: list[dict[str, object]] | None = None)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L26) — Build a fake trace_impact result dict.
- `tool()` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_modification_guard_tool.py#L21) — Create a fresh ModificationGuardTool instance for each test.

