---
title: 'Module: tests/unit/formatters/test_kotlin_formatter.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_kotlin_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_kotlin_formatter`/TestKotlinF
symbols:
  TestKotlinFormatterSignaturesUnsupported.test_format_structure_signatures_raises_enumerable: ormatterSignaturesUnsupported#test_format_structure_signatures_raises_enumerable().
  TestKotlinFormatterInit.test_init_default: ormatterInit#test_init_default().
  TestKotlinFormatterInit.test_init_with_format_type: ormatterInit#test_init_with_format_type().
  TestKotlinFormatterFormatFullTable.test_format_full_with_package: ormatterFormatFullTable#test_format_full_with_package().
  TestKotlinFormatterFormatFullTable.test_format_full_without_package: ormatterFormatFullTable#test_format_full_without_package().
  TestKotlinFormatterFormatFullTable.test_format_full_with_imports: ormatterFormatFullTable#test_format_full_with_imports().
  TestKotlinFormatterFormatFullTable.test_format_full_with_classes: ormatterFormatFullTable#test_format_full_with_classes().
  TestKotlinFormatterFormatFullTable.test_format_full_with_functions: ormatterFormatFullTable#test_format_full_with_functions().
  TestKotlinFormatterFormatFullTable.test_format_full_with_properties: ormatterFormatFullTable#test_format_full_with_properties().
  TestKotlinFormatterFormatCompactTable.test_format_compact_with_package: ormatterFormatCompactTable#test_format_compact_with_package().
  TestKotlinFormatterFormatCompactTable.test_format_compact_with_functions: ormatterFormatCompactTable#test_format_compact_with_functions().
  TestKotlinFormatterFormatFnRow.test_format_fn_row_with_params: ormatterFormatFnRow#test_format_fn_row_with_params().
  TestKotlinFormatterFormatFnRow.test_format_fn_row_suspend: ormatterFormatFnRow#test_format_fn_row_suspend().
  TestKotlinFormatterFormatPropRow.test_format_prop_row_val: ormatterFormatPropRow#test_format_prop_row_val().
  TestKotlinFormatterFormatPropRow.test_format_prop_row_var: ormatterFormatPropRow#test_format_prop_row_var().
  TestKotlinFormatterCreateSignature.test_create_full_signature_with_params: ormatterCreateSignature#test_create_full_signature_with_params().
  TestKotlinFormatterCreateSignature.test_create_full_signature_no_return: ormatterCreateSignature#test_create_full_signature_no_return().
  TestKotlinFormatterCreateSignature.test_create_compact_signature: ormatterCreateSignature#test_create_compact_signature().
  TestKotlinFormatterConvertVisibility.test_convert_visibility_public: ormatterConvertVisibility#test_convert_visibility_public().
  TestKotlinFormatterConvertVisibility.test_convert_visibility_private: ormatterConvertVisibility#test_convert_visibility_private().
  TestKotlinFormatterConvertVisibility.test_convert_visibility_protected: ormatterConvertVisibility#test_convert_visibility_protected().
  TestKotlinFormatterConvertVisibility.test_convert_visibility_internal: ormatterConvertVisibility#test_convert_visibility_internal().
  TestKotlinFormatterConvertVisibility.test_convert_visibility_unknown: ormatterConvertVisibility#test_convert_visibility_unknown().
  TestKotlinFormatterFormatTable.test_format_table_full: ormatterFormatTable#test_format_table_full().
  TestKotlinFormatterFormatTable.test_format_table_compact: ormatterFormatTable#test_format_table_compact().
  TestKotlinFormatterFormatTable.test_format_table_json: ormatterFormatTable#test_format_table_json().
  TestKotlinFormatterFormatSummary.test_format_summary: ormatterFormatSummary#test_format_summary().
  TestKotlinFormatterFormatStructure.test_format_structure_full: ormatterFormatStructure#test_format_structure_full().
  TestKotlinFormatterFormatStructure.test_format_structure_compact: ormatterFormatStructure#test_format_structure_compact().
  TestKotlinFormatterFormatAdvanced.test_format_advanced_json: ormatterFormatAdvanced#test_format_advanced_json().
  TestKotlinFormatterFormatAdvanced.test_format_advanced_csv: ormatterFormatAdvanced#test_format_advanced_csv().
  TestKotlinFormatterFormatAdvanced.test_format_advanced_default: ormatterFormatAdvanced#test_format_advanced_default().
  TestKotlinFormatterFormatJson.test_format_json_valid_data: ormatterFormatJson#test_format_json_valid_data().
  TestKotlinFormatterFormatJson.test_format_json_invalid_data: ormatterFormatJson#test_format_json_invalid_data().
  TestKotlinFormatterEdgeCases.test_empty_data: ormatterEdgeCases#test_empty_data().
  TestKotlinFormatterEdgeCases.test_windows_path: ormatterEdgeCases#test_windows_path().
  TestKotlinFormatterEdgeCases.test_unix_path: ormatterEdgeCases#test_unix_path().
  TestKotlinFormatterEdgeCases.test_long_function_signature: ormatterEdgeCases#test_long_function_signature().
  TestKotlinFullTableComplexityColumn.test_full_table_has_cx_column_with_value: ullTableComplexityColumn#test_full_table_has_cx_column_with_value().
  TestKotlinFormatterSignaturesUnsupported: ormatterSignaturesUnsupported#
  TestKotlinFormatterInit: ormatterInit#
  TestKotlinFormatterFormatFullTable: ormatterFormatFullTable#
  TestKotlinFormatterFormatCompactTable: ormatterFormatCompactTable#
  TestKotlinFormatterFormatFnRow: ormatterFormatFnRow#
  TestKotlinFormatterFormatPropRow: ormatterFormatPropRow#
  TestKotlinFormatterCreateSignature: ormatterCreateSignature#
  TestKotlinFormatterConvertVisibility: ormatterConvertVisibility#
  TestKotlinFormatterFormatTable: ormatterFormatTable#
  TestKotlinFormatterFormatSummary: ormatterFormatSummary#
  TestKotlinFormatterFormatStructure: ormatterFormatStructure#
  TestKotlinFormatterFormatAdvanced: ormatterFormatAdvanced#
  TestKotlinFormatterFormatJson: ormatterFormatJson#
  TestKotlinFormatterEdgeCases: ormatterEdgeCases#
  TestKotlinFullTableComplexityColumn: ullTableComplexityColumn#
---
# Module: [`tests/unit/formatters/test_kotlin_formatter.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py)

## Classes
### `TestKotlinFormatterConvertVisibility`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L342)
- doc: Test visibility conversion
- signature: `class TestKotlinFormatterConvertVisibility:`
- members:
  - `test_convert_visibility_internal(self)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L363) — Test converting internal visibility
  - `test_convert_visibility_private(self)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L351) — Test converting private visibility
  - `test_convert_visibility_protected(self)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L357) — Test converting protected visibility
  - `test_convert_visibility_public(self)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L345) — Test converting public visibility
  - `test_convert_visibility_unknown(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L369) — Test converting unknown visibility
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`_convert_visibility`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter._convert_visibility)

### `TestKotlinFormatterCreateSignature`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L298)
- doc: Test signature creation
- signature: `class TestKotlinFormatterCreateSignature:`
- members:
  - `test_create_compact_signature(self)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L327) — Test creating compact signature
  - `test_create_full_signature_no_return(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L315) — Test creating full signature without return type
  - `test_create_full_signature_with_params(self)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L301) — Test creating full signature with parameters
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`_create_full_signature`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter._create_full_signature), [`_create_compact_signature`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter._create_compact_signature)

### `TestKotlinFormatterEdgeCases`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L519)
- doc: Test edge cases
- signature: `class TestKotlinFormatterEdgeCases:`
- members:
  - `test_empty_data(self)` — [`L522`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L522) — Test with empty data
  - `test_long_function_signature(self)` — [`L561`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L561) — Test with long function signature
  - `test_unix_path(self)` — [`L548`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L548) — Test with Unix file path
  - `test_windows_path(self)` — [`L535`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L535) — Test with Windows file path
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`_format_fn_row`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter._format_fn_row), [`format_structure`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter.format_structure)

### `TestKotlinFormatterFormatAdvanced`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:460`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L460)
- doc: Test format_advanced method
- signature: `class TestKotlinFormatterFormatAdvanced:`
- members:
  - `test_format_advanced_csv(self)` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L471) — Test format_advanced with CSV output
  - `test_format_advanced_default(self)` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L484) — Test format_advanced with default output
  - `test_format_advanced_json(self)` — [`L463`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L463) — Test format_advanced with JSON output
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`format_advanced`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter.format_advanced)

### `TestKotlinFormatterFormatCompactTable`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L189)
- doc: Test compact table format for Kotlin
- signature: `class TestKotlinFormatterFormatCompactTable:`
- members:
  - `test_format_compact_with_functions(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L206) — Test compact format with functions
  - `test_format_compact_with_package(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L192) — Test compact format with package
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`_format_compact_table`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter._format_compact_table)

### `TestKotlinFormatterFormatFnRow`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L227)
- doc: Test function row formatting
- signature: `class TestKotlinFormatterFormatFnRow:`
- members:
  - `test_format_fn_row_suspend(self)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L249) — Test formatting suspend function
  - `test_format_fn_row_with_params(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L230) — Test formatting function with parameters
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`_format_fn_row`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter._format_fn_row)

### `TestKotlinFormatterFormatFullTable`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L42)
- doc: Test full table format for Kotlin
- signature: `class TestKotlinFormatterFormatFullTable:`
- members:
  - `test_format_full_with_classes(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L90) — Test formatting with classes
  - `test_format_full_with_functions(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L120) — Test formatting with functions
  - `test_format_full_with_imports(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L72) — Test formatting with imports
  - `test_format_full_with_package(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L45) — Test formatting with package name
  - `test_format_full_with_properties(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L154) — Test formatting with properties
  - `test_format_full_without_package(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L59) — Test formatting without package name
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter._format_full_table)

### `TestKotlinFormatterFormatJson`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:498`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L498)
- doc: Test _format_json method
- signature: `class TestKotlinFormatterFormatJson:`
- members:
  - `test_format_json_invalid_data(self)` — [`L509`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L509) — Test formatting invalid JSON data
  - `test_format_json_valid_data(self)` — [`L501`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L501) — Test formatting valid JSON data
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`_format_json`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter._format_json)

### `TestKotlinFormatterFormatPropRow`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L264)
- doc: Test property row formatting
- signature: `class TestKotlinFormatterFormatPropRow:`
- members:
  - `test_format_prop_row_val(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L267) — Test formatting val property
  - `test_format_prop_row_var(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L282) — Test formatting var property
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`_format_prop_row`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter._format_prop_row)

### `TestKotlinFormatterFormatStructure`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L430)
- doc: Test format_structure method
- signature: `class TestKotlinFormatterFormatStructure:`
- members:
  - `test_format_structure_compact(self)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L447) — Test format_structure with compact type
  - `test_format_structure_full(self)` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L433) — Test format_structure with full type
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter.format_structure)

### `TestKotlinFormatterFormatSummary`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L414)
- doc: Test format_summary method
- signature: `class TestKotlinFormatterFormatSummary:`
- members:
  - `test_format_summary(self)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L417) — Test format_summary method
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`format_summary`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter.format_summary)

### `TestKotlinFormatterFormatTable`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L376)
- doc: Test format_table method
- signature: `class TestKotlinFormatterFormatTable:`
- members:
  - `test_format_table_compact(self)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L393) — Test format_table with compact type
  - `test_format_table_full(self)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L379) — Test format_table with full type
  - `test_format_table_json(self)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L405) — Test format_table with JSON type
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter.format_table)

### `TestKotlinFormatterInit`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L27)
- doc: Test KotlinTableFormatter initialization
- signature: `class TestKotlinFormatterInit:`
- members:
  - `test_init_default(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L30) — Test default initialization
  - `test_init_with_format_type(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L36) — Test initialization with format type
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`format_type`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter.format_type)

### `TestKotlinFormatterSignaturesUnsupported`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L11)
- doc: Kotlin does not support the signatures directory mode; it must raise the
- signature: `class TestKotlinFormatterSignaturesUnsupported:`
- members:
  - `test_format_structure_signatures_raises_enumerable(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L16)
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter.format_structure)

### `TestKotlinFullTableComplexityColumn`
- def: [`tests/unit/formatters/test_kotlin_formatter.py:579`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L579)
- doc: The full table shows a Cx (cyclomatic complexity) column, matching the
- signature: `class TestKotlinFullTableComplexityColumn:`
- members:
  - `test_full_table_has_cx_column_with_value(self)` — [`L583`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_kotlin_formatter.py#L583)
- uses (calls/refs, reference-scoped): [`KotlinTableFormatter`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/kotlin_formatter.md#KotlinTableFormatter._format_full_table)

