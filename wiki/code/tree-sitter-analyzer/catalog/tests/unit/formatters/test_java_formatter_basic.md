---
title: 'Module: tests/unit/formatters/test_java_formatter_basic.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_java_formatter_basic.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_java_formatter_basic`/Test
symbols:
  TestJavaTableFormatterInstantiation.test_formatter_with_format_type: JavaTableFormatterInstantiation#test_formatter_with_format_type().
  TestJavaTableFormatterInstantiation.test_formatter_with_compact_format: JavaTableFormatterInstantiation#test_formatter_with_compact_format().
  TestJavaTableFormatterInstantiation.test_formatter_inheritance: JavaTableFormatterInstantiation#test_formatter_inheritance().
  TestFormatFullTable.test_format_simple_class: FormatFullTable#test_format_simple_class().
  TestFormatFullTable.test_format_class_with_package: FormatFullTable#test_format_class_with_package().
  TestFormatFullTable.test_format_class_with_imports: FormatFullTable#test_format_class_with_imports().
  TestFormatFullTable.test_format_class_with_fields: FormatFullTable#test_format_class_with_fields().
  TestFormatFullTable.test_format_class_with_methods: FormatFullTable#test_format_class_with_methods().
  TestFormatFullTable.test_format_constructor: FormatFullTable#test_format_constructor().
  TestFormatFullTable.test_format_enum_class: FormatFullTable#test_format_enum_class().
  TestFormatFullTable.test_format_multiple_classes: FormatFullTable#test_format_multiple_classes().
  TestFormatCompactTable.test_format_compact_basic: FormatCompactTable#test_format_compact_basic().
  TestFormatCompactTable.test_format_compact_with_methods: FormatCompactTable#test_format_compact_with_methods().
  TestMethodFormatting.test_format_method_row: MethodFormatting#test_format_method_row().
  TestMethodFormatting.test_create_compact_signature: MethodFormatting#test_create_compact_signature().
  TestMethodFormatting.test_create_full_signature: MethodFormatting#test_create_full_signature().
  TestVisibilityConversion.test_convert_visibility: VisibilityConversion#test_convert_visibility().
  TestFormatTable.test_format_table_json: FormatTable#test_format_table_json().
  TestFormatSummary.test_format_summary_basic: FormatSummary#test_format_summary_basic().
  TestJavaTableFormatterInstantiation.test_create_formatter: JavaTableFormatterInstantiation#test_create_formatter().
  TestTypeShortening.test_shorten_primitive_types: TypeShortening#test_shorten_primitive_types().
  TestTypeShortening.test_shorten_common_types: TypeShortening#test_shorten_common_types().
  TestTypeShortening.test_shorten_collection_types: TypeShortening#test_shorten_collection_types().
  TestTypeShortening.test_shorten_map_types: TypeShortening#test_shorten_map_types().
  TestTypeShortening.test_shorten_array_types: TypeShortening#test_shorten_array_types().
  TestTypeShortening.test_shorten_none_type: TypeShortening#test_shorten_none_type().
  TestTypeShortening.test_shorten_unknown_type: TypeShortening#test_shorten_unknown_type().
  TestTypeShortening.test_shorten_empty_array_type: TypeShortening#test_shorten_empty_array_type().
  TestJavaTableFormatterInstantiation: JavaTableFormatterInstantiation#
  TestFormatFullTable: FormatFullTable#
  TestFormatCompactTable: FormatCompactTable#
  TestMethodFormatting: MethodFormatting#
  TestTypeShortening: TypeShortening#
  TestVisibilityConversion: VisibilityConversion#
  TestFormatTable: FormatTable#
  TestFormatSummary: FormatSummary#
---
# Module: [`tests/unit/formatters/test_java_formatter_basic.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py)

## Classes
### `TestFormatCompactTable`
- def: [`tests/unit/formatters/test_java_formatter_basic.py:292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L292)
- doc: Test compact table formatting
- signature: `class TestFormatCompactTable:`
- members:
  - `test_format_compact_basic(self)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L295) — Test basic compact formatting
  - `test_format_compact_with_methods(self)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L319) — Test compact format with methods
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`_format_compact_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.md#JavaTableFormatterCompactMixin._format_compact_table)

### `TestFormatFullTable`
- def: [`tests/unit/formatters/test_java_formatter_basic.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L42)
- doc: Test full table formatting
- signature: `class TestFormatFullTable:`
- members:
  - `test_format_class_with_fields(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L120) — Test formatting class with fields
  - `test_format_class_with_imports(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L92) — Test formatting class with imports
  - `test_format_class_with_methods(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L164) — Test formatting class with methods
  - `test_format_class_with_package(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L69) — Test formatting class with package name
  - `test_format_constructor(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L199) — Test formatting constructor method
  - `test_format_enum_class(self)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L234) — Test formatting enum class
  - `test_format_multiple_classes(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L259) — Test formatting file with multiple classes
  - `test_format_simple_class(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L45) — Test formatting a simple Java class
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/_java_formatter_full_mixin.md#JavaTableFormatterFullMixin._format_full_table)

### `TestFormatSummary`
- def: [`tests/unit/formatters/test_java_formatter_basic.py:508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L508)
- doc: Test format_summary method
- signature: `class TestFormatSummary:`
- members:
  - `test_format_summary_basic(self)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L511) — Test basic summary formatting
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`format_summary`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_summary)

### `TestFormatTable`
- def: [`tests/unit/formatters/test_java_formatter_basic.py:490`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L490)
- doc: Test format_table method
- signature: `class TestFormatTable:`
- members:
  - `test_format_table_json(self)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L493) — Test format_table with json type
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_table)

### `TestJavaTableFormatterInstantiation`
- def: [`tests/unit/formatters/test_java_formatter_basic.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L16)
- doc: Test JavaTableFormatter creation and basic properties
- signature: `class TestJavaTableFormatterInstantiation:`
- members:
  - `test_create_formatter(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L19) — Test creating a JavaTableFormatter instance
  - `test_formatter_inheritance(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L34) — Test that JavaTableFormatter inherits from BaseTableFormatter
  - `test_formatter_with_compact_format(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L29) — Test creating formatter with compact format
  - `test_formatter_with_format_type(self)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L24) — Test creating formatter with specific format type
- uses (calls/refs, reference-scoped): [`BaseTableFormatter`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter), [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`format_type`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter.format_type)

### `TestMethodFormatting`
- def: [`tests/unit/formatters/test_java_formatter_basic.py:355`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L355)
- doc: Test method signature formatting
- signature: `class TestMethodFormatting:`
- members:
  - `test_create_compact_signature(self)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L377) — Test creating compact method signature
  - `test_create_full_signature(self)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L394) — Test creating full method signature
  - `test_format_method_row(self)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L358) — Test formatting a method row
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`_create_full_signature`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._create_full_signature), [`_format_method_row`](../../../tree_sitter_analyzer/formatters/_java_formatter_class_mixin.md#JavaTableFormatterClassMixin._format_method_row), [`_create_compact_signature`](../../../tree_sitter_analyzer/formatters/_java_formatter_compact_mixin.md#JavaTableFormatterCompactMixin._create_compact_signature)

### `TestTypeShortening`
- def: [`tests/unit/formatters/test_java_formatter_basic.py:408`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L408)
- doc: Test type name shortening
- signature: `class TestTypeShortening:`
- members:
  - `test_shorten_array_types(self)` — [`L444`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L444) — Test shortening array types
  - `test_shorten_collection_types(self)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L429) — Test shortening collection types
  - `test_shorten_common_types(self)` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L421) — Test shortening common object types
  - `test_shorten_empty_array_type(self)` — [`L465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L465) — Test shortening empty array type (edge case)
  - `test_shorten_map_types(self)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L437) — Test shortening map types
  - `test_shorten_none_type(self)` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L451) — Test shortening None type
  - `test_shorten_primitive_types(self)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L411) — Test shortening primitive types
  - `test_shorten_unknown_type(self)` — [`L458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L458) — Test shortening unknown type
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter)

### `TestVisibilityConversion`
- def: [`tests/unit/formatters/test_java_formatter_basic.py:473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L473)
- doc: Test visibility indicator conversion
- signature: `class TestVisibilityConversion:`
- members:
  - `test_convert_visibility(self)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_java_formatter_basic.py#L476) — Test converting visibility to indicators
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](../../../tree_sitter_analyzer/formatters/java_formatter.md#JavaTableFormatter), [`_convert_visibility`](../../../tree_sitter_analyzer/formatters/base_formatter.md#BaseTableFormatter._convert_visibility)

