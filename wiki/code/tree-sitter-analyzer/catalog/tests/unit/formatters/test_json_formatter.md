---
title: 'Module: tests/unit/formatters/test_json_formatter.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_json_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_json_formatter`/
symbols:
  _prop: _prop().
  TestFormatTable.test_delegates_to_format_structure: TestFormatTable#test_delegates_to_format_structure().
  TestFormatSummary.test_with_doc_and_props: TestFormatSummary#test_with_doc_and_props().
  TestFormatStructure.test_props_shown_in_table: TestFormatStructure#test_props_shown_in_table().
  TestFormatStructure.test_level_2_props_shown: TestFormatStructure#test_level_2_props_shown().
  TestFormatStructure.test_deeper_props_not_shown_but_counted: TestFormatStructure#test_deeper_props_not_shown_but_counted().
  _doc: _doc().
  TestFormatPropRow.test_simple_string_value: TestFormatPropRow#test_simple_string_value().
  TestFormatPropRow.test_long_value_truncated: TestFormatPropRow#test_long_value_truncated().
  TestFormatPropRow.test_object_child_count_shows_props: TestFormatPropRow#test_object_child_count_shows_props().
  TestFormatPropRow.test_array_child_count_shows_items: TestFormatPropRow#test_array_child_count_shows_items().
  TestFormatPropRow.test_same_start_end_single_line: TestFormatPropRow#test_same_start_end_single_line().
  TestFormatPropRow.test_different_start_end_range: TestFormatPropRow#test_different_start_end_range().
  TestFormatPropRow.test_uses_name_key_when_key_missing: TestFormatPropRow#test_uses_name_key_when_key_missing().
  TestFormatStructure.test_doc_only_renders_document_info: TestFormatStructure#test_doc_only_renders_document_info().
  TestFormatStructure.test_array_root_uses_items_label: TestFormatStructure#test_array_root_uses_items_label().
  TestFormatStructure.test_line_count_from_statistics_key: TestFormatStructure#test_line_count_from_statistics_key().
  TestFormatAdvanced.test_value_type_distribution: TestFormatAdvanced#test_value_type_distribution().
  TestFormatAdvanced.test_max_nesting_depth: TestFormatAdvanced#test_max_nesting_depth().
  TestFormatAdvanced.test_properties_per_level_keys_are_strings: TestFormatAdvanced#test_properties_per_level_keys_are_strings().
  TestInit.test_language_attribute: TestInit#test_language_attribute().
  TestFormatJsonOutput.test_contains_title_separator: TestFormatJsonOutput#test_contains_title_separator().
  TestFormatJsonOutput.test_contains_valid_json: TestFormatJsonOutput#test_contains_valid_json().
  TestFormatJsonOutput.test_non_ascii_preserved: TestFormatJsonOutput#test_non_ascii_preserved().
  TestFormatPropRow.test_no_value_empty_display: TestFormatPropRow#test_no_value_empty_display().
  TestFormatPropRow.test_question_mark_fallback_when_no_key_or_name: TestFormatPropRow#test_question_mark_fallback_when_no_key_or_name().
  TestFormatSummary.test_no_elements_returns_unknown: TestFormatSummary#test_no_elements_returns_unknown().
  TestFormatSummary.test_pair_element_type_counts_as_prop: TestFormatSummary#test_pair_element_type_counts_as_prop().
  TestFormatSummary.test_non_prop_elements_ignored: TestFormatSummary#test_non_prop_elements_ignored().
  TestFormatStructure.test_no_elements_returns_no_elements_message: TestFormatStructure#test_no_elements_returns_no_elements_message().
  TestFormatStructure.test_no_root_children_no_label: TestFormatStructure#test_no_root_children_no_label().
  TestFormatAdvanced.test_empty_elements: TestFormatAdvanced#test_empty_elements().
  TestFormatAdvanced.test_missing_value_type_classified_as_unknown: TestFormatAdvanced#test_missing_value_type_classified_as_unknown().
  TestFormatTable.test_table_type_ignored: TestFormatTable#test_table_type_ignored().
  fmt: fmt().
  TestInit: TestInit#
  TestFormatJsonOutput: TestFormatJsonOutput#
  TestFormatPropRow: TestFormatPropRow#
  TestFormatSummary: TestFormatSummary#
  TestFormatStructure: TestFormatStructure#
  TestFormatAdvanced: TestFormatAdvanced#
  TestFormatTable: TestFormatTable#
---
# Module: [`tests/unit/formatters/test_json_formatter.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py)

## Classes
### `TestFormatAdvanced`
- def: [`tests/unit/formatters/test_json_formatter.py:308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L308)
- signature: `class TestFormatAdvanced:`
- members:
  - `test_empty_elements(self, fmt: JSONFormatter)` — [`L309`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L309)
  - `test_max_nesting_depth(self, fmt: JSONFormatter)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L331)
  - `test_missing_value_type_classified_as_unknown(self, fmt: JSONFormatter)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L344)
  - `test_properties_per_level_keys_are_strings(self, fmt: JSONFormatter)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L353)
  - `test_value_type_distribution(self, fmt: JSONFormatter)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L316)
- uses (calls/refs, reference-scoped): [`JSONFormatter`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter), [`format_advanced`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter.format_advanced)  (1 test-only)

### `TestFormatJsonOutput`
- def: [`tests/unit/formatters/test_json_formatter.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L67)
- signature: `class TestFormatJsonOutput:`
- members:
  - `test_contains_title_separator(self, fmt: JSONFormatter)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L68)
  - `test_contains_valid_json(self, fmt: JSONFormatter)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L72)
  - `test_non_ascii_preserved(self, fmt: JSONFormatter)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L78)
- uses (calls/refs, reference-scoped): [`JSONFormatter`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter), [`_format_json_output`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter._format_json_output)

### `TestFormatPropRow`
- def: [`tests/unit/formatters/test_json_formatter.py:88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L88)
- signature: `class TestFormatPropRow:`
- members:
  - `test_array_child_count_shows_items(self, fmt: JSONFormatter)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L109)
  - `test_different_start_end_range(self, fmt: JSONFormatter)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L133)
  - `test_long_value_truncated(self, fmt: JSONFormatter)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L96)
  - `test_no_value_empty_display(self, fmt: JSONFormatter)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L114)
  - `test_object_child_count_shows_props(self, fmt: JSONFormatter)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L104)
  - `test_question_mark_fallback_when_no_key_or_name(self, fmt: JSONFormatter)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L143)
  - `test_same_start_end_single_line(self, fmt: JSONFormatter)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L127)
  - `test_simple_string_value(self, fmt: JSONFormatter)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L89)
  - `test_uses_name_key_when_key_missing(self, fmt: JSONFormatter)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L138)
- uses (calls/refs, reference-scoped): [`JSONFormatter`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter), [`_format_prop_row`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter._format_prop_row)  (1 test-only)

### `TestFormatStructure`
- def: [`tests/unit/formatters/test_json_formatter.py:218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L218)
- signature: `class TestFormatStructure:`
- members:
  - `test_array_root_uses_items_label(self, fmt: JSONFormatter)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L236)
  - `test_deeper_props_not_shown_but_counted(self, fmt: JSONFormatter)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L271)
  - `test_doc_only_renders_document_info(self, fmt: JSONFormatter)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L224)
  - `test_level_2_props_shown(self, fmt: JSONFormatter)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L258)
  - `test_line_count_from_statistics_key(self, fmt: JSONFormatter)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L284)
  - `test_no_elements_returns_no_elements_message(self, fmt: JSONFormatter)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L219)
  - `test_no_root_children_no_label(self, fmt: JSONFormatter)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L293)
  - `test_props_shown_in_table(self, fmt: JSONFormatter)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L244)
- uses (calls/refs, reference-scoped): [`JSONFormatter`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter.format_structure)  (2 test-only)

### `TestFormatSummary`
- def: [`tests/unit/formatters/test_json_formatter.py:162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L162)
- signature: `class TestFormatSummary:`
- members:
  - `test_no_elements_returns_unknown(self, fmt: JSONFormatter)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L179)
  - `test_non_prop_elements_ignored(self, fmt: JSONFormatter)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L203)
  - `test_pair_element_type_counts_as_prop(self, fmt: JSONFormatter)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L186)
  - `test_with_doc_and_props(self, fmt: JSONFormatter)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L163)
- uses (calls/refs, reference-scoped): [`JSONFormatter`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter), [`format_summary`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter.format_summary)  (2 test-only)

### `TestFormatTable`
- def: [`tests/unit/formatters/test_json_formatter.py:368`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L368)
- signature: `class TestFormatTable:`
- members:
  - `test_delegates_to_format_structure(self, fmt: JSONFormatter)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L369)
  - `test_table_type_ignored(self, fmt: JSONFormatter)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L373)
- uses (calls/refs, reference-scoped): [`JSONFormatter`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter.format_structure), [`format_table`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter.format_table)  (2 test-only)

### `TestInit`
- def: [`tests/unit/formatters/test_json_formatter.py:57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L57)
- signature: `class TestInit:`
- members:
  - `test_language_attribute(self, fmt: JSONFormatter)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L58)
- uses (calls/refs, reference-scoped): [`JSONFormatter`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter), [`language`](../../../tree_sitter_analyzer/formatters/json_formatter.md#JSONFormatter.language)

## Functions
- `_doc(value_type: str = "object", child_count: int | None = None)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L17)
- `_prop(key: str = "name", value_type: str = "string", value: str = "hello", nesting_level: int = 1, start_line: int = 1, end_line: int = 1, child_count: int | None = None, name: str | None = None)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L24)
- `fmt()` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_json_formatter.py#L13)

