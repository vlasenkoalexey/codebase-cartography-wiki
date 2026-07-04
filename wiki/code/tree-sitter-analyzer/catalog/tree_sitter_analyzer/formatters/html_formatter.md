---
title: 'Module: tree_sitter_analyzer/formatters/html_formatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/html_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters.html_formatter`/
symbols:
  HtmlFormatter.format: HtmlFormatter#format().
  HtmlFormatter: HtmlFormatter#
  HtmlJsonFormatter.format: HtmlJsonFormatter#format().
  HtmlFormatter.format_analysis_result: HtmlFormatter#format_analysis_result().
  HtmlJsonFormatter._markup_to_dict: HtmlJsonFormatter#_markup_to_dict().
  HtmlCompactFormatter.format: HtmlCompactFormatter#format().
  HtmlJsonFormatter._style_to_dict: HtmlJsonFormatter#_style_to_dict().
  HtmlCompactFormatter: HtmlCompactFormatter#
  HtmlJsonFormatter: HtmlJsonFormatter#
  HtmlCsvFormatter.format: HtmlCsvFormatter#format().
  HtmlFormatter.format_table: HtmlFormatter#format_table().
  HtmlJsonFormatter._element_to_dict: HtmlJsonFormatter#_element_to_dict().
  HtmlFormatter.format_advanced: HtmlFormatter#format_advanced().
  HtmlFormatter.format_summary: HtmlFormatter#format_summary().
  HtmlFormatter._format_markup_elements: HtmlFormatter#_format_markup_elements().
  HtmlFormatter._format_style_elements: HtmlFormatter#_format_style_elements().
  HtmlFormatter._element_to_dict: HtmlFormatter#_element_to_dict().
  HtmlCsvFormatter: HtmlCsvFormatter#
  HtmlFormatter._format_element_tree: HtmlFormatter#_format_element_tree().
  HtmlFormatter._format_other_elements: HtmlFormatter#_format_other_elements().
  HtmlFormatter.format_structure: HtmlFormatter#format_structure().
  MockMarkupElement.children: MockMarkupElement#children.
  MockMarkupElement.language: MockMarkupElement#language.
  MockStyleElement.language: MockStyleElement#language.
  HtmlFormatter._dict_to_markup_element.MockMarkupElement: HtmlFormatter#_dict_to_markup_element().MockMarkupElement#
  HtmlFormatter.get_format_name: HtmlFormatter#get_format_name().
  HtmlFormatter._dict_to_markup_element: HtmlFormatter#_dict_to_markup_element().
  HtmlFormatter._dict_to_style_element: HtmlFormatter#_dict_to_style_element().
  HtmlFormatter._dict_to_style_element.MockStyleElement: HtmlFormatter#_dict_to_style_element().MockStyleElement#
  HtmlJsonFormatter.get_format_name: HtmlJsonFormatter#get_format_name().
  HtmlCompactFormatter.get_format_name: HtmlCompactFormatter#get_format_name().
  HtmlCsvFormatter.get_format_name: HtmlCsvFormatter#get_format_name().
  HtmlFormatter.__init__: HtmlFormatter#__init__().
  HtmlFormatter._dict_to_markup_element.MockMarkupElement.__init__: HtmlFormatter#_dict_to_markup_element().MockMarkupElement#__init__().
  MockMarkupElement.name: MockMarkupElement#name.
  MockMarkupElement.tag_name: MockMarkupElement#tag_name.
  MockMarkupElement.element_class: MockMarkupElement#element_class.
  MockMarkupElement.start_line: MockMarkupElement#start_line.
  MockMarkupElement.end_line: MockMarkupElement#end_line.
  MockMarkupElement.attributes: MockMarkupElement#attributes.
  MockMarkupElement.parent: MockMarkupElement#parent.
  HtmlFormatter._dict_to_style_element.MockStyleElement.__init__: HtmlFormatter#_dict_to_style_element().MockStyleElement#__init__().
  MockStyleElement.name: MockStyleElement#name.
  MockStyleElement.selector: MockStyleElement#selector.
  MockStyleElement.element_class: MockStyleElement#element_class.
  MockStyleElement.start_line: MockStyleElement#start_line.
  MockStyleElement.end_line: MockStyleElement#end_line.
  MockStyleElement.properties: MockStyleElement#properties.
---
# Module: [`tree_sitter_analyzer/formatters/html_formatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py)

## Classes
### `HtmlCompactFormatter`
- def: [`tree_sitter_analyzer/formatters/html_formatter.py:247`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L247)
- members:
  - `format(self, elements: list[CodeElement], file_path: str = "")` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L254) — Format HTML elements in compact table format
  - `get_format_name()` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L251)
- uses (calls/refs, reference-scoped): [`CodeElement`](../models/base.md#CodeElement), [`IFormatter`](_formatter_interface.md#IFormatter), [`format_compact_html`](_html_compact_formatter_helpers.md#format_compact_html)
- used by: [`format`](_formatter_interface.md#IFormatter.format), [`get_format_name`](_formatter_interface.md#IFormatter.get_format_name), [`format_analysis_result`](html_formatter.md#HtmlFormatter.format_analysis_result), [`format_table`](html_formatter.md#HtmlFormatter.format_table)  (20 test-only)

### `HtmlCsvFormatter`
- def: [`tree_sitter_analyzer/formatters/html_formatter.py:259`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L259)
- members:
  - `format(self, elements: list[CodeElement])` — [`L266`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L266) — Format HTML elements as CSV
  - `get_format_name()` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L263)
- uses (calls/refs, reference-scoped): [`CodeElement`](../models/base.md#CodeElement), [`IFormatter`](_formatter_interface.md#IFormatter), [`format_html_csv`](_html_csv_formatter_helpers.md#format_html_csv)
- used by: [`format`](_formatter_interface.md#IFormatter.format), [`get_format_name`](_formatter_interface.md#IFormatter.get_format_name), [`format_analysis_result`](html_formatter.md#HtmlFormatter.format_analysis_result)  (14 test-only)

### `HtmlFormatter`  ·  implements/extends BaseFormatter, IFormatter
- def: [`tree_sitter_analyzer/formatters/html_formatter.py:28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L28)
- doc: HTML-specific formatter for MarkupElement and StyleElement
- signature: `class HtmlFormatter(BaseFormatter, IFormatter):`
- members:
  - `__init__(self)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L31) — Initialize HTML formatter
  - `_dict_to_markup_element(self, data: dict)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L154) — Convert dictionary to MarkupElement-like object
  - `_dict_to_style_element(self, data: dict)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L172) — Convert dictionary to StyleElement-like object
  - `_element_to_dict(self, element: CodeElement)` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L188) — Convert generic CodeElement to dictionary
  - `_format_element_tree(self, element: MarkupElement, depth: int)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L142) — Format element tree hierarchy
  - `_format_markup_elements(self, elements: list[MarkupElement])` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L138) — Format MarkupElement list with hierarchy
  - `_format_other_elements(self, elements: list)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L150) — Format other code elements
  - `_format_style_elements(self, elements: list[StyleElement])` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L146) — Format StyleElement list
  - `format(self, elements: list[CodeElement])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L39) — Format HTML elements with hierarchy and classification
  - `format_advanced(self, analysis_result: dict[str, Any], output_format: str = "json")` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L86) — Format advanced analysis output
  - `format_analysis_result(self, analysis_result: Any, table_type: str = "full")` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L98) — Format AnalysisResult directly for HTML files.
  - `format_structure(self, analysis_result: dict[str, Any])` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L81) — Format structure analysis output
  - `format_summary(self, analysis_result: dict[str, Any])` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L61) — Format summary output for HTML elements
  - `format_table(self, analysis_result: dict[str, Any], table_type: str = "full")` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L121) — Format table output
  - `get_format_name()` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L36)
- uses (calls/refs, reference-scoped): [`CodeElement`](../models/base.md#CodeElement), [`MarkupElement`](../models/markup_models.md#MarkupElement), [`BaseFormatter`](base_formatter.md#BaseFormatter), [`StyleElement`](../models/markup_models.md#StyleElement), [`IFormatter`](_formatter_interface.md#IFormatter), [`format`](html_formatter.md#HtmlJsonFormatter.format), [`format`](html_formatter.md#HtmlCompactFormatter.format), [`format_element_tree`](_html_formatter_helpers.md#format_element_tree), [`HtmlCompactFormatter`](html_formatter.md#HtmlCompactFormatter), [`HtmlJsonFormatter`](html_formatter.md#HtmlJsonFormatter), [`format`](html_formatter.md#HtmlCsvFormatter.format), [`element_to_dict`](_html_formatter_helpers.md#element_to_dict), [`format_markup_elements`](_html_formatter_helpers.md#format_markup_elements), [`classify_html_elements`](_html_classification_helpers.md#classify_html_elements), [`format_style_elements`](_html_formatter_helpers.md#format_style_elements), [`HtmlCsvFormatter`](html_formatter.md#HtmlCsvFormatter), [`format_other_elements`](_html_formatter_helpers.md#format_other_elements), [`markup_elements`](_html_classification_helpers.md#ClassifiedHtmlElements.markup_elements), [`other_elements`](_html_classification_helpers.md#ClassifiedHtmlElements.other_elements), [`style_elements`](_html_classification_helpers.md#ClassifiedHtmlElements.style_elements)
- used by: [`BaseFormatter`](base_formatter.md#BaseFormatter), [`IFormatter`](_formatter_interface.md#IFormatter), [`_register_language_formatters_safe`](formatter_registry.md#_register_language_formatters_safe), [`get_format_name`](_formatter_interface.md#IFormatter.get_format_name), [`_formatters`](language_formatter_factory.md#LanguageFormatterFactory._formatters), [`format`](base_formatter.md#BaseFormatter.format), [`format_structure`](base_formatter.md#BaseFormatter.format_structure), [`format_advanced`](base_formatter.md#BaseFormatter.format_advanced), [`format_summary`](base_formatter.md#BaseFormatter.format_summary), [`format_table`](base_formatter.md#BaseFormatter.format_table)  (48 test-only)

### `HtmlJsonFormatter`
- def: [`tree_sitter_analyzer/formatters/html_formatter.py:193`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L193)
- members:
  - `_element_to_dict(self, element: CodeElement)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L236) — Convert generic CodeElement to dictionary
  - `_markup_to_dict(self, element: MarkupElement)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L210) — Convert MarkupElement to dictionary — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
  - `_style_to_dict(self, element: StyleElement)` — [`L224`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L224) — Convert StyleElement to dictionary
  - `format(self, elements: list[CodeElement])` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L200) — Format HTML elements as JSON with hierarchy
  - `get_format_name()` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L197)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`language`](../models/base.md#CodeElement.language), [`CodeElement`](../models/base.md#CodeElement), [`MarkupElement`](../models/markup_models.md#MarkupElement), [`tag_name`](../models/markup_models.md#MarkupElement.tag_name), [`StyleElement`](../models/markup_models.md#StyleElement), [`element_class`](../models/markup_models.md#MarkupElement.element_class), [`IFormatter`](_formatter_interface.md#IFormatter), [`attributes`](../models/markup_models.md#MarkupElement.attributes), [`selector`](../models/markup_models.md#StyleElement.selector), [`element_class`](../models/markup_models.md#StyleElement.element_class), [`properties`](../models/markup_models.md#StyleElement.properties), [`children`](../models/markup_models.md#MarkupElement.children), [`build_html_json_result`](_html_json_formatter_helpers.md#build_html_json_result)
- used by: [`format`](_formatter_interface.md#IFormatter.format), [`get_format_name`](_formatter_interface.md#IFormatter.get_format_name), [`format_analysis_result`](html_formatter.md#HtmlFormatter.format_analysis_result), [`format_table`](html_formatter.md#HtmlFormatter.format_table), [`format_advanced`](html_formatter.md#HtmlFormatter.format_advanced)  (17 test-only)

### `MockMarkupElement`
- def: [`tree_sitter_analyzer/formatters/html_formatter.py:158`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L158)
- signature: `class MockMarkupElement:`
- members:
  - `attributes` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L165)
  - `children` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L166)
  - `element_class` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L162)
  - `end_line` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L164)
  - `language` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L168)
  - `name` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L160)
  - `parent` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L167)
  - `start_line` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L163)
  - `tag_name` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L161)
- protocol/private: `__init__`[`L159`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L159)

### `MockStyleElement`
- def: [`tree_sitter_analyzer/formatters/html_formatter.py:176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L176)
- signature: `class MockStyleElement:`
- members:
  - `element_class` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L180)
  - `end_line` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L182)
  - `language` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L184)
  - `name` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L178)
  - `properties` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L183)
  - `selector` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L179)
  - `start_line` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L181)
- protocol/private: `__init__`[`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/html_formatter.py#L177)

