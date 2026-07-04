---
title: 'Module: tests/unit/formatters/test_markdown_formatter_new_elements.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_markdown_formatter_new_elements.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_markdown_formatter_new_elements`/TestMarkdownFormatter
symbols:
  TestMarkdownFormatterNewElements.formatter: NewElements#formatter.
  TestMarkdownFormatterCSVTable.formatter: CSVTable#formatter.
  TestMarkdownFormatterNewElements.test_format_table_with_blockquotes: NewElements#test_format_table_with_blockquotes().
  TestMarkdownFormatterNewElements.test_format_table_with_horizontal_rules: NewElements#test_format_table_with_horizontal_rules().
  TestMarkdownFormatterNewElements.test_format_table_with_html_elements: NewElements#test_format_table_with_html_elements().
  TestMarkdownFormatterNewElements.test_format_table_with_text_formatting: NewElements#test_format_table_with_text_formatting().
  TestMarkdownFormatterNewElements.test_format_table_with_footnotes: NewElements#test_format_table_with_footnotes().
  TestMarkdownFormatterNewElements.test_format_table_with_all_new_elements: NewElements#test_format_table_with_all_new_elements().
  TestMarkdownFormatterNewElements.test_format_table_with_no_new_elements: NewElements#test_format_table_with_no_new_elements().
  TestMarkdownFormatterNewElements.test_format_summary_with_new_elements: NewElements#test_format_summary_with_new_elements().
  TestMarkdownFormatterNewElements.test_format_structure_with_new_elements: NewElements#test_format_structure_with_new_elements().
  TestMarkdownFormatterNewElements.test_format_advanced_includes_new_elements_in_count: NewElements#test_format_advanced_includes_new_elements_in_count().
  TestMarkdownFormatterNewElements.test_format_advanced_text_format: NewElements#test_format_advanced_text_format().
  TestMarkdownFormatterNewElements.test_empty_elements_sections_not_shown: NewElements#test_empty_elements_sections_not_shown().
  TestMarkdownFormatterCompactTable.test_compact_basic: CompactTable#test_compact_basic().
  TestMarkdownFormatterCompactTable.test_compact_with_images: CompactTable#test_compact_with_images().
  TestMarkdownFormatterCompactTable.test_compact_headers_truncated_at_20: CompactTable#test_compact_headers_truncated_at_20().
  TestMarkdownFormatterCompactTable.test_compact_no_headers_skips_structure: CompactTable#test_compact_no_headers_skips_structure().
  TestMarkdownFormatterCSVTable.test_csv_header_row: CSVTable#test_csv_header_row().
  TestMarkdownFormatterCSVTable.test_csv_heading_element: CSVTable#test_csv_heading_element().
  TestMarkdownFormatterCSVTable.test_csv_link_element: CSVTable#test_csv_link_element().
  TestMarkdownFormatterCSVTable.test_csv_image_element: CSVTable#test_csv_image_element().
  TestMarkdownFormatterCSVTable.test_csv_code_block_element: CSVTable#test_csv_code_block_element().
  TestMarkdownFormatterCSVTable.test_csv_list_element: CSVTable#test_csv_list_element().
  TestMarkdownFormatterCSVTable.test_csv_table_element: CSVTable#test_csv_table_element().
  TestMarkdownFormatterCSVTable.test_csv_unknown_element: CSVTable#test_csv_unknown_element().
  TestMarkdownFormatterCSVTable.test_csv_autolink_element: CSVTable#test_csv_autolink_element().
  TestMarkdownFormatterCSVTable.test_csv_task_list_element: CSVTable#test_csv_task_list_element().
  TestMarkdownFormatterCompactTable.formatter: CompactTable#formatter.
  TestMarkdownFormatterCompactTable.setup_method: CompactTable#setup_method().
  TestMarkdownFormatterCSVTable.setup_method: CSVTable#setup_method().
  TestMarkdownFormatterNewElements: NewElements#
  TestMarkdownFormatterNewElements.setup_method: NewElements#setup_method().
  TestMarkdownFormatterCompactTable: CompactTable#
  TestMarkdownFormatterCSVTable: CSVTable#
---
# Module: [`tests/unit/formatters/test_markdown_formatter_new_elements.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py)

## Classes
### `TestMarkdownFormatterCSVTable`
- def: [`tests/unit/formatters/test_markdown_formatter_new_elements.py:550`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L550)
- doc: Test CSV table output format.
- signature: `class TestMarkdownFormatterCSVTable:`
- members:
  - `setup_method(self)` — [`L553`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L553)
  - `test_csv_autolink_element(self)` — [`L668`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L668)
  - `test_csv_code_block_element(self)` — [`L609`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L609)
  - `test_csv_header_row(self)` — [`L556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L556)
  - `test_csv_heading_element(self)` — [`L563`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L563)
  - `test_csv_image_element(self)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L594)
  - `test_csv_link_element(self)` — [`L579`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L579)
  - `test_csv_list_element(self)` — [`L624`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L624)
  - `test_csv_table_element(self)` — [`L639`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L639)
  - `test_csv_task_list_element(self)` — [`L683`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L683)
  - `test_csv_unknown_element(self)` — [`L654`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L654)
  - `formatter` — [`L554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L554)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_table)

### `TestMarkdownFormatterCompactTable`
- def: [`tests/unit/formatters/test_markdown_formatter_new_elements.py:461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L461)
- doc: Test compact table output format.
- signature: `class TestMarkdownFormatterCompactTable:`
- members:
  - `setup_method(self)` — [`L464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L464)
  - `test_compact_basic(self)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L467)
  - `test_compact_headers_truncated_at_20(self)` — [`L523`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L523)
  - `test_compact_no_headers_skips_structure(self)` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L539)
  - `test_compact_with_images(self)` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L508)
  - `formatter` — [`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L465)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_table)

### `TestMarkdownFormatterNewElements`
- def: [`tests/unit/formatters/test_markdown_formatter_new_elements.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L20)
- doc: Test Markdown formatter with new element types
- signature: `class TestMarkdownFormatterNewElements:`
- members:
  - `setup_method(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L23) — Setup test fixtures
  - `test_empty_elements_sections_not_shown(self)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L429) — Test that empty sections for new elements are not displayed
  - `test_format_advanced_includes_new_elements_in_count(self)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L377) — Test advanced formatting includes new elements in total count
  - `test_format_advanced_text_format(self)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L404) — Test advanced formatting in text format
  - `test_format_structure_with_new_elements(self)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L337) — Test structure formatting includes traditional elements (new elements not in structure)
  - `test_format_summary_with_new_elements(self)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L309) — Test summary formatting includes traditional elements (new elements not in summary)
  - `test_format_table_with_all_new_elements(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L226) — Test table formatting with all new element types combined
  - `test_format_table_with_blockquotes(self)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L27) — Test table formatting with blockquotes
  - `test_format_table_with_footnotes(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L177) — Test table formatting with footnotes
  - `test_format_table_with_horizontal_rules(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L62) — Test table formatting with horizontal rules
  - `test_format_table_with_html_elements(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L89) — Test table formatting with HTML elements
  - `test_format_table_with_no_new_elements(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L274) — Test table formatting when no new elements are present
  - `test_format_table_with_text_formatting(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L130) — Test table formatting with text formatting elements
  - `formatter` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_new_elements.py#L25)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_table), [`format_advanced`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_advanced), [`format_summary`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_summary), [`format_structure`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_structure)

