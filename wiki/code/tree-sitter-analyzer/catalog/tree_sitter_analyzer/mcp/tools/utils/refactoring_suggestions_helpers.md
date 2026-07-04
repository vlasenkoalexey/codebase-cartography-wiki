---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.refactoring_suggestions_helpers`/
symbols:
  make_agent_summary: make_agent_summary().
  build_success_response: build_success_response().
  make_pattern: make_pattern().
  make_extraction: make_extraction().
  error_response: error_response().
  get_nesting_depth: get_nesting_depth().
  get_nesting_depth.walk: get_nesting_depth().walk().
  finalize_suggestions: finalize_suggestions().
  _to_project_relative: _to_project_relative().
  is_static_method: is_static_method().
  get_refactoring_tool_schema: get_refactoring_tool_schema().
  _add_line_range: _add_line_range().
  make_summary: make_summary().
  strip_precise_plan_skeletons: strip_precise_plan_skeletons().
  _agent_risk: _agent_risk().
  _agent_verdict: _agent_verdict().
  _next_step_for: _next_step_for().
  _tests_for: _tests_for().
  _stop_condition_for: _stop_condition_for().
  _dedupe_tests: _dedupe_tests().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py)

## Functions
- `_add_line_range(result: dict[str, Any], kwargs: dict[str, Any])` — [`L344`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L344) — Attach a line_range object to a suggestion when present.
- `_agent_risk(suggestions: list[dict[str, Any]])` — [`L352`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L352)
- `_agent_verdict(suggestions: list[dict[str, Any]])` — [`L361`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L361) — J9 (round-22): map suggestion severities to the cross-tool verdict.
- `_dedupe_tests(commands: list[str])` — [`L418`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L418)
- `_next_step_for(suggestion: dict[str, Any])` — [`L379`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L379)
- `_stop_condition_for(suggestion: dict[str, Any])` — [`L406`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L406)
- `_tests_for(suggestion: dict[str, Any])` — [`L399`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L399)
- `_to_project_relative(file_path: str, project_root: str | None)` — [`L10`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L10) — Return ``file_path`` rendered as a project-relative path when possible.
- `build_success_response(file_path: str, suggestions: list[dict[str, Any]], max_suggestions: int, include_skeleton: bool, *, project_root: str | None = None)` — [`L246`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L246) — Build the final successful refactoring response.
- `error_response(file_path: str, error: str, *, project_root: str | None = None)` — [`L320`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L320) — Return a standardized error response.
- `finalize_suggestions(suggestions: list[dict[str, Any]], max_suggestions: int, include_skeleton: bool)` — [`L297`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L297) — Apply presentation defaults and ordering to suggestions.
- `get_nesting_depth(node: ast.AST)` — [`L39`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L39) — Calculate the maximum nesting depth of a function.
- `get_refactoring_tool_schema()` — [`L200`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L200) — Return the JSON schema for refactoring suggestion tool input.
- `is_static_method(node: ast.FunctionDef)` — [`L57`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L57) — Detect if a method body never references self/cls.
- `make_agent_summary(file_path: str, suggestions: list[dict[str, Any]])` — [`L123`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L123) — Build a compact next-action summary for agent workflows.
- `make_extraction(rule: dict[str, Any], priority_score: int = 50, **kwargs: Any)` — [`L89`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L89) — Build an extraction suggestion dict from a rule template.
- `make_pattern(rule: dict[str, Any], priority_score: int = 50, **kwargs: Any)` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L71) — Build a pattern suggestion dict from a rule template.
- `make_summary(suggestions: list[dict[str, Any]])` — [`L106`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L106) — Build a human-readable summary of all suggestions.
- `strip_precise_plan_skeletons(suggestions: list[dict[str, Any]])` — [`L310`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L310) — Remove extraction skeletons from precise plans in place.
- `walk(n: ast.AST, depth: int)` — [`L43`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_helpers.py#L43)

