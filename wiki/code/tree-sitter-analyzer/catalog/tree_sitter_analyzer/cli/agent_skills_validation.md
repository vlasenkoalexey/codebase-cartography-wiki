---
title: 'Module: tree_sitter_analyzer/cli/agent_skills_validation.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/agent_skills_validation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.agent_skills_validation`/
symbols:
  build_skill_validation: build_skill_validation().
  _next_fix: _next_fix().
  _selected_gaps: _selected_gaps().
  _total_gap_count: _total_gap_count().
  BLOCKING_GAP_KEYS: BLOCKING_GAP_KEYS.
  CAUTION_GAP_KEYS: CAUTION_GAP_KEYS.
  OPTIONAL_GAP_KEYS: OPTIONAL_GAP_KEYS.
  _validation_status: _validation_status().
  _blocking_fix: _blocking_fix().
---
# Module: [`tree_sitter_analyzer/cli/agent_skills_validation.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_validation.py)

## Functions
- `_blocking_fix(blocking: dict[str, Any])` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_validation.py#L83) — Suggest a fix for blocking skill metadata gaps.
- `_next_fix(status: str, blocking: dict[str, Any], caution: dict[str, Any], optional: dict[str, Any])` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_validation.py#L66) — Suggest the next metadata cleanup action.
- `_selected_gaps(gaps: dict[str, Any], keys: tuple[str, ...])` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_validation.py#L33) — Return non-empty gap entries for the requested keys.
- `_total_gap_count(grouped_gaps: dict[str, Any])` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_validation.py#L46) — Count booleans and list-like gap values in a grouped gap map.
- `_validation_status(blocking_count: int, caution_count: int)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_validation.py#L57) — Return a coarse readiness status for agent skill use.
- `build_skill_validation(gaps: dict[str, Any])` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_validation.py#L12) — Build an agent-friendly validation summary from inventory gaps.

## Module values
- `BLOCKING_GAP_KEYS` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_validation.py#L7)
- `CAUTION_GAP_KEYS` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_validation.py#L8)
- `OPTIONAL_GAP_KEYS` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_validation.py#L9)

