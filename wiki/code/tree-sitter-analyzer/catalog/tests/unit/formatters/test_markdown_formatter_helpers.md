---
title: 'Module: tests/unit/formatters/test_markdown_formatter_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_markdown_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_markdown_formatter_helpers`/Test
symbols:
  TestFormatTable.test_format_table_basic: FormatTable#test_format_table_basic().
  TestFormatTable.test_format_table_headers_section: FormatTable#test_format_table_headers_section().
  TestFormatTable.test_format_table_links_section: FormatTable#test_format_table_links_section().
  TestFormatTable.test_format_table_images_section: FormatTable#test_format_table_images_section().
  TestFormatTable.test_format_table_code_blocks_section: FormatTable#test_format_table_code_blocks_section().
  TestFormatTable.test_format_table_lists_section: FormatTable#test_format_table_lists_section().
  TestFormatTable.test_format_table_tables_section: FormatTable#test_format_table_tables_section().
  TestFormatTable.test_format_table_blockquotes_section: FormatTable#test_format_table_blockquotes_section().
  TestFormatTable.test_format_table_horizontal_rules_section: FormatTable#test_format_table_horizontal_rules_section().
  TestFormatTable.test_format_table_html_elements_section: FormatTable#test_format_table_html_elements_section().
  TestFormatTable.test_format_table_text_formatting_section: FormatTable#test_format_table_text_formatting_section().
  TestFormatTable.test_format_table_footnotes_section: FormatTable#test_format_table_footnotes_section().
  TestFormatTable.test_format_table_reference_definitions_section: FormatTable#test_format_table_reference_definitions_section().
  TestFormatTable.test_format_table_no_headers_uses_filename: FormatTable#test_format_table_no_headers_uses_filename().
  TestFormatTable.test_format_table_long_content_truncation: FormatTable#test_format_table_long_content_truncation().
  TestFormatAnalysisResult.test_format_analysis_result: FormatAnalysisResult#test_format_analysis_result().
  TestFormatAnalysisResult.test_convert_analysis_result_to_format: FormatAnalysisResult#test_convert_analysis_result_to_format().
  TestCollectImages.test_collect_images_basic: CollectImages#test_collect_images_basic().
  TestCollectImages.test_collect_images_with_ref_defs: CollectImages#test_collect_images_with_ref_defs().
  TestCollectImages.test_collect_images_fallback_to_ref_defs: CollectImages#test_collect_images_fallback_to_ref_defs().
  TestCollectImages.test_collect_images_parse_from_name_field: CollectImages#test_collect_images_parse_from_name_field().
  TestCollectImages.test_collect_images_various_extensions: CollectImages#test_collect_images_various_extensions().
  TestCollectImages.test_collect_images_exception_handling: CollectImages#test_collect_images_exception_handling().
  TestCalculateDocumentComplexity.test_complexity_simple: CalculateDocumentComplexity#test_complexity_simple().
  TestCalculateDocumentComplexity.test_complexity_moderate: CalculateDocumentComplexity#test_complexity_moderate().
  TestCalculateDocumentComplexity.test_complexity_complex: CalculateDocumentComplexity#test_complexity_complex().
  TestCalculateDocumentComplexity.test_complexity_very_complex: CalculateDocumentComplexity#test_complexity_very_complex().
  TestCalculateDocumentComplexity.test_complexity_no_headers: CalculateDocumentComplexity#test_complexity_no_headers().
  TestComputeRobustCounts.test_compute_robust_counts_basic: ComputeRobustCounts#test_compute_robust_counts_basic().
  TestComputeRobustCounts.test_compute_robust_counts_autolinks: ComputeRobustCounts#test_compute_robust_counts_autolinks().
  TestComputeRobustCounts.test_compute_robust_counts_reference_links: ComputeRobustCounts#test_compute_robust_counts_reference_links().
  TestComputeRobustCounts.test_compute_robust_counts_image_references: ComputeRobustCounts#test_compute_robust_counts_image_references().
  TestComputeRobustCounts.test_compute_robust_counts_mixed_content: ComputeRobustCounts#test_compute_robust_counts_mixed_content().
  TestComputeRobustCounts.test_compute_robust_counts_file_read_error: ComputeRobustCounts#test_compute_robust_counts_file_read_error().
  TestComputeRobustCounts.test_compute_robust_counts_empty_path: ComputeRobustCounts#test_compute_robust_counts_empty_path().
  TestComputeRobustCounts.test_compute_robust_counts_image_extensions: ComputeRobustCounts#test_compute_robust_counts_image_extensions().
  TestFormatJsonOutput.test_format_json_output_basic: FormatJsonOutput#test_format_json_output_basic().
  TestFormatJsonOutput.test_format_json_output_nested: FormatJsonOutput#test_format_json_output_nested().
  TestFormatJsonOutput.test_format_json_output_unicode: FormatJsonOutput#test_format_json_output_unicode().
  TestFormatTable: FormatTable#
  TestFormatAnalysisResult: FormatAnalysisResult#
  TestCollectImages: CollectImages#
  TestCalculateDocumentComplexity: CalculateDocumentComplexity#
  TestComputeRobustCounts: ComputeRobustCounts#
  TestFormatJsonOutput: FormatJsonOutput#
---
# Module: [`tests/unit/formatters/test_markdown_formatter_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py)

## Classes
### `TestCalculateDocumentComplexity`
- def: [`tests/unit/formatters/test_markdown_formatter_helpers.py:590`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L590)
- signature: `class TestCalculateDocumentComplexity:`
- members:
  - `test_complexity_complex(self)` — [`L617`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L617)
  - `test_complexity_moderate(self)` — [`L604`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L604)
  - `test_complexity_no_headers(self)` — [`L643`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L643)
  - `test_complexity_simple(self)` — [`L591`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L591)
  - `test_complexity_very_complex(self)` — [`L630`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L630)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`_calculate_document_complexity`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter._calculate_document_complexity)

### `TestCollectImages`
- def: [`tests/unit/formatters/test_markdown_formatter_helpers.py:492`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L492)
- signature: `class TestCollectImages:`
- members:
  - `test_collect_images_basic(self)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L493)
  - `test_collect_images_exception_handling(self)` — [`L579`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L579)
  - `test_collect_images_fallback_to_ref_defs(self)` — [`L524`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L524)
  - `test_collect_images_parse_from_name_field(self)` — [`L546`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L546)
  - `test_collect_images_various_extensions(self)` — [`L562`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L562)
  - `test_collect_images_with_ref_defs(self)` — [`L509`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L509)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`_collect_images`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter._collect_images)

### `TestComputeRobustCounts`
- def: [`tests/unit/formatters/test_markdown_formatter_helpers.py:657`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L657)
- signature: `class TestComputeRobustCounts:`
- members:
  - `test_compute_robust_counts_autolinks(self, mock_read)` — [`L672`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L672)
  - `test_compute_robust_counts_basic(self, mock_read)` — [`L659`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L659)
  - `test_compute_robust_counts_empty_path(self)` — [`L739`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L739)
  - `test_compute_robust_counts_file_read_error(self, mock_read)` — [`L730`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L730)
  - `test_compute_robust_counts_image_extensions(self, mock_read)` — [`L748`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L748)
  - `test_compute_robust_counts_image_references(self, mock_read)` — [`L696`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L696)
  - `test_compute_robust_counts_mixed_content(self, mock_read)` — [`L708`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L708)
  - `test_compute_robust_counts_reference_links(self, mock_read)` — [`L684`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L684)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`_compute_robust_counts_from_file`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter._compute_robust_counts_from_file)

### `TestFormatAnalysisResult`
- def: [`tests/unit/formatters/test_markdown_formatter_helpers.py:419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L419)
- signature: `class TestFormatAnalysisResult:`
- members:
  - `test_convert_analysis_result_to_format(self)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L452)
  - `test_format_analysis_result(self)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L420)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_analysis_result`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_analysis_result), [`_convert_analysis_result_to_format`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter._convert_analysis_result_to_format)

### `TestFormatJsonOutput`
- def: [`tests/unit/formatters/test_markdown_formatter_helpers.py:765`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L765)
- signature: `class TestFormatJsonOutput:`
- members:
  - `test_format_json_output_basic(self)` — [`L766`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L766)
  - `test_format_json_output_nested(self)` — [`L776`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L776)
  - `test_format_json_output_unicode(self)` — [`L785`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L785)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`_format_json_output`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter._format_json_output)

### `TestFormatTable`
- def: [`tests/unit/formatters/test_markdown_formatter_helpers.py:6`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L6)
- signature: `class TestFormatTable:`
- members:
  - `test_format_table_basic(self)` — [`L7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L7)
  - `test_format_table_blockquotes_section(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L201)
  - `test_format_table_code_blocks_section(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L119)
  - `test_format_table_footnotes_section(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L324)
  - `test_format_table_headers_section(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L30)
  - `test_format_table_horizontal_rules_section(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L226)
  - `test_format_table_html_elements_section(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L250)
  - `test_format_table_images_section(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L92)
  - `test_format_table_links_section(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L57)
  - `test_format_table_lists_section(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L147)
  - `test_format_table_long_content_truncation(self)` — [`L392`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L392)
  - `test_format_table_no_headers_uses_filename(self)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L380)
  - `test_format_table_reference_definitions_section(self)` — [`L355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L355)
  - `test_format_table_tables_section(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L174)
  - `test_format_table_text_formatting_section(self)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_helpers.py#L281)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_table)

