---
title: 'Module: tests/integration/cli/test_toon_error_handling.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_toon_error_handling.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.cli.test_toon_error_handling`/Test
symbols:
  TestToonEncodeError.test_error_basic_creation: ToonEncodeError#test_error_basic_creation().
  TestToonEncodeError.test_error_with_all_attributes: ToonEncodeError#test_error_with_all_attributes().
  TestMaxDepthLimit.test_max_depth_exceeded: MaxDepthLimit#test_max_depth_exceeded().
  TestMaxDepthLimit.test_custom_max_depth: MaxDepthLimit#test_custom_max_depth().
  TestErrorRecovery.test_partial_encoding_on_error: ErrorRecovery#test_partial_encoding_on_error().
  TestToonEncodeError.test_error_with_data: ToonEncodeError#test_error_with_data().
  TestToonEncodeError.test_error_with_cause: ToonEncodeError#test_error_with_cause().
  TestCircularReferenceDetection.test_detect_simple_circular_dict: CircularReferenceDetection#test_detect_simple_circular_dict().
  TestCircularReferenceDetection.test_detect_nested_circular_dict: CircularReferenceDetection#test_detect_nested_circular_dict().
  TestCircularReferenceDetection.test_detect_circular_list: CircularReferenceDetection#test_detect_circular_list().
  TestCircularReferenceDetection.test_static_circular_reference_check: CircularReferenceDetection#test_static_circular_reference_check().
  TestCircularReferenceDetection.test_no_false_positive_same_value: CircularReferenceDetection#test_no_false_positive_same_value().
  TestJsonFallback.test_fallback_on_circular_reference: JsonFallback#test_fallback_on_circular_reference().
  TestJsonFallback.test_encode_safe_always_returns_string: JsonFallback#test_encode_safe_always_returns_string().
  TestJsonFallback.test_fallback_disabled_raises_error: JsonFallback#test_fallback_disabled_raises_error().
  TestJsonFallback.test_formatter_fallback: JsonFallback#test_formatter_fallback().
  TestToonContentDetection.test_detect_toon_key_value: ToonContentDetection#test_detect_toon_key_value().
  TestToonContentDetection.test_detect_toon_array_table: ToonContentDetection#test_detect_toon_array_table().
  TestToonContentDetection.test_reject_json_content: ToonContentDetection#test_reject_json_content().
  TestToonContentDetection.test_reject_empty_content: ToonContentDetection#test_reject_empty_content().
  TestToonContentDetection.test_reject_json_array: ToonContentDetection#test_reject_json_array().
  TestErrorRecovery.test_safe_encode_with_none: ErrorRecovery#test_safe_encode_with_none().
  TestErrorRecovery.test_safe_encode_with_special_types: ErrorRecovery#test_safe_encode_with_special_types().
  TestErrorRecovery.test_partial_encoding_on_error.CustomObject: ErrorRecovery#test_partial_encoding_on_error().CustomObject#
  TestToonEncodeError: ToonEncodeError#
  TestCircularReferenceDetection: CircularReferenceDetection#
  TestJsonFallback: JsonFallback#
  TestMaxDepthLimit: MaxDepthLimit#
  TestToonContentDetection: ToonContentDetection#
  TestErrorRecovery: ErrorRecovery#
  TestErrorRecovery.test_partial_encoding_on_error.CustomObject.__str__: ErrorRecovery#test_partial_encoding_on_error().CustomObject#__str__().
---
# Module: [`tests/integration/cli/test_toon_error_handling.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py)

## Classes
### `CustomObject`
- def: [`tests/integration/cli/test_toon_error_handling.py:264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L264)
- signature: `class CustomObject:`
- protocol/private: `__str__`[`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L265)
- used by: (1 test-only callers)

### `TestCircularReferenceDetection`
- def: [`tests/integration/cli/test_toon_error_handling.py:60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L60)
- doc: Tests for circular reference detection.
- signature: `class TestCircularReferenceDetection:`
- members:
  - `test_detect_circular_list(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L87) — Test graceful degradation for circular reference in list.
  - `test_detect_nested_circular_dict(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L74) — Test graceful degradation for nested circular reference.
  - `test_detect_simple_circular_dict(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L63) — Test graceful degradation for simple circular reference in dict.
  - `test_no_false_positive_same_value(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L109) — Test that same values at different paths don't trigger false positive.
  - `test_static_circular_reference_check(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L98) — Test static method for circular reference detection.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode), [`detect_circular_reference`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.detect_circular_reference)

### `TestErrorRecovery`
- def: [`tests/integration/cli/test_toon_error_handling.py:257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L257)
- doc: Tests for error recovery scenarios.
- signature: `class TestErrorRecovery:`
- members:
  - `test_partial_encoding_on_error(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L260) — Test behavior when encoding partially fails. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `test_safe_encode_with_none(self)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L276) — Test safe encoding of None values.
  - `test_safe_encode_with_special_types(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L283) — Test safe encoding of special Python types.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode), [`encode_safe`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode_safe)  (1 test-only)

### `TestJsonFallback`
- def: [`tests/integration/cli/test_toon_error_handling.py:124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L124)
- doc: Tests for JSON fallback mechanism.
- signature: `class TestJsonFallback:`
- members:
  - `test_encode_safe_always_returns_string(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L140) — Test that encode_safe always returns a string.
  - `test_fallback_disabled_raises_error(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L155) — Test that disabling fallback returns placeholder on circular reference.
  - `test_fallback_on_circular_reference(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L127) — Test JSON fallback when circular reference is detected.
  - `test_formatter_fallback(self)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L166) — Test ToonFormatter fallback mechanism.
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode), [`ToonFormatter`](../../../tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter), [`format`](../../../tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter.format), [`encode_safe`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode_safe)

### `TestMaxDepthLimit`
- def: [`tests/integration/cli/test_toon_error_handling.py:179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L179)
- doc: Tests for maximum nesting depth limit.
- signature: `class TestMaxDepthLimit:`
- members:
  - `test_custom_max_depth(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L198) — Test custom max depth setting. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
  - `test_max_depth_exceeded(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L182) — Test that deeply nested structures are rejected. — documented in [tree_sitter_analyzer-formatters-toon_encoder](../../../../concepts/tree_sitter_analyzer-formatters-toon_encoder.md)
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode), [`ToonEncodeError`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError)

### `TestToonContentDetection`
- def: [`tests/integration/cli/test_toon_error_handling.py:218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L218)
- doc: Tests for TOON content format detection.
- signature: `class TestToonContentDetection:`
- members:
  - `test_detect_toon_array_table(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L229) — Test detection of TOON array table format.
  - `test_detect_toon_key_value(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L221) — Test detection of TOON key-value format.
  - `test_reject_empty_content(self)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L245) — Test that empty content is not detected as TOON.
  - `test_reject_json_array(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L250) — Test that JSON arrays are not detected as TOON.
  - `test_reject_json_content(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L239) — Test that JSON content is not detected as TOON.
- uses (calls/refs, reference-scoped): [`ToonFormatter`](../../../tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter), [`is_toon_content`](../../../tree_sitter_analyzer/formatters/toon_formatter.md#ToonFormatter.is_toon_content)

### `TestToonEncodeError`
- def: [`tests/integration/cli/test_toon_error_handling.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L18)
- doc: Tests for ToonEncodeError exception class.
- signature: `class TestToonEncodeError:`
- members:
  - `test_error_basic_creation(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L21) — Test basic error creation.
  - `test_error_with_all_attributes(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L47) — Test error with all attributes.
  - `test_error_with_cause(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L38) — Test error with cause exception.
  - `test_error_with_data(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/cli/test_toon_error_handling.py#L30) — Test error with data attribute.
- uses (calls/refs, reference-scoped): [`ToonEncodeError`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError), [`cause`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError.cause), [`message`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError.message), [`data`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncodeError.data)

