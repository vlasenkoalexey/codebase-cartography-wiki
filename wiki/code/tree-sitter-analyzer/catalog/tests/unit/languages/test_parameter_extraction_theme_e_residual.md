---
title: 'Module: tests/unit/languages/test_parameter_extraction_theme_e_residual.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_parameter_extraction_theme_e_residual.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_parameter_extraction_theme_e_residual`/
symbols:
  TestJSDefaultParameterExtraction.test_fibonacciSequence_only_default_param: TestJSDefaultParameterExtraction#test_fibonacciSequence_only_default_param().
  TestJSDefaultParameterExtraction.test_processData_mixed_plain_and_default: TestJSDefaultParameterExtraction#test_processData_mixed_plain_and_default().
  TestJSDefaultParameterExtraction.test_generateSequence_all_defaults: TestJSDefaultParameterExtraction#test_generateSequence_all_defaults().
  TestJSDefaultParameterExtraction.test_full_plugin_fibonacciSequence_count: TestJSDefaultParameterExtraction#test_full_plugin_fibonacciSequence_count().
  TestJSDefaultParameterExtraction.test_full_plugin_processData_param_list: TestJSDefaultParameterExtraction#test_full_plugin_processData_param_list().
  TestJSDefaultParameterExtraction.test_full_plugin_processData_param_values: TestJSDefaultParameterExtraction#test_full_plugin_processData_param_values().
  TestPythonTypedDefaultParameterExtraction.test_dog_init_three_params: TestPythonTypedDefaultParameterExtraction#test_dog_init_three_params().
  TestPythonTypedDefaultParameterExtraction.test_dog_init_param_values: TestPythonTypedDefaultParameterExtraction#test_dog_init_param_values().
  TestPythonTypedDefaultParameterExtraction.test_cat_init_bool_default: TestPythonTypedDefaultParameterExtraction#test_cat_init_bool_default().
  TestPythonTypedDefaultParameterExtraction.test_cat_init_param_values: TestPythonTypedDefaultParameterExtraction#test_cat_init_param_values().
  TestPythonTypedDefaultParameterExtraction.test_untyped_default_still_works: TestPythonTypedDefaultParameterExtraction#test_untyped_default_still_works().
  TestPythonTypedDefaultParameterExtraction.test_args_kwargs_unaffected: TestPythonTypedDefaultParameterExtraction#test_args_kwargs_unaffected().
  TestBashParamStructuralNa.test_greet_params_empty: TestBashParamStructuralNa#test_greet_params_empty().
  TestBashParamStructuralNa.test_function_keyword_params_empty: TestBashParamStructuralNa#test_function_keyword_params_empty().
  TestJSDefaultParameterExtraction.get_text: TestJSDefaultParameterExtraction#get_text().
  TestJSDefaultParameterExtraction.test_fibonacciSequence_only_default_param._MinimalExtractor: TestJSDefaultParameterExtraction#test_fibonacciSequence_only_default_param()._MinimalExtractor#
  TestJSDefaultParameterExtraction.test_processData_mixed_plain_and_default._MinimalExtractor: TestJSDefaultParameterExtraction#test_processData_mixed_plain_and_default()._MinimalExtractor#
  TestJSDefaultParameterExtraction.test_generateSequence_all_defaults._MinimalExtractor: TestJSDefaultParameterExtraction#test_generateSequence_all_defaults()._MinimalExtractor#
  _js_parser: _js_parser().
  TestJSDefaultParameterExtraction.test_fibonacciSequence_only_default_param._MinimalExtractor._get_node_text_optimized: TestJSDefaultParameterExtraction#test_fibonacciSequence_only_default_param()._MinimalExtractor#_get_node_text_optimized().
  TestJSDefaultParameterExtraction.test_processData_mixed_plain_and_default._MinimalExtractor._get_node_text_optimized: TestJSDefaultParameterExtraction#test_processData_mixed_plain_and_default()._MinimalExtractor#_get_node_text_optimized().
  TestJSDefaultParameterExtraction.test_generateSequence_all_defaults._MinimalExtractor._get_node_text_optimized: TestJSDefaultParameterExtraction#test_generateSequence_all_defaults()._MinimalExtractor#_get_node_text_optimized().
  TestStructureConversionOfDefaults.test_js_default_param_parses: TestStructureConversionOfDefaults#test_js_default_param_parses().
  TestStructureConversionOfDefaults.test_python_typed_default_parses: TestStructureConversionOfDefaults#test_python_typed_default_parses().
  TestStructureConversionOfDefaults.test_legacy_java_form_unchanged: TestStructureConversionOfDefaults#test_legacy_java_form_unchanged().
  TestStructureConversionOfDefaults.test_get_method_parameters_string_form: TestStructureConversionOfDefaults#test_get_method_parameters_string_form().
  TestStructureConversionOfDefaults.test_empty_and_blank_param_strings: TestStructureConversionOfDefaults#test_empty_and_blank_param_strings().
  _py_parser: _py_parser().
  _bash_parser: _bash_parser().
  TestJSDefaultParameterExtraction: TestJSDefaultParameterExtraction#
  TestPythonTypedDefaultParameterExtraction: TestPythonTypedDefaultParameterExtraction#
  TestBashParamStructuralNa: TestBashParamStructuralNa#
  TestStructureConversionOfDefaults: TestStructureConversionOfDefaults#
---
# Module: [`tests/unit/languages/test_parameter_extraction_theme_e_residual.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py)

## Classes
### `TestBashParamStructuralNa`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e_residual.py:367`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L367)
- doc: Issue #533 (Bash): Bash grammar has no formal parameter nodes.
- signature: `class TestBashParamStructuralNa:`
- members:
  - `test_function_keyword_params_empty(self)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L395) — function process() { ... } → parameters == [] (same structural reason).
  - `test_greet_params_empty(self)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L376) — greet() { echo $1 $2; } → parameters == [] (Bash has no formal params).
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`BashPlugin`](../../../tree_sitter_analyzer/languages/bash_plugin.md#BashPlugin), [`get_extractor`](../../../tree_sitter_analyzer/languages/bash_plugin.md#BashPlugin.get_extractor)

### `TestJSDefaultParameterExtraction`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e_residual.py:52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L52)
- doc: Issue #533 (JS half): assignment_pattern (param = default) was silently
- signature: `class TestJSDefaultParameterExtraction:`
- members:
  - `get_text(node: object)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L77)
  - `test_fibonacciSequence_only_default_param(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L61) — function fibonacciSequence(limit = 10) → ['limit = 10'] (1 param).
  - `test_full_plugin_fibonacciSequence_count(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L168) — End-to-end: fibonacciSequence(limit = 10) function has 1 parameter.
  - `test_full_plugin_processData_param_list(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L189) — End-to-end: processData(items, options = {}) yields exactly 2 params.
  - `test_full_plugin_processData_param_values(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L210) — End-to-end: processData params are ['items', 'options = {}'].
  - `test_generateSequence_all_defaults(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L133) — generateSequence(start = 0, end = 10) → ['start = 0', 'end = 10'] (2 params).
  - `test_processData_mixed_plain_and_default(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L98) — function processData(items, options = {}) → ['items', 'options = {}'].
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`JavaScriptPlugin`](../../../tree_sitter_analyzer/languages/javascript_plugin/plugin.md#JavaScriptPlugin), [`get_node_text_optimized`](../../../tree_sitter_analyzer/languages/javascript_plugin/_text_helpers.md#get_node_text_optimized), [`JavaScriptFunctionExtractionMixin`](../../../tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.md#JavaScriptFunctionExtractionMixin), [`get_extractor`](../../../tree_sitter_analyzer/languages/javascript_plugin/plugin.md#JavaScriptPlugin.get_extractor), [`_extract_parameters`](../../../tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.md#JavaScriptFunctionExtractionMixin._extract_parameters)  (4 test-only)
- used by: (3 test-only callers)

### `TestPythonTypedDefaultParameterExtraction`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e_residual.py:237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L237)
- doc: Issue #533 (Python half): typed_default_parameter (name: type = default)
- signature: `class TestPythonTypedDefaultParameterExtraction:`
- members:
  - `test_args_kwargs_unaffected(self)` — [`L342`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L342) — *args/**kwargs are not broken by the fix.
  - `test_cat_init_bool_default(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L285) — __init__(self, name: str, indoor: bool = True) → 3 params.
  - `test_cat_init_param_values(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L304) — params are ['self', 'name: str', 'indoor: bool = True'].
  - `test_dog_init_param_values(self)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L266) — params are ['self', 'name: str', 'breed: str = "Mixed"'].
  - `test_dog_init_three_params(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L247) — __init__(self, name: str, breed: str = 'Mixed') → 3 params.
  - `test_untyped_default_still_works(self)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L323) — Plain default_parameter (no type) still extracted: def f(x=5) → ['x=5'].
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`PythonPlugin`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin), [`get_extractor`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.get_extractor)

### `TestStructureConversionOfDefaults`
- def: [`tests/unit/languages/test_parameter_extraction_theme_e_residual.py:415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L415)
- doc: Codex P2 on #581: get_method_parameters must not whitespace-split
- signature: `class TestStructureConversionOfDefaults:`
- members:
  - `test_empty_and_blank_param_strings(self)` — [`L464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L464)
  - `test_get_method_parameters_string_form(self)` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L451)
  - `test_js_default_param_parses(self)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L419)
  - `test_legacy_java_form_unchanged(self)` — [`L441`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L441)
  - `test_python_typed_default_parses(self)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L430)
- uses (calls/refs, reference-scoped): [`_parse_string_parameter`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.md#_parse_string_parameter), [`get_method_parameters`](../../../tree_sitter_analyzer/mcp/tools/analyze_code_structure_helpers.md#get_method_parameters)

### `_MinimalExtractor`  ·  implements/extends JavaScriptFunctionExtractionMixin
- def: [`tests/unit/languages/test_parameter_extraction_theme_e_residual.py:160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L160)
- signature: `class _MinimalExtractor(JavaScriptFunctionExtractionMixin):`
- protocol/private: `_get_node_text_optimized`[`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L91), `_get_node_text_optimized`[`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L126), `_get_node_text_optimized`[`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L161)
- uses (calls/refs, reference-scoped): [`JavaScriptFunctionExtractionMixin`](../../../tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.md#JavaScriptFunctionExtractionMixin)  (1 test-only)
- used by: [`JavaScriptFunctionExtractionMixin`](../../../tree_sitter_analyzer/languages/javascript_plugin/_function_mixin.md#JavaScriptFunctionExtractionMixin)  (1 test-only)

## Functions
- `_bash_parser()` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L43)
- `_js_parser()` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L35)
- `_py_parser()` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_parameter_extraction_theme_e_residual.py#L39)

