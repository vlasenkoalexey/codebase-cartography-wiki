---
title: 'Module: tests/property/test_format_properties.py'
type: catalog
provenance: extracted
module: tests/property/test_format_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.property.test_format_properties`/
symbols:
  TestFormatProperties.test_format_idempotency: TestFormatProperties#test_format_idempotency().
  TestFormatProperties.test_empty_elements_list: TestFormatProperties#test_empty_elements_list().
  TestFormatProperties.test_json_format_validity: TestFormatProperties#test_json_format_validity().
  TestFormatProperties.test_csv_format_validity: TestFormatProperties#test_csv_format_validity().
  TestFormatProperties.test_format_preserves_element_count: TestFormatProperties#test_format_preserves_element_count().
  TestFormatProperties.test_format_preserves_element_names: TestFormatProperties#test_format_preserves_element_names().
  TestFormatProperties.test_format_preserves_element_types: TestFormatProperties#test_format_preserves_element_types().
  FormatStatefulMachine.format_elements: FormatStatefulMachine#format_elements().
  TestFormatEdgeCases.test_very_long_element_name: TestFormatEdgeCases#test_very_long_element_name().
  TestFormatEdgeCases.test_special_characters_in_element_name: TestFormatEdgeCases#test_special_characters_in_element_name().
  TestFormatEdgeCases.test_unicode_in_element_name: TestFormatEdgeCases#test_unicode_in_element_name().
  TestFormatEdgeCases.test_negative_line_numbers: TestFormatEdgeCases#test_negative_line_numbers().
  TestFormatEdgeCases.test_zero_line_numbers: TestFormatEdgeCases#test_zero_line_numbers().
  TestFormatEdgeCases.test_very_large_line_numbers: TestFormatEdgeCases#test_very_large_line_numbers().
  TestFormatEdgeCases.test_extra_fields: TestFormatEdgeCases#test_extra_fields().
  TestFormatEdgeCases.test_nested_structures: TestFormatEdgeCases#test_nested_structures().
  TestFormatProperties.test_valid_format_types: TestFormatProperties#test_valid_format_types().
  TestFormatProperties.test_format_type_case_insensitivity: TestFormatProperties#test_format_type_case_insensitivity().
  FormatStatefulMachine.format_history: FormatStatefulMachine#format_history.
  FormatStatefulMachine.all_formats_are_strings: FormatStatefulMachine#all_formats_are_strings().
  FormatStatefulMachine.all_formats_are_non_empty: FormatStatefulMachine#all_formats_are_non_empty().
  FormatStatefulMachine: FormatStatefulMachine#
  TestFormatProperties: TestFormatProperties#
  FormatStatefulMachine.__init__: FormatStatefulMachine#__init__().
  TestFormatEdgeCases: TestFormatEdgeCases#
---
# Module: [`tests/property/test_format_properties.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py)

## Classes
### `FormatStatefulMachine`
- def: [`tests/property/test_format_properties.py:398`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L398)
- doc: 格式状态机测试。
- signature: `class FormatStatefulMachine(RuleBasedStateMachine):`
- members:
  - `all_formats_are_non_empty(self)` — [`L430`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L430) — 验证所有格式都是非空的。
  - `all_formats_are_strings(self)` — [`L424`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L424) — 验证所有格式都是字符串。
  - `format_elements(self, format_type: str)` — [`L406`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L406) — 格式化元素。
  - `format_history` — [`L403`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L403)
- protocol/private: `__init__`[`L401`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L401)
- uses (calls/refs, reference-scoped): [`name`](../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`CodeElement`](../../tree_sitter_analyzer/models/base.md#CodeElement), [`FormatterRegistry`](../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry), [`element_type`](../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`get_formatter_for_language`](../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_formatter_for_language)

### `TestFormatEdgeCases`
- def: [`tests/property/test_format_properties.py:439`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L439)
- doc: 格式边界情况测试。
- signature: `class TestFormatEdgeCases:`
- members:
  - `test_extra_fields(self)` — [`L532`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L532) — 测试额外字段。
  - `test_negative_line_numbers(self)` — [`L487`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L487) — 测试负行号。
  - `test_nested_structures(self)` — [`L546`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L546) — 测试嵌套结构。
  - `test_special_characters_in_element_name(self)` — [`L456`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L456) — 测试元素名称中的特殊字符。
  - `test_unicode_in_element_name(self)` — [`L473`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L473) — 测试元素名称中的Unicode字符。
  - `test_very_large_line_numbers(self)` — [`L515`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L515) — 测试非常大的行号。
  - `test_very_long_element_name(self)` — [`L442`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L442) — 测试非常长的元素名称。
  - `test_zero_line_numbers(self)` — [`L501`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L501) — 测试零行号。
- uses (calls/refs, reference-scoped): [`name`](../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`CodeElement`](../../tree_sitter_analyzer/models/base.md#CodeElement), [`element_type`](../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`JsonFormatter`](../../tree_sitter_analyzer/formatters/formatter_registry.md#JsonFormatter), [`format`](../../tree_sitter_analyzer/formatters/formatter_registry.md#JsonFormatter.format)

### `TestFormatProperties`
- def: [`tests/property/test_format_properties.py:26`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L26)
- doc: 格式属性测试类。
- signature: `class TestFormatProperties:`
- members:
  - `test_csv_format_validity(self, elements: list[dict[str, Any]])` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L178) — 测试CSV格式有效性的属性。
  - `test_empty_elements_list(self, elements: list[dict[str, Any]])` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L87) — 测试空元素列表的属性。
  - `test_format_idempotency(self, elements: list[dict[str, Any]], format_type: str)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L223) — 测试格式化的幂等性。
  - `test_format_preserves_element_count(self, elements: list[dict[str, Any]])` — [`L272`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L272) — 测试格式化保留元素数量的属性。
  - `test_format_preserves_element_names(self, elements: list[dict[str, Any]])` — [`L317`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L317) — 测试格式化保留元素名称的属性。
  - `test_format_preserves_element_types(self, elements: list[dict[str, Any]])` — [`L365`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L365) — 测试格式化保留元素类型的属性。
  - `test_format_type_case_insensitivity(self, format_type: str)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L45) — 测试格式类型大小写不敏感的属性。
  - `test_json_format_validity(self, elements: list[dict[str, Any]])` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L128) — 测试JSON格式有效性的属性。
  - `test_valid_format_types(self, format_type: str)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/property/test_format_properties.py#L31) — 测试有效格式类型的属性。
- uses (calls/refs, reference-scoped): [`name`](../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`CodeElement`](../../tree_sitter_analyzer/models/base.md#CodeElement), [`FormatterRegistry`](../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry), [`element_type`](../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`get_formatter_for_language`](../../tree_sitter_analyzer/formatters/formatter_registry.md#FormatterRegistry.get_formatter_for_language), [`JsonFormatter`](../../tree_sitter_analyzer/formatters/formatter_registry.md#JsonFormatter), [`format`](../../tree_sitter_analyzer/formatters/formatter_registry.md#CsvFormatter.format), [`format`](../../tree_sitter_analyzer/formatters/formatter_registry.md#JsonFormatter.format), [`CsvFormatter`](../../tree_sitter_analyzer/formatters/formatter_registry.md#CsvFormatter), [`CompactFormatter`](../../tree_sitter_analyzer/formatters/formatter_registry.md#CompactFormatter), [`FullFormatter`](../../tree_sitter_analyzer/formatters/formatter_registry.md#FullFormatter)

