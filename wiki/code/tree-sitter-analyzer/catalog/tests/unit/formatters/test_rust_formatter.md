---
title: 'Module: tests/unit/formatters/test_rust_formatter.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_rust_formatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_rust_formatter`/TestRustFormatter
symbols:
  TestRustFormatterSignaturesUnsupported.test_format_structure_signatures_raises_enumerable: SignaturesUnsupported#test_format_structure_signatures_raises_enumerable().
  TestRustFormatterInit.test_init_default: Init#test_init_default().
  TestRustFormatterInit.test_init_with_format_type: Init#test_init_with_format_type().
  TestRustFormatterFormatFullTable.test_format_full_with_modules: FormatFullTable#test_format_full_with_modules().
  TestRustFormatterFormatFullTable.test_format_full_with_structs: FormatFullTable#test_format_full_with_structs().
  TestRustFormatterFormatFullTable.test_format_full_with_impls: FormatFullTable#test_format_full_with_impls().
  TestRustFormatterFormatFullTable.test_format_full_with_functions: FormatFullTable#test_format_full_with_functions().
  TestRustFormatterFormatFullTable.test_full_table_has_complexity_column: FormatFullTable#test_full_table_has_complexity_column().
  TestRustFormatterFormatCompactTable.test_format_compact_with_modules: FormatCompactTable#test_format_compact_with_modules().
  TestRustFormatterFormatCompactTable.test_format_compact_with_functions: FormatCompactTable#test_format_compact_with_functions().
  TestRustFormatterFormatFnRow.test_format_fn_row_with_params: FormatFnRow#test_format_fn_row_with_params().
  TestRustFormatterFormatFnRow.test_format_fn_row_async: FormatFnRow#test_format_fn_row_async().
  TestRustFormatterCreateSignature.test_create_full_signature_with_params: CreateSignature#test_create_full_signature_with_params().
  TestRustFormatterCreateSignature.test_create_full_signature_no_return: CreateSignature#test_create_full_signature_no_return().
  TestRustFormatterCreateSignature.test_create_compact_signature: CreateSignature#test_create_compact_signature().
  TestRustFormatterConvertVisibility.test_convert_visibility_pub: ConvertVisibility#test_convert_visibility_pub().
  TestRustFormatterConvertVisibility.test_convert_visibility_pub_crate: ConvertVisibility#test_convert_visibility_pub_crate().
  TestRustFormatterConvertVisibility.test_convert_visibility_private: ConvertVisibility#test_convert_visibility_private().
  TestRustFormatterConvertVisibility.test_convert_visibility_unknown: ConvertVisibility#test_convert_visibility_unknown().
  TestRustFormatterFormatTable.test_format_table_full: FormatTable#test_format_table_full().
  TestRustFormatterFormatTable.test_format_table_compact: FormatTable#test_format_table_compact().
  TestRustFormatterFormatTable.test_format_table_json: FormatTable#test_format_table_json().
  TestRustFormatterFormatSummary.test_format_summary: FormatSummary#test_format_summary().
  TestRustFormatterFormatStructure.test_format_structure_full: FormatStructure#test_format_structure_full().
  TestRustFormatterFormatStructure.test_format_structure_compact: FormatStructure#test_format_structure_compact().
  TestRustFormatterFormatAdvanced.test_format_advanced_json: FormatAdvanced#test_format_advanced_json().
  TestRustFormatterFormatAdvanced.test_format_advanced_csv: FormatAdvanced#test_format_advanced_csv().
  TestRustFormatterFormatAdvanced.test_format_advanced_default: FormatAdvanced#test_format_advanced_default().
  TestRustFormatterFormatJson.test_format_json_valid_data: FormatJson#test_format_json_valid_data().
  TestRustFormatterFormatJson.test_format_json_invalid_data: FormatJson#test_format_json_invalid_data().
  TestRustFormatterParamDictLeak.test_format_rust_param_dict_self: ParamDictLeak#test_format_rust_param_dict_self().
  TestRustFormatterParamDictLeak.test_format_rust_param_dict_ref_self: ParamDictLeak#test_format_rust_param_dict_ref_self().
  TestRustFormatterParamDictLeak.test_format_rust_param_dict_mut_self: ParamDictLeak#test_format_rust_param_dict_mut_self().
  TestRustFormatterParamDictLeak.test_format_rust_param_dict_typed: ParamDictLeak#test_format_rust_param_dict_typed().
  TestRustFormatterParamDictLeak.test_format_rust_param_dict_i32: ParamDictLeak#test_format_rust_param_dict_i32().
  TestRustFormatterParamDictLeak.test_format_rust_param_string: ParamDictLeak#test_format_rust_param_string().
  TestRustFormatterParamDictLeak.test_create_full_signature_dict_params_no_leak: ParamDictLeak#test_create_full_signature_dict_params_no_leak().
  TestRustFormatterParamDictLeak.test_create_full_signature_add_dict_params: ParamDictLeak#test_create_full_signature_add_dict_params().
  TestRustFormatterParamDictLeak.test_format_full_table_dict_params_no_leak: ParamDictLeak#test_format_full_table_dict_params_no_leak().
  TestRustFormatterEdgeCases.test_empty_data: EdgeCases#test_empty_data().
  TestRustFormatterEdgeCases.test_windows_path: EdgeCases#test_windows_path().
  TestRustFormatterEdgeCases.test_unix_path: EdgeCases#test_unix_path().
  TestRustFormatterEdgeCases.test_long_function_signature: EdgeCases#test_long_function_signature().
  TestRustFormatterSignaturesUnsupported: SignaturesUnsupported#
  TestRustFormatterInit: Init#
  TestRustFormatterFormatFullTable: FormatFullTable#
  TestRustFormatterFormatCompactTable: FormatCompactTable#
  TestRustFormatterFormatFnRow: FormatFnRow#
  TestRustFormatterCreateSignature: CreateSignature#
  TestRustFormatterConvertVisibility: ConvertVisibility#
  TestRustFormatterFormatTable: FormatTable#
  TestRustFormatterFormatSummary: FormatSummary#
  TestRustFormatterFormatStructure: FormatStructure#
  TestRustFormatterFormatAdvanced: FormatAdvanced#
  TestRustFormatterFormatJson: FormatJson#
  TestRustFormatterParamDictLeak: ParamDictLeak#
  TestRustFormatterEdgeCases: EdgeCases#
---
# Module: [`tests/unit/formatters/test_rust_formatter.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py)

## Classes
### `TestRustFormatterConvertVisibility`
- def: [`tests/unit/formatters/test_rust_formatter.py:295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L295)
- doc: Test visibility conversion
- signature: `class TestRustFormatterConvertVisibility:`
- members:
  - `test_convert_visibility_private(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L310) — Test converting private visibility
  - `test_convert_visibility_pub(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L298) — Test converting pub visibility
  - `test_convert_visibility_pub_crate(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L304) — Test converting pub(crate) visibility
  - `test_convert_visibility_unknown(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L316) — Test converting unknown visibility
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`_convert_visibility`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._convert_visibility)

### `TestRustFormatterCreateSignature`
- def: [`tests/unit/formatters/test_rust_formatter.py:257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L257)
- doc: Test signature creation
- signature: `class TestRustFormatterCreateSignature:`
- members:
  - `test_create_compact_signature(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L283) — Test creating compact signature
  - `test_create_full_signature_no_return(self)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L271) — Test creating full signature without return type
  - `test_create_full_signature_with_params(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L260) — Test creating full signature with parameters
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`_create_full_signature`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._create_full_signature), [`_create_compact_signature`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._create_compact_signature)

### `TestRustFormatterEdgeCases`
- def: [`tests/unit/formatters/test_rust_formatter.py:586`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L586)
- doc: Test edge cases
- signature: `class TestRustFormatterEdgeCases:`
- members:
  - `test_empty_data(self)` — [`L589`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L589) — Test with empty data
  - `test_long_function_signature(self)` — [`L628`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L628) — Test with long function signature
  - `test_unix_path(self)` — [`L615`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L615) — Test with Unix file path
  - `test_windows_path(self)` — [`L602`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L602) — Test with Windows file path
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`_format_fn_row`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._format_fn_row), [`format_structure`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter.format_structure)

### `TestRustFormatterFormatAdvanced`
- def: [`tests/unit/formatters/test_rust_formatter.py:407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L407)
- doc: Test format_advanced method
- signature: `class TestRustFormatterFormatAdvanced:`
- members:
  - `test_format_advanced_csv(self)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L418) — Test format_advanced with CSV output
  - `test_format_advanced_default(self)` — [`L431`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L431) — Test format_advanced with default output
  - `test_format_advanced_json(self)` — [`L410`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L410) — Test format_advanced with JSON output
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`format_advanced`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter.format_advanced)

### `TestRustFormatterFormatCompactTable`
- def: [`tests/unit/formatters/test_rust_formatter.py:185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L185)
- doc: Test compact table format for Rust
- signature: `class TestRustFormatterFormatCompactTable:`
- members:
  - `test_format_compact_with_functions(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L202) — Test compact format with functions
  - `test_format_compact_with_modules(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L188) — Test compact format with modules
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`_format_compact_table`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._format_compact_table)

### `TestRustFormatterFormatFnRow`
- def: [`tests/unit/formatters/test_rust_formatter.py:223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L223)
- doc: Test function row formatting
- signature: `class TestRustFormatterFormatFnRow:`
- members:
  - `test_format_fn_row_async(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L242) — Test formatting async function
  - `test_format_fn_row_with_params(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L226) — Test formatting function with parameters
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`_format_fn_row`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._format_fn_row)

### `TestRustFormatterFormatFullTable`
- def: [`tests/unit/formatters/test_rust_formatter.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L42)
- doc: Test full table format for Rust
- signature: `class TestRustFormatterFormatFullTable:`
- members:
  - `test_format_full_with_functions(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L122) — Test formatting with functions
  - `test_format_full_with_impls(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L95) — Test formatting with impl blocks
  - `test_format_full_with_modules(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L45) — Test formatting with modules
  - `test_format_full_with_structs(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L65) — Test formatting with structs
  - `test_full_table_has_complexity_column(self)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L156) — The full Functions table must expose a Cx column with the computed
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._format_full_table)

### `TestRustFormatterFormatJson`
- def: [`tests/unit/formatters/test_rust_formatter.py:445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L445)
- doc: Test _format_json method
- signature: `class TestRustFormatterFormatJson:`
- members:
  - `test_format_json_invalid_data(self)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L456) — Test formatting invalid JSON data
  - `test_format_json_valid_data(self)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L448) — Test formatting valid JSON data
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`_format_json`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._format_json)

### `TestRustFormatterFormatStructure`
- def: [`tests/unit/formatters/test_rust_formatter.py:377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L377)
- doc: Test format_structure method
- signature: `class TestRustFormatterFormatStructure:`
- members:
  - `test_format_structure_compact(self)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L394) — Test format_structure with compact type
  - `test_format_structure_full(self)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L380) — Test format_structure with full type
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter.format_structure)

### `TestRustFormatterFormatSummary`
- def: [`tests/unit/formatters/test_rust_formatter.py:361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L361)
- doc: Test format_summary method
- signature: `class TestRustFormatterFormatSummary:`
- members:
  - `test_format_summary(self)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L364) — Test format_summary method
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`format_summary`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter.format_summary)

### `TestRustFormatterFormatTable`
- def: [`tests/unit/formatters/test_rust_formatter.py:323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L323)
- doc: Test format_table method
- signature: `class TestRustFormatterFormatTable:`
- members:
  - `test_format_table_compact(self)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L340) — Test format_table with compact type
  - `test_format_table_full(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L326) — Test format_table with full type
  - `test_format_table_json(self)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L352) — Test format_table with JSON type
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`format_table`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter.format_table)

### `TestRustFormatterInit`
- def: [`tests/unit/formatters/test_rust_formatter.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L27)
- doc: Test RustTableFormatter initialization
- signature: `class TestRustFormatterInit:`
- members:
  - `test_init_default(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L30) — Test default initialization
  - `test_init_with_format_type(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L36) — Test initialization with format type
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`format_type`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter.format_type)

### `TestRustFormatterParamDictLeak`
- def: [`tests/unit/formatters/test_rust_formatter.py:468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L468)
- doc: Regression tests: parameters must never render as raw Python dicts.
- signature: `class TestRustFormatterParamDictLeak:`
- members:
  - `test_create_full_signature_add_dict_params(self)` — [`L532`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L532) — fn(a: i32, b: i32) -> i32 from dict params.
  - `test_create_full_signature_dict_params_no_leak(self)` — [`L517`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L517) — Full signature with dict params must not contain literal braces.
  - `test_format_full_table_dict_params_no_leak(self)` — [`L547`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L547) — Full table output must not contain raw dict reprs in any row.
  - `test_format_rust_param_dict_i32(self)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L504) — Typed param with primitive type renders correctly.
  - `test_format_rust_param_dict_mut_self(self)` — [`L490`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L490) — &mut self param as dict renders as '&mut self'.
  - `test_format_rust_param_dict_ref_self(self)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L483) — &self param as dict renders as '&self'.
  - `test_format_rust_param_dict_self(self)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L476) — self param as dict renders as bare 'self' (Rust convention).
  - `test_format_rust_param_dict_typed(self)` — [`L497`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L497) — Typed param renders as 'name: type'.
  - `test_format_rust_param_string(self)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L511) — String params (already formatted) pass through unchanged.
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`_format_full_table`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._format_full_table), [`_format_rust_param`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._format_rust_param), [`_create_full_signature`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter._create_full_signature)

### `TestRustFormatterSignaturesUnsupported`
- def: [`tests/unit/formatters/test_rust_formatter.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L11)
- doc: Rust does not support the signatures directory mode; it must raise the
- signature: `class TestRustFormatterSignaturesUnsupported:`
- members:
  - `test_format_structure_signatures_raises_enumerable(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_rust_formatter.py#L16)
- uses (calls/refs, reference-scoped): [`RustTableFormatter`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter), [`format_structure`](../../../tree_sitter_analyzer/formatters/rust_formatter.md#RustTableFormatter.format_structure)

