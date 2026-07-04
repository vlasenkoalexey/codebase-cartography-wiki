---
title: 'Module: tests/unit/languages/test_js_class_field_bugs_890_891_892.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_js_class_field_bugs_890_891_892.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_js_class_field_bugs_890_891_892`/
symbols:
  _TREE_SITTER_AVAILABLE: _TREE_SITTER_AVAILABLE.
  _ARROW_CLASS: _ARROW_CLASS.
  _COMPUTED_STRING_NUMERIC_FIELDS: _COMPUTED_STRING_NUMERIC_FIELDS.
  pytestmark: pytestmark.
  extractor: extractor().
  plugin: plugin().
  TestBug890ArrowFieldIsMethod.test_arrow_field_is_method_true: TestBug890ArrowFieldIsMethod#test_arrow_field_is_method_true().
  TestBug890ArrowFieldIsMethod.test_arrow_field_parent_class_set: TestBug890ArrowFieldIsMethod#test_arrow_field_parent_class_set().
  TestBug890ArrowFieldIsMethod.test_async_arrow_field_is_method_true: TestBug890ArrowFieldIsMethod#test_async_arrow_field_is_method_true().
  TestBug890ArrowFieldIsMethod.test_async_arrow_field_parent_class_set: TestBug890ArrowFieldIsMethod#test_async_arrow_field_parent_class_set().
  TestBug890ArrowFieldIsMethod.test_is_arrow_still_true: TestBug890ArrowFieldIsMethod#test_is_arrow_still_true().
  TestBug891FieldDefinitionQuerySurface.test_variables_query_string_includes_field_definition: TestBug891FieldDefinitionQuerySurface#test_variables_query_string_includes_field_definition().
  TestBug891FieldDefinitionQuerySurface.test_fields_only_file_returns_variables: TestBug891FieldDefinitionQuerySurface#test_fields_only_file_returns_variables().
  TestBug892ComputedStringNumericFieldNames.test_computed_property_name_extracted: TestBug892ComputedStringNumericFieldNames#test_computed_property_name_extracted().
  TestBug892ComputedStringNumericFieldNames.test_string_key_field_extracted: TestBug892ComputedStringNumericFieldNames#test_string_key_field_extracted().
  TestBug892ComputedStringNumericFieldNames.test_numeric_key_field_extracted: TestBug892ComputedStringNumericFieldNames#test_numeric_key_field_extracted().
  TestBug892ComputedStringNumericFieldNames.test_normal_field_still_extracted: TestBug892ComputedStringNumericFieldNames#test_normal_field_still_extracted().
  TestBug892ComputedStringNumericFieldNames.test_exact_variable_count_fancy_class: TestBug892ComputedStringNumericFieldNames#test_exact_variable_count_fancy_class().
  _ONLY_CLASS_FIELDS: _ONLY_CLASS_FIELDS.
  js_parser: js_parser().
  TestBug890ArrowFieldIsMethod: TestBug890ArrowFieldIsMethod#
  TestBug891FieldDefinitionQuerySurface: TestBug891FieldDefinitionQuerySurface#
  TestBug891FieldDefinitionQuerySurface.test_element_categories_variable_includes_field_definition: TestBug891FieldDefinitionQuerySurface#test_element_categories_variable_includes_field_definition().
  TestBug891FieldDefinitionQuerySurface.test_element_categories_variables_plural_includes_field_definition: TestBug891FieldDefinitionQuerySurface#test_element_categories_variables_plural_includes_field_definition().
  TestBug892ComputedStringNumericFieldNames: TestBug892ComputedStringNumericFieldNames#
---
# Module: [`tests/unit/languages/test_js_class_field_bugs_890_891_892.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py)

## Classes
### `TestBug890ArrowFieldIsMethod`
- def: [`tests/unit/languages/test_js_class_field_bugs_890_891_892.py:101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L101)
- doc: Arrow-function class fields must be extracted with is_method=True
- signature: `class TestBug890ArrowFieldIsMethod:`
- members:
  - `test_arrow_field_is_method_true(self, extractor, js_parser)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L105) — `build = () => {}` inside a class must yield is_method=True.
  - `test_arrow_field_parent_class_set(self, extractor, js_parser)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L118) — `build = () => {}` inside class Widget must have parent_class='Widget'.
  - `test_async_arrow_field_is_method_true(self, extractor, js_parser)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L131) — `render = async (ctx) => {}` must also get is_method=True.
  - `test_async_arrow_field_parent_class_set(self, extractor, js_parser)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L144) — `render = async (ctx) => {}` must have parent_class='Widget'.
  - `test_is_arrow_still_true(self, extractor, js_parser)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L157) — Arrow class fields must keep is_arrow=True alongside is_method=True.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestBug891FieldDefinitionQuerySurface`
- def: [`tests/unit/languages/test_js_class_field_bugs_890_891_892.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L173)
- doc: field_definition must appear in VARIABLES query string and in
- signature: `class TestBug891FieldDefinitionQuerySurface:`
- members:
  - `test_element_categories_variable_includes_field_definition(self, plugin)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L185) — plugin.get_element_categories()['variable'] must include 'field_definition'.
  - `test_element_categories_variables_plural_includes_field_definition(self, plugin)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L194) — plugin.get_element_categories()['variables'] must also include 'field_definition'.
  - `test_fields_only_file_returns_variables(self, extractor, js_parser)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L205) — A file containing only class fields must return > 0 variables.
  - `test_variables_query_string_includes_field_definition(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L178) — The VARIABLES legacy query string must contain 'field_definition'.
- uses (calls/refs, reference-scoped): [`VARIABLES`](../../../tree_sitter_analyzer/queries/javascript.md#VARIABLES)  (1 test-only)

### `TestBug892ComputedStringNumericFieldNames`
- def: [`tests/unit/languages/test_js_class_field_bugs_890_891_892.py:220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L220)
- doc: Computed, string, and numeric class field names must be extracted.
- signature: `class TestBug892ComputedStringNumericFieldNames:`
- members:
  - `test_computed_property_name_extracted(self, extractor, js_parser)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L223) — `['computed'] = 'yes'` must appear as a variable (name contains 'computed').
  - `test_exact_variable_count_fancy_class(self, extractor, js_parser)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L260) — All four fields in Fancy must be extracted (computed, string, numeric, plain).
  - `test_normal_field_still_extracted(self, extractor, js_parser)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L253) — `name = 'normal'` (plain property_identifier) must still be extracted.
  - `test_numeric_key_field_extracted(self, extractor, js_parser)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L246) — `0 = 'zero'` must appear as a variable (name is '0').
  - `test_string_key_field_extracted(self, extractor, js_parser)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L235) — `'string_key' = 'value'` must appear as a variable.
- uses (calls/refs, reference-scoped): (1 test-only callers)

## Functions
- `extractor()` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L55)
- `js_parser()` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L49)
- `plugin()` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L60)

## Module values
- `_ARROW_CLASS` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L68)
- `_COMPUTED_STRING_NUMERIC_FIELDS` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L86)
- `_ONLY_CLASS_FIELDS` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L79)
- `_TREE_SITTER_AVAILABLE` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L28)
- `pytestmark` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_bugs_890_891_892.py#L38)

