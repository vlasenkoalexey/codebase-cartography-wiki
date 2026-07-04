---
title: 'Module: tree_sitter_analyzer/models/markup_models.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/models/markup_models.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.models.markup_models`/
symbols:
  MarkupElement: MarkupElement#
  MarkupElement.tag_name: MarkupElement#tag_name.
  StyleElement: StyleElement#
  MarkupElement.element_class: MarkupElement#element_class.
  MarkupElement.attributes: MarkupElement#attributes.
  StyleElement.selector: StyleElement#selector.
  StyleElement.element_class: StyleElement#element_class.
  StyleElement.properties: StyleElement#properties.
  MarkupElement.children: MarkupElement#children.
  MarkupElement.parent: MarkupElement#parent.
  YAMLElement.to_summary_item: YAMLElement#to_summary_item().
  MarkupElement.to_summary_item: MarkupElement#to_summary_item().
  StyleElement.to_summary_item: StyleElement#to_summary_item().
  YAMLElement: YAMLElement#
  YAMLElement.element_type: YAMLElement#element_type.
  YAMLElement.value_type: YAMLElement#value_type.
  YAMLElement.key: YAMLElement#key.
  YAMLElement.nesting_level: YAMLElement#nesting_level.
  YAMLElement.document_index: YAMLElement#document_index.
  StyleElement.element_type: StyleElement#element_type.
  YAMLElement.value: YAMLElement#value.
  YAMLElement.anchor_name: YAMLElement#anchor_name.
  YAMLElement.alias_target: YAMLElement#alias_target.
  YAMLElement.child_count: YAMLElement#child_count.
  MarkupElement.element_type: MarkupElement#element_type.
  YAMLElement.language: YAMLElement#language.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/models/markup_models.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py)

## Classes
### `MarkupElement`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/markup_models.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L15) — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
- doc: HTML要素を表現するデータモデル。
- signature: `class MarkupElement(CodeElement):`
- members:
  - `to_summary_item(self)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L28) — Return dictionary for summary item
  - `attributes` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L22)
  - `children` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L24) — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
  - `element_class` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L25) — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
  - `element_type` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L26)
  - `parent` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L23) — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
  - `tag_name` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L21) — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
- uses (calls/refs, reference-scoped): [`name`](base.md#CodeElement.name), [`start_line`](base.md#CodeElement.start_line), [`end_line`](base.md#CodeElement.end_line), [`CodeElement`](base.md#CodeElement)  (1 test-only)
- used by: [`CodeElement`](base.md#CodeElement), [`_analyze_html_fallback`](../languages/html_plugin.md#_analyze_html_fallback), [`create_markup_element`](../languages/html_helpers.md#create_markup_element), [`_append_compact_markup_element`](../formatters/_html_compact_formatter_helpers.md#_append_compact_markup_element), [`_markup_to_dict`](../formatters/html_formatter.md#HtmlJsonFormatter._markup_to_dict), [`to_summary_item`](base.md#CodeElement.to_summary_item), [`_markup_csv_row`](../formatters/_html_csv_formatter_helpers.md#_markup_csv_row), [`format_element_tree`](../formatters/_html_formatter_helpers.md#format_element_tree), [`_add_classified_element`](../formatters/_html_classification_helpers.md#_add_classified_element), [`_markup_table_row`](../formatters/_html_formatter_helpers.md#_markup_table_row), [`_csv_row`](../formatters/_html_csv_formatter_helpers.md#_csv_row), [`_compact_element_row`](../formatters/_html_compact_formatter_helpers.md#_compact_element_row), [`format_markup_elements`](../formatters/_html_formatter_helpers.md#format_markup_elements), [`_traverse_for_html_elements`](../languages/html_plugin.md#HtmlElementExtractor._traverse_for_html_elements), [`build_html_json_result`](../formatters/_html_json_formatter_helpers.md#build_html_json_result), [`_append_json_element`](../formatters/_html_json_formatter_helpers.md#_append_json_element), [`_create_markup_element`](../languages/html_plugin.md#HtmlElementExtractor._create_markup_element), [`_is_compact_important_element`](../formatters/_html_compact_formatter_helpers.md#_is_compact_important_element), [`_try_create_html_element`](../languages/html_plugin.md#HtmlElementExtractor._try_create_html_element), [`group_compact_markup_elements`](../formatters/_html_compact_formatter_helpers.md#group_compact_markup_elements), [`format_summary`](../formatters/html_formatter.md#HtmlFormatter.format_summary), [`compact_important_elements`](../formatters/_html_compact_formatter_helpers.md#compact_important_elements), [`extract_html_elements`](../languages/html_plugin.md#HtmlElementExtractor.extract_html_elements), [`_compact_id_class`](../formatters/_html_compact_formatter_helpers.md#_compact_id_class), [`_compact_top_level_lines`](../formatters/_html_compact_formatter_helpers.md#_compact_top_level_lines), [`_format_markup_elements`](../formatters/html_formatter.md#HtmlFormatter._format_markup_elements), [`_markup_group_lines`](../formatters/_html_formatter_helpers.md#_markup_group_lines), [`other_elements`](../formatters/_html_compact_formatter_helpers.md#CompactMarkupGroups.other_elements), [`_format_element_tree`](../formatters/html_formatter.md#HtmlFormatter._format_element_tree), [`form_elements`](../formatters/_html_compact_formatter_helpers.md#CompactMarkupGroups.form_elements), [`heading_elements`](../formatters/_html_compact_formatter_helpers.md#CompactMarkupGroups.heading_elements), [`list_elements`](../formatters/_html_compact_formatter_helpers.md#CompactMarkupGroups.list_elements), [`media_elements`](../formatters/_html_compact_formatter_helpers.md#CompactMarkupGroups.media_elements), [`metadata_elements`](../formatters/_html_compact_formatter_helpers.md#CompactMarkupGroups.metadata_elements), [`structure_elements`](../formatters/_html_compact_formatter_helpers.md#CompactMarkupGroups.structure_elements), [`table_elements`](../formatters/_html_compact_formatter_helpers.md#CompactMarkupGroups.table_elements), [`text_elements`](../formatters/_html_compact_formatter_helpers.md#CompactMarkupGroups.text_elements)  (58 test-only)

### `StyleElement`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/markup_models.py:40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L40) — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
- doc: CSSルールを表現するデータモデル。
- signature: `class StyleElement(CodeElement):`
- members:
  - `to_summary_item(self)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L53) — Return dictionary for summary item
  - `element_class` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L48)
  - `element_type` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L51)
  - `properties` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L47)
  - `selector` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L46)
- uses (calls/refs, reference-scoped): [`name`](base.md#CodeElement.name), [`start_line`](base.md#CodeElement.start_line), [`end_line`](base.md#CodeElement.end_line), [`CodeElement`](base.md#CodeElement)
- used by: [`CodeElement`](base.md#CodeElement), [`_analyze_css_fallback`](../languages/css_plugin.md#_analyze_css_fallback), [`create_style_element`](../languages/css_helpers.md#create_style_element), [`_compact_summary_lines`](../formatters/_html_compact_formatter_helpers.md#_compact_summary_lines), [`to_summary_item`](base.md#CodeElement.to_summary_item), [`_style_csv_row`](../formatters/_html_csv_formatter_helpers.md#_style_csv_row), [`_add_classified_element`](../formatters/_html_classification_helpers.md#_add_classified_element), [`_style_to_dict`](../formatters/html_formatter.md#HtmlJsonFormatter._style_to_dict), [`_csv_row`](../formatters/_html_csv_formatter_helpers.md#_csv_row), [`_style_table_row`](../formatters/_html_formatter_helpers.md#_style_table_row), [`_traverse_for_css_rules`](../languages/css_plugin.md#CssElementExtractor._traverse_for_css_rules), [`_create_style_element`](../languages/css_plugin.md#CssElementExtractor._create_style_element), [`build_html_json_result`](../formatters/_html_json_formatter_helpers.md#build_html_json_result), [`_append_json_element`](../formatters/_html_json_formatter_helpers.md#_append_json_element), [`extract_css_rules`](../languages/css_plugin.md#CssElementExtractor.extract_css_rules), [`format_style_elements`](../formatters/_html_formatter_helpers.md#format_style_elements), [`format_summary`](../formatters/html_formatter.md#HtmlFormatter.format_summary), [`_format_style_elements`](../formatters/html_formatter.md#HtmlFormatter._format_style_elements), [`_style_group_lines`](../formatters/_html_formatter_helpers.md#_style_group_lines)  (37 test-only)

### `YAMLElement`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/markup_models.py:65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L65)
- doc: YAML要素を表現するデータモデル。
- signature: `class YAMLElement(CodeElement):`
- members:
  - `to_summary_item(self)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L92) — Return dictionary for summary item with YAML-specific information.
  - `alias_target` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L87)
  - `anchor_name` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L86)
  - `child_count` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L90)
  - `document_index` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L89)
  - `element_type` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L82)
  - `key` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L83)
  - `language` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L81)
  - `nesting_level` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L88)
  - `value` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L84)
  - `value_type` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L85)
- uses (calls/refs, reference-scoped): [`name`](base.md#CodeElement.name), [`start_line`](base.md#CodeElement.start_line), [`end_line`](base.md#CodeElement.end_line), [`CodeElement`](base.md#CodeElement)
- used by: [`CodeElement`](base.md#CodeElement), [`to_summary_item`](base.md#CodeElement.to_summary_item)  (4 test-only)

## Module values
- `__all__` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/markup_models.py#L105)

