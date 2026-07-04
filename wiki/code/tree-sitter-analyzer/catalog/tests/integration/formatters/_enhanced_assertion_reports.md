---
title: 'Module: tests/integration/formatters/_enhanced_assertion_reports.py'
type: catalog
provenance: extracted
module: tests/integration/formatters/_enhanced_assertion_reports.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.formatters._enhanced_assertion_reports`/
symbols:
  build_assertion_report: build_assertion_report().
  _compare_one_format_count: _compare_one_format_count().
  _group_by_severity: _group_by_severity().
  _group_by_message_type: _group_by_message_type().
  compare_format_counts: compare_format_counts().
  count_format_elements: count_format_elements().
---
# Module: [`tests/integration/formatters/_enhanced_assertion_reports.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_reports.py)

## Functions
- `_compare_one_format_count(base_format: str, base_counts: dict[str, int], other_format: str, other_counts: dict[str, int])` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_reports.py#L95)
- `_group_by_message_type(results: list[AssertionResult])` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_reports.py#L135)
- `_group_by_severity(results: list[AssertionResult])` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_reports.py#L123)
- `build_assertion_report(results: list[AssertionResult])` — [`L8`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_reports.py#L8) — Build a grouped assertion report with summary and detail sections.
- `compare_format_counts(format_counts: dict[str, dict[str, int]])` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_reports.py#L73) — Compare element counts across format outputs.
- `count_format_elements(output: str)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/formatters/_enhanced_assertion_reports.py#L51) — Count table rows and section headings in format output.

