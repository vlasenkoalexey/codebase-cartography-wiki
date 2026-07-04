---
title: 'Module: tests/unit/languages/test_javascript_plugin_parsing.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_javascript_plugin_parsing.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_javascript_plugin_parsing`/
symbols:
  TestGetNodeTypeForElement.test_arrow_function: TestGetNodeTypeForElement#test_arrow_function().
  TestGetNodeTypeForElement.test_method: TestGetNodeTypeForElement#test_method().
  TestGetNodeTypeForElement.test_regular_function: TestGetNodeTypeForElement#test_regular_function().
  TestGetNodeTypeForElement.test_class_element: TestGetNodeTypeForElement#test_class_element().
  TestGetNodeTypeForElement.test_variable_element: TestGetNodeTypeForElement#test_variable_element().
  TestGetNodeTypeForElement.test_import_element: TestGetNodeTypeForElement#test_import_element().
  TestExtractDynamicImport.test_dynamic_import: TestExtractDynamicImport#test_dynamic_import().
  extractor: extractor().
  plugin: plugin().
  TestParseImportStatement: TestParseImportStatement#
  TestParseImportStatement.test_namespace_import: TestParseImportStatement#test_namespace_import().
  TestParseImportStatement.test_named_imports: TestParseImportStatement#test_named_imports().
  TestParseImportStatement.test_default_import: TestParseImportStatement#test_default_import().
  TestParseImportStatement.test_no_source_returns_none: TestParseImportStatement#test_no_source_returns_none().
  TestParseImportStatement.test_exception_returns_none: TestParseImportStatement#test_exception_returns_none().
  TestParseExportStatement: TestParseExportStatement#
  TestParseExportStatement.test_default_export_with_name: TestParseExportStatement#test_default_export_with_name().
  TestParseExportStatement.test_default_export_no_name: TestParseExportStatement#test_default_export_no_name().
  TestParseExportStatement.test_named_exports: TestParseExportStatement#test_named_exports().
  TestParseExportStatement.test_direct_export_function: TestParseExportStatement#test_direct_export_function().
  TestParseExportStatement.test_direct_export_class: TestParseExportStatement#test_direct_export_class().
  TestParseExportStatement.test_direct_export_const: TestParseExportStatement#test_direct_export_const().
  TestParseExportStatement.test_direct_export_unknown: TestParseExportStatement#test_direct_export_unknown().
  TestParseExportStatement.test_invalid_export_returns_none: TestParseExportStatement#test_invalid_export_returns_none().
  TestParseExportStatement.test_non_export_returns_none: TestParseExportStatement#test_non_export_returns_none().
  TestParseExportStatement.test_exception_returns_none: TestParseExportStatement#test_exception_returns_none().
  TestExtractDynamicImport: TestExtractDynamicImport#
  TestExtractDynamicImport.test_dynamic_import_not_found: TestExtractDynamicImport#test_dynamic_import_not_found().
  TestExtractDynamicImport.test_dynamic_import_exception: TestExtractDynamicImport#test_dynamic_import_exception().
  TestExtractCommonjsRequires: TestExtractCommonjsRequires#
  TestExtractCommonjsRequires.test_const_require: TestExtractCommonjsRequires#test_const_require().
  TestExtractCommonjsRequires.test_let_require: TestExtractCommonjsRequires#test_let_require().
  TestExtractCommonjsRequires.test_var_require: TestExtractCommonjsRequires#test_var_require().
  TestExtractCommonjsRequires.test_multiple_requires: TestExtractCommonjsRequires#test_multiple_requires().
  TestExtractCommonjsRequires.test_no_requires: TestExtractCommonjsRequires#test_no_requires().
  TestExtractCommonjsExports: TestExtractCommonjsExports#
  TestExtractCommonjsExports.test_module_exports_assignment: TestExtractCommonjsExports#test_module_exports_assignment().
  TestExtractCommonjsExports.test_module_exports_property: TestExtractCommonjsExports#test_module_exports_property().
  TestExtractCommonjsExports.test_exports_property: TestExtractCommonjsExports#test_exports_property().
  TestExtractCommonjsExports.test_no_commonjs_exports: TestExtractCommonjsExports#test_no_commonjs_exports().
  TestInferTypeFromValue: TestInferTypeFromValue#
  TestInferTypeFromValue.test_string_double_quotes: TestInferTypeFromValue#test_string_double_quotes().
  TestInferTypeFromValue.test_string_single_quotes: TestInferTypeFromValue#test_string_single_quotes().
  TestInferTypeFromValue.test_string_template_literal: TestInferTypeFromValue#test_string_template_literal().
  TestInferTypeFromValue.test_boolean_true: TestInferTypeFromValue#test_boolean_true().
  TestInferTypeFromValue.test_boolean_false: TestInferTypeFromValue#test_boolean_false().
  TestInferTypeFromValue.test_null: TestInferTypeFromValue#test_null().
  TestInferTypeFromValue.test_undefined: TestInferTypeFromValue#test_undefined().
  TestInferTypeFromValue.test_array: TestInferTypeFromValue#test_array().
  TestInferTypeFromValue.test_object: TestInferTypeFromValue#test_object().
  TestInferTypeFromValue.test_number: TestInferTypeFromValue#test_number().
  TestInferTypeFromValue.test_float: TestInferTypeFromValue#test_float().
  TestInferTypeFromValue.test_negative_number: TestInferTypeFromValue#test_negative_number().
  TestInferTypeFromValue.test_function_value: TestInferTypeFromValue#test_function_value().
  TestInferTypeFromValue.test_arrow_function: TestInferTypeFromValue#test_arrow_function().
  TestInferTypeFromValue.test_none_value: TestInferTypeFromValue#test_none_value().
  TestInferTypeFromValue.test_empty_value: TestInferTypeFromValue#test_empty_value().
  TestInferTypeFromValue.test_unknown_value: TestInferTypeFromValue#test_unknown_value().
  TestGetVariableKind: TestGetVariableKind#
  TestGetVariableKind.test_const: TestGetVariableKind#test_const().
  TestGetVariableKind.test_let: TestGetVariableKind#test_let().
  TestGetVariableKind.test_var: TestGetVariableKind#test_var().
  TestGetVariableKind.test_dict_input: TestGetVariableKind#test_dict_input().
  TestGetVariableKind.test_dict_empty: TestGetVariableKind#test_dict_empty().
  TestGetVariableKind.test_empty_string: TestGetVariableKind#test_empty_string().
  TestGetVariableKind.test_unknown_prefix: TestGetVariableKind#test_unknown_prefix().
  TestCleanJsdoc: TestCleanJsdoc#
  TestCleanJsdoc.test_basic_jsdoc: TestCleanJsdoc#test_basic_jsdoc().
  TestCleanJsdoc.test_empty_jsdoc: TestCleanJsdoc#test_empty_jsdoc().
  TestCleanJsdoc.test_jsdoc_with_params: TestCleanJsdoc#test_jsdoc_with_params().
  TestGetNodeTypeForElement: TestGetNodeTypeForElement#
  TestGetNodeTypeForElement.test_unknown_element: TestGetNodeTypeForElement#test_unknown_element().
---
# Module: [`tests/unit/languages/test_javascript_plugin_parsing.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py)

## Classes
### `TestCleanJsdoc`
- def: [`tests/unit/languages/test_javascript_plugin_parsing.py:320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L320)
- signature: `class TestCleanJsdoc:`
- members:
  - `test_basic_jsdoc(self, extractor)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L321)
  - `test_empty_jsdoc(self, extractor)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L326)
  - `test_jsdoc_with_params(self, extractor)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L329)

### `TestExtractCommonjsExports`
- def: [`tests/unit/languages/test_javascript_plugin_parsing.py:215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L215)
- signature: `class TestExtractCommonjsExports:`
- members:
  - `test_exports_property(self, extractor)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L230)
  - `test_module_exports_assignment(self, extractor)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L216)
  - `test_module_exports_property(self, extractor)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L223)
  - `test_no_commonjs_exports(self, extractor)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L237)

### `TestExtractCommonjsRequires`
- def: [`tests/unit/languages/test_javascript_plugin_parsing.py:179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L179)
- signature: `class TestExtractCommonjsRequires:`
- members:
  - `test_const_require(self, extractor)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L180)
  - `test_let_require(self, extractor)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L188)
  - `test_multiple_requires(self, extractor)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L202)
  - `test_no_requires(self, extractor)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L208)
  - `test_var_require(self, extractor)` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L195)

### `TestExtractDynamicImport`
- def: [`tests/unit/languages/test_javascript_plugin_parsing.py:135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L135)
- signature: `class TestExtractDynamicImport:`
- members:
  - `test_dynamic_import(self, extractor)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L136)
  - `test_dynamic_import_exception(self, extractor)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L169)
  - `test_dynamic_import_not_found(self, extractor)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L154)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`module_path`](../../../tree_sitter_analyzer/models/base.md#Import.module_path)

### `TestGetNodeTypeForElement`
- def: [`tests/unit/languages/test_javascript_plugin_parsing.py:336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L336)
- signature: `class TestGetNodeTypeForElement:`
- members:
  - `test_arrow_function(self, plugin)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L337)
  - `test_class_element(self, plugin)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L369)
  - `test_import_element(self, plugin)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L389)
  - `test_method(self, plugin)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L348)
  - `test_regular_function(self, plugin)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L359)
  - `test_unknown_element(self, plugin)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L399)
  - `test_variable_element(self, plugin)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L379)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`Class`](../../../tree_sitter_analyzer/models/base.md#Class), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`is_arrow`](../../../tree_sitter_analyzer/models/base.md#Function.is_arrow)

### `TestGetVariableKind`
- def: [`tests/unit/languages/test_javascript_plugin_parsing.py:297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L297)
- signature: `class TestGetVariableKind:`
- members:
  - `test_const(self, extractor)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L298)
  - `test_dict_empty(self, extractor)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L310)
  - `test_dict_input(self, extractor)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L307)
  - `test_empty_string(self, extractor)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L313)
  - `test_let(self, extractor)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L301)
  - `test_unknown_prefix(self, extractor)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L316)
  - `test_var(self, extractor)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L304)

### `TestInferTypeFromValue`
- def: [`tests/unit/languages/test_javascript_plugin_parsing.py:244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L244)
- signature: `class TestInferTypeFromValue:`
- members:
  - `test_array(self, extractor)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L266)
  - `test_arrow_function(self, extractor)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L284)
  - `test_boolean_false(self, extractor)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L257)
  - `test_boolean_true(self, extractor)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L254)
  - `test_empty_value(self, extractor)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L290)
  - `test_float(self, extractor)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L275)
  - `test_function_value(self, extractor)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L281)
  - `test_negative_number(self, extractor)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L278)
  - `test_none_value(self, extractor)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L287)
  - `test_null(self, extractor)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L260)
  - `test_number(self, extractor)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L272)
  - `test_object(self, extractor)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L269)
  - `test_string_double_quotes(self, extractor)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L245)
  - `test_string_single_quotes(self, extractor)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L248)
  - `test_string_template_literal(self, extractor)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L251)
  - `test_undefined(self, extractor)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L263)
  - `test_unknown_value(self, extractor)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L293)

### `TestParseExportStatement`
- def: [`tests/unit/languages/test_javascript_plugin_parsing.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L67)
- signature: `class TestParseExportStatement:`
- members:
  - `test_default_export_no_name(self, extractor)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L76)
  - `test_default_export_with_name(self, extractor)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L68)
  - `test_direct_export_class(self, extractor)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L101)
  - `test_direct_export_const(self, extractor)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L108)
  - `test_direct_export_function(self, extractor)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L93)
  - `test_direct_export_unknown(self, extractor)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L115)
  - `test_exception_returns_none(self, extractor)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L130)
  - `test_invalid_export_returns_none(self, extractor)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L122)
  - `test_named_exports(self, extractor)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L84)
  - `test_non_export_returns_none(self, extractor)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L126)

### `TestParseImportStatement`
- def: [`tests/unit/languages/test_javascript_plugin_parsing.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L27)
- signature: `class TestParseImportStatement:`
- members:
  - `test_default_import(self, extractor)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L49)
  - `test_exception_returns_none(self, extractor)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L62)
  - `test_named_imports(self, extractor)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L37)
  - `test_namespace_import(self, extractor)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L28)
  - `test_no_source_returns_none(self, extractor)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L58)

## Functions
- `extractor()` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L18)
- `plugin()` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_parsing.py#L23)

