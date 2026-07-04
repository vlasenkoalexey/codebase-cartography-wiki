---
title: 'Module: tests/unit/formatters/test_html_formatter_advanced.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_html_formatter_advanced.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_html_formatter_advanced`/TestHtml
symbols:
  TestHtmlFormatterFalsyAttributes.test_markup_with_empty_string_attribute: FormatterFalsyAttributes#test_markup_with_empty_string_attribute().
  TestHtmlFormatterFalsyAttributes.test_markup_with_none_attribute: FormatterFalsyAttributes#test_markup_with_none_attribute().
  TestHtmlFormatterFalsyAttributes.test_markup_with_boolean_false_attribute: FormatterFalsyAttributes#test_markup_with_boolean_false_attribute().
  TestHtmlCompactFormatterFilepath.test_filepath_html_extension_stripped: CompactFormatterFilepath#test_filepath_html_extension_stripped().
  TestHtmlCompactFormatterFilepath.test_filepath_htm_extension_stripped: CompactFormatterFilepath#test_filepath_htm_extension_stripped().
  TestHtmlCompactFormatterFilepath.test_filepath_non_html_extension_kept: CompactFormatterFilepath#test_filepath_non_html_extension_kept().
  TestHtmlCompactFormatterFilepath.test_filepath_backslash_path: CompactFormatterFilepath#test_filepath_backslash_path().
  TestHtmlCompactElementClassification.test_heading_element_classification: CompactElementClassification#test_heading_element_classification().
  TestHtmlCompactElementClassification.test_table_element_classification: CompactElementClassification#test_table_element_classification().
  TestHtmlCompactElementClassification.test_list_element_classification: CompactElementClassification#test_list_element_classification().
  TestHtmlCompactElementClassification.test_metadata_element_classification: CompactElementClassification#test_metadata_element_classification().
  TestHtmlCompactOver20Elements.test_more_than_20_important_elements: CompactOver20Elements#test_more_than_20_important_elements().
  TestHtmlFormatterUnknownElementType.test_unknown_object_in_format: FormatterUnknownElementType#test_unknown_object_in_format().
  TestHtmlFormatOtherElementsNonDict.test_format_other_elements_non_dict_non_markup: FormatOtherElementsNonDict#test_format_other_elements_non_dict_non_markup().
  TestHtmlOtherElementsNonDict.test_json_format_dict_with_tag_name: OtherElementsNonDict#test_json_format_dict_with_tag_name().
  TestHtmlOtherElementsNonDict.test_json_format_dict_with_element_type_tag: OtherElementsNonDict#test_json_format_dict_with_element_type_tag().
  TestHtmlOtherElementsNonDict.test_json_format_dict_with_selector: OtherElementsNonDict#test_json_format_dict_with_selector().
  TestHtmlOtherElementsNonDict.test_json_format_dict_with_type_rule: OtherElementsNonDict#test_json_format_dict_with_type_rule().
  TestHtmlOtherElementsNonDict.test_json_format_dict_unknown_type: OtherElementsNonDict#test_json_format_dict_unknown_type().
  TestHtmlFormatterUnknownElementType.test_unknown_object_in_format.UnknownType: FormatterUnknownElementType#test_unknown_object_in_format().UnknownType#
  TestHtmlFormatOtherElementsNonDict.test_format_other_elements_non_dict_non_markup.UnknownThing: FormatOtherElementsNonDict#test_format_other_elements_non_dict_non_markup().UnknownThing#
  TestHtmlFormatterFalsyAttributes: FormatterFalsyAttributes#
  TestHtmlFormatterUnknownElementType: FormatterUnknownElementType#
  TestHtmlOtherElementsNonDict: OtherElementsNonDict#
  TestHtmlCompactFormatterFilepath: CompactFormatterFilepath#
  TestHtmlCompactElementClassification: CompactElementClassification#
  TestHtmlCompactOver20Elements: CompactOver20Elements#
  TestHtmlFormatOtherElementsNonDict: FormatOtherElementsNonDict#
---
# Module: [`tests/unit/formatters/test_html_formatter_advanced.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py)

## Classes
### `TestHtmlCompactElementClassification`
- def: [`tests/unit/formatters/test_html_formatter_advanced.py:232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L232)
- doc: Cover element classification in compact formatter (lines 481-493)
- signature: `class TestHtmlCompactElementClassification:`
- members:
  - `test_heading_element_classification(self)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L235) — Compact format classifies heading elements
  - `test_list_element_classification(self)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L265) — Compact format classifies list elements
  - `test_metadata_element_classification(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L280) — Compact format classifies metadata elements
  - `test_table_element_classification(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L250) — Compact format classifies table elements
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`format`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlCompactFormatter.format), [`HtmlCompactFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlCompactFormatter)

### `TestHtmlCompactFormatterFilepath`
- def: [`tests/unit/formatters/test_html_formatter_advanced.py:168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L168)
- doc: Cover filename extraction in compact formatter (lines 455-457)
- signature: `class TestHtmlCompactFormatterFilepath:`
- members:
  - `test_filepath_backslash_path(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L216) — Compact format handles Windows-style backslash paths
  - `test_filepath_htm_extension_stripped(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L186) — Compact format strips .htm extension from filename
  - `test_filepath_html_extension_stripped(self)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L171) — Compact format strips .html extension from filename
  - `test_filepath_non_html_extension_kept(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L201) — Compact format keeps non-html filename as-is
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`format`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlCompactFormatter.format), [`HtmlCompactFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlCompactFormatter)

### `TestHtmlCompactOver20Elements`
- def: [`tests/unit/formatters/test_html_formatter_advanced.py:296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L296)
- doc: Cover &gt;20 elements truncation message (line 570)
- signature: `class TestHtmlCompactOver20Elements:`
- members:
  - `test_more_than_20_important_elements(self)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L299) — Compact format shows '(N more)' when >20 important elements
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`format`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlCompactFormatter.format), [`HtmlCompactFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlCompactFormatter)

### `TestHtmlFormatOtherElementsNonDict`
- def: [`tests/unit/formatters/test_html_formatter_advanced.py:324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L324)
- doc: Cover _format_other_elements getattr fallback (lines 295-299)
- signature: `class TestHtmlFormatOtherElementsNonDict:`
- members:
  - `test_format_other_elements_non_dict_non_markup(self)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L327) — Directly call _format_other_elements with non-dict, non-MarkupElement
- uses (calls/refs, reference-scoped): [`HtmlFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter), [`_format_other_elements`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter._format_other_elements)  (1 test-only)

### `TestHtmlFormatterFalsyAttributes`
- def: [`tests/unit/formatters/test_html_formatter_advanced.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L20)
- doc: Cover attribute formatting with falsy values (line 185)
- signature: `class TestHtmlFormatterFalsyAttributes:`
- members:
  - `test_markup_with_boolean_false_attribute(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L53) — Format markup element with False attribute value
  - `test_markup_with_empty_string_attribute(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L23) — Format markup element with empty string attribute value
  - `test_markup_with_none_attribute(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L38) — Format markup element with None attribute value
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`format`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter.format), [`HtmlFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter)

### `TestHtmlFormatterUnknownElementType`
- def: [`tests/unit/formatters/test_html_formatter_advanced.py:69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L69)
- doc: Cover getattr fallback for unknown element types (lines 295-299)
- signature: `class TestHtmlFormatterUnknownElementType:`
- members:
  - `test_unknown_object_in_format(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L72) — Format with unknown object type uses getattr fallback
- uses (calls/refs, reference-scoped): [`format`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter.format), [`HtmlFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter)  (1 test-only)

### `TestHtmlOtherElementsNonDict`
- def: [`tests/unit/formatters/test_html_formatter_advanced.py:91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L91)
- doc: Cover HtmlJsonFormatter dict element handling (lines 381-393)
- signature: `class TestHtmlOtherElementsNonDict:`
- members:
  - `test_json_format_dict_unknown_type(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L153) — JSON format dict element with unknown type goes to other
  - `test_json_format_dict_with_element_type_tag(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L110) — JSON format dict element with type='tag'
  - `test_json_format_dict_with_selector(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L124) — JSON format dict element with selector
  - `test_json_format_dict_with_tag_name(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L94) — JSON format dict element with tag_name
  - `test_json_format_dict_with_type_rule(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L139) — JSON format dict element with element_type='rule'
- uses (calls/refs, reference-scoped): [`format`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlJsonFormatter.format), [`HtmlJsonFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlJsonFormatter)

### `UnknownThing`
- def: [`tests/unit/formatters/test_html_formatter_advanced.py:331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L331)
- signature: `class UnknownThing:`
- used by: (1 test-only callers)

### `UnknownType`
- def: [`tests/unit/formatters/test_html_formatter_advanced.py:76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_html_formatter_advanced.py#L76)
- signature: `class UnknownType:`
- used by: (1 test-only callers)

