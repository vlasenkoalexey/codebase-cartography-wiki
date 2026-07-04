---
title: 'Module: tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._html_compact_formatter_helpers`/
symbols:
  _append_compact_markup_element: _append_compact_markup_element().
  _compact_summary_lines: _compact_summary_lines().
  format_compact_html: format_compact_html().
  _compact_element_row: _compact_element_row().
  group_compact_markup_elements: group_compact_markup_elements().
  _is_compact_important_element: _is_compact_important_element().
  compact_important_elements: compact_important_elements().
  _compact_top_level_lines: _compact_top_level_lines().
  _compact_id_class: _compact_id_class().
  CompactMarkupGroups.other_elements: CompactMarkupGroups#other_elements.
  CompactMarkupGroups.structure_elements: CompactMarkupGroups#structure_elements.
  CompactMarkupGroups.heading_elements: CompactMarkupGroups#heading_elements.
  CompactMarkupGroups.text_elements: CompactMarkupGroups#text_elements.
  CompactMarkupGroups.form_elements: CompactMarkupGroups#form_elements.
  CompactMarkupGroups.media_elements: CompactMarkupGroups#media_elements.
  CompactMarkupGroups.table_elements: CompactMarkupGroups#table_elements.
  CompactMarkupGroups.list_elements: CompactMarkupGroups#list_elements.
  CompactMarkupGroups.metadata_elements: CompactMarkupGroups#metadata_elements.
  CompactMarkupGroups: CompactMarkupGroups#
  IMPORTANT_HTML_TAGS: IMPORTANT_HTML_TAGS.
  _compact_filename: _compact_filename().
---
# Module: [`tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py)

## Classes
### `CompactMarkupGroups`
- def: [`tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py:24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L24)
- signature: `class CompactMarkupGroups:`
- members:
  - `form_elements` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L28)
  - `heading_elements` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L26)
  - `list_elements` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L31)
  - `media_elements` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L29)
  - `metadata_elements` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L32)
  - `other_elements` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L33)
  - `structure_elements` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L25)
  - `table_elements` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L30)
  - `text_elements` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L27)
- uses (calls/refs, reference-scoped): [`MarkupElement`](../models/markup_models.md#MarkupElement)
- used by: [`_append_compact_markup_element`](_html_compact_formatter_helpers.md#_append_compact_markup_element), [`_compact_summary_lines`](_html_compact_formatter_helpers.md#_compact_summary_lines), [`group_compact_markup_elements`](_html_compact_formatter_helpers.md#group_compact_markup_elements)

## Functions
- `_append_compact_markup_element(groups: CompactMarkupGroups, element: MarkupElement)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L78) — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
- `_compact_element_row(element: MarkupElement)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L137)
- `_compact_filename(file_path: str)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L69)
- `_compact_id_class(element: MarkupElement)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L146)
- `_compact_summary_lines(elements: list[CodeElement], groups: CompactMarkupGroups)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L95) — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
- `_compact_top_level_lines(important_elements: list[MarkupElement])` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L122)
- `_is_compact_important_element(element: MarkupElement)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L156)
- `compact_important_elements(elements: list[CodeElement])` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L59)
- `format_compact_html(elements: list[CodeElement], file_path: str = "")` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L36) — Format HTML elements in compact table format.
- `group_compact_markup_elements(elements: list[CodeElement])` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L51)

## Module values
- `IMPORTANT_HTML_TAGS` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_html_compact_formatter_helpers.py#L7)

