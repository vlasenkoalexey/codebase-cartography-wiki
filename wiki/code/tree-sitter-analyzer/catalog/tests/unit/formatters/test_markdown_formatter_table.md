---
title: 'Module: tests/unit/formatters/test_markdown_formatter_table.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_markdown_formatter_table.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_markdown_formatter_table`/TestFormat
symbols:
  TestFormatTable.test_format_table_basic: Table#test_format_table_basic().
  TestFormatTable.test_format_table_headers_section: Table#test_format_table_headers_section().
  TestFormatTable.test_format_table_links_section: Table#test_format_table_links_section().
  TestFormatTable.test_format_table_images_section: Table#test_format_table_images_section().
  TestFormatTable.test_format_table_code_blocks_section: Table#test_format_table_code_blocks_section().
  TestFormatTable.test_format_table_lists_section: Table#test_format_table_lists_section().
  TestFormatTable.test_format_table_tables_section: Table#test_format_table_tables_section().
  TestFormatTable.test_format_table_blockquotes_section: Table#test_format_table_blockquotes_section().
  TestFormatTable.test_format_table_horizontal_rules_section: Table#test_format_table_horizontal_rules_section().
  TestFormatTable.test_format_table_html_elements_section: Table#test_format_table_html_elements_section().
  TestFormatTable.test_format_table_text_formatting_section: Table#test_format_table_text_formatting_section().
  TestFormatTable.test_format_table_footnotes_section: Table#test_format_table_footnotes_section().
  TestFormatTable.test_format_table_reference_definitions_section: Table#test_format_table_reference_definitions_section().
  TestFormatTable.test_format_table_no_headers_uses_filename: Table#test_format_table_no_headers_uses_filename().
  TestFormatTable.test_format_table_long_content_truncation: Table#test_format_table_long_content_truncation().
  TestFormatAnalysisResult.test_format_analysis_result: AnalysisResult#test_format_analysis_result().
  TestFormatAnalysisResult.test_convert_analysis_result_to_format: AnalysisResult#test_convert_analysis_result_to_format().
  TestFormatTable: Table#
  TestFormatAnalysisResult: AnalysisResult#
---
# Module: [`tests/unit/formatters/test_markdown_formatter_table.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py)

## Classes
### `TestFormatAnalysisResult`
- def: [`tests/unit/formatters/test_markdown_formatter_table.py:444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L444)
- doc: Test format_analysis_result method
- signature: `class TestFormatAnalysisResult:`
- members:
  - `test_convert_analysis_result_to_format(self)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L483) — Test _convert_analysis_result_to_format helper
  - `test_format_analysis_result(self)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L447) — Test formatting AnalysisResult object
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_analysis_result`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_analysis_result), [`_convert_analysis_result_to_format`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter._convert_analysis_result_to_format)

### `TestFormatTable`
- def: [`tests/unit/formatters/test_markdown_formatter_table.py:10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L10)
- doc: Test format_table method
- signature: `class TestFormatTable:`
- members:
  - `test_format_table_basic(self)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L13) — Test basic table formatting
  - `test_format_table_blockquotes_section(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L216) — Test blockquotes section in table
  - `test_format_table_code_blocks_section(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L131) — Test code blocks section in table
  - `test_format_table_footnotes_section(self)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L343) — Test footnotes section in table
  - `test_format_table_headers_section(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L39) — Test headers section in table
  - `test_format_table_horizontal_rules_section(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L242) — Test horizontal rules section in table
  - `test_format_table_html_elements_section(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L267) — Test HTML elements section in table
  - `test_format_table_images_section(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L103) — Test images section in table
  - `test_format_table_links_section(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L67) — Test links section in table
  - `test_format_table_lists_section(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L160) — Test lists section in table
  - `test_format_table_long_content_truncation(self)` — [`L415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L415) — Test that long content is truncated properly
  - `test_format_table_no_headers_uses_filename(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L401) — Test table uses filename as title when no headers
  - `test_format_table_reference_definitions_section(self)` — [`L375`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L375) — Test reference definitions section in table
  - `test_format_table_tables_section(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L188) — Test tables section in table
  - `test_format_table_text_formatting_section(self)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_table.py#L299) — Test text formatting section in table
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_table)

