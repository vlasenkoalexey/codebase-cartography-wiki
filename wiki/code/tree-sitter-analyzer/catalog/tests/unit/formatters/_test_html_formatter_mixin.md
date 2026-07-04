---
title: 'Module: tests/unit/formatters/_test_html_formatter_mixin.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/_test_html_formatter_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters._test_html_formatter_mixin`/TestHtml
symbols:
  TestHtmlJsonFormatterMixin.test_elements: JsonFormatterMixin#test_elements.
  TestHtmlCompactFormatterMixin.test_elements: CompactFormatterMixin#test_elements.
  TestHtmlFormatterMixin.test_format_element_hierarchy: FormatterMixin#test_format_element_hierarchy().
  TestHtmlJsonFormatterMixin.test_format_markup_element_json: JsonFormatterMixin#test_format_markup_element_json().
  TestHtmlCompactFormatterMixin.test_format_counts_accuracy: CompactFormatterMixin#test_format_counts_accuracy().
  TestHtmlFormatterMixin.test_format_long_attributes: FormatterMixin#test_format_long_attributes().
  TestHtmlFormatterMixin.test_format_long_css_properties: FormatterMixin#test_format_long_css_properties().
  TestHtmlFormatterMixin.test_format_elements_without_attributes: FormatterMixin#test_format_elements_without_attributes().
  TestHtmlFormatterMixin.test_format_elements_without_properties: FormatterMixin#test_format_elements_without_properties().
  TestHtmlJsonFormatterMixin.test_format_style_element_json: JsonFormatterMixin#test_format_style_element_json().
  TestHtmlJsonFormatterMixin.test_json_unicode_handling: JsonFormatterMixin#test_json_unicode_handling().
  TestHtmlCompactFormatterMixin.test_format_markup_element_with_attributes: CompactFormatterMixin#test_format_markup_element_with_attributes().
  TestHtmlCompactFormatterMixin.test_format_markup_element_without_attributes: CompactFormatterMixin#test_format_markup_element_without_attributes().
  TestHtmlCompactFormatterMixin.test_format_style_element: CompactFormatterMixin#test_format_style_element().
  TestHtmlFormatterMixin.markup_elements: FormatterMixin#markup_elements.
  TestHtmlFormatterMixin.style_elements: FormatterMixin#style_elements.
  TestHtmlJsonFormatterMixin.test_format_other_element_json: JsonFormatterMixin#test_format_other_element_json().
  TestHtmlCompactFormatterMixin.test_format_other_element: CompactFormatterMixin#test_format_other_element().
  TestHtmlFormatterMixin.other_elements: FormatterMixin#other_elements.
  TestHtmlFormatterMixin.formatter: FormatterMixin#formatter.
  TestHtmlFormatterMixin.test_format_mixed_elements: FormatterMixin#test_format_mixed_elements().
  TestHtmlFormatterRegistrationMixin.test_get_html_formatters: FormatterRegistrationMixin#test_get_html_formatters().
  TestHtmlCompactFormatterMixin.formatter: CompactFormatterMixin#formatter.
  TestHtmlJsonFormatterMixin.formatter: JsonFormatterMixin#formatter.
  TestHtmlFormatterMixin.test_format_markup_elements_only: FormatterMixin#test_format_markup_elements_only().
  TestHtmlFormatterMixin.test_format_style_elements_only: FormatterMixin#test_format_style_elements_only().
  TestHtmlJsonFormatterMixin.test_format_mixed_elements: JsonFormatterMixin#test_format_mixed_elements().
  TestHtmlCompactFormatterMixin.test_format_mixed_elements: CompactFormatterMixin#test_format_mixed_elements().
  TestHtmlFormatterMixin.test_formatter_inheritance: FormatterMixin#test_formatter_inheritance().
  TestHtmlFormatterMixin.test_get_format_name: FormatterMixin#test_get_format_name().
  TestHtmlFormatterMixin.test_format_empty_list: FormatterMixin#test_format_empty_list().
  TestHtmlJsonFormatterMixin.test_formatter_inheritance: JsonFormatterMixin#test_formatter_inheritance().
  TestHtmlJsonFormatterMixin.test_get_format_name: JsonFormatterMixin#test_get_format_name().
  TestHtmlJsonFormatterMixin.test_format_empty_list: JsonFormatterMixin#test_format_empty_list().
  TestHtmlCompactFormatterMixin.test_formatter_inheritance: CompactFormatterMixin#test_formatter_inheritance().
  TestHtmlCompactFormatterMixin.test_get_format_name: CompactFormatterMixin#test_get_format_name().
  TestHtmlCompactFormatterMixin.test_format_empty_list: CompactFormatterMixin#test_format_empty_list().
  TestHtmlFormatterRegistrationMixin.test_html_formatters_auto_registration: FormatterRegistrationMixin#test_html_formatters_auto_registration().
  TestHtmlFormatterMixin: FormatterMixin#
  TestHtmlJsonFormatterMixin: JsonFormatterMixin#
  TestHtmlCompactFormatterMixin: CompactFormatterMixin#
  TestHtmlFormatterRegistrationMixin: FormatterRegistrationMixin#
  TestHtmlFormatterMixin.__test__: FormatterMixin#__test__.
  TestHtmlFormatterMixin.setup_method: FormatterMixin#setup_method().
  TestHtmlJsonFormatterMixin.__test__: JsonFormatterMixin#__test__.
  TestHtmlJsonFormatterMixin.setup_method: JsonFormatterMixin#setup_method().
  TestHtmlCompactFormatterMixin.__test__: CompactFormatterMixin#__test__.
  TestHtmlCompactFormatterMixin.setup_method: CompactFormatterMixin#setup_method().
  TestHtmlFormatterRegistrationMixin.__test__: FormatterRegistrationMixin#__test__.
---
# Module: [`tests/unit/formatters/_test_html_formatter_mixin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py)

## Classes
### `TestHtmlCompactFormatterMixin`
- def: [`tests/unit/formatters/_test_html_formatter_mixin.py:506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L506)
- doc: Test HtmlCompactFormatter functionality
- signature: `class TestHtmlCompactFormatterMixin:`
- members:
  - `setup_method(self)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L511) — Setup test data
  - `test_format_counts_accuracy(self)` — [`L642`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L642) — Test that element counts are accurate
  - `test_format_empty_list(self)` — [`L637`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L637) — Test compact formatting of empty list
  - `test_format_markup_element_with_attributes(self)` — [`L572`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L572) — Test compact formatting of MarkupElement with attributes
  - `test_format_markup_element_without_attributes(self)` — [`L590`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L590) — Test compact formatting of MarkupElement without attributes
  - `test_format_mixed_elements(self)` — [`L554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L554) — Test compact formatting of mixed elements
  - `test_format_other_element(self)` — [`L626`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L626) — Test compact formatting of other CodeElement
  - `test_format_style_element(self)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L608) — Test compact formatting of StyleElement
  - `test_formatter_inheritance(self)` — [`L546`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L546) — Test that HtmlCompactFormatter inherits from IFormatter
  - `test_get_format_name(self)` — [`L550`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L550) — Test format name
  - `formatter` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L513)
  - `test_elements` — [`L515`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L515)
- protocol/private: `__test__`[`L509`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L509)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`StyleElement`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`IFormatter`](../../../tree_sitter_analyzer/formatters/_formatter_interface.md#IFormatter), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`selector`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.selector), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.element_class), [`properties`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.properties), [`format`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlCompactFormatter.format), [`HtmlCompactFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlCompactFormatter), [`get_format_name`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlCompactFormatter.get_format_name)  (1 test-only)
- used by: (1 test-only callers)

### `TestHtmlFormatterMixin`
- def: [`tests/unit/formatters/_test_html_formatter_mixin.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L17)
- doc: Test HtmlFormatter functionality
- signature: `class TestHtmlFormatterMixin:`
- members:
  - `setup_method(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L22) — Setup test data
  - `test_format_element_hierarchy(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L208) — Test element hierarchy formatting
  - `test_format_elements_without_attributes(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L304) — Test formatting elements without attributes
  - `test_format_elements_without_properties(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L321) — Test formatting CSS elements without properties
  - `test_format_empty_list(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L124) — Test formatting empty element list
  - `test_format_long_attributes(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L259) — Test formatting with long attributes
  - `test_format_long_css_properties(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L282) — Test formatting with long CSS properties
  - `test_format_markup_elements_only(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L129) — Test formatting only MarkupElements
  - `test_format_mixed_elements(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L183) — Test formatting mixed element types
  - `test_format_style_elements_only(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L158) — Test formatting only StyleElements
  - `test_formatter_inheritance(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L116) — Test that HtmlFormatter inherits from IFormatter
  - `test_get_format_name(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L120) — Test format name
  - `formatter` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L24)
  - `markup_elements` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L27)
  - `other_elements` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L111)
  - `style_elements` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L76)
- protocol/private: `__test__`[`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L20)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`StyleElement`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`IFormatter`](../../../tree_sitter_analyzer/formatters/_formatter_interface.md#IFormatter), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`format`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter.format), [`selector`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.selector), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.element_class), [`properties`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.properties), [`children`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.children), [`parent`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.parent), [`HtmlFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter), [`get_format_name`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter.get_format_name)  (1 test-only)
- used by: (1 test-only callers)

### `TestHtmlFormatterRegistrationMixin`
- def: [`tests/unit/formatters/_test_html_formatter_mixin.py:668`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L668)
- doc: Test HTML formatter registration
- signature: `class TestHtmlFormatterRegistrationMixin:`
- members:
  - `test_get_html_formatters(self)` — [`L689`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L689) — Test getting HTML formatter instances
  - `test_html_formatters_auto_registration(self)` — [`L676`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L676) — Test that HTML formatters are automatically registered
- protocol/private: `__test__`[`L671`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L671)
- uses (calls/refs, reference-scoped): [`FormatterRegistry`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry), [`HtmlFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter), [`HtmlCompactFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlCompactFormatter), [`get_formatter`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_formatter), [`HtmlJsonFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlJsonFormatter), [`get_available_formats`](../../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_available_formats)  (1 test-only)
- used by: (1 test-only callers)

### `TestHtmlJsonFormatterMixin`
- def: [`tests/unit/formatters/_test_html_formatter_mixin.py:339`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L339)
- doc: Test HtmlJsonFormatter functionality
- signature: `class TestHtmlJsonFormatterMixin:`
- members:
  - `setup_method(self)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L344) — Setup test data
  - `test_format_empty_list(self)` — [`L475`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L475) — Test JSON formatting of empty list
  - `test_format_markup_element_json(self)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L393) — Test MarkupElement JSON formatting
  - `test_format_mixed_elements(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L378) — Test JSON formatting of mixed elements
  - `test_format_other_element_json(self)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L458) — Test other CodeElement JSON formatting
  - `test_format_style_element_json(self)` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L433) — Test StyleElement JSON formatting
  - `test_formatter_inheritance(self)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L370) — Test that HtmlJsonFormatter inherits from IFormatter
  - `test_get_format_name(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L374) — Test format name
  - `test_json_unicode_handling(self)` — [`L486`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L486) — Test JSON formatting with Unicode content
  - `formatter` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L346)
  - `test_elements` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L348)
- protocol/private: `__test__`[`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/_test_html_formatter_mixin.py#L342)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`MarkupElement`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement), [`tag_name`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.tag_name), [`StyleElement`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.element_class), [`IFormatter`](../../../tree_sitter_analyzer/formatters/_formatter_interface.md#IFormatter), [`attributes`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.attributes), [`selector`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.selector), [`element_class`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.element_class), [`properties`](../../../tree_sitter_analyzer/models/markup_models.md#StyleElement.properties), [`children`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.children), [`parent`](../../../tree_sitter_analyzer/models/markup_models.md#MarkupElement.parent), [`format`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlJsonFormatter.format), [`HtmlJsonFormatter`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlJsonFormatter), [`get_format_name`](../../../tree_sitter_analyzer/formatters/html_formatter.md#HtmlJsonFormatter.get_format_name)  (1 test-only)
- used by: (1 test-only callers)

