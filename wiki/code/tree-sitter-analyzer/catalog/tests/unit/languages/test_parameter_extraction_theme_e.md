---
title: 'Module: tests/unit/languages/test_parameter_extraction_theme_e.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_parameter_extraction_theme_e.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_parameter_extraction_theme_e`/
symbols:
  TestPHPVariadicParameterExtraction.test_method_variadic_count: TestPHPVariadicParameterExtraction#test_method_variadic_count().
  TestPHPVariadicParameterExtraction.test_method_variadic_text_contains_parts: TestPHPVariadicParameterExtraction#test_method_variadic_text_contains_parts().
  TestPHPVariadicParameterExtraction.test_function_variadic_count: TestPHPVariadicParameterExtraction#test_function_variadic_count().
  TestPHPVariadicParameterExtraction.test_function_variadic_text_contains_parts: TestPHPVariadicParameterExtraction#test_function_variadic_text_contains_parts().
  TestCppVariadicParameterExtraction.test_c_style_variadic_printf: TestCppVariadicParameterExtraction#test_c_style_variadic_printf().
  TestPHPByReferenceVariadic.test_by_reference_variadic_text: TestPHPByReferenceVariadic#test_by_reference_variadic_text().
  TestCppCStyleVariadicExact.test_c_style_variadic_exact_string: TestCppCStyleVariadicExact#test_c_style_variadic_exact_string().
  TestKotlinParameterExtraction.test_three_params_including_vararg_count: TestKotlinParameterExtraction#test_three_params_including_vararg_count().
  TestKotlinParameterExtraction.test_three_params_names_and_types: TestKotlinParameterExtraction#test_three_params_names_and_types().
  TestKotlinParameterExtraction.test_two_regular_params_count: TestKotlinParameterExtraction#test_two_regular_params_count().
  TestKotlinParameterExtraction.test_zero_params: TestKotlinParameterExtraction#test_zero_params().
  TestGoVariadicParameterExtraction.test_variadic_sum_count: TestGoVariadicParameterExtraction#test_variadic_sum_count().
  TestGoVariadicParameterExtraction.test_variadic_sum_contains_variadic_param: TestGoVariadicParameterExtraction#test_variadic_sum_contains_variadic_param().
  TestGoVariadicParameterExtraction.test_regular_params_unchanged: TestGoVariadicParameterExtraction#test_regular_params_unchanged().
  TestGoVariadicParameterExtraction.test_only_variadic_param: TestGoVariadicParameterExtraction#test_only_variadic_param().
  TestCppVariadicParameterExtraction.test_template_variadic_full_text: TestCppVariadicParameterExtraction#test_template_variadic_full_text().
  TestKotlinDefaultValue.test_default_value_dropped: TestKotlinDefaultValue#test_default_value_dropped().
  TestPHPVariadicParameterExtraction.extract_mod: TestPHPVariadicParameterExtraction#extract_mod().
  TestPHPVariadicParameterExtraction.get_text: TestPHPVariadicParameterExtraction#get_text().
  _kotlin_parser: _kotlin_parser().
  _php_parser: _php_parser().
  TestCppVariadicParameterExtraction.find_param_list: TestCppVariadicParameterExtraction#find_param_list().
  TestCppCStyleVariadicExact.find_param_list: TestCppCStyleVariadicExact#find_param_list().
  _go_parser: _go_parser().
  TestKotlinParameterExtraction.get_text: TestKotlinParameterExtraction#get_text().
  TestGoVariadicParameterExtraction.get_text: TestGoVariadicParameterExtraction#get_text().
  _cpp_parser: _cpp_parser().
  TestPHPVariadicParameterExtraction.extract_attr: TestPHPVariadicParameterExtraction#extract_attr().
  TestCppVariadicParameterExtraction.get_text: TestCppVariadicParameterExtraction#get_text().
  TestPHPByReferenceVariadic.get_text: TestPHPByReferenceVariadic#get_text().
  TestKotlinDefaultValue.get_text: TestKotlinDefaultValue#get_text().
  TestCppCStyleVariadicExact.get_text: TestCppCStyleVariadicExact#get_text().
  TestKotlinParameterExtraction: TestKotlinParameterExtraction#
  TestGoVariadicParameterExtraction: TestGoVariadicParameterExtraction#
  TestPHPVariadicParameterExtraction: TestPHPVariadicParameterExtraction#
  TestCppVariadicParameterExtraction: TestCppVariadicParameterExtraction#
  TestPHPByReferenceVariadic: TestPHPByReferenceVariadic#
  TestKotlinDefaultValue: TestKotlinDefaultValue#
  TestCppCStyleVariadicExact: TestCppCStyleVariadicExact#
---
# Module: [`tests/unit/languages/test_parameter_extraction_theme_e.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py)

## Classes
### `TestCppCStyleVariadicExact`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e.py:468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L468)
- doc: C-style variadic '...' in printf must appear as the exact string '...'.
- signature: `class TestCppCStyleVariadicExact:`
- members:
  - `find_param_list(node: object)` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L481)
  - `get_text(n: object)` — [`L493`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L493)
  - `test_c_style_variadic_exact_string(self)` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L471) — int printf(const char* fmt, ...) → params[1] == '...' (exact).
- uses (calls/refs, reference-scoped): [`extract_parameters`](../../../tree_sitter_analyzer/languages/_cpp_signature_helpers.md#extract_parameters)  (1 test-only)

### `TestCppVariadicParameterExtraction`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L330)
- doc: Theme E (C++): _cpp_signature_helpers.extract_parameters previously
- signature: `class TestCppVariadicParameterExtraction:`
- members:
  - `find_param_list(node: object)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L390)
  - `get_text(n: object)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L367)
  - `test_c_style_variadic_printf(self)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L376) — C-style printf(const char* fmt, ...) variadic: '...' node type is
  - `test_template_variadic_full_text(self)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L338) — template variadic param 'Args... args' must appear as full text,
- uses (calls/refs, reference-scoped): [`extract_parameters`](../../../tree_sitter_analyzer/languages/_cpp_signature_helpers.md#extract_parameters)  (1 test-only)

### `TestGoVariadicParameterExtraction`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e.py:132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L132)
- doc: Theme E: variadic_parameter_declaration (e.g. numbers ...int)
- signature: `class TestGoVariadicParameterExtraction:`
- members:
  - `get_text(n: object)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L147)
  - `test_only_variadic_param(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L187) — func with only a variadic param must yield exactly 1 parameter.
  - `test_regular_params_unchanged(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L170) — Regular (non-variadic) parameters still work.
  - `test_variadic_sum_contains_variadic_param(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L153) — The variadic parameter text must contain 'numbers' and '...'.
  - `test_variadic_sum_count(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L136) — func sum(a int, numbers ...int) must yield exactly 2 parameters.
- uses (calls/refs, reference-scoped): [`extract_parameters`](../../../tree_sitter_analyzer/languages/_go_common_helpers.md#extract_parameters)  (1 test-only)

### `TestKotlinDefaultValue`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e.py:443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L443)
- doc: Kotlin default value: fun f(x: Int = 5)
- signature: `class TestKotlinDefaultValue:`
- members:
  - `get_text(n: object)` — [`L460`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L460)
  - `test_default_value_dropped(self)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L447) — fun f(x: Int = 5) → ['x: Int']
- uses (calls/refs, reference-scoped): [`extract_kotlin_parameters`](../../../tree_sitter_analyzer/languages/kotlin_helpers.md#extract_kotlin_parameters)  (1 test-only)

### `TestKotlinParameterExtraction`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e.py:53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L53)
- doc: Theme E: Kotlin parameters were all empty because child_by_field_name
- signature: `class TestKotlinParameterExtraction:`
- members:
  - `get_text(n: object)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L69)
  - `test_three_params_including_vararg_count(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L58) — greet(name, age, vararg tags) must yield exactly 3 parameters.
  - `test_three_params_names_and_types(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L75) — Each parameter must carry its name and type.
  - `test_two_regular_params_count(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L92) — Functions without vararg still work after the fix.
  - `test_zero_params(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L109) — Functions with no parameters yield an empty list.
- uses (calls/refs, reference-scoped): [`extract_kotlin_parameters`](../../../tree_sitter_analyzer/languages/kotlin_helpers.md#extract_kotlin_parameters)  (1 test-only)

### `TestPHPByReferenceVariadic`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e.py:418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L418)
- doc: PHP by-reference variadic: function join(string &...$parts)
- signature: `class TestPHPByReferenceVariadic:`
- members:
  - `get_text(n: object)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L435)
  - `test_by_reference_variadic_text(self)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L422) — function join(string &...$parts) → parameter text is '&...$parts'
- uses (calls/refs, reference-scoped): [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`extract_php_function_element`](../../../tree_sitter_analyzer/languages/php_helpers.md#extract_php_function_element)  (1 test-only)

### `TestPHPVariadicParameterExtraction`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e.py:211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L211)
- doc: Theme E: variadic_parameter (e.g. ...$parts) was silently dropped
- signature: `class TestPHPVariadicParameterExtraction:`
- members:
  - `extract_attr(_n: object)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L237)
  - `extract_mod(n: object)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L234)
  - `get_text(n: object)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L231)
  - `test_function_variadic_count(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L285) — Free function implode(string $sep, ...$parts) must yield 2 params.
  - `test_function_variadic_text_contains_parts(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L304) — The variadic param entry must include '...$parts' or 'parts'.
  - `test_method_variadic_count(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L215) — Method format(string $sep, ...$parts) must yield exactly 2 params.
  - `test_method_variadic_text_contains_parts(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L250) — The variadic param entry must mention '$parts' or 'parts'.
- uses (calls/refs, reference-scoped): [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`extract_php_method_element`](../../../tree_sitter_analyzer/languages/php_helpers.md#extract_php_method_element), [`extract_php_function_element`](../../../tree_sitter_analyzer/languages/php_helpers.md#extract_php_function_element), [`extract_modifiers`](../../../tree_sitter_analyzer/languages/php_helpers.md#extract_modifiers)  (1 test-only)

## Functions
- `_cpp_parser()` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L44)
- `_go_parser()` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L36)
- `_kotlin_parser()` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L32)
- `_php_parser()` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e.py#L40)

