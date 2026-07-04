---
title: 'Module: tests/unit/test_issue_446_envelope_polish.py'
type: catalog
provenance: extracted
module: tests/unit/test_issue_446_envelope_polish.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_issue_446_envelope_polish`/
symbols:
  TestOverviewVerdictHonesty.test_plain_informational_overview_verdict_is_info: TestOverviewVerdictHonesty#test_plain_informational_overview_verdict_is_info().
  TestOverviewVerdictHonesty.test_overview_with_health_checks_verdict_reflects_findings: TestOverviewVerdictHonesty#test_overview_with_health_checks_verdict_reflects_findings().
  TestSummaryLineShipping.test_overview_tool_summary_line_canonical_location: TestSummaryLineShipping#test_overview_tool_summary_line_canonical_location().
  TestStatusToolNullFields.test_indexed_status_omits_null_schema_version: TestStatusToolNullFields#test_indexed_status_omits_null_schema_version().
  TestStatusToolNullFields.test_warn_status_omits_null_hint: TestStatusToolNullFields#test_warn_status_omits_null_hint().
  TestStatusToolNullFields.test_indexed_status_real_next_step_not_empty: TestStatusToolNullFields#test_indexed_status_real_next_step_not_empty().
  TestSummaryLineShipping.test_status_tool_summary_line_canonical_location: TestSummaryLineShipping#test_status_tool_summary_line_canonical_location().
  test_status_stale_lag_next_step: test_status_stale_lag_next_step().
  test_status_schema_version_included_when_present: test_status_schema_version_included_when_present().
  test_status_warn_branch_schema_version_included: test_status_warn_branch_schema_version_included().
  _run: _run().
  _write: _write().
  test_overview_risk_unknown_maps_to_info: test_overview_risk_unknown_maps_to_info().
  test_overview_review_requires_real_signals: test_overview_review_requires_real_signals().
  TestStatusToolNullFields: TestStatusToolNullFields#
  TestOverviewVerdictHonesty: TestOverviewVerdictHonesty#
  TestSummaryLineShipping: TestSummaryLineShipping#
---
# Module: [`tests/unit/test_issue_446_envelope_polish.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py)

## Classes
### `TestOverviewVerdictHonesty`
- def: [`tests/unit/test_issue_446_envelope_polish.py:128`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L128)
- doc: Issue #446 Item 3: overview verdict should be INFO for plain info, REVIEW only when code needs review.
- signature: `class TestOverviewVerdictHonesty:`
- members:
  - `test_overview_with_health_checks_verdict_reflects_findings(self)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L156) — overview with include_health=true should have verdict=REVIEW only when problems found.
  - `test_plain_informational_overview_verdict_is_info(self)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L131) — Plain project overview (include_health=False) → verdict=INFO, not REVIEW.
- uses (calls/refs, reference-scoped): [`ProjectOverviewTool`](../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.execute)  (2 test-only)

### `TestStatusToolNullFields`
- def: [`tests/unit/test_issue_446_envelope_polish.py:34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L34)
- doc: Issue #446 Item 1: status tool should omit None/null fields.
- signature: `class TestStatusToolNullFields:`
- members:
  - `test_indexed_status_omits_null_schema_version(self)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L38) — When schema_version is None, it should be omitted (not sent as null).
  - `test_indexed_status_real_next_step_not_empty(self)` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L91) — indexed status (verdict=INFO) should have real next_step, not empty string.
  - `test_warn_status_omits_null_hint(self)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L74) — When hint is None (not provided), it should be omitted.
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_status_tool.md#CodeGraphStatusTool.execute), [`CodeGraphStatusTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_status_tool.md#CodeGraphStatusTool)

### `TestSummaryLineShipping`
- def: [`tests/unit/test_issue_446_envelope_polish.py:179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L179)
- doc: Issue #446 Item 2: summary_line appears in 3 places; reduce to agent_summary.
- signature: `class TestSummaryLineShipping:`
- members:
  - `test_overview_tool_summary_line_canonical_location(self)` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L219) — overview tool summary_line should be canonical in agent_summary.
  - `test_status_tool_summary_line_canonical_location(self)` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L183) — status tool summary_line should be canonical in agent_summary, may appear top-level.
- uses (calls/refs, reference-scoped): [`ProjectOverviewTool`](../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/codegraph_status_tool.md#CodeGraphStatusTool.execute), [`CodeGraphStatusTool`](../../tree_sitter_analyzer/mcp/tools/codegraph_status_tool.md#CodeGraphStatusTool), [`execute`](../../tree_sitter_analyzer/mcp/tools/project_overview_tool.md#ProjectOverviewTool.execute)  (2 test-only)

## Functions
- `_run(coro)` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L22)
- `_write(tmp_path, rel, content, encoding="utf-8")` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L26)
- `test_overview_review_requires_real_signals()` — [`L325`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L325) — REVIEW comes from observable signals (≥3 files ≥800 lines), never
- `test_overview_risk_unknown_maps_to_info()` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L243)
- `test_status_schema_version_included_when_present(tmp_path, monkeypatch)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L278) — Non-None schema_version IS emitted (only None is omitted).
- `test_status_stale_lag_next_step(tmp_path, monkeypatch)` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L253) — lag > 300s → next_step suggests sync before nav/search.
- `test_status_warn_branch_schema_version_included(tmp_path, monkeypatch)` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_issue_446_envelope_polish.py#L303) — WARN (empty index) branch also emits non-None schema_version.

