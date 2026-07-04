---
title: 'Module: tests/unit/languages/_test_csharp_helpers_primitives.py'
type: catalog
provenance: extracted
module: tests/unit/languages/_test_csharp_helpers_primitives.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages._test_csharp_helpers_primitives`/
symbols:
  FakeNode: FakeNode#
  FakeNode.children: FakeNode#children.
  _get_node_text: _get_node_text().
  TestExtractUsingDirective.test_basic_using: TestExtractUsingDirective#test_basic_using().
  TestExtractUsingDirective.test_using_static: TestExtractUsingDirective#test_using_static().
  TestExtractAttributes.test_caches_result: TestExtractAttributes#test_caches_result().
  TestExtractUsingDirective.test_using_with_qualified_name: TestExtractUsingDirective#test_using_with_qualified_name().
  TestExtractUsingDirective.test_using_fallback_name_from_children: TestExtractUsingDirective#test_using_fallback_name_from_children().
  TestExtractUsingDirective.test_using_no_name_returns_none: TestExtractUsingDirective#test_using_no_name_returns_none().
  _make_attribute_list: _make_attribute_list().
  TestExtractModifiers.test_single_modifier: TestExtractModifiers#test_single_modifier().
  TestExtractModifiers.test_multiple_modifiers: TestExtractModifiers#test_multiple_modifiers().
  TestExtractModifiers.test_skips_non_modifier_children: TestExtractModifiers#test_skips_non_modifier_children().
  TestExtractAttributes.test_single_attribute_child: TestExtractAttributes#test_single_attribute_child().
  TestExtractAttributes.test_multiple_attributes: TestExtractAttributes#test_multiple_attributes().
  TestExtractAttributes.test_stops_at_first_non_attribute_list_child: TestExtractAttributes#test_stops_at_first_non_attribute_list_child().
  TestExtractAttributes.test_method_attributes: TestExtractAttributes#test_method_attributes().
  TestExtractParameters.test_no_parameter_children: TestExtractParameters#test_no_parameter_children().
  TestExtractParameters.test_single_parameter: TestExtractParameters#test_single_parameter().
  TestExtractParameters.test_multiple_parameters: TestExtractParameters#test_multiple_parameters().
  TestExtractParameters.test_skips_non_parameter_children: TestExtractParameters#test_skips_non_parameter_children().
  TestExtractModifiers.test_no_modifiers: TestExtractModifiers#test_no_modifiers().
  TestCalculateComplexity._traverse: TestCalculateComplexity#_traverse().
  TestCalculateComplexity.test_single_if_increments: TestCalculateComplexity#test_single_if_increments().
  TestCalculateComplexity.test_all_decision_keywords: TestCalculateComplexity#test_all_decision_keywords().
  TestCalculateComplexity.test_nested_decisions: TestCalculateComplexity#test_nested_decisions().
  TestCalculateComplexity.test_non_decision_nodes_ignored: TestCalculateComplexity#test_non_decision_nodes_ignored().
  TestExtractAttributes.test_no_attribute_list_children_returns_empty: TestExtractAttributes#test_no_attribute_list_children_returns_empty().
  TestExtractTypeName.test_returns_node_text: TestExtractTypeName#test_returns_node_text().
  TestExtractTypeName.test_generic_name: TestExtractTypeName#test_generic_name().
  TestCalculateComplexity.test_base_complexity_is_one: TestCalculateComplexity#test_base_complexity_is_one().
  FakeNode.start_point: FakeNode#start_point.
  FakeNode.fields: FakeNode#fields.
  _make_modifier: _make_modifier().
  FakeNode.end_point: FakeNode#end_point.
  FakeNode.child_by_field_name: FakeNode#child_by_field_name().
  FakeNode.prev_sibling: FakeNode#prev_sibling().
  TestExtractParameters.test_none_node_returns_empty: TestExtractParameters#test_none_node_returns_empty().
  TestExtractTypeName.test_none_returns_void: TestExtractTypeName#test_none_returns_void().
  FakeNode._prev_sibling: FakeNode#_prev_sibling.
  TestDetermineVisibility.test_public: TestDetermineVisibility#test_public().
  TestDetermineVisibility.test_private: TestDetermineVisibility#test_private().
  TestDetermineVisibility.test_protected: TestDetermineVisibility#test_protected().
  TestDetermineVisibility.test_internal: TestDetermineVisibility#test_internal().
  TestDetermineVisibility.test_default_is_private: TestDetermineVisibility#test_default_is_private().
  TestDetermineVisibility.test_public_priority_over_private: TestDetermineVisibility#test_public_priority_over_private().
  TestDetermineVisibility.test_protected_priority_over_internal: TestDetermineVisibility#test_protected_priority_over_internal().
  TestDetermineVisibility.test_non_visibility_modifiers_ignored: TestDetermineVisibility#test_non_visibility_modifiers_ignored().
  FakeNode.text: FakeNode#text.
  FakeNode.start_byte: FakeNode#start_byte.
  FakeNode.end_byte: FakeNode#end_byte.
  TestDetermineVisibility: TestDetermineVisibility#
  TestExtractParameters: TestExtractParameters#
  TestExtractTypeName: TestExtractTypeName#
  TestExtractModifiers: TestExtractModifiers#
  TestCalculateComplexity: TestCalculateComplexity#
  TestExtractAttributes: TestExtractAttributes#
  TestExtractUsingDirective: TestExtractUsingDirective#
---
# Module: [`tests/unit/languages/_test_csharp_helpers_primitives.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/_test_csharp_helpers_primitives.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L20)
- signature: `class FakeNode:`
- members:
  - `child_by_field_name(self, name: str)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L31)
  - `prev_sibling(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L35)
  - `children` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L23)
  - `end_byte` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L28)
  - `end_point` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L26)
  - `fields` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L24)
  - `start_byte` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L27)
  - `start_point` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L25)
  - `text` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L22)
- protocol/private: `_prev_sibling`[`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L29)
- used by: (29 test-only callers)

### `TestCalculateComplexity`
- def: [`tests/unit/languages/_test_csharp_helpers_primitives.py:146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L146)
- signature: `class TestCalculateComplexity:`
- members:
  - `test_all_decision_keywords(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L167)
  - `test_base_complexity_is_one(self)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L156)
  - `test_nested_decisions(self)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L181)
  - `test_non_decision_nodes_ignored(self)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L186)
  - `test_single_if_increments(self)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L160)
- protocol/private: `_traverse`[`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L147)
- uses (calls/refs, reference-scoped): [`calculate_complexity`](../../../tree_sitter_analyzer/languages/csharp_helpers.md#calculate_complexity)  (2 test-only)

### `TestDetermineVisibility`
- def: [`tests/unit/languages/_test_csharp_helpers_primitives.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L47)
- signature: `class TestDetermineVisibility:`
- members:
  - `test_default_is_private(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L60)
  - `test_internal(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L57)
  - `test_non_visibility_modifiers_ignored(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L69)
  - `test_private(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L51)
  - `test_protected(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L54)
  - `test_protected_priority_over_internal(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L66)
  - `test_public(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L48)
  - `test_public_priority_over_private(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L63)
- uses (calls/refs, reference-scoped): [`determine_visibility`](../../../tree_sitter_analyzer/languages/csharp_helpers.md#determine_visibility)

### `TestExtractAttributes`
- def: [`tests/unit/languages/_test_csharp_helpers_primitives.py:209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L209)
- doc: Tests for extract_attributes — reads attribute_list direct children.
- signature: `class TestExtractAttributes:`
- members:
  - `test_caches_result(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L260)
  - `test_method_attributes(self)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L251)
  - `test_multiple_attributes(self)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L229)
  - `test_no_attribute_list_children_returns_empty(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L212)
  - `test_single_attribute_child(self)` — [`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L218)
  - `test_stops_at_first_non_attribute_list_child(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L240)
- uses (calls/refs, reference-scoped): [`extract_attributes`](../../../tree_sitter_analyzer/languages/csharp_helpers.md#extract_attributes)  (6 test-only)

### `TestExtractModifiers`
- def: [`tests/unit/languages/_test_csharp_helpers_primitives.py:115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L115)
- signature: `class TestExtractModifiers:`
- members:
  - `test_multiple_modifiers(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L127)
  - `test_no_modifiers(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L116)
  - `test_single_modifier(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L120)
  - `test_skips_non_modifier_children(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L138)
- uses (calls/refs, reference-scoped): [`extract_modifiers`](../../../tree_sitter_analyzer/languages/csharp_helpers.md#extract_modifiers)  (4 test-only)

### `TestExtractParameters`
- def: [`tests/unit/languages/_test_csharp_helpers_primitives.py:73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L73)
- signature: `class TestExtractParameters:`
- members:
  - `test_multiple_parameters(self)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L87)
  - `test_no_parameter_children(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L77)
  - `test_none_node_returns_empty(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L74)
  - `test_single_parameter(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L81)
  - `test_skips_non_parameter_children(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L94)
- uses (calls/refs, reference-scoped): [`extract_parameters`](../../../tree_sitter_analyzer/languages/csharp_helpers.md#extract_parameters)  (3 test-only)

### `TestExtractTypeName`
- def: [`tests/unit/languages/_test_csharp_helpers_primitives.py:102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L102)
- signature: `class TestExtractTypeName:`
- members:
  - `test_generic_name(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L110)
  - `test_none_returns_void(self)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L103)
  - `test_returns_node_text(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L106)
- uses (calls/refs, reference-scoped): [`extract_type_name`](../../../tree_sitter_analyzer/languages/csharp_helpers.md#extract_type_name)  (2 test-only)

### `TestExtractUsingDirective`
- def: [`tests/unit/languages/_test_csharp_helpers_primitives.py:275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L275)
- signature: `class TestExtractUsingDirective:`
- members:
  - `test_basic_using(self)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L276)
  - `test_using_fallback_name_from_children(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L330)
  - `test_using_no_name_returns_none(self)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L319)
  - `test_using_static(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L304)
  - `test_using_with_qualified_name(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L291)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`extract_using_directive`](../../../tree_sitter_analyzer/languages/csharp_helpers.md#extract_using_directive), [`is_static`](../../../tree_sitter_analyzer/models/base.md#Import.is_static)  (6 test-only)

## Functions
- `_get_node_text(node: Any)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L39)
- `_make_attribute_list(name: str, line: int = 0)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L197) — Build a FakeNode tree matching tree-sitter C# attribute_list structure.
- `_make_modifier(text: str)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_csharp_helpers_primitives.py#L43)

