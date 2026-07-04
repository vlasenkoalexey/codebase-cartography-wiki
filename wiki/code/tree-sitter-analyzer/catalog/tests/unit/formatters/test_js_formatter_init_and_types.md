---
title: 'Module: tests/unit/formatters/test_js_formatter_init_and_types.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_js_formatter_init_and_types.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_js_formatter_init_and_types`/TestJavaScript
symbols:
  TestJavaScriptFormatterInit.test_formatter_initialization: FormatterInit#test_formatter_initialization().
  TestJavaScriptFormatterInit.test_formatter_initialization_with_format_type: FormatterInit#test_formatter_initialization_with_format_type().
  TestJavaScriptFormatterInit.test_format_delegation: FormatterInit#test_format_delegation().
  TestJavaScriptParamCreation.formatter: ParamCreation#formatter().
  TestJavaScriptFunctionTypes.formatter: FunctionTypes#formatter().
  TestJavaScriptMethodHelpers.formatter: MethodHelpers#formatter().
  TestJavaScriptTypeInference.formatter: TypeInference#formatter().
  TestJavaScriptFormatterInit: FormatterInit#
  TestJavaScriptParamCreation: ParamCreation#
  TestJavaScriptParamCreation.test_create_full_params_empty: ParamCreation#test_create_full_params_empty().
  TestJavaScriptParamCreation.test_create_full_params_with_types: ParamCreation#test_create_full_params_with_types().
  TestJavaScriptParamCreation.test_create_full_params_string_parameters: ParamCreation#test_create_full_params_string_parameters().
  TestJavaScriptParamCreation.test_create_full_params_long_truncation: ParamCreation#test_create_full_params_long_truncation().
  TestJavaScriptParamCreation.test_create_compact_params_empty: ParamCreation#test_create_compact_params_empty().
  TestJavaScriptParamCreation.test_create_compact_params_few_params: ParamCreation#test_create_compact_params_few_params().
  TestJavaScriptParamCreation.test_create_compact_params_many_params: ParamCreation#test_create_compact_params_many_params().
  TestJavaScriptFunctionTypes: FunctionTypes#
  TestJavaScriptFunctionTypes.test_get_function_type_async: FunctionTypes#test_get_function_type_async().
  TestJavaScriptFunctionTypes.test_get_function_type_generator: FunctionTypes#test_get_function_type_generator().
  TestJavaScriptFunctionTypes.test_get_function_type_arrow: FunctionTypes#test_get_function_type_arrow().
  TestJavaScriptFunctionTypes.test_get_function_type_constructor_method: FunctionTypes#test_get_function_type_constructor_method().
  TestJavaScriptFunctionTypes.test_get_function_type_getter_method: FunctionTypes#test_get_function_type_getter_method().
  TestJavaScriptFunctionTypes.test_get_function_type_setter_method: FunctionTypes#test_get_function_type_setter_method().
  TestJavaScriptFunctionTypes.test_get_function_type_static_method: FunctionTypes#test_get_function_type_static_method().
  TestJavaScriptFunctionTypes.test_get_function_type_regular_method: FunctionTypes#test_get_function_type_regular_method().
  TestJavaScriptFunctionTypes.test_get_function_type_regular_function: FunctionTypes#test_get_function_type_regular_function().
  TestJavaScriptFunctionTypes.test_get_function_type_short: FunctionTypes#test_get_function_type_short().
  TestJavaScriptFunctionTypes.test_get_method_type: FunctionTypes#test_get_method_type().
  TestJavaScriptMethodHelpers: MethodHelpers#
  TestJavaScriptMethodHelpers.test_is_method_with_flag: MethodHelpers#test_is_method_with_flag().
  TestJavaScriptMethodHelpers.test_is_method_with_class_name: MethodHelpers#test_is_method_with_class_name().
  TestJavaScriptMethodHelpers.test_is_method_without_either: MethodHelpers#test_is_method_without_either().
  TestJavaScriptMethodHelpers.test_get_method_class_present: MethodHelpers#test_get_method_class_present().
  TestJavaScriptMethodHelpers.test_get_method_class_missing: MethodHelpers#test_get_method_class_missing().
  TestJavaScriptTypeInference: TypeInference#
  TestJavaScriptTypeInference.test_infer_js_type: TypeInference#test_infer_js_type().
  TestJavaScriptTypeInference.test_determine_scope: TypeInference#test_determine_scope().
  TestJavaScriptTypeInference.test_get_variable_kind: TypeInference#test_get_variable_kind().
  TestJavaScriptTypeInference.test_get_export_type: TypeInference#test_get_export_type().
---
# Module: [`tests/unit/formatters/test_js_formatter_init_and_types.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py)

## Classes
### `TestJavaScriptFormatterInit`
- def: [`tests/unit/formatters/test_js_formatter_init_and_types.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L13)
- doc: Tests for JavaScriptTableFormatter initialization.
- signature: `class TestJavaScriptFormatterInit:`
- members:
  - `test_format_delegation(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L31)
  - `test_formatter_initialization(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L16)
  - `test_formatter_initialization_with_format_type(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L21)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter), [`format_type`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter.format_type), [`format`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter.format)

### `TestJavaScriptFunctionTypes`
- def: [`tests/unit/formatters/test_js_formatter_init_and_types.py:96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L96)
- doc: Tests for function/method type detection methods.
- signature: `class TestJavaScriptFunctionTypes:`
- members:
  - `formatter(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L100)
  - `test_get_function_type_arrow(self, formatter)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L113)
  - `test_get_function_type_async(self, formatter)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L103)
  - `test_get_function_type_constructor_method(self, formatter)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L118)
  - `test_get_function_type_generator(self, formatter)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L108)
  - `test_get_function_type_getter_method(self, formatter)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L130)
  - `test_get_function_type_regular_function(self, formatter)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L177)
  - `test_get_function_type_regular_method(self, formatter)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L166)
  - `test_get_function_type_setter_method(self, formatter)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L142)
  - `test_get_function_type_short(self, formatter)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L188)
  - `test_get_function_type_static_method(self, formatter)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L154)
  - `test_get_method_type(self, formatter)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L203)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter)

### `TestJavaScriptMethodHelpers`
- def: [`tests/unit/formatters/test_js_formatter_init_and_types.py:217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L217)
- doc: Tests for method detection and class extraction helpers.
- signature: `class TestJavaScriptMethodHelpers:`
- members:
  - `formatter(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L221)
  - `test_get_method_class_missing(self, formatter)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L241)
  - `test_get_method_class_present(self, formatter)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L236)
  - `test_is_method_with_class_name(self, formatter)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L228)
  - `test_is_method_with_flag(self, formatter)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L224)
  - `test_is_method_without_either(self, formatter)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L232)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter)

### `TestJavaScriptParamCreation`
- def: [`tests/unit/formatters/test_js_formatter_init_and_types.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L41)
- doc: Tests for parameter creation methods.
- signature: `class TestJavaScriptParamCreation:`
- members:
  - `formatter(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L45)
  - `test_create_compact_params_empty(self, formatter)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L78)
  - `test_create_compact_params_few_params(self, formatter)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L83)
  - `test_create_compact_params_many_params(self, formatter)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L90)
  - `test_create_full_params_empty(self, formatter)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L48)
  - `test_create_full_params_long_truncation(self, formatter)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L71)
  - `test_create_full_params_string_parameters(self, formatter)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L66)
  - `test_create_full_params_with_types(self, formatter)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L53)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter)

### `TestJavaScriptTypeInference`
- def: [`tests/unit/formatters/test_js_formatter_init_and_types.py:247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L247)
- doc: Tests for JS type inference and variable helpers.
- signature: `class TestJavaScriptTypeInference:`
- members:
  - `formatter(self)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L251)
  - `test_determine_scope(self, formatter)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L276)
  - `test_get_export_type(self, formatter)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L308)
  - `test_get_variable_kind(self, formatter)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L296)
  - `test_infer_js_type(self, formatter)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_js_formatter_init_and_types.py#L254)
- uses (calls/refs, reference-scoped): [`JavaScriptTableFormatter`](../../../tree_sitter_analyzer/formatters/javascript_formatter.md#JavaScriptTableFormatter)

