---
title: 'Module: tests/unit/languages/test_go_bugs_749_750.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_bugs_749_750.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_bugs_749_750`/
symbols:
  _parse_and_extract: _parse_and_extract().
  TestGenericReceiverMultilineAndUnnamed.test_multiline_generic_receiver_type_strips_type_params: TestGenericReceiverMultilineAndUnnamed#test_multiline_generic_receiver_type_strips_type_params().
  TestGenericReceiverMultilineAndUnnamed.test_unnamed_generic_receiver_keeps_type: TestGenericReceiverMultilineAndUnnamed#test_unnamed_generic_receiver_keeps_type().
  TestNonGenericReceiverUnchanged.test_pointer_receiver_unchanged: TestNonGenericReceiverUnchanged#test_pointer_receiver_unchanged().
  TestNonGenericReceiverUnchanged.test_value_receiver_unchanged: TestNonGenericReceiverUnchanged#test_value_receiver_unchanged().
  TestExtractMethodReceiverRegex._extract: TestExtractMethodReceiverRegex#_extract().
  TestInterfaceSpecIsAbstract.test_read_is_abstract: TestInterfaceSpecIsAbstract#test_read_is_abstract().
  TestInterfaceSpecIsAbstract.test_close_is_abstract: TestInterfaceSpecIsAbstract#test_close_is_abstract().
  TestInterfaceSpecIsAbstract.test_receiver_type_still_set: TestInterfaceSpecIsAbstract#test_receiver_type_still_set().
  TestInterfaceSpecIsAbstract.test_receiver_is_none: TestInterfaceSpecIsAbstract#test_receiver_is_none().
  TestInterfaceSpecIsAbstract.test_is_method_true: TestInterfaceSpecIsAbstract#test_is_method_true().
  TestMultiMethodInterface.test_all_three_specs_are_abstract: TestMultiMethodInterface#test_all_three_specs_are_abstract().
  TestGenericReceiverExtraction.test_push_receiver_name: TestGenericReceiverExtraction#test_push_receiver_name().
  TestGenericReceiverExtraction.test_push_receiver_type_strips_type_param: TestGenericReceiverExtraction#test_push_receiver_type_strips_type_param().
  TestGenericReceiverExtraction.test_pop_receiver_name: TestGenericReceiverExtraction#test_pop_receiver_name().
  TestGenericReceiverExtraction.test_pop_receiver_type_strips_type_param: TestGenericReceiverExtraction#test_pop_receiver_type_strips_type_param().
  TestGenericReceiverExtraction.test_is_method_true_for_generic_methods: TestGenericReceiverExtraction#test_is_method_true_for_generic_methods().
  TestGenericReceiverValueType.test_value_receiver_name: TestGenericReceiverValueType#test_value_receiver_name().
  TestGenericReceiverValueType.test_value_receiver_type_strips_type_params: TestGenericReceiverValueType#test_value_receiver_type_strips_type_params().
  TestInterfaceSpecIsAbstract.test_concrete_method_not_abstract: TestInterfaceSpecIsAbstract#test_concrete_method_not_abstract().
  TestInterfaceSpecIsAbstract.SRC: TestInterfaceSpecIsAbstract#SRC.
  TestGenericReceiverExtraction.SRC: TestGenericReceiverExtraction#SRC.
  TestExtractMethodReceiverRegex.test_pointer_generic_two_type_params: TestExtractMethodReceiverRegex#test_pointer_generic_two_type_params().
  TestExtractMethodReceiverRegex.test_pointer_generic_single_type_param: TestExtractMethodReceiverRegex#test_pointer_generic_single_type_param().
  TestExtractMethodReceiverRegex.test_value_generic: TestExtractMethodReceiverRegex#test_value_generic().
  TestExtractMethodReceiverRegex.test_value_generic_multiline: TestExtractMethodReceiverRegex#test_value_generic_multiline().
  TestExtractMethodReceiverRegex.test_unnamed_pointer_generic: TestExtractMethodReceiverRegex#test_unnamed_pointer_generic().
  TestExtractMethodReceiverRegex.test_unnamed_pointer_generic_multiline: TestExtractMethodReceiverRegex#test_unnamed_pointer_generic_multiline().
  TestExtractMethodReceiverRegex.test_non_generic_pointer_unchanged: TestExtractMethodReceiverRegex#test_non_generic_pointer_unchanged().
  TestExtractMethodReceiverRegex.test_non_generic_value_unchanged: TestExtractMethodReceiverRegex#test_non_generic_value_unchanged().
  TestExtractMethodReceiverRegex.test_no_receiver_returns_none: TestExtractMethodReceiverRegex#test_no_receiver_returns_none().
  TestGenericReceiverValueType.SRC: TestGenericReceiverValueType#SRC.
  TestGenericReceiverMultilineAndUnnamed.SRC: TestGenericReceiverMultilineAndUnnamed#SRC.
  TestNonGenericReceiverUnchanged.SRC: TestNonGenericReceiverUnchanged#SRC.
  TestMultiMethodInterface.SRC: TestMultiMethodInterface#SRC.
  TestInterfaceSpecIsAbstract: TestInterfaceSpecIsAbstract#
  TestMultiMethodInterface: TestMultiMethodInterface#
  TestGenericReceiverExtraction: TestGenericReceiverExtraction#
  TestGenericReceiverValueType: TestGenericReceiverValueType#
  TestGenericReceiverMultilineAndUnnamed: TestGenericReceiverMultilineAndUnnamed#
  TestNonGenericReceiverUnchanged: TestNonGenericReceiverUnchanged#
  TestExtractMethodReceiverRegex: TestExtractMethodReceiverRegex#
---
# Module: [`tests/unit/languages/test_go_bugs_749_750.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py)

## Classes
### `TestExtractMethodReceiverRegex`
- def: [`tests/unit/languages/test_go_bugs_749_750.py:281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L281)
- doc: Unit tests for the extract_method_receiver helper (#750).
- signature: `class TestExtractMethodReceiverRegex:`
- members:
  - `_extract(self, receiver_text: str)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L284) — Invoke extract_method_receiver with a fake node yielding receiver_text.
  - `test_no_receiver_returns_none(self)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L340)
  - `test_non_generic_pointer_unchanged(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L330)
  - `test_non_generic_value_unchanged(self)` — [`L335`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L335)
  - `test_pointer_generic_single_type_param(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L305)
  - `test_pointer_generic_two_type_params(self)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L300)
  - `test_unnamed_pointer_generic(self)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L320)
  - `test_unnamed_pointer_generic_multiline(self)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L325)
  - `test_value_generic(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L310)
  - `test_value_generic_multiline(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L315)
- uses (calls/refs, reference-scoped): [`extract_method_receiver`](../../../tree_sitter_analyzer/languages/_go_common_helpers.md#extract_method_receiver)

### `TestGenericReceiverExtraction`
- def: [`tests/unit/languages/test_go_bugs_749_750.py:130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L130)
- doc: Methods with generic receivers must have receiver and receiver_type (#750).
- signature: `class TestGenericReceiverExtraction:`
- members:
  - `test_is_method_true_for_generic_methods(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L181)
  - `test_pop_receiver_name(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L170)
  - `test_pop_receiver_type_strips_type_param(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L176)
  - `test_push_receiver_name(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L155)
  - `test_push_receiver_type_strips_type_param(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L163)
  - `SRC` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L133)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`receiver`](../../../tree_sitter_analyzer/models/base.md#Function.receiver)  (1 test-only)

### `TestGenericReceiverMultilineAndUnnamed`
- def: [`tests/unit/languages/test_go_bugs_749_750.py:217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L217)
- doc: Generic receivers may be multiline or omit the receiver variable (#958).
- signature: `class TestGenericReceiverMultilineAndUnnamed:`
- members:
  - `test_multiline_generic_receiver_type_strips_type_params(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L238)
  - `test_unnamed_generic_receiver_keeps_type(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L244)
  - `SRC` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L220)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`receiver`](../../../tree_sitter_analyzer/models/base.md#Function.receiver)  (1 test-only)

### `TestGenericReceiverValueType`
- def: [`tests/unit/languages/test_go_bugs_749_750.py:188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L188)
- doc: Value (non-pointer) generic receiver: `(s Stack[T])`.
- signature: `class TestGenericReceiverValueType:`
- members:
  - `test_value_receiver_name(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L204)
  - `test_value_receiver_type_strips_type_params(self)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L210)
  - `SRC` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L191)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`receiver`](../../../tree_sitter_analyzer/models/base.md#Function.receiver)  (1 test-only)

### `TestInterfaceSpecIsAbstract`
- def: [`tests/unit/languages/test_go_bugs_749_750.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L43)
- doc: Interface method signatures must carry is_abstract=True (#749).
- signature: `class TestInterfaceSpecIsAbstract:`
- members:
  - `test_close_is_abstract(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L61)
  - `test_concrete_method_not_abstract(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L87) — Concrete method on a struct must NOT have is_abstract=True.
  - `test_is_method_true(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L81)
  - `test_read_is_abstract(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L55)
  - `test_receiver_is_none(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L74) — Interface specs have no receiver variable.
  - `test_receiver_type_still_set(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L67) — The #588 fix (receiver_type = interface name) must be preserved.
  - `SRC` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L46)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`is_abstract`](../../../tree_sitter_analyzer/models/base.md#Function.is_abstract), [`receiver`](../../../tree_sitter_analyzer/models/base.md#Function.receiver)  (1 test-only)

### `TestMultiMethodInterface`
- def: [`tests/unit/languages/test_go_bugs_749_750.py:102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L102)
- doc: Multiple interface specs all carry is_abstract=True.
- signature: `class TestMultiMethodInterface:`
- members:
  - `test_all_three_specs_are_abstract(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L115)
  - `SRC` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L105)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`is_abstract`](../../../tree_sitter_analyzer/models/base.md#Function.is_abstract)  (1 test-only)

### `TestNonGenericReceiverUnchanged`
- def: [`tests/unit/languages/test_go_bugs_749_750.py:251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L251)
- doc: Existing non-generic receivers must not be affected by the fix.
- signature: `class TestNonGenericReceiverUnchanged:`
- members:
  - `test_pointer_receiver_unchanged(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L263)
  - `test_value_receiver_unchanged(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L269)
  - `SRC` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L254)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`receiver`](../../../tree_sitter_analyzer/models/base.md#Function.receiver)  (1 test-only)

## Functions
- `_parse_and_extract(src: str)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_bugs_749_750.py#L24) — Run the Go extractor over ``src`` and return all functions.

