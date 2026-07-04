---
title: 'Module: tests/unit/languages/test_js_class_field_extraction_746.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_js_class_field_extraction_746.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_js_class_field_extraction_746`/
symbols:
  _CLASS_WITH_FIELDS: _CLASS_WITH_FIELDS.
  _TREE_SITTER_AVAILABLE: _TREE_SITTER_AVAILABLE.
  pytestmark: pytestmark.
  extractor: extractor().
  TestClassFieldVariableExtraction.test_public_data_field_extracted: TestClassFieldVariableExtraction#test_public_data_field_extracted().
  TestClassFieldVariableExtraction.test_private_data_field_extracted: TestClassFieldVariableExtraction#test_private_data_field_extracted().
  TestClassFieldVariableExtraction.test_object_initialised_field_extracted: TestClassFieldVariableExtraction#test_object_initialised_field_extracted().
  TestClassFieldVariableExtraction.test_static_field_extracted: TestClassFieldVariableExtraction#test_static_field_extracted().
  TestClassFieldVariableExtraction.test_static_field_is_static: TestClassFieldVariableExtraction#test_static_field_is_static().
  TestClassFieldVariableExtraction.test_arrow_method_not_extracted_as_variable: TestClassFieldVariableExtraction#test_arrow_method_not_extracted_as_variable().
  TestClassFieldVariableExtraction.test_exact_data_field_count: TestClassFieldVariableExtraction#test_exact_data_field_count().
  TestClassFieldArrowMethodExtraction.test_arrow_method_extracted_as_function: TestClassFieldArrowMethodExtraction#test_arrow_method_extracted_as_function().
  TestClassFieldArrowMethodExtraction.test_arrow_method_not_anonymous: TestClassFieldArrowMethodExtraction#test_arrow_method_not_anonymous().
  TestClassFieldVisibility.test_public_field_has_public_visibility: TestClassFieldVisibility#test_public_field_has_public_visibility().
  TestClassFieldVisibility.test_private_field_has_private_visibility: TestClassFieldVisibility#test_private_field_has_private_visibility().
  TestClassFieldInitializer.test_object_initializer_preserved: TestClassFieldInitializer#test_object_initializer_preserved().
  js_parser: js_parser().
  TestClassFieldVariableExtraction: TestClassFieldVariableExtraction#
  TestClassFieldArrowMethodExtraction: TestClassFieldArrowMethodExtraction#
  TestClassFieldVisibility: TestClassFieldVisibility#
  TestClassFieldInitializer: TestClassFieldInitializer#
---
# Module: [`tests/unit/languages/test_js_class_field_extraction_746.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py)

## Classes
### `TestClassFieldArrowMethodExtraction`
- def: [`tests/unit/languages/test_js_class_field_extraction_746.py:128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L128)
- doc: Issue #746 — arrow-function class fields must be Functions with correct name.
- signature: `class TestClassFieldArrowMethodExtraction:`
- members:
  - `test_arrow_method_extracted_as_function(self, extractor, js_parser)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L131) — handleClick = () => {} must appear as a Function.
  - `test_arrow_method_not_anonymous(self, extractor, js_parser)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L140) — handleClick must NOT have name 'anonymous'.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestClassFieldInitializer`
- def: [`tests/unit/languages/test_js_class_field_extraction_746.py:177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L177)
- doc: Codex P2 on #746 — non-primitive initializers must not be silently dropped.
- signature: `class TestClassFieldInitializer:`
- members:
  - `test_object_initializer_preserved(self, extractor, js_parser)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L180) — state = { running: false } must have a non-None initializer.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestClassFieldVariableExtraction`
- def: [`tests/unit/languages/test_js_class_field_extraction_746.py:59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L59)
- doc: Issue #746 — public / private data fields must be extracted as Variable.
- signature: `class TestClassFieldVariableExtraction:`
- members:
  - `test_arrow_method_not_extracted_as_variable(self, extractor, js_parser)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L104) — handleClick (arrow fn) must NOT appear as a Variable — it is a Function.
  - `test_exact_data_field_count(self, extractor, js_parser)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L113) — Exactly 4 data fields (count, #privateCounter, state, defaultStep).
  - `test_object_initialised_field_extracted(self, extractor, js_parser)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L78) — state = { running: false } must appear as a Variable named 'state'.
  - `test_private_data_field_extracted(self, extractor, js_parser)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L69) — #privateCounter = 0 must appear as a Variable named '#privateCounter'.
  - `test_public_data_field_extracted(self, extractor, js_parser)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L62) — count = 0 must appear as a Variable named 'count'.
  - `test_static_field_extracted(self, extractor, js_parser)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L85) — static defaultStep = 1 must appear as a Variable named 'defaultStep'.
  - `test_static_field_is_static(self, extractor, js_parser)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L94) — static defaultStep must have is_static=True.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestClassFieldVisibility`
- def: [`tests/unit/languages/test_js_class_field_extraction_746.py:150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L150)
- doc: Codex P2 on #746 — visibility must reflect JS privacy rules.
- signature: `class TestClassFieldVisibility:`
- members:
  - `test_private_field_has_private_visibility(self, extractor, js_parser)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L164) — #privateCounter = 0 is private; visibility must be 'private'.
  - `test_public_field_has_public_visibility(self, extractor, js_parser)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L153) — count = 0 is public; visibility must be 'public' not 'private'.
- uses (calls/refs, reference-scoped): (1 test-only callers)

## Functions
- `extractor()` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L55)
- `js_parser()` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L49)

## Module values
- `_CLASS_WITH_FIELDS` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L35)
- `_TREE_SITTER_AVAILABLE` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L22)
- `pytestmark` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_class_field_extraction_746.py#L30)

