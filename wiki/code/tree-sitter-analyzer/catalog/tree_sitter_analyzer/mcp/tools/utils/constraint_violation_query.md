---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/constraint_violation_query.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/constraint_violation_query.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.constraint_violation_query`/
symbols:
  verdict_from_violations: verdict_from_violations().
  violations_for_files: violations_for_files().
  constraint_risk_factor: constraint_risk_factor().
  logger: logger.
  _BLOCKING_SEVERITIES._BLOCKING_SEVERITIES: _BLOCKING_SEVERITIES._BLOCKING_SEVERITIES.
  _WARNING_SEVERITIES._WARNING_SEVERITIES: _WARNING_SEVERITIES._WARNING_SEVERITIES.
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/constraint_violation_query.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/constraint_violation_query.py)

## Functions
- `constraint_risk_factor(row: dict[str, Any])` — [`L127`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/constraint_violation_query.py#L127) — Render one violation row as a safe_to_edit risk_factor entry.
- `verdict_from_violations(rows: list[dict[str, Any]])` — [`L113`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/constraint_violation_query.py#L113) — Return the verdict implied by a violations list.
- `violations_for_files(project_root: str | None, file_paths: Iterable[str])` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/constraint_violation_query.py#L32) — Return violation rows touching any of the given files.

## Module values
- `_BLOCKING_SEVERITIES` — [`L28`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/constraint_violation_query.py#L28)
- `_WARNING_SEVERITIES` — [`L29`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/constraint_violation_query.py#L29)
- `logger` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/constraint_violation_query.py#L25)

