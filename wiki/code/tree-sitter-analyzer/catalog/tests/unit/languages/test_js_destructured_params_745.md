---
title: 'Module: tests/unit/languages/test_js_destructured_params_745.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_js_destructured_params_745.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_js_destructured_params_745`/Test
symbols:
  TestParseStringParameterDestructuring.test_object_destructuring_name_preserved: ParseStringParameterDestructuring#test_object_destructuring_name_preserved().
  TestParseStringParameterDestructuring.test_object_destructuring_no_closing_brace_as_name: ParseStringParameterDestructuring#test_object_destructuring_no_closing_brace_as_name().
  TestParseStringParameterDestructuring.test_simple_object_destructuring: ParseStringParameterDestructuring#test_simple_object_destructuring().
  TestParseStringParameterDestructuring.test_array_destructuring_name_preserved: ParseStringParameterDestructuring#test_array_destructuring_name_preserved().
  TestParseStringParameterDestructuring.test_array_destructuring_no_bracket_as_name: ParseStringParameterDestructuring#test_array_destructuring_no_bracket_as_name().
  TestParseStringParameterDestructuring.test_normal_typed_param_unchanged: ParseStringParameterDestructuring#test_normal_typed_param_unchanged().
  TestParseStringParameterDestructuring.test_default_valued_param_unchanged: ParseStringParameterDestructuring#test_default_valued_param_unchanged().
  TestParseStringParameterDestructuring.test_destructuring_with_default_preserves_pattern_and_default: ParseStringParameterDestructuring#test_destructuring_with_default_preserves_pattern_and_default().
  TestParseStringParameterDestructuring.test_ts_typed_destructuring_preserves_type: ParseStringParameterDestructuring#test_ts_typed_destructuring_preserves_type().
  TestParseStringParameterDestructuring.test_ts_typed_destructuring_with_default: ParseStringParameterDestructuring#test_ts_typed_destructuring_with_default().
  TestProcessParametersDestructuring.test_js_destructured_param_not_mangled: ProcessParametersDestructuring#test_js_destructured_param_not_mangled().
  TestProcessParametersDestructuring.test_js_destructured_name_not_closing_brace: ProcessParametersDestructuring#test_js_destructured_name_not_closing_brace().
  TestProcessParametersDestructuring.test_js_array_destructuring_preserved: ProcessParametersDestructuring#test_js_array_destructuring_preserved().
  TestProcessParametersDestructuring.test_js_normal_param_unchanged: ProcessParametersDestructuring#test_js_normal_param_unchanged().
  TestProcessParametersDestructuring.test_mixed_params_all_correct: ProcessParametersDestructuring#test_mixed_params_all_correct().
  TestTypePrefixParameterCSharpAttributes.test_csharp_frombody_attribute_preserved: TypePrefixParameterCSharpAttributes#test_csharp_frombody_attribute_preserved().
  TestTypePrefixParameterCSharpAttributes.test_cpp_maybe_unused_attribute_preserved: TypePrefixParameterCSharpAttributes#test_cpp_maybe_unused_attribute_preserved().
  TestParseStringParameterDestructuring: ParseStringParameterDestructuring#
  TestProcessParametersDestructuring: ProcessParametersDestructuring#
  TestTypePrefixParameterCSharpAttributes: TypePrefixParameterCSharpAttributes#
---
# Module: [`tests/unit/languages/test_js_destructured_params_745.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py)

## Classes
### `TestParseStringParameterDestructuring`
- def: [`tests/unit/languages/test_js_destructured_params_745.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L27)
- doc: _parse_string_parameter must preserve destructuring patterns intact.
- signature: `class TestParseStringParameterDestructuring:`
- members:
  - `test_array_destructuring_name_preserved(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L50)
  - `test_array_destructuring_no_bracket_as_name(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L56)
  - `test_default_valued_param_unchanged(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L67)
  - `test_destructuring_with_default_preserves_pattern_and_default(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L73)
  - `test_normal_typed_param_unchanged(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L61)
  - `test_object_destructuring_name_preserved(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L30)
  - `test_object_destructuring_no_closing_brace_as_name(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L38)
  - `test_simple_object_destructuring(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L45)
  - `test_ts_typed_destructuring_preserves_type(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L80)
  - `test_ts_typed_destructuring_with_default(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L87)
- uses (calls/refs, reference-scoped): [`_parse_string_parameter`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.md#_parse_string_parameter)

### `TestProcessParametersDestructuring`
- def: [`tests/unit/languages/test_js_destructured_params_745.py:96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L96)
- doc: process_parameters must preserve JS object-destructuring param names.
- signature: `class TestProcessParametersDestructuring:`
- members:
  - `test_js_array_destructuring_preserved(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L110)
  - `test_js_destructured_name_not_closing_brace(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L105)
  - `test_js_destructured_param_not_mangled(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L99)
  - `test_js_normal_param_unchanged(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L116)
  - `test_mixed_params_all_correct(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L122)
- uses (calls/refs, reference-scoped): [`process_parameters`](../../../tree_sitter_analyzer/cli/commands/table_command_helpers.md#process_parameters)

### `TestTypePrefixParameterCSharpAttributes`
- def: [`tests/unit/languages/test_js_destructured_params_745.py:131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L131)
- doc: C# attribute parameters must NOT be treated as destructuring (#745 Codex P2).
- signature: `class TestTypePrefixParameterCSharpAttributes:`
- members:
  - `test_cpp_maybe_unused_attribute_preserved(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L140)
  - `test_csharp_frombody_attribute_preserved(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_destructured_params_745.py#L134)
- uses (calls/refs, reference-scoped): [`_process_type_prefix_parameter`](../../../tree_sitter_analyzer/cli/commands/table_command_helpers.md#_process_type_prefix_parameter)

