---
title: 'Module: tests/unit/formatters/test_toon_encoder.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_toon_encoder.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_toon_encoder`/TestToonEncode
symbols:
  TestToonEncoderInit.test_init_default: rInit#test_init_default().
  TestToonEncodeError.test_init_basic: Error#test_init_basic().
  TestToonEncodeError.test_init_with_data: Error#test_init_with_data().
  TestToonEncodeError.test_init_with_cause: Error#test_init_with_cause().
  TestToonEncoderInit.test_init_with_tabs: rInit#test_init_with_tabs().
  TestToonEncoderErrorHandling.test_fallback_to_json_on_error: rErrorHandling#test_fallback_to_json_on_error().
  TestToonEncoderErrorHandling.test_no_fallback_raises_error: rErrorHandling#test_no_fallback_raises_error().
  TestToonEncoderErrorHandling.test_encode_safe_always_returns_string: rErrorHandling#test_encode_safe_always_returns_string().
  TestToonEncoderEdgeCases.test_encode_max_depth_exceeded: rEdgeCases#test_encode_max_depth_exceeded().
  TestToonEncoderInit.test_init_without_fallback: rInit#test_init_without_fallback().
  TestToonEncoderInit.test_init_custom_max_depth: rInit#test_init_custom_max_depth().
  TestToonEncoderInit.test_init_without_path_normalization: rInit#test_init_without_path_normalization().
  TestToonEncoderEncodePrimitive.test_encode_none: rEncodePrimitive#test_encode_none().
  TestToonEncoderEncodePrimitive.test_encode_bool_true: rEncodePrimitive#test_encode_bool_true().
  TestToonEncoderEncodePrimitive.test_encode_bool_false: rEncodePrimitive#test_encode_bool_false().
  TestToonEncoderEncodePrimitive.test_encode_int: rEncodePrimitive#test_encode_int().
  TestToonEncoderEncodePrimitive.test_encode_float: rEncodePrimitive#test_encode_float().
  TestToonEncoderEncodePrimitive.test_encode_string_simple: rEncodePrimitive#test_encode_string_simple().
  TestToonEncoderEncodePrimitive.test_encode_string_with_special_chars: rEncodePrimitive#test_encode_string_with_special_chars().
  TestToonEncoderEncodeDict.test_encode_empty_dict: rEncodeDict#test_encode_empty_dict().
  TestToonEncoderEncodeDict.test_encode_simple_dict: rEncodeDict#test_encode_simple_dict().
  TestToonEncoderEncodeDict.test_encode_nested_dict: rEncodeDict#test_encode_nested_dict().
  TestToonEncoderEncodeDict.test_encode_dict_with_list: rEncodeDict#test_encode_dict_with_list().
  TestToonEncoderEncodeList.test_encode_empty_list: rEncodeList#test_encode_empty_list().
  TestToonEncoderEncodeList.test_encode_simple_list: rEncodeList#test_encode_simple_list().
  TestToonEncoderEncodeList.test_encode_list_with_tabs: rEncodeList#test_encode_list_with_tabs().
  TestToonEncoderEncodeList.test_encode_nested_list: rEncodeList#test_encode_nested_list().
  TestToonEncoderEncodeArrayTable.test_encode_homogeneous_dict_array: rEncodeArrayTable#test_encode_homogeneous_dict_array().
  TestToonEncoderEncodeArrayTable.test_encode_empty_array_table: rEncodeArrayTable#test_encode_empty_array_table().
  TestToonEncoderEncodeArrayTable.test_encode_array_table_with_tabs: rEncodeArrayTable#test_encode_array_table_with_tabs().
  TestToonEncoderEncodeString.test_encode_string_with_newline: rEncodeString#test_encode_string_with_newline().
  TestToonEncoderEncodeString.test_encode_string_with_tab: rEncodeString#test_encode_string_with_tab().
  TestToonEncoderEncodeString.test_encode_string_with_backslash: rEncodeString#test_encode_string_with_backslash().
  TestToonEncoderEncodeString.test_encode_string_with_quote: rEncodeString#test_encode_string_with_quote().
  TestToonEncoderEncodeString.test_encode_string_with_braces: rEncodeString#test_encode_string_with_braces().
  TestToonEncoderNormalizePath.test_normalize_windows_path_drive_letter: rNormalizePath#test_normalize_windows_path_drive_letter().
  TestToonEncoderNormalizePath.test_normalize_unc_path: rNormalizePath#test_normalize_unc_path().
  TestToonEncoderNormalizePath.test_normalize_relative_path: rNormalizePath#test_normalize_relative_path().
  TestToonEncoderNormalizePath.test_normalize_parent_path: rNormalizePath#test_normalize_parent_path().
  TestToonEncoderNormalizePath.test_no_normalize_non_path_string: rNormalizePath#test_no_normalize_non_path_string().
  TestToonEncoderNormalizePath.test_no_normalize_when_disabled: rNormalizePath#test_no_normalize_when_disabled().
  TestToonEncoderCircularReference.test_detect_circular_reference_in_dict: rCircularReference#test_detect_circular_reference_in_dict().
  TestToonEncoderCircularReference.test_detect_circular_reference_in_list: rCircularReference#test_detect_circular_reference_in_list().
  TestToonEncoderCircularReference.test_detect_circular_reference_static_method: rCircularReference#test_detect_circular_reference_static_method().
  TestToonEncoderCircularReference.test_no_circular_reference: rCircularReference#test_no_circular_reference().
  TestToonEncoderEdgeCases.test_encode_with_indent: rEdgeCases#test_encode_with_indent().
  TestToonEncoderEdgeCases.test_encode_dict_in_list: rEdgeCases#test_encode_dict_in_list().
  TestToonEncoderEdgeCases.test_encode_list_in_dict: rEdgeCases#test_encode_list_in_dict().
  TestToonEncoderConvenienceMethods.test_encode_dict_method: rConvenienceMethods#test_encode_dict_method().
  TestToonEncoderConvenienceMethods.test_encode_list_method: rConvenienceMethods#test_encode_list_method().
  TestToonEncoderConvenienceMethods.test_encode_array_header_simple: rConvenienceMethods#test_encode_array_header_simple().
  TestToonEncoderConvenienceMethods.test_encode_array_header_with_schema: rConvenienceMethods#test_encode_array_header_with_schema().
  TestToonEncoderConvenienceMethods.test_encode_array_table_method: rConvenienceMethods#test_encode_array_table_method().
  TestToonEncoderCompactFormats.test_encode_tuple_in_array_table: rCompactFormats#test_encode_tuple_in_array_table().
  TestToonEncoderCompactFormats.test_encode_dict_in_array_table: rCompactFormats#test_encode_dict_in_array_table().
  TestToonEncoderEncodeValue.test_encode_value_none: rEncodeValue#test_encode_value_none().
  TestToonEncoderEncodeValue.test_encode_value_bool: rEncodeValue#test_encode_value_bool().
  TestToonEncoderEncodeValue.test_encode_value_number: rEncodeValue#test_encode_value_number().
  TestToonEncoderEncodeValue.test_encode_value_string: rEncodeValue#test_encode_value_string().
  TestToonEncoderEncodeValue.test_encode_value_dict_inline: rEncodeValue#test_encode_value_dict_inline().
  TestToonEncoderEncodeValue.test_encode_value_list_inline: rEncodeValue#test_encode_value_list_inline().
  TestToonEncoderInferSchema.test_infer_schema_from_items: rInferSchema#test_infer_schema_from_items().
  TestToonEncoderInferSchema.test_infer_schema_empty: rInferSchema#test_infer_schema_empty().
  TestToonEncoderEncodeInlineDict.test_encode_inline_dict_simple: rEncodeInlineDict#test_encode_inline_dict_simple().
  TestToonEncoderEncodeInlineDict.test_encode_inline_dict_empty: rEncodeInlineDict#test_encode_inline_dict_empty().
  TestToonEncoderEncodeInlineDict.test_encode_inline_dict_nested: rEncodeInlineDict#test_encode_inline_dict_nested().
  TestToonEncoderEncodeSimpleList.test_encode_simple_list_empty: rEncodeSimpleList#test_encode_simple_list_empty().
  TestToonEncoderEncodeSimpleList.test_encode_simple_list_primitives: rEncodeSimpleList#test_encode_simple_list_primitives().
  TestToonEncoderEncodeSimpleList.test_encode_simple_list_nested: rEncodeSimpleList#test_encode_simple_list_nested().
  TestToonEncoderComplexStructures.test_encode_deeply_nested_dict: rComplexStructures#test_encode_deeply_nested_dict().
  TestToonEncoderComplexStructures.test_encode_mixed_structure: rComplexStructures#test_encode_mixed_structure().
  TestToonEncoderSpecialCharacters.test_encode_string_with_colon: rSpecialCharacters#test_encode_string_with_colon().
  TestToonEncoderSpecialCharacters.test_encode_string_with_brackets: rSpecialCharacters#test_encode_string_with_brackets().
  TestToonEncoderSpecialCharacters.test_encode_string_with_carriage_return: rSpecialCharacters#test_encode_string_with_carriage_return().
  TestToonEncoderSpecialCharacters.test_encode_string_with_all_special_chars: rSpecialCharacters#test_encode_string_with_all_special_chars().
  TestToonEncoderLongFlatStringList.test_long_path_list_renders_as_array_table: rLongFlatStringList#test_long_path_list_renders_as_array_table().
  TestToonEncoderLongFlatStringList.test_short_path_list_stays_inline: rLongFlatStringList#test_short_path_list_stays_inline().
  TestToonEncoderLongFlatStringList.test_threshold_boundary_inclusive_at_five: rLongFlatStringList#test_threshold_boundary_inclusive_at_five().
  TestToonEncoderLongFlatStringList.test_threshold_boundary_table_at_six: rLongFlatStringList#test_threshold_boundary_table_at_six().
  TestToonEncoderLongFlatStringList.test_mixed_list_str_and_dict_unchanged: rLongFlatStringList#test_mixed_list_str_and_dict_unchanged().
  TestToonEncoderLongFlatStringList.test_non_string_list_falls_back_to_inline: rLongFlatStringList#test_non_string_list_falls_back_to_inline().
  TestToonEncoderLongFlatStringList.test_column_name_picked_from_key_suffix: rLongFlatStringList#test_column_name_picked_from_key_suffix().
  TestToonEncoderLongFlatStringList.test_column_name_falls_back_to_item: rLongFlatStringList#test_column_name_falls_back_to_item().
  TestToonEncoderLongFlatStringList.test_empty_string_list_stays_empty: rLongFlatStringList#test_empty_string_list_stays_empty().
  TestToonEncodeError.test_str_basic: Error#test_str_basic().
  TestToonEncodeError.test_str_with_cause: Error#test_str_with_cause().
  TestToonEncoderErrorHandling.test_fallback_to_json_on_error.CustomObject: rErrorHandling#test_fallback_to_json_on_error().CustomObject#
  TestToonEncoderErrorHandling.test_encode_safe_always_returns_string.CustomObject: rErrorHandling#test_encode_safe_always_returns_string().CustomObject#
  TestToonEncodeError: Error#
  TestToonEncoderInit: rInit#
  TestToonEncoderEncodePrimitive: rEncodePrimitive#
  TestToonEncoderEncodeDict: rEncodeDict#
  TestToonEncoderEncodeList: rEncodeList#
  TestToonEncoderEncodeArrayTable: rEncodeArrayTable#
  TestToonEncoderEncodeString: rEncodeString#
  TestToonEncoderNormalizePath: rNormalizePath#
  TestToonEncoderCircularReference: rCircularReference#
  TestToonEncoderErrorHandling: rErrorHandling#
  TestToonEncoderEdgeCases: rEdgeCases#
  TestToonEncoderConvenienceMethods: rConvenienceMethods#
  TestToonEncoderCompactFormats: rCompactFormats#
  TestToonEncoderEncodeValue: rEncodeValue#
  TestToonEncoderInferSchema: rInferSchema#
  TestToonEncoderEncodeInlineDict: rEncodeInlineDict#
  TestToonEncoderEncodeSimpleList: rEncodeSimpleList#
  TestToonEncoderComplexStructures: rComplexStructures#
  TestToonEncoderSpecialCharacters: rSpecialCharacters#
  TestToonEncoderLongFlatStringList: rLongFlatStringList#
---
# Module: [`tests/unit/formatters/test_toon_encoder.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py)

## Classes
### `CustomObject`
- def: [`tests/unit/formatters/test_toon_encoder.py:383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L383)
- signature: `class CustomObject:`
- used by: (1 test-only callers)

### `TestToonEncodeError`
- def: [`tests/unit/formatters/test_toon_encoder.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L16)
- doc: Tests for ToonEncodeError exception class.
- signature: `class TestToonEncodeError:`
- members:
  - `test_init_basic(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L19) — Test basic initialization of ToonEncodeError.
  - `test_init_with_cause(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L32) — Test initialization with cause exception.
  - `test_init_with_data(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L26) — Test initialization with data.
  - `test_str_basic(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L39) — Test string representation without cause.
  - `test_str_with_cause(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L44) — Test string representation with cause.
- uses (calls/refs, reference-scoped): [`ToonEncodeError`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError), [`cause`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError.cause), [`message`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError.message), [`data`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError.data)

### `TestToonEncoderCircularReference`
- def: [`tests/unit/formatters/test_toon_encoder.py:313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L313)
- doc: Tests for circular reference detection.
- signature: `class TestToonEncoderCircularReference:`
- members:
  - `test_detect_circular_reference_in_dict(self)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L316) — Test graceful degradation for circular reference in dictionary.
  - `test_detect_circular_reference_in_list(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L326) — Test graceful degradation for circular reference in list.
  - `test_detect_circular_reference_static_method(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L336) — Test static method for circular reference detection.
  - `test_no_circular_reference(self)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L344) — Test that non-circular structures are not flagged.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode), [`detect_circular_reference`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.detect_circular_reference)

### `TestToonEncoderCompactFormats`
- def: [`tests/unit/formatters/test_toon_encoder.py:470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L470)
- doc: Tests for compact format features.
- signature: `class TestToonEncoderCompactFormats:`
- members:
  - `test_encode_dict_in_array_table(self)` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L484) — Test encoding dict values in array table.
  - `test_encode_tuple_in_array_table(self)` — [`L473`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L473) — Test encoding tuple values in array table.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

### `TestToonEncoderComplexStructures`
- def: [`tests/unit/formatters/test_toon_encoder.py:600`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L600)
- doc: Tests for complex nested structures.
- signature: `class TestToonEncoderComplexStructures:`
- members:
  - `test_encode_deeply_nested_dict(self)` — [`L603`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L603) — Test encoding deeply nested dictionary.
  - `test_encode_mixed_structure(self)` — [`L614`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L614) — Test encoding mixed structure with dicts and lists.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

### `TestToonEncoderConvenienceMethods`
- def: [`tests/unit/formatters/test_toon_encoder.py:432`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L432)
- doc: Tests for convenience methods.
- signature: `class TestToonEncoderConvenienceMethods:`
- members:
  - `test_encode_array_header_simple(self)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L447) — Test encode_array_header without schema.
  - `test_encode_array_header_with_schema(self)` — [`L453`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L453) — Test encode_array_header with schema.
  - `test_encode_array_table_method(self)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L459) — Test encode_array_table convenience method.
  - `test_encode_dict_method(self)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L435) — Test encode_dict convenience method.
  - `test_encode_list_method(self)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L441) — Test encode_list convenience method.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode_array_table`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode_array_table), [`encode_dict`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode_dict), [`encode_array_header`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode_array_header), [`encode_list`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode_list)

### `TestToonEncoderEdgeCases`
- def: [`tests/unit/formatters/test_toon_encoder.py:391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L391)
- doc: Tests for edge cases and special scenarios.
- signature: `class TestToonEncoderEdgeCases:`
- members:
  - `test_encode_dict_in_list(self)` — [`L417`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L417) — Test encoding dict inside list.
  - `test_encode_list_in_dict(self)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L425) — Test encoding list inside dict.
  - `test_encode_max_depth_exceeded(self)` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L402) — Test that max depth limit is enforced. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `test_encode_with_indent(self)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L394) — Test encoding with indentation.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode), [`ToonEncodeError`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError)

### `TestToonEncoderEncodeArrayTable`
- def: [`tests/unit/formatters/test_toon_encoder.py:195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L195)
- doc: Tests for encoding arrays as tables.
- signature: `class TestToonEncoderEncodeArrayTable:`
- members:
  - `test_encode_array_table_with_tabs(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L218) — Test encoding array table with tab delimiter.
  - `test_encode_empty_array_table(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L212) — Test encoding empty array table.
  - `test_encode_homogeneous_dict_array(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L198) — Test encoding homogeneous array of dicts as table.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

### `TestToonEncoderEncodeDict`
- def: [`tests/unit/formatters/test_toon_encoder.py:133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L133)
- doc: Tests for encoding dictionaries.
- signature: `class TestToonEncoderEncodeDict:`
- members:
  - `test_encode_dict_with_list(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L159) — Test encoding dictionary with list value.
  - `test_encode_empty_dict(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L136) — Test encoding empty dictionary.
  - `test_encode_nested_dict(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L151) — Test encoding nested dictionary.
  - `test_encode_simple_dict(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L143) — Test encoding simple dictionary.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

### `TestToonEncoderEncodeInlineDict`
- def: [`tests/unit/formatters/test_toon_encoder.py:556`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L556)
- doc: Tests for inline dict encoding.
- signature: `class TestToonEncoderEncodeInlineDict:`
- members:
  - `test_encode_inline_dict_empty(self)` — [`L565`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L565) — Test encoding empty inline dict.
  - `test_encode_inline_dict_nested(self)` — [`L571`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L571) — Test encoding nested inline dict.
  - `test_encode_inline_dict_simple(self)` — [`L559`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L559) — Test encoding simple inline dict.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`_encode_inline_dict`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder._encode_inline_dict)

### `TestToonEncoderEncodeList`
- def: [`tests/unit/formatters/test_toon_encoder.py:167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L167)
- doc: Tests for encoding lists.
- signature: `class TestToonEncoderEncodeList:`
- members:
  - `test_encode_empty_list(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L170) — Test encoding empty list.
  - `test_encode_list_with_tabs(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L182) — Test encoding list with tab delimiter.
  - `test_encode_nested_list(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L188) — Test encoding nested list.
  - `test_encode_simple_list(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L176) — Test encoding simple list.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

### `TestToonEncoderEncodePrimitive`
- def: [`tests/unit/formatters/test_toon_encoder.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L87)
- doc: Tests for encoding primitive values.
- signature: `class TestToonEncoderEncodePrimitive:`
- members:
  - `test_encode_bool_false(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L102) — Test encoding False boolean.
  - `test_encode_bool_true(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L96) — Test encoding True boolean.
  - `test_encode_float(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L114) — Test encoding float.
  - `test_encode_int(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L108) — Test encoding integer.
  - `test_encode_none(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L90) — Test encoding None value.
  - `test_encode_string_simple(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L120) — Test encoding simple string.
  - `test_encode_string_with_special_chars(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L126) — Test encoding string with special characters.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

### `TestToonEncoderEncodeSimpleList`
- def: [`tests/unit/formatters/test_toon_encoder.py:578`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L578)
- doc: Tests for simple list encoding.
- signature: `class TestToonEncoderEncodeSimpleList:`
- members:
  - `test_encode_simple_list_empty(self)` — [`L581`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L581) — Test encoding empty simple list.
  - `test_encode_simple_list_nested(self)` — [`L593`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L593) — Test encoding list with nested lists.
  - `test_encode_simple_list_primitives(self)` — [`L587`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L587) — Test encoding list of primitives.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`_encode_simple_list`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder._encode_simple_list)

### `TestToonEncoderEncodeString`
- def: [`tests/unit/formatters/test_toon_encoder.py:230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L230)
- doc: Tests for string encoding and escaping.
- signature: `class TestToonEncoderEncodeString:`
- members:
  - `test_encode_string_with_backslash(self)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L245) — Test encoding string with backslash.
  - `test_encode_string_with_braces(self)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L257) — Test encoding string with braces.
  - `test_encode_string_with_newline(self)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L233) — Test encoding string with newline.
  - `test_encode_string_with_quote(self)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L251) — Test encoding string with quote.
  - `test_encode_string_with_tab(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L239) — Test encoding string with tab.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

### `TestToonEncoderEncodeValue`
- def: [`tests/unit/formatters/test_toon_encoder.py:496`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L496)
- doc: Tests for encode_value method.
- signature: `class TestToonEncoderEncodeValue:`
- members:
  - `test_encode_value_bool(self)` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L505) — Test encode_value with boolean.
  - `test_encode_value_dict_inline(self)` — [`L523`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L523) — Test encode_value with inline dict.
  - `test_encode_value_list_inline(self)` — [`L529`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L529) — Test encode_value with inline list.
  - `test_encode_value_none(self)` — [`L499`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L499) — Test encode_value with None.
  - `test_encode_value_number(self)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L511) — Test encode_value with number.
  - `test_encode_value_string(self)` — [`L517`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L517) — Test encode_value with string.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode_value`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode_value)

### `TestToonEncoderErrorHandling`
- def: [`tests/unit/formatters/test_toon_encoder.py:353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L353)
- doc: Tests for error handling and fallback.
- signature: `class TestToonEncoderErrorHandling:`
- members:
  - `test_encode_safe_always_returns_string(self)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L379) — Test that encode_safe always returns a string.
  - `test_fallback_to_json_on_error(self)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L356) — Test fallback to JSON on encoding error.
  - `test_no_fallback_raises_error(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L369) — Test that error is raised when fallback is disabled.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode), [`ToonEncodeError`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError), [`encode_safe`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode_safe)  (2 test-only)

### `TestToonEncoderInferSchema`
- def: [`tests/unit/formatters/test_toon_encoder.py:536`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L536)
- doc: Tests for schema inference.
- signature: `class TestToonEncoderInferSchema:`
- members:
  - `test_infer_schema_empty(self)` — [`L549`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L549) — Test inferring schema from empty array.
  - `test_infer_schema_from_items(self)` — [`L539`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L539) — Test inferring schema from array items.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`_infer_schema`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder._infer_schema)

### `TestToonEncoderInit`
- def: [`tests/unit/formatters/test_toon_encoder.py:53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L53)
- doc: Tests for ToonEncoder initialization.
- signature: `class TestToonEncoderInit:`
- members:
  - `test_init_custom_max_depth(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L76) — Test initialization with custom max depth.
  - `test_init_default(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L56) — Test default initialization.
  - `test_init_with_tabs(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L65) — Test initialization with tab delimiter.
  - `test_init_without_fallback(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L71) — Test initialization without JSON fallback.
  - `test_init_without_path_normalization(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L81) — Test initialization without path normalization.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`delimiter`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.delimiter), [`fallback_to_json`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.fallback_to_json), [`max_depth`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.max_depth), [`normalize_paths`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.normalize_paths), [`use_tabs`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.use_tabs)

### `TestToonEncoderLongFlatStringList`
- def: [`tests/unit/formatters/test_toon_encoder.py:658`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L658)
- doc: Regression — M9: long flat `list[str]` rendering.
- signature: `class TestToonEncoderLongFlatStringList:`
- members:
  - `test_column_name_falls_back_to_item(self)` — [`L750`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L750)
  - `test_column_name_picked_from_key_suffix(self)` — [`L740`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L740)
  - `test_empty_string_list_stays_empty(self)` — [`L757`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L757)
  - `test_long_path_list_renders_as_array_table(self)` — [`L668`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L668)
  - `test_mixed_list_str_and_dict_unchanged(self)` — [`L716`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L716)
  - `test_non_string_list_falls_back_to_inline(self)` — [`L732`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L732)
  - `test_short_path_list_stays_inline(self)` — [`L693`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L693)
  - `test_threshold_boundary_inclusive_at_five(self)` — [`L701`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L701)
  - `test_threshold_boundary_table_at_six(self)` — [`L708`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L708)
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

### `TestToonEncoderNormalizePath`
- def: [`tests/unit/formatters/test_toon_encoder.py:264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L264)
- doc: Tests for path normalization.
- signature: `class TestToonEncoderNormalizePath:`
- members:
  - `test_no_normalize_non_path_string(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L292) — Test that non-path strings are not normalized.
  - `test_no_normalize_when_disabled(self)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L300) — Test that normalization is disabled when normalize_paths=False.
  - `test_normalize_parent_path(self)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L286) — Test normalization of parent path.
  - `test_normalize_relative_path(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L280) — Test normalization of relative path.
  - `test_normalize_unc_path(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L274) — Test normalization of UNC path.
  - `test_normalize_windows_path_drive_letter(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L267) — Test normalization of Windows path with drive letter.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

### `TestToonEncoderSpecialCharacters`
- def: [`tests/unit/formatters/test_toon_encoder.py:629`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L629)
- doc: Tests for handling special characters.
- signature: `class TestToonEncoderSpecialCharacters:`
- members:
  - `test_encode_string_with_all_special_chars(self)` — [`L650`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L650) — Test encoding string with multiple special characters.
  - `test_encode_string_with_brackets(self)` — [`L638`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L638) — Test encoding string with brackets.
  - `test_encode_string_with_carriage_return(self)` — [`L644`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L644) — Test encoding string with carriage return.
  - `test_encode_string_with_colon(self)` — [`L632`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_encoder.py#L632) — Test encoding string with colon.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

