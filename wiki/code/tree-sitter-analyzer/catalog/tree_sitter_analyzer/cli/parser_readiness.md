---
title: 'Module: tree_sitter_analyzer/cli/parser_readiness.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/parser_readiness.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.parser_readiness`/
symbols:
  build_parser_readiness_advice: build_parser_readiness_advice().
  _build_result: _build_result().
  _metadata_summary: _metadata_summary().
  _build_agent_summary: _build_agent_summary().
  _build_toon_content: _build_toon_content().
  _LANG_NAME_RE: _LANG_NAME_RE.
  _ensure_no_gap_consistency: _ensure_no_gap_consistency().
  _build_report_records: _build_report_records().
  _base_result: _base_result().
  _build_recommendations: _build_recommendations().
  _toon_readiness_lines: _toon_readiness_lines().
  _toon_readiness_line: _toon_readiness_line().
  _readiness_url: _readiness_url().
  _build_summary_line: _build_summary_line().
  _status_distribution: _status_distribution().
  _high_priority_languages: _high_priority_languages().
  _candidate_count: _candidate_count().
  _recommendation: _recommendation().
  _summary_next_step: _summary_next_step().
  _summary_verification_command: _summary_verification_command().
  _first_project_url: _first_project_url().
  _toon_recommendation_lines: _toon_recommendation_lines().
---
# Module: [`tree_sitter_analyzer/cli/parser_readiness.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py)

## Functions
- `_base_result(root: Path, requested_language: str | None)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L164) — Return result fields that do not depend on parser inventory size.
- `_build_agent_summary(records: list[dict[str, Any]], recommendations: list[dict[str, Any]], requested_language: str | None)` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L261) — Build the agent_summary block for parser-readiness output.
- `_build_recommendations(records: list[dict[str, Any]])` — [`L245`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L245)
- `_build_report_records(root: Path, inputs: dict[str, Any], *, requested_language: str | None, include_supported: bool)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L81) — Build readiness records without hiding hardening gaps.
- `_build_result(root: Path, inputs: dict[str, Any], requested_language: str | None, records: list[dict[str, Any]], recommendations: list[dict[str, Any]], agent_summary: dict[str, Any])` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L107) — Assemble the final parser-readiness response.
- `_build_summary_line(result: dict[str, Any], recommendations: list[dict[str, Any]])` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L146) — Build the canonical one-line headline for parser-readiness output.
- `_build_toon_content(result: dict[str, Any])` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L315)
- `_candidate_count(records: list[dict[str, Any]])` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L241)
- `_ensure_no_gap_consistency(result: dict[str, Any])` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L209) — When no gaps are reported, populate empty fields with explicit
- `_first_project_url(project_urls: dict[str, str])` — [`L361`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L361)
- `_high_priority_languages(recommendations: list[dict[str, Any]])` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L236) — Expose top language names by score for quick CLI triage.
- `_metadata_summary(inputs: dict[str, Any], records: list[dict[str, Any]])` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L176) — Return compact inventory counts and package display fields.
- `_readiness_url(signals: dict[str, Any])` — [`L367`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L367)
- `_recommendation(record: dict[str, Any])` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L251)
- `_status_distribution(records: list[dict[str, Any]])` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L200) — Return a compact status histogram for workflow-aware prioritization.
- `_summary_next_step(first: dict[str, Any] | None)` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L303)
- `_summary_verification_command(first: dict[str, Any] | None)` — [`L309`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L309)
- `_toon_readiness_line(record: dict[str, Any])` — [`L342`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L342)
- `_toon_readiness_lines(records: list[dict[str, Any]])` — [`L338`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L338)
- `_toon_recommendation_lines(recommendations: list[dict[str, Any]])` — [`L376`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L376)
- `build_parser_readiness_advice(project_root: str, *, language: str | None = None, include_supported: bool = False)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L24) — Build a local parser-readiness report for language plugin planning.

## Module values
- `_LANG_NAME_RE` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/parser_readiness.py#L21)

