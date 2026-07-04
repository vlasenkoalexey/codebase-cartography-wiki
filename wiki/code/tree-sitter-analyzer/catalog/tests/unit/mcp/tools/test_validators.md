---
title: 'Module: tests/unit/mcp/tools/test_validators.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_validators.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_validators`/test_
symbols:
  test_invalid_enum_error_routes_to_validation_recovery_hint: invalid_enum_error_routes_to_validation_recovery_hint().
  test_valid_int_passes: valid_int_passes().
  test_none_is_noop: none_is_noop().
  test_missing_key_is_noop: missing_key_is_noop().
  test_whole_number_float_coerced: whole_number_float_coerced().
  test_whole_number_float_1_coerced: whole_number_float_1_coerced().
  test_fractional_float_rejected: fractional_float_rejected().
  test_float_zero_rejected: float_zero_rejected().
  test_float_negative_rejected: float_negative_rejected().
  test_bool_true_rejected: bool_true_rejected().
  test_bool_false_rejected: bool_false_rejected().
  test_zero_int_rejected: zero_int_rejected().
  test_negative_int_rejected: negative_int_rejected().
  test_string_rejected: string_rejected().
  test_invalid_enum_error_basic: invalid_enum_error_basic().
  test_invalid_enum_error_single_valid: invalid_enum_error_single_valid().
  test_invalid_enum_error_with_context: invalid_enum_error_with_context().
  test_invalid_enum_error_preserves_value_type: invalid_enum_error_preserves_value_type().
  test_invalid_enum_error_empty_list: invalid_enum_error_empty_list().
---
# Module: [`tests/unit/mcp/tools/test_validators.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py)

## Functions
- `test_bool_false_rejected()` — [`L73`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L73)
- `test_bool_true_rejected()` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L68)
- `test_float_negative_rejected()` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L63)
- `test_float_zero_rejected()` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L58)
- `test_fractional_float_rejected()` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L53)
- `test_invalid_enum_error_basic()` — [`L96`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L96) — Error message enumerates valid values in sorted order.
- `test_invalid_enum_error_empty_list()` — [`L126`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L126) — Edge case: empty valid list (should not happen in practice).
- `test_invalid_enum_error_preserves_value_type()` — [`L120`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L120) — The received value is quoted with repr().
- `test_invalid_enum_error_routes_to_validation_recovery_hint()` — [`L133`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L133) — opencode P2 (#490): the enumerated message must classify as a
- `test_invalid_enum_error_single_valid()` — [`L103`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L103) — Works with a single valid value.
- `test_invalid_enum_error_with_context()` — [`L109`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L109) — Context string is appended to the message.
- `test_missing_key_is_noop()` — [`L30`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L30)
- `test_negative_int_rejected()` — [`L83`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L83)
- `test_none_is_noop()` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L24)
- `test_string_rejected()` — [`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L88)
- `test_valid_int_passes()` — [`L18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L18)
- `test_whole_number_float_1_coerced()` — [`L43`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L43)
- `test_whole_number_float_coerced()` — [`L36`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L36)
- `test_zero_int_rejected()` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_validators.py#L78)

