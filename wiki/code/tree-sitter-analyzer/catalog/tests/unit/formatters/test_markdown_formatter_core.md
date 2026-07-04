---
title: 'Module: tests/unit/formatters/test_markdown_formatter_core.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_markdown_formatter_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_markdown_formatter_core`/Test
symbols:
  TestMarkdownFormatterInitialization.test_init: MarkdownFormatterInitialization#test_init().
  TestMarkdownFormatterInitialization.test_inherits_from_base: MarkdownFormatterInitialization#test_inherits_from_base().
  TestFormatSummary.test_format_summary_basic: FormatSummary#test_format_summary_basic().
  TestFormatSummary.test_format_summary_empty_elements: FormatSummary#test_format_summary_empty_elements().
  TestFormatSummary.test_format_summary_multiple_link_types: FormatSummary#test_format_summary_multiple_link_types().
  TestFormatSummary.test_format_summary_with_images: FormatSummary#test_format_summary_with_images().
  TestFormatSummary.test_format_summary_with_lists: FormatSummary#test_format_summary_with_lists().
  TestFormatSummary.test_format_summary_with_robust_counts_links: FormatSummary#test_format_summary_with_robust_counts_links().
  TestFormatSummary.test_format_summary_with_robust_counts_images: FormatSummary#test_format_summary_with_robust_counts_images().
  TestFormatStructure.test_format_structure_basic: FormatStructure#test_format_structure_basic().
  TestFormatStructure.test_format_structure_all_element_types: FormatStructure#test_format_structure_all_element_types().
  TestFormatStructure.test_format_structure_with_robust_counts: FormatStructure#test_format_structure_with_robust_counts().
  TestFormatStructure.test_format_structure_robust_fallback: FormatStructure#test_format_structure_robust_fallback().
  TestFormatAdvanced.test_format_advanced_json: FormatAdvanced#test_format_advanced_json().
  TestFormatAdvanced.test_format_advanced_text: FormatAdvanced#test_format_advanced_text().
  TestFormatAdvanced.test_format_advanced_document_metrics: FormatAdvanced#test_format_advanced_document_metrics().
  TestFormatAdvanced.test_format_advanced_content_analysis: FormatAdvanced#test_format_advanced_content_analysis().
  TestFormatAdvanced.test_format_advanced_no_headers: FormatAdvanced#test_format_advanced_no_headers().
  TestFormatAdvanced.test_format_advanced_with_robust_counts: FormatAdvanced#test_format_advanced_with_robust_counts().
  TestMarkdownFormatterInitialization: MarkdownFormatterInitialization#
  TestFormatSummary: FormatSummary#
  TestFormatStructure: FormatStructure#
  TestFormatAdvanced: FormatAdvanced#
---
# Module: [`tests/unit/formatters/test_markdown_formatter_core.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py)

## Classes
### `TestFormatAdvanced`
- def: [`tests/unit/formatters/test_markdown_formatter_core.py:279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L279)
- signature: `class TestFormatAdvanced:`
- members:
  - `test_format_advanced_content_analysis(self)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L361)
  - `test_format_advanced_document_metrics(self)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L322)
  - `test_format_advanced_json(self)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L281)
  - `test_format_advanced_no_headers(self)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L391)
  - `test_format_advanced_text(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L304)
  - `test_format_advanced_with_robust_counts(self, mock_robust)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L405)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_advanced`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_advanced)

### `TestFormatStructure`
- def: [`tests/unit/formatters/test_markdown_formatter_core.py:150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L150)
- signature: `class TestFormatStructure:`
- members:
  - `test_format_structure_all_element_types(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L184)
  - `test_format_structure_basic(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L152)
  - `test_format_structure_robust_fallback(self, mock_robust)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L259)
  - `test_format_structure_with_robust_counts(self, mock_robust)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L241)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_structure)

### `TestFormatSummary`
- def: [`tests/unit/formatters/test_markdown_formatter_core.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L20)
- signature: `class TestFormatSummary:`
- members:
  - `test_format_summary_basic(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L22)
  - `test_format_summary_empty_elements(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L45)
  - `test_format_summary_multiple_link_types(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L57)
  - `test_format_summary_with_images(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L78)
  - `test_format_summary_with_lists(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L98)
  - `test_format_summary_with_robust_counts_images(self, mock_robust)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L134)
  - `test_format_summary_with_robust_counts_links(self, mock_robust)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L116)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`format_summary`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.format_summary)

### `TestMarkdownFormatterInitialization`
- def: [`tests/unit/formatters/test_markdown_formatter_core.py:7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L7)
- signature: `class TestMarkdownFormatterInitialization:`
- members:
  - `test_inherits_from_base(self)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L13)
  - `test_init(self)` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_markdown_formatter_core.py#L9)
- uses (calls/refs, reference-scoped): [`MarkdownFormatter`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter), [`BaseFormatter`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseFormatter), [`language`](../../../tree_sitter_analyzer/formatters/markdown_formatter.md#MarkdownFormatter.language)

