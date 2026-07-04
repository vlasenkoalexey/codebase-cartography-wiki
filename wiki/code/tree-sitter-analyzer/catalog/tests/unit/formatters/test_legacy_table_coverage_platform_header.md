---
title: 'Module: tests/unit/formatters/test_legacy_table_coverage_platform_header.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_legacy_table_coverage_platform_header.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_legacy_table_coverage_platform_header`/Test
symbols:
  TestFullTableMultiClassParamTypes.test_string_parameter: FullTableMultiClassParamTypes#test_string_parameter().
  TestFullTableMultiClassParamTypes.test_fallback_parameter_non_dict_non_string: FullTableMultiClassParamTypes#test_fallback_parameter_non_dict_non_string().
  TestFullTableMultiClassParamTypes.test_mixed_param_types: FullTableMultiClassParamTypes#test_mixed_param_types().
  TestPlatformNewlineWindows.test_get_platform_newline_windows: PlatformNewlineWindows#test_get_platform_newline_windows().
  TestPlatformNewlineWindows.test_convert_to_platform_newlines_on_windows: PlatformNewlineWindows#test_convert_to_platform_newlines_on_windows().
  TestFullTableHeaderEdgeCases.test_package_with_no_classes_and_file_path: FullTableHeaderEdgeCases#test_package_with_no_classes_and_file_path().
  TestFullTableHeaderEdgeCases.test_no_file_path_with_package: FullTableHeaderEdgeCases#test_no_file_path_with_package().
  TestFullTableHeaderEdgeCases.test_file_path_equals_unknown_string: FullTableHeaderEdgeCases#test_file_path_equals_unknown_string().
  TestFullTableHeaderEdgeCases.test_python_file_header: FullTableHeaderEdgeCases#test_python_file_header().
  TestFullTableHeaderEdgeCases.test_js_file_header: FullTableHeaderEdgeCases#test_js_file_header().
  TestFullTableMultiClassParamTypes.test_multi_class_fields_section: FullTableMultiClassParamTypes#test_multi_class_fields_section().
  TestFormatClassDetails.test_class_with_fields: FormatClassDetails#test_class_with_fields().
  TestFormatClassDetails.test_class_with_fields_and_javadoc: FormatClassDetails#test_class_with_fields_and_javadoc().
  TestFormatClassDetails.test_class_with_constructors: FormatClassDetails#test_class_with_constructors().
  TestFormatClassDetails.test_class_with_constructors_and_javadoc: FormatClassDetails#test_class_with_constructors_and_javadoc().
  TestFormatClassDetails.test_class_with_protected_methods: FormatClassDetails#test_class_with_protected_methods().
  TestFormatClassDetails.test_class_with_package_methods: FormatClassDetails#test_class_with_package_methods().
  TestFormatClassDetails.test_class_with_private_methods: FormatClassDetails#test_class_with_private_methods().
  TestFormatClassDetails.test_class_empty_fields: FormatClassDetails#test_class_empty_fields().
  TestFormatClassDetails.test_class_empty_constructors: FormatClassDetails#test_class_empty_constructors().
  TestFormatClassDetails.test_all_visibility_groups: FormatClassDetails#test_all_visibility_groups().
  TestFormatClassDetails.test_public_methods_absent: FormatClassDetails#test_public_methods_absent().
  TestFormatClassDetails.test_include_javadoc_for_method: FormatClassDetails#test_include_javadoc_for_method().
  TestFullTableMultiClassParamTypes._make_multi_data: FullTableMultiClassParamTypes#_make_multi_data().
  TestPlatformNewlineWindows: PlatformNewlineWindows#
  TestFullTableHeaderEdgeCases: FullTableHeaderEdgeCases#
  TestFullTableMultiClassParamTypes: FullTableMultiClassParamTypes#
  TestFormatClassDetails: FormatClassDetails#
---
# Module: [`tests/unit/formatters/test_legacy_table_coverage_platform_header.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py)

## Classes
### `TestFormatClassDetails`
- def: [`tests/unit/formatters/test_legacy_table_coverage_platform_header.py:220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L220)
- doc: Tests for _format_class_details via direct invocation.
- signature: `class TestFormatClassDetails:`
- members:
  - `test_all_visibility_groups(self)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L419) — All four visibility method groups present.
  - `test_class_empty_constructors(self)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L410) — Line 496: when constructors list is empty, skip constructors.
  - `test_class_empty_fields(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L401) — Line 467: when class_fields is empty, skip fields section.
  - `test_class_with_constructors(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L277) — Lines 496-503: class with constructors section.
  - `test_class_with_constructors_and_javadoc(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L306) — Constructors with include_javadoc=True.
  - `test_class_with_fields(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L223) — Lines 467-487: class with fields section.
  - `test_class_with_fields_and_javadoc(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L256) — Lines 478-482: fields with include_javadoc=True.
  - `test_class_with_package_methods(self)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L359) — Lines 512-513, 522: package methods group.
  - `test_class_with_private_methods(self)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L380) — Lines 515-517, 523: private methods group.
  - `test_class_with_protected_methods(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L329) — Lines 509-510, 521: protected methods group.
  - `test_include_javadoc_for_method(self)` — [`L508`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L508) — Lines 544-548: method with include_javadoc=True.
  - `test_public_methods_absent(self)` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L487) — Line 525: public_methods empty, skip Public Methods.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_format_class_details`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._format_class_details)

### `TestFullTableHeaderEdgeCases`
- def: [`tests/unit/formatters/test_legacy_table_coverage_platform_header.py:45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L45)
- doc: Tests for _format_full_table header generation edge cases.
- signature: `class TestFullTableHeaderEdgeCases:`
- members:
  - `test_file_path_equals_unknown_string(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L69) — file_path == 'Unknown' should fall to default.
  - `test_js_file_header(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L90) — Test .js extension stripping in header.
  - `test_no_file_path_with_package(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L59) — Line 120: no file path + package -> package.Unknown.
  - `test_package_with_no_classes_and_file_path(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L48) — Line 114: package name + no classes + file path -> package.filename.
  - `test_python_file_header(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L79) — Test .py extension stripping in header.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestFullTableMultiClassParamTypes`
- def: [`tests/unit/formatters/test_legacy_table_coverage_platform_header.py:102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L102)
- doc: Tests for _format_full_table with multiple classes (param type branches).
- signature: `class TestFullTableMultiClassParamTypes:`
- members:
  - `test_fallback_parameter_non_dict_non_string(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L141) — Lines 246-247: fallback for non-dict non-string params. — documented in [tree_sitter_analyzer-legacy_table_formatter](../../../../concepts/tree_sitter_analyzer-legacy_table_formatter.md)
  - `test_mixed_param_types(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L158) — Mix of dict, string, and other params.
  - `test_multi_class_fields_section(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L181) — Lines 259-286: multi-class fields with static/final modifiers.
  - `test_string_parameter(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L124) — Lines 244-245: string parameters in multi-class path.
- protocol/private: `_make_multi_data`[`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L105)
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter.format_structure)

### `TestPlatformNewlineWindows`
- def: [`tests/unit/formatters/test_legacy_table_coverage_platform_header.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L27)
- doc: Tests for platform-specific newline on Windows (os.name == 'nt').
- signature: `class TestPlatformNewlineWindows:`
- members:
  - `test_convert_to_platform_newlines_on_windows(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L37) — Test _convert_to_platform_newlines converts \n to \r\n on Windows.
  - `test_get_platform_newline_windows(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_legacy_table_coverage_platform_header.py#L30) — Test _get_platform_newline returns \r\n on Windows.
- uses (calls/refs, reference-scoped): [`LegacyTableFormatter`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter), [`_convert_to_platform_newlines`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._convert_to_platform_newlines), [`_get_platform_newline`](../../../tree_sitter_analyzer/legacy_table_formatter.md#LegacyTableFormatter._get_platform_newline)

