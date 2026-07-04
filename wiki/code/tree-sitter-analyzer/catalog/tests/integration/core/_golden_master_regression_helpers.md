---
title: 'Module: tests/integration/core/_golden_master_regression_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/core/_golden_master_regression_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.core._golden_master_regression_helpers`/
symbols:
  normalize_analyzer_output: normalize_analyzer_output().
  _should_skip_sql_misdetection: _should_skip_sql_misdetection().
  build_golden_master_diff: build_golden_master_diff().
  normalize_toon_output: normalize_toon_output().
  _normalize_markdown_unstable_locations: _normalize_markdown_unstable_locations().
  _looks_like_sql_trigger_misdetection: _looks_like_sql_trigger_misdetection().
  _append_first_differences: _append_first_differences().
  SQL_TYPE_KEYWORDS: SQL_TYPE_KEYWORDS.
  _stable_lines: _stable_lines().
  _join_normalized_lines: _join_normalized_lines().
  SQL_COLUMN_NAMES: SQL_COLUMN_NAMES.
  MARKDOWN_UNSTABLE_MARKERS: MARKDOWN_UNSTABLE_MARKERS.
  _normalize_markdown_counts: _normalize_markdown_counts().
  _normalize_python_type_variance: _normalize_python_type_variance().
  _looks_like_sql_function_misdetection: _looks_like_sql_function_misdetection().
  _extract_name_field: _extract_name_field().
  _count_different_lines: _count_different_lines().
  _render_line_difference: _render_line_difference().
---
# Module: [`tests/integration/core/_golden_master_regression_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py)

## Functions
- `_append_first_differences(diff_lines: list[str], golden_lines: list[str], current_lines: list[str], max_lines: int, *, limit: int)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L207)
- `_count_different_lines(golden_lines: list[str], current_lines: list[str], max_lines: int)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L195)
- `_extract_name_field(line: str)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L188)
- `_join_normalized_lines(lines: list[str])` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L121)
- `_looks_like_sql_function_misdetection(line: str, keyword: str)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L177)
- `_looks_like_sql_trigger_misdetection(line: str, keyword: str)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L181)
- `_normalize_markdown_counts(line: str)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L125)
- `_normalize_markdown_unstable_locations(line: str)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L143)
- `_normalize_python_type_variance(line: str)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L150)
- `_render_line_difference(golden_lines: list[str], current_lines: list[str], line_index: int)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L228)
- `_should_skip_sql_misdetection(line: str)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L156)
- `_stable_lines(content: str)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L115)
- `build_golden_master_diff(golden_normalized: str, current_normalized: str, *, prefix: str = "Output")` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L88) — Build the compact diff message used by golden master assertions.
- `normalize_analyzer_output(content: str)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L44) — Normalize analyzer output by removing known environment variance.
- `normalize_toon_output(content: str)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L70) — Normalize TOON output by removing timing variance.

## Module values
- `MARKDOWN_UNSTABLE_MARKERS` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L36)
- `SQL_COLUMN_NAMES` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L22)
- `SQL_TYPE_KEYWORDS` — [`L7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/core/_golden_master_regression_helpers.py#L7)

