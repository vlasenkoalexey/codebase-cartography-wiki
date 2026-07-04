---
title: 'Module: tests/unit/languages/test_javascript_bugs_747_748.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_javascript_bugs_747_748.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_javascript_bugs_747_748`/
symbols:
  _TREE_SITTER_AVAILABLE: _TREE_SITTER_AVAILABLE.
  pytestmark: pytestmark.
  extractor: extractor().
  js_parser: js_parser().
  TestDestructuringPhantomFields: TestDestructuringPhantomFields#
  TestDestructuringPhantomFields.test_object_destructuring_rhs_not_extracted: TestDestructuringPhantomFields#test_object_destructuring_rhs_not_extracted().
  TestDestructuringPhantomFields.test_array_destructuring_rhs_not_extracted: TestDestructuringPhantomFields#test_array_destructuring_rhs_not_extracted().
  TestDestructuringPhantomFields.test_plain_variable_still_extracted: TestDestructuringPhantomFields#test_plain_variable_still_extracted().
  TestDestructuringPhantomFields.test_mixed_declarations: TestDestructuringPhantomFields#test_mixed_declarations().
  TestDestructuringPhantomFields.test_object_destructuring_empty_result: TestDestructuringPhantomFields#test_object_destructuring_empty_result().
  TestComputedPropertyMethodName: TestComputedPropertyMethodName#
  TestComputedPropertyMethodName.test_simple_computed_identifier: TestComputedPropertyMethodName#test_simple_computed_identifier().
  TestComputedPropertyMethodName.test_member_expression_computed_name: TestComputedPropertyMethodName#test_member_expression_computed_name().
  TestComputedPropertyMethodName.test_regular_method_name_unchanged: TestComputedPropertyMethodName#test_regular_method_name_unchanged().
  TestComputedPropertyMethodName.test_mixed_class_methods: TestComputedPropertyMethodName#test_mixed_class_methods().
---
# Module: [`tests/unit/languages/test_javascript_bugs_747_748.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py)

## Classes
### `TestComputedPropertyMethodName`
- def: [`tests/unit/languages/test_javascript_bugs_747_748.py:105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L105)
- doc: Bug #748: method_definition with computed_property_name must yield non-empty name.
- signature: `class TestComputedPropertyMethodName:`
- members:
  - `test_member_expression_computed_name(self, extractor, js_parser)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L117) — class Foo { [Symbol.iterator]() {} }  →  method name is '[Symbol.iterator]'.
  - `test_mixed_class_methods(self, extractor, js_parser)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L135) — Class with computed and regular methods: all names are non-empty.
  - `test_regular_method_name_unchanged(self, extractor, js_parser)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L126) — Regular method name is still extracted correctly (regression guard).
  - `test_simple_computed_identifier(self, extractor, js_parser)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L108) — class Foo { [post]() {} }  →  method name is '[post]', not ''.

### `TestDestructuringPhantomFields`
- def: [`tests/unit/languages/test_javascript_bugs_747_748.py:49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L49)
- doc: Bug #747: RHS identifier of destructuring must not be extracted as a variable.
- signature: `class TestDestructuringPhantomFields:`
- members:
  - `test_array_destructuring_rhs_not_extracted(self, extractor, js_parser)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L62) — const [x, y] = arr  →  no variable named 'arr' extracted.
  - `test_mixed_declarations(self, extractor, js_parser)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L80) — Mix of destructuring and plain declarations: only plain ones are extracted.
  - `test_object_destructuring_empty_result(self, extractor, js_parser)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L90) — A lone destructuring produces zero extracted variables (no phantom names).
  - `test_object_destructuring_rhs_not_extracted(self, extractor, js_parser)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L52) — const { a, b } = obj  →  no variable named 'obj' extracted.
  - `test_plain_variable_still_extracted(self, extractor, js_parser)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L72) — const name = 'hello'  →  variable 'name' IS extracted (regression guard).

## Functions
- `extractor()` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L40)
- `js_parser()` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L34)

## Module values
- `_TREE_SITTER_AVAILABLE` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L20)
- `pytestmark` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_bugs_747_748.py#L28)

