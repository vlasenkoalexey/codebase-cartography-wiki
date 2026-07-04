---
title: 'Module: tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._markdown_formatter_rendering`/
symbols:
  markdown_csv_row: markdown_csv_row().
  format_advanced_text: format_advanced_text().
  format_compact_output: format_compact_output().
  format_csv_output: format_csv_output().
  calculate_document_complexity: calculate_document_complexity().
  compact_summary_lines: compact_summary_lines().
  append_compact_headers: append_compact_headers().
  compact_header_rows: compact_header_rows().
  format_json_output: format_json_output().
  format_advanced_basic_lines: format_advanced_basic_lines().
  format_advanced_metric_lines: format_advanced_metric_lines().
  format_advanced_content_lines: format_advanced_content_lines().
  document_complexity_score: document_complexity_score().
  markdown_display_filename: markdown_display_filename().
  compact_header_row: compact_header_row().
  link_csv_row: link_csv_row().
  image_csv_row: image_csv_row().
  code_block_csv_row: code_block_csv_row().
  list_csv_row: list_csv_row().
  table_csv_row: table_csv_row().
---
# Module: [`tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py)

## Functions
- `append_compact_headers(output: list[str], headers: list[dict[str, Any]])` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L150) — Append compact document structure rows.
- `calculate_document_complexity(headers: list[dict[str, Any]], links: list[dict[str, Any]], code_blocks: list[dict[str, Any]], tables: list[dict[str, Any]])` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L63) — Calculate document complexity based on structure and content.
- `code_block_csv_row(element: dict[str, Any], elem_type: str, start_line: int, end_line: int)` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L238) — Build a CSV row for a Markdown code block.
- `compact_header_row(header: dict[str, Any])` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L170) — Build one compact header row.
- `compact_header_rows(headers: list[dict[str, Any]])` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L162) — Build compact header rows.
- `compact_summary_lines(file_path: str, groups: dict[str, list[Any]], images: list[dict[str, Any]], total_elements: int)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L119) — Build compact summary table lines.
- `document_complexity_score(headers: list[dict[str, Any]], links: list[dict[str, Any]], code_blocks: list[dict[str, Any]], tables: list[dict[str, Any]])` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L80) — Return the numeric complexity score before label classification.
- `format_advanced_basic_lines(data: dict[str, Any])` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L27) — Build basic advanced-analysis text lines.
- `format_advanced_content_lines(content: dict[str, Any])` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L52) — Build content-analysis text lines.
- `format_advanced_metric_lines(metrics: dict[str, Any])` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L37) — Build document metric text lines.
- `format_advanced_text(data: dict[str, Any])` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L18) — Format advanced analysis in text format.
- `format_compact_output(analysis_result: dict[str, Any], images: list[dict[str, Any]])` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L106) — Format compact table output for Markdown files.
- `format_csv_output(analysis_result: dict[str, Any])` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L178) — Format CSV output for Markdown files.
- `format_json_output(title: str, data: dict[str, Any])` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L99) — Format JSON output with title.
- `image_csv_row(element: dict[str, Any], elem_type: str, start_line: int, end_line: int)` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L230) — Build a CSV row for a Markdown image.
- `link_csv_row(element: dict[str, Any], elem_type: str, start_line: int, end_line: int)` — [`L222`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L222) — Build a CSV row for a Markdown link.
- `list_csv_row(element: dict[str, Any], elem_type: str, start_line: int, end_line: int)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L251) — Build a CSV row for a Markdown list.
- `markdown_csv_row(element: dict[str, Any])` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L195) — Return one Markdown element as a CSV row.
- `markdown_display_filename(file_path: str)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L142) — Return display filename for compact output.
- `table_csv_row(element: dict[str, Any], elem_type: str, start_line: int, end_line: int)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_markdown_formatter_rendering.py#L264) — Build a CSV row for a Markdown table.

