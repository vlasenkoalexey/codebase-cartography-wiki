---
title: 'Module: tree_sitter_analyzer/formatters/markdown_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/markdown_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.markdown_formatter`/MarkdownFormatter#
symbols:
  MarkdownFormatter: ''
  MarkdownFormatter.format_table: format_table().
  MarkdownFormatter.format_advanced: format_advanced().
  MarkdownFormatter.format_summary: format_summary().
  MarkdownFormatter._format_compact: _format_compact().
  MarkdownFormatter._collect_images: _collect_images().
  MarkdownFormatter._format_csv: _format_csv().
  MarkdownFormatter.format_structure: format_structure().
  MarkdownFormatter._compute_robust_counts_from_file: _compute_robust_counts_from_file().
  MarkdownFormatter._format_json_output: _format_json_output().
  MarkdownFormatter._calculate_document_complexity: _calculate_document_complexity().
  MarkdownFormatter.format_analysis_result: format_analysis_result().
  MarkdownFormatter._format_full: _format_full().
  MarkdownFormatter._format_advanced_text: _format_advanced_text().
  MarkdownFormatter._convert_analysis_result_to_format: _convert_analysis_result_to_format().
  MarkdownFormatter.language: language.
  MarkdownFormatter.__init__: __init__().
---
# Module: [`tree_sitter_analyzer/formatters/markdown_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py)

## Classes
### `MarkdownFormatter`  ·  implements/extends BaseFormatter
- def: [`tree_sitter_analyzer/formatters/markdown_formatter.py:27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L27)
- doc: Formatter specialized for Markdown documents
- signature: `class MarkdownFormatter(BaseFormatter):`
- members:
  - `_calculate_document_complexity(self, headers: list[dict], links: list[dict], code_blocks: list[dict], tables: list[dict])` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L138) — Calculate document complexity based on structure and content
  - `_collect_images(self, elements: list[dict[str, Any]])` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L130) — Collect images including reference definitions that point to images.
  - `_compute_robust_counts_from_file(self, file_path: str)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L152) — Compute robust counts for links and images directly from file content.
  - `_convert_analysis_result_to_format(self, analysis_result: Any)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L79) — Convert AnalysisResult to format expected by format_table
  - `_format_advanced_text(self, data: dict[str, Any])` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L134) — Format advanced analysis in text format
  - `_format_compact(self, analysis_result: dict[str, Any])` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L156) — Format compact table output for Markdown files
  - `_format_csv(self, analysis_result: dict[str, Any])` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L162) — Format CSV output for Markdown files
  - `_format_full(self, analysis_result: dict[str, Any])` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L126) — Format full table output for Markdown files
  - `_format_json_output(self, title: str, data: dict[str, Any])` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L148) — Format JSON output with title
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L56) — Format advanced analysis for Markdown files
  - `format_analysis_result(self, analysis_result: Any, table_type: str = "full")` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L72) — Format AnalysisResult directly for Markdown files
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L45) — Format structure analysis for Markdown files
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L33) — Format summary for Markdown files
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L116) — Format table output for Markdown files
  - `language` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L31)
- protocol/private: `__init__`[`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/markdown_formatter.py#L30)
- uses (calls/refs, reference-scoped): [`BaseFormatter`](base_formatter.md#BaseFormatter), [`format_full`](markdown_full_formatter.md#format_full), [`build_structure_result`](_markdown_formatter_payloads.md#build_structure_result), [`build_summary_result`](_markdown_formatter_payloads.md#build_summary_result), [`build_advanced_result`](_markdown_formatter_payloads.md#build_advanced_result), [`collect_images`](_markdown_formatter_elements.md#collect_images), [`compute_robust_counts_from_file`](_markdown_formatter_counts.md#compute_robust_counts_from_file), [`format_advanced_text`](_markdown_formatter_rendering.md#format_advanced_text), [`format_compact_output`](_markdown_formatter_rendering.md#format_compact_output), [`format_csv_output`](_markdown_formatter_rendering.md#format_csv_output), [`calculate_document_complexity`](_markdown_formatter_rendering.md#calculate_document_complexity), [`format_json_output`](_markdown_formatter_rendering.md#format_json_output)
- used by: [`BaseFormatter`](base_formatter.md#BaseFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`format_structure`](base_formatter.md#BaseFormatter.format_structure), [`format_advanced`](base_formatter.md#BaseFormatter.format_advanced), [`format_summary`](base_formatter.md#BaseFormatter.format_summary), [`format_table`](base_formatter.md#BaseFormatter.format_table)  (137 test-only)

