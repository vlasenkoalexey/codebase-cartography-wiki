---
title: 'Module: tree_sitter_analyzer/cli/commands/advanced_command_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/commands/advanced_command_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.commands.advanced_command_helpers`/
symbols:
  _count_line: _count_line().
  calculate_content_metrics: calculate_content_metrics().
  _adjust_blank_lines: _adjust_blank_lines().
  calculate_file_metrics: calculate_file_metrics().
  LineMetricCounts.comment_lines: LineMetricCounts#comment_lines.
  _count_lines: _count_lines().
  LineMetricCounts.blank_lines: LineMetricCounts#blank_lines.
  LineMetricCounts: LineMetricCounts#
  LineMetricCounts.code_lines: LineMetricCounts#code_lines.
  LineMetricCounts.in_multiline_comment: LineMetricCounts#in_multiline_comment.
  _starts_c_style_multiline_comment: _starts_c_style_multiline_comment().
  _is_single_line_comment: _is_single_line_comment().
  _zero_metrics: _zero_metrics().
---
# Module: [`tree_sitter_analyzer/cli/commands/advanced_command_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py)

## Classes
### `LineMetricCounts`
- def: [`tree_sitter_analyzer/cli/commands/advanced_command_helpers.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L11)
- doc: Mutable line-counting state.
- signature: `class LineMetricCounts:`
- members:
  - `blank_lines` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L16)
  - `code_lines` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L14)
  - `comment_lines` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L15)
  - `in_multiline_comment` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L17)
- used by: [`_count_line`](advanced_command_helpers.md#_count_line), [`calculate_content_metrics`](advanced_command_helpers.md#calculate_content_metrics), [`_adjust_blank_lines`](advanced_command_helpers.md#_adjust_blank_lines), [`_count_lines`](advanced_command_helpers.md#_count_lines)

## Functions
- `_adjust_blank_lines(counts: LineMetricCounts, total_lines: int)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L100) — Adjust blank lines so counted categories sum to total lines.
- `_count_line(stripped: str, language: str, counts: LineMetricCounts)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L55) — Count one stripped line into code, comment, or blank categories.
- `_count_lines(lines: list[str], language: str)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L47) — Count line categories while preserving multiline comment state.
- `_is_single_line_comment(stripped: str, language: str)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L90) — Return whether a line is a single-line comment.
- `_starts_c_style_multiline_comment(stripped: str)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L85) — Return whether a line starts a C-style multiline comment.
- `_zero_metrics()` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L108) — Return zero-valued file metrics.
- `calculate_content_metrics(content: str, language: str)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L29) — Calculate code, comment, and blank line counts from file content.
- `calculate_file_metrics(file_path: str, language: str)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/commands/advanced_command_helpers.py#L20) — Calculate accurate file metrics including line counts.

