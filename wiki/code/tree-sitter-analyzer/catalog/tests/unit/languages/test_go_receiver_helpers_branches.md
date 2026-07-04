---
title: 'Module: tests/unit/languages/test_go_receiver_helpers_branches.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_receiver_helpers_branches.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_receiver_helpers_branches`/
symbols:
  _FakeNode: _FakeNode#
  _FakeMethod: _FakeMethod#
  TestExtractMethodReceiver.test_text_fallback_when_no_parameter_declaration_child: TestExtractMethodReceiver#test_text_fallback_when_no_parameter_declaration_child().
  TestExtractMethodReceiver.test_parameter_declaration_qualified_type: TestExtractMethodReceiver#test_parameter_declaration_qualified_type().
  TestExtractMethodReceiver.test_none_receiver_node: TestExtractMethodReceiver#test_none_receiver_node().
  TestExtractReceiverParts.test_qualified_type_with_generic_suffix_stripped: TestExtractReceiverParts#test_qualified_type_with_generic_suffix_stripped().
  TestExtractReceiverParts.test_no_recognized_type_returns_none_none: TestExtractReceiverParts#test_no_recognized_type_returns_none_none().
  TestExtractReceiverParts.test_unrelated_child_is_skipped: TestExtractReceiverParts#test_unrelated_child_is_skipped().
  TestFindReceiverTypeGo.test_qualified_type_receiver: TestFindReceiverTypeGo#test_qualified_type_receiver().
  TestFindReceiverTypeGo.test_generic_pointer_receiver_strips_pointer_and_param: TestFindReceiverTypeGo#test_generic_pointer_receiver_strips_pointer_and_param().
  TestFindReceiverTypeGo.test_nested_leaf_type_identifier: TestFindReceiverTypeGo#test_nested_leaf_type_identifier().
  TestFindReceiverTypeGo.test_no_parameter_declaration_returns_none: TestFindReceiverTypeGo#test_no_parameter_declaration_returns_none().
  TestFindReceiverTypeGo.test_parameter_declaration_without_type_returns_none: TestFindReceiverTypeGo#test_parameter_declaration_without_type_returns_none().
  TestFindReceiverTypeGo.test_non_matching_leaf_is_skipped: TestFindReceiverTypeGo#test_non_matching_leaf_is_skipped().
  TestFindReceiverTypeGo.test_first_param_decl_none_then_second_resolves: TestFindReceiverTypeGo#test_first_param_decl_none_then_second_resolves().
  _gnt: _gnt().
  TestFindReceiverTypeGo.test_non_method_node: TestFindReceiverTypeGo#test_non_method_node().
  TestFindReceiverTypeGo.test_no_receiver_field: TestFindReceiverTypeGo#test_no_receiver_field().
  _FakeNode.__init__: _FakeNode#__init__().
  _FakeNode.text: _FakeNode#text().
  _FakeMethod.child_by_field_name: _FakeMethod#child_by_field_name().
  TestStripGenericSuffix.test_plain_type_unchanged: TestStripGenericSuffix#test_plain_type_unchanged().
  TestStripGenericSuffix.test_pointer_generic_strips_param: TestStripGenericSuffix#test_pointer_generic_strips_param().
  TestStripGenericSuffix.test_two_type_params_stripped: TestStripGenericSuffix#test_two_type_params_stripped().
  TestStripGenericSuffix.test_trailing_space_stripped: TestStripGenericSuffix#test_trailing_space_stripped().
  TestStripGenericSuffix.test_unbalanced_open_bracket_returned_verbatim: TestStripGenericSuffix#test_unbalanced_open_bracket_returned_verbatim().
  TestStripGenericSuffix.test_only_brackets_yields_none: TestStripGenericSuffix#test_only_brackets_yields_none().
  TestStripGenericSuffix.test_empty_input_yields_none: TestStripGenericSuffix#test_empty_input_yields_none().
  TestStripGenericSuffix.test_no_bracket_close_only_returns_verbatim: TestStripGenericSuffix#test_no_bracket_close_only_returns_verbatim().
  TestStripGenericSuffix.test_unbalanced_start_none_fallthrough: TestStripGenericSuffix#test_unbalanced_start_none_fallthrough().
  TestExtractReceiverFromText.test_named_pointer_generic: TestExtractReceiverFromText#test_named_pointer_generic().
  TestExtractReceiverFromText.test_unnamed_pointer_generic: TestExtractReceiverFromText#test_unnamed_pointer_generic().
  TestExtractReceiverFromText.test_empty_string: TestExtractReceiverFromText#test_empty_string().
  TestExtractReceiverFromText.test_only_parens_whitespace: TestExtractReceiverFromText#test_only_parens_whitespace().
  TestExtractReceiverFromText.test_without_surrounding_parens: TestExtractReceiverFromText#test_without_surrounding_parens().
  TestExtractReceiverFromText.test_single_token_no_space: TestExtractReceiverFromText#test_single_token_no_space().
  TestExtractReceiverFromText.test_two_param_generic_named: TestExtractReceiverFromText#test_two_param_generic_named().
  TestNormalizeReceiverTypeForGraph.test_none_input: TestNormalizeReceiverTypeForGraph#test_none_input().
  TestNormalizeReceiverTypeForGraph.test_empty_string: TestNormalizeReceiverTypeForGraph#test_empty_string().
  TestNormalizeReceiverTypeForGraph.test_pointer_generic_strips_pointer_and_param: TestNormalizeReceiverTypeForGraph#test_pointer_generic_strips_pointer_and_param().
  TestNormalizeReceiverTypeForGraph.test_two_type_params: TestNormalizeReceiverTypeForGraph#test_two_type_params().
  TestNormalizeReceiverTypeForGraph.test_plain_type: TestNormalizeReceiverTypeForGraph#test_plain_type().
  TestNormalizeReceiverTypeForGraph.test_pointer_only: TestNormalizeReceiverTypeForGraph#test_pointer_only().
  TestNormalizeReceiverTypeForGraph.test_only_brackets_yields_none: TestNormalizeReceiverTypeForGraph#test_only_brackets_yields_none().
  TestNormalizeReceiverTypeForGraph.test_trailing_space: TestNormalizeReceiverTypeForGraph#test_trailing_space().
  TestNormalizeReceiverTypeForGraph.test_unbalanced_open_bracket_returns_base: TestNormalizeReceiverTypeForGraph#test_unbalanced_open_bracket_returns_base().
  TestNormalizeReceiverTypeForGraph.test_no_bracket_close_only_returns_base: TestNormalizeReceiverTypeForGraph#test_no_bracket_close_only_returns_base().
  TestNormalizeReceiverTypeForGraph.test_pointer_only_yields_none: TestNormalizeReceiverTypeForGraph#test_pointer_only_yields_none().
  TestNormalizeReceiverTypeForGraph.test_unbalanced_start_none_fallthrough: TestNormalizeReceiverTypeForGraph#test_unbalanced_start_none_fallthrough().
  TestFindReceiverTypeGo.test_none_node: TestFindReceiverTypeGo#test_none_node().
  _FakeNode._text: _FakeNode#_text.
  _FakeMethod._receiver: _FakeMethod#_receiver.
  _FakeNode.children: _FakeNode#children.
  _FakeMethod.__init__: _FakeMethod#__init__().
  TestStripGenericSuffix: TestStripGenericSuffix#
  TestExtractReceiverFromText: TestExtractReceiverFromText#
  TestExtractMethodReceiver: TestExtractMethodReceiver#
  TestExtractReceiverParts: TestExtractReceiverParts#
  TestNormalizeReceiverTypeForGraph: TestNormalizeReceiverTypeForGraph#
  TestFindReceiverTypeGo: TestFindReceiverTypeGo#
---
# Module: [`tests/unit/languages/test_go_receiver_helpers_branches.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py)

## Classes
### `TestExtractMethodReceiver`
- def: [`tests/unit/languages/test_go_receiver_helpers_branches.py:139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L139)
- signature: `class TestExtractMethodReceiver:`
- members:
  - `test_none_receiver_node(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L140)
  - `test_parameter_declaration_qualified_type(self)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L148)
  - `test_text_fallback_when_no_parameter_declaration_child(self)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L143)
- uses (calls/refs, reference-scoped): [`extract_method_receiver`](../../../tree_sitter_analyzer/languages/_go_common_helpers.md#extract_method_receiver)  (3 test-only)

### `TestExtractReceiverFromText`
- def: [`tests/unit/languages/test_go_receiver_helpers_branches.py:111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L111)
- signature: `class TestExtractReceiverFromText:`
- members:
  - `test_empty_string(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L119)
  - `test_named_pointer_generic(self)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L112)
  - `test_only_parens_whitespace(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L122)
  - `test_single_token_no_space(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L128)
  - `test_two_param_generic_named(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L132)
  - `test_unnamed_pointer_generic(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L115)
  - `test_without_surrounding_parens(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L125)
- uses (calls/refs, reference-scoped): [`_extract_receiver_from_text`](../../../tree_sitter_analyzer/languages/_go_common_helpers.md#_extract_receiver_from_text)

### `TestExtractReceiverParts`
- def: [`tests/unit/languages/test_go_receiver_helpers_branches.py:163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L163)
- signature: `class TestExtractReceiverParts:`
- members:
  - `test_no_recognized_type_returns_none_none(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L172)
  - `test_qualified_type_with_generic_suffix_stripped(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L164)
  - `test_unrelated_child_is_skipped(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L178)
- uses (calls/refs, reference-scoped): [`_extract_receiver_parts`](../../../tree_sitter_analyzer/languages/_go_common_helpers.md#_extract_receiver_parts)  (2 test-only)

### `TestFindReceiverTypeGo`
- def: [`tests/unit/languages/test_go_receiver_helpers_branches.py:243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L243)
- signature: `class TestFindReceiverTypeGo:`
- members:
  - `test_first_param_decl_none_then_second_resolves(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L305)
  - `test_generic_pointer_receiver_strips_pointer_and_param(self)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L264)
  - `test_nested_leaf_type_identifier(self)` — [`L270`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L270)
  - `test_no_parameter_declaration_returns_none(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L280)
  - `test_no_receiver_field(self)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L252)
  - `test_non_matching_leaf_is_skipped(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L292)
  - `test_non_method_node(self)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L247)
  - `test_none_node(self)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L244)
  - `test_parameter_declaration_without_type_returns_none(self)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L284)
  - `test_qualified_type_receiver(self)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L255)
- uses (calls/refs, reference-scoped): [`find_receiver_type_go`](../../../tree_sitter_analyzer/function_extraction.md#find_receiver_type_go)  (2 test-only)

### `TestNormalizeReceiverTypeForGraph`
- def: [`tests/unit/languages/test_go_receiver_helpers_branches.py:195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L195)
- signature: `class TestNormalizeReceiverTypeForGraph:`
- members:
  - `test_empty_string(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L199)
  - `test_no_bracket_close_only_returns_base(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L226)
  - `test_none_input(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L196)
  - `test_only_brackets_yields_none(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L215)
  - `test_plain_type(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L209)
  - `test_pointer_generic_strips_pointer_and_param(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L202)
  - `test_pointer_only(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L212)
  - `test_pointer_only_yields_none(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L230)
  - `test_trailing_space(self)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L219)
  - `test_two_type_params(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L206)
  - `test_unbalanced_open_bracket_returns_base(self)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L222)
  - `test_unbalanced_start_none_fallthrough(self)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L234)
- uses (calls/refs, reference-scoped): [`_normalize_go_receiver_type_for_graph`](../../../tree_sitter_analyzer/function_extraction.md#_normalize_go_receiver_type_for_graph)

### `TestStripGenericSuffix`
- def: [`tests/unit/languages/test_go_receiver_helpers_branches.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L71)
- signature: `class TestStripGenericSuffix:`
- members:
  - `test_empty_input_yields_none(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L94)
  - `test_no_bracket_close_only_returns_verbatim(self)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L97)
  - `test_only_brackets_yields_none(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L90)
  - `test_plain_type_unchanged(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L72)
  - `test_pointer_generic_strips_param(self)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L75)
  - `test_trailing_space_stripped(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L82)
  - `test_two_type_params_stripped(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L78)
  - `test_unbalanced_open_bracket_returned_verbatim(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L86)
  - `test_unbalanced_start_none_fallthrough(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L102)
- uses (calls/refs, reference-scoped): [`_strip_generic_suffix`](../../../tree_sitter_analyzer/languages/_go_common_helpers.md#_strip_generic_suffix)

### `_FakeMethod`
- def: [`tests/unit/languages/test_go_receiver_helpers_branches.py:52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L52)
- doc: Minimal stand-in for a method_declaration node.
- signature: `class _FakeMethod:`
- members:
  - `child_by_field_name(self, name: str)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L59)
- protocol/private: `__init__`[`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L55), `_receiver`[`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L56)
- used by: (11 test-only callers)

### `_FakeNode`
- def: [`tests/unit/languages/test_go_receiver_helpers_branches.py:39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L39)
- signature: `class _FakeNode:`
- members:
  - `text(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L48)
  - `children` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L45)
- protocol/private: `__init__`[`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L40), `_text`[`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L43)
- used by: (13 test-only callers)

## Functions
- `_gnt(node: Any)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_receiver_helpers_branches.py#L63)

