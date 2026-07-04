---
title: 'Module: tests/unit/formatters/test_markdown_formatter_coverage_boost.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_markdown_formatter_coverage_boost.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_markdown_formatter_coverage_boost`/Test
symbols:
  TestFormatCSV.formatter: FormatCSV#formatter.
  TestFormatCompact.formatter: FormatCompact#formatter.
  TestCollectImagesException.test_collect_images_exception_in_element: CollectImagesException#test_collect_images_exception_in_element().
  TestFormatTableCompactAndCSV.test_format_table_csv: FormatTableCompactAndCSV#test_format_table_csv().
  TestFormatCompact.test_format_compact_empty: FormatCompact#test_format_compact_empty().
  TestFormatCompact.test_format_compact_with_headers: FormatCompact#test_format_compact_with_headers().
  TestFormatCompact.test_format_compact_with_links: FormatCompact#test_format_compact_with_links().
  TestFormatCompact.test_format_compact_with_images: FormatCompact#test_format_compact_with_images().
  TestFormatCompact.test_format_compact_with_code_blocks: FormatCompact#test_format_compact_with_code_blocks().
  TestFormatCompact.test_format_compact_with_lists: FormatCompact#test_format_compact_with_lists().
  TestFormatCompact.test_format_compact_with_tables: FormatCompact#test_format_compact_with_tables().
  TestFormatCompact.test_format_compact_filename_without_extension: FormatCompact#test_format_compact_filename_without_extension().
  TestFormatCompact.test_format_compact_filename_markdown_extension: FormatCompact#test_format_compact_filename_markdown_extension().
  TestFormatCompact.test_format_compact_windows_path: FormatCompact#test_format_compact_windows_path().
  TestFormatCompact.test_format_compact_many_headers: FormatCompact#test_format_compact_many_headers().
  TestFormatCompact.test_format_compact_no_headers: FormatCompact#test_format_compact_no_headers().
  TestFormatCSV.test_format_csv_empty: FormatCSV#test_format_csv_empty().
  TestFormatCSV.test_format_csv_heading: FormatCSV#test_format_csv_heading().
  TestFormatCSV.test_format_csv_link: FormatCSV#test_format_csv_link().
  TestFormatCSV.test_format_csv_autolink: FormatCSV#test_format_csv_autolink().
  TestFormatCSV.test_format_csv_image: FormatCSV#test_format_csv_image().
  TestFormatCSV.test_format_csv_code_block: FormatCSV#test_format_csv_code_block().
  TestFormatCSV.test_format_csv_list: FormatCSV#test_format_csv_list().
  TestFormatCSV.test_format_csv_task_list: FormatCSV#test_format_csv_task_list().
  TestFormatCSV.test_format_csv_table: FormatCSV#test_format_csv_table().
  TestFormatCSV.test_format_csv_unknown_type: FormatCSV#test_format_csv_unknown_type().
  TestFormatCSV.test_format_csv_all_element_types: FormatCSV#test_format_csv_all_element_types().
  TestFormatCSV.test_format_csv_truncates_long_text: FormatCSV#test_format_csv_truncates_long_text().
  TestFormatCSV.test_format_csv_truncates_link_text: FormatCSV#test_format_csv_truncates_link_text().
  TestCollectImagesException.test_collect_images_with_malformed_element: CollectImagesException#test_collect_images_with_malformed_element().
  TestCollectImagesException.test_collect_images_empty_list: CollectImagesException#test_collect_images_empty_list().
  TestCollectImagesException.formatter: CollectImagesException#formatter.
  TestFormatTableCompactAndCSV.setup_method: FormatTableCompactAndCSV#setup_method().
  TestFormatCompact.setup_method: FormatCompact#setup_method().
  TestFormatCSV.setup_method: FormatCSV#setup_method().
  TestCollectImagesException.setup_method: CollectImagesException#setup_method().
  TestFormatTableCompactAndCSV.formatter: FormatTableCompactAndCSV#formatter.
  TestCollectImagesException.test_collect_images_exception_in_element.BadElement: CollectImagesException#test_collect_images_exception_in_element().BadElement#
  TestFormatTableCompactAndCSV: FormatTableCompactAndCSV#
  TestFormatCompact: FormatCompact#
  TestFormatCSV: FormatCSV#
  TestCollectImagesException: CollectImagesException#
  TestCollectImagesException.test_collect_images_exception_in_element.BadElement.get: CollectImagesException#test_collect_images_exception_in_element().BadElement#get().
---
# Module: [`tests/unit/formatters/test_markdown_formatter_coverage_boost.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py)

## Classes
### `BadElement`  ·  implements/extends dict
- def: [`tests/unit/formatters/test_markdown_formatter_coverage_boost.py:577`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L577)
- signature: `class BadElement(dict):`
- members:
  - `get(self, key, default=None)` — [`L578`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L578)
- used by: (1 test-only callers)

### `TestCollectImagesException`
- def: [`tests/unit/formatters/test_markdown_formatter_coverage_boost.py:557`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L557)
- doc: Tests for _collect_images exception handling.
- signature: `class TestCollectImagesException:`
- members:
  - `setup_method(self)` — [`L560`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L560)
  - `test_collect_images_empty_list(self)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L594) — Test _collect_images with empty list.
  - `test_collect_images_exception_in_element(self)` — [`L574`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L574) — Test _collect_images catches exception in fallback loop (lines 589-591).
  - `test_collect_images_with_malformed_element(self)` — [`L563`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L563) — Test _collect_images handles malformed elements gracefully.
  - `formatter` — [`L561`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L561)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`_collect_images`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter._collect_images)  (1 test-only)

### `TestFormatCSV`
- def: [`tests/unit/formatters/test_markdown_formatter_coverage_boost.py:283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L283)
- doc: Tests for _format_csv method.
- signature: `class TestFormatCSV:`
- members:
  - `setup_method(self)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L286)
  - `test_format_csv_all_element_types(self)` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L453) — Test _format_csv with all supported element types.
  - `test_format_csv_autolink(self)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L334) — Test _format_csv with autolink element.
  - `test_format_csv_code_block(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L369) — Test _format_csv with code block element.
  - `test_format_csv_empty(self)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L289) — Test _format_csv with empty elements.
  - `test_format_csv_heading(self)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L299) — Test _format_csv with heading element.
  - `test_format_csv_image(self)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L351) — Test _format_csv with image element.
  - `test_format_csv_link(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L316) — Test _format_csv with link element.
  - `test_format_csv_list(self)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L386) — Test _format_csv with list element.
  - `test_format_csv_table(self)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L420) — Test _format_csv with table element.
  - `test_format_csv_task_list(self)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L403) — Test _format_csv with task list element.
  - `test_format_csv_truncates_link_text(self)` — [`L536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L536) — Test _format_csv truncates link text to 30 chars.
  - `test_format_csv_truncates_long_text(self)` — [`L515`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L515) — Test _format_csv truncates long heading text to 50 chars.
  - `test_format_csv_unknown_type(self)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L437) — Test _format_csv with unknown element type (else branch).
  - `formatter` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L287)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`_format_csv`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter._format_csv)

### `TestFormatCompact`
- def: [`tests/unit/formatters/test_markdown_formatter_coverage_boost.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L47)
- doc: Tests for _format_compact method.
- signature: `class TestFormatCompact:`
- members:
  - `setup_method(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L50)
  - `test_format_compact_empty(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L53) — Test _format_compact with empty elements.
  - `test_format_compact_filename_markdown_extension(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L220) — Test _format_compact strips .markdown extension.
  - `test_format_compact_filename_without_extension(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L202) — Test _format_compact with filename that has no extension.
  - `test_format_compact_many_headers(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L242) — Test _format_compact with more than 20 headers (truncation).
  - `test_format_compact_no_headers(self)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L264) — Test _format_compact without heading elements (no structure section).
  - `test_format_compact_windows_path(self)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L231) — Test _format_compact with Windows-style path.
  - `test_format_compact_with_code_blocks(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L139) — Test _format_compact with code block elements.
  - `test_format_compact_with_headers(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L66) — Test _format_compact with heading elements.
  - `test_format_compact_with_images(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L120) — Test _format_compact with image elements.
  - `test_format_compact_with_links(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L95) — Test _format_compact with link elements.
  - `test_format_compact_with_lists(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L158) — Test _format_compact with list elements.
  - `test_format_compact_with_tables(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L183) — Test _format_compact with table elements.
  - `formatter` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L51)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`_format_compact`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter._format_compact)

### `TestFormatTableCompactAndCSV`
- def: [`tests/unit/formatters/test_markdown_formatter_coverage_boost.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L14)
- doc: Tests for format_table with compact and csv table_type.
- signature: `class TestFormatTableCompactAndCSV:`
- members:
  - `setup_method(self)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L17)
  - `test_format_table_csv(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L20) — Test format_table with table_type='csv'.
  - `formatter` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_coverage_boost.py#L18)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_table)

