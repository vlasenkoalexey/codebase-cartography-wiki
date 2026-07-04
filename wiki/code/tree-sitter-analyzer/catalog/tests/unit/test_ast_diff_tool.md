---
title: 'Module: tests/unit/test_ast_diff_tool.py'
type: catalog
provenance: extracted
module: tests/unit/test_ast_diff_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ast_diff_tool`/
symbols:
  TestASTDiffNodeBudget.test_default_bytes_smaller_than_include_bodies_bytes: TestASTDiffNodeBudget#test_default_bytes_smaller_than_include_bodies_bytes().
  _OLD_SRC: _OLD_SRC.
  TestASTDiffNodeBudget.test_default_response_has_no_children_key: TestASTDiffNodeBudget#test_default_response_has_no_children_key().
  TestASTDiffNodeBudget.test_default_response_has_child_count: TestASTDiffNodeBudget#test_default_response_has_child_count().
  TestASTDiffNodeBudget.test_include_node_bodies_true_has_children: TestASTDiffNodeBudget#test_include_node_bodies_true_has_children().
  TestASTDiffNodeBudget.test_over_budget_sets_children_truncated: TestASTDiffNodeBudget#test_over_budget_sets_children_truncated().
  TestAstDiffAgentSummaryEnvelope.test_response_has_agent_summary_with_hunks: TestAstDiffAgentSummaryEnvelope#test_response_has_agent_summary_with_hunks().
  _LANG: _LANG.
  _NEW_SRC: _NEW_SRC.
  TestASTDiffToolInit.test_default_project_root: TestASTDiffToolInit#test_default_project_root().
  TestASTDiffToolInit.test_custom_project_root: TestASTDiffToolInit#test_custom_project_root().
  TestAstDiffAgentSummaryEnvelope.test_response_has_agent_summary_no_hunks: TestAstDiffAgentSummaryEnvelope#test_response_has_agent_summary_no_hunks().
  tool: tool().
  TestASTDiffToolExecution.test_execute_git_timeout_fallback: TestASTDiffToolExecution#test_execute_git_timeout_fallback().
  TestAstDiffAgentSummaryEnvelope.tool: TestAstDiffAgentSummaryEnvelope#tool().
  TestASTDiffNodeBudget._stable_bytes: TestASTDiffNodeBudget#_stable_bytes().
  TestASTDiffToolExecution._subprocess_timeout: TestASTDiffToolExecution#_subprocess_timeout().
  TestASTDiffToolInit: TestASTDiffToolInit#
  TestASTDiffToolDefinition: TestASTDiffToolDefinition#
  TestASTDiffToolDefinition.test_get_tool_definition: TestASTDiffToolDefinition#test_get_tool_definition().
  TestASTDiffToolDefinition.test_get_tool_schema: TestASTDiffToolDefinition#test_get_tool_schema().
  TestASTDiffToolDefinition.test_schema_has_file_path_property: TestASTDiffToolDefinition#test_schema_has_file_path_property().
  TestASTDiffToolValidation: TestASTDiffToolValidation#
  TestASTDiffToolValidation.test_validate_with_file_path: TestASTDiffToolValidation#test_validate_with_file_path().
  TestASTDiffToolValidation.test_validate_missing_file_path: TestASTDiffToolValidation#test_validate_missing_file_path().
  TestASTDiffToolValidation.test_validate_empty_file_path: TestASTDiffToolValidation#test_validate_empty_file_path().
  TestASTDiffToolValidation.test_validate_diff_files_missing_new_file: TestASTDiffToolValidation#test_validate_diff_files_missing_new_file().
  TestASTDiffToolValidation.test_validate_diff_strings_missing_new_source: TestASTDiffToolValidation#test_validate_diff_strings_missing_new_source().
  TestASTDiffToolValidation.test_validate_diff_strings_missing_language: TestASTDiffToolValidation#test_validate_diff_strings_missing_language().
  TestASTDiffToolValidation.test_validate_diff_files_valid: TestASTDiffToolValidation#test_validate_diff_files_valid().
  TestASTDiffToolValidation.test_validate_diff_strings_valid: TestASTDiffToolValidation#test_validate_diff_strings_valid().
  TestASTDiffToolExecution: TestASTDiffToolExecution#
  TestASTDiffToolExecution.test_execute_file_not_found: TestASTDiffToolExecution#test_execute_file_not_found().
  TestASTDiffToolExecution.test_execute_diff_files_mode: TestASTDiffToolExecution#test_execute_diff_files_mode().
  TestASTDiffToolExecution.test_execute_git_mode: TestASTDiffToolExecution#test_execute_git_mode().
  TestASTDiffToolExecution.test_execute_with_invalid_mode: TestASTDiffToolExecution#test_execute_with_invalid_mode().
  TestASTDiffModeInference: TestASTDiffModeInference#
  TestASTDiffModeInference.test_infer_diff_git_from_refs: TestASTDiffModeInference#test_infer_diff_git_from_refs().
  TestASTDiffModeInference.test_infer_diff_strings_from_sources: TestASTDiffModeInference#test_infer_diff_strings_from_sources().
  TestASTDiffModeInference.test_infer_diff_files_default: TestASTDiffModeInference#test_infer_diff_files_default().
  TestASTDiffModeInference.test_default_refs_do_not_steal_string_diff: TestASTDiffModeInference#test_default_refs_do_not_steal_string_diff().
  TestASTDiffModeInference.test_refs_without_file_path_do_not_infer_git: TestASTDiffModeInference#test_refs_without_file_path_do_not_infer_git().
  TestASTDiffModeInference.test_explicit_mode_wins_over_inference: TestASTDiffModeInference#test_explicit_mode_wins_over_inference().
  TestASTDiffModeInference.test_validate_git_mode_inferred_no_explicit_mode: TestASTDiffModeInference#test_validate_git_mode_inferred_no_explicit_mode().
  TestASTDiffModeInference.test_validate_strings_mode_inferred_no_explicit_mode: TestASTDiffModeInference#test_validate_strings_mode_inferred_no_explicit_mode().
  TestASTDiffModeInference.test_execute_git_inferred_no_explicit_mode: TestASTDiffModeInference#test_execute_git_inferred_no_explicit_mode().
  TestASTDiffModeInference.test_execute_strings_inferred_no_explicit_mode: TestASTDiffModeInference#test_execute_strings_inferred_no_explicit_mode().
  TestASTDiffSchemaHonesty: TestASTDiffSchemaHonesty#
  TestASTDiffSchemaHonesty.test_mode_not_in_required: TestASTDiffSchemaHonesty#test_mode_not_in_required().
  TestASTDiffErrorQuality: TestASTDiffErrorQuality#
  TestASTDiffErrorQuality.test_no_match_error_mentions_all_three_modes: TestASTDiffErrorQuality#test_no_match_error_mentions_all_three_modes().
  TestASTDiffNodeBudget: TestASTDiffNodeBudget#
  TestASTDiffNodeBudget.test_schema_has_include_node_bodies_param: TestASTDiffNodeBudget#test_schema_has_include_node_bodies_param().
  TestAstDiffAgentSummaryEnvelope: TestAstDiffAgentSummaryEnvelope#
  TestAstDiffAgentSummaryEnvelope.test_response_has_agent_summary_parse_failure: TestAstDiffAgentSummaryEnvelope#test_response_has_agent_summary_parse_failure().
---
# Module: [`tests/unit/test_ast_diff_tool.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py)

## Classes
### `TestASTDiffErrorQuality`
- def: [`tests/unit/test_ast_diff_tool.py:329`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L329)
- doc: Leg E — no-signature-match error enumerates all three mode signatures.
- signature: `class TestASTDiffErrorQuality:`
- members:
  - `test_no_match_error_mentions_all_three_modes(self, tool)` — [`L332`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L332)

### `TestASTDiffModeInference`
- def: [`tests/unit/test_ast_diff_tool.py:190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L190)
- doc: Leg A+B — mode is inferred from argument shape when omitted.
- signature: `class TestASTDiffModeInference:`
- members:
  - `test_default_refs_do_not_steal_string_diff(self, tool)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L218)
  - `test_execute_git_inferred_no_explicit_mode(self, tool)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L278)
  - `test_execute_strings_inferred_no_explicit_mode(self, tool)` — [`L296`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L296)
  - `test_explicit_mode_wins_over_inference(self, tool)` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L238)
  - `test_infer_diff_files_default(self, tool)` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L213)
  - `test_infer_diff_git_from_refs(self, tool)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L193)
  - `test_infer_diff_strings_from_sources(self, tool)` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L202)
  - `test_refs_without_file_path_do_not_infer_git(self, tool)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L232)
  - `test_validate_git_mode_inferred_no_explicit_mode(self, tool)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L251)
  - `test_validate_strings_mode_inferred_no_explicit_mode(self, tool)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L264)

### `TestASTDiffNodeBudget`
- def: [`tests/unit/test_ast_diff_tool.py:356`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L356)
- doc: Issue #552 — default response must NOT contain children; opt-in adds them.
- signature: `class TestASTDiffNodeBudget:`
- members:
  - `test_default_bytes_smaller_than_include_bodies_bytes(self, tool)` — [`L414`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L414) — DOCUMENTED RELATIONSHIP: default response < include_node_bodies=True response.
  - `test_default_response_has_child_count(self, tool)` — [`L381`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L381) — Hunk nodes MUST have child_count (exact pin) when include_node_bodies is omitted.
  - `test_default_response_has_no_children_key(self, tool)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L360) — Hunk nodes must NOT contain a 'children' key when include_node_bodies is omitted.
  - `test_include_node_bodies_true_has_children(self, tool)` — [`L452`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L452) — When include_node_bodies=True, hunk nodes MUST contain 'children' key.
  - `test_over_budget_sets_children_truncated(self, tool)` — [`L474`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L474) — When include_node_bodies=True and response exceeds budget, set children_truncated.
  - `test_schema_has_include_node_bodies_param(self, tool)` — [`L402`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L402) — Schema must expose include_node_bodies boolean param.
- protocol/private: `_stable_bytes`[`L439`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L439)
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestASTDiffSchemaHonesty`
- def: [`tests/unit/test_ast_diff_tool.py:318`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L318)
- doc: Leg C — mode must NOT be in schema required.
- signature: `class TestASTDiffSchemaHonesty:`
- members:
  - `test_mode_not_in_required(self, tool)` — [`L321`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L321)

### `TestASTDiffToolDefinition`
- def: [`tests/unit/test_ast_diff_tool.py:27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L27)
- signature: `class TestASTDiffToolDefinition:`
- members:
  - `test_get_tool_definition(self, tool)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L28)
  - `test_get_tool_schema(self, tool)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L34)
  - `test_schema_has_file_path_property(self, tool)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L41)

### `TestASTDiffToolExecution`
- def: [`tests/unit/test_ast_diff_tool.py:115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L115)
- signature: `class TestASTDiffToolExecution:`
- members:
  - `test_execute_diff_files_mode(self, tool)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L126)
  - `test_execute_file_not_found(self, tool)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L117)
  - `test_execute_git_mode(self, tool)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L145)
  - `test_execute_git_timeout_fallback(self, tool)` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L160) — _diff_git falls back to empty string on subprocess TimeoutExpired (lines 234-235, 247-248).
  - `test_execute_with_invalid_mode(self, tool)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L178)
- protocol/private: `_subprocess_timeout`[`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L164)

### `TestASTDiffToolInit`
- def: [`tests/unit/test_ast_diff_tool.py:17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L17)
- signature: `class TestASTDiffToolInit:`
- members:
  - `test_custom_project_root(self)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L22)
  - `test_default_project_root(self)` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L18)
- uses (calls/refs, reference-scoped): [`project_root`](../../tree_sitter_analyzer/mcp/tools/base_tool.md#BaseMCPTool.project_root), [`ASTDiffTool`](../../tree_sitter_analyzer/mcp/tools/ast_diff_tool.md#ASTDiffTool)

### `TestASTDiffToolValidation`
- def: [`tests/unit/test_ast_diff_tool.py:46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L46)
- signature: `class TestASTDiffToolValidation:`
- members:
  - `test_validate_diff_files_missing_new_file(self, tool)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L64)
  - `test_validate_diff_files_valid(self, tool)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L87)
  - `test_validate_diff_strings_missing_language(self, tool)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L76)
  - `test_validate_diff_strings_missing_new_source(self, tool)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L69)
  - `test_validate_diff_strings_valid(self, tool)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L100)
  - `test_validate_empty_file_path(self, tool)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L59)
  - `test_validate_missing_file_path(self, tool)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L54)
  - `test_validate_with_file_path(self, tool)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L47)

### `TestAstDiffAgentSummaryEnvelope`
- def: [`tests/unit/test_ast_diff_tool.py:500`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L500)
- doc: #744: ast_diff must include agent_summary and summary_line in response.
- signature: `class TestAstDiffAgentSummaryEnvelope:`
- members:
  - `test_response_has_agent_summary_no_hunks(self, tool)` — [`L529`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L529) — When old == new (no hunks), agent_summary dict says 'No AST changes'.
  - `test_response_has_agent_summary_parse_failure(self, tool)` — [`L545`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L545) — When both sources fail to parse (unsupported language), verdict is ERROR.
  - `test_response_has_agent_summary_with_hunks(self, tool)` — [`L508`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L508) — When diff produces hunks, agent_summary is a dict with count in summary_line.
  - `tool(self)` — [`L504`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L504)
- uses (calls/refs, reference-scoped): [`ASTDiffTool`](../../tree_sitter_analyzer/mcp/tools/ast_diff_tool.md#ASTDiffTool)  (3 test-only)

## Functions
- `tool()` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L13)

## Module values
- `_LANG` — [`L353`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L353)
- `_NEW_SRC` — [`L352`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L352)
- `_OLD_SRC` — [`L351`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff_tool.py#L351)

