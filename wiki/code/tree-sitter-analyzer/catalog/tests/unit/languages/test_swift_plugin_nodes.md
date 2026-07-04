---
title: 'Module: tests/unit/languages/test_swift_plugin_nodes.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_swift_plugin_nodes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_swift_plugin_nodes`/
symbols:
  _make_node: _make_node().
  _make_extractor_with_source: _make_extractor_with_source().
  TestNamedChildText.test_finds_matching_descendant: TestNamedChildText#test_finds_matching_descendant().
  TestNamedChildText.test_fallback_name: TestNamedChildText#test_fallback_name().
  TestFirstDescendantText.test_matching_type: TestFirstDescendantText#test_matching_type().
  TestFirstDescendantText.test_no_match: TestFirstDescendantText#test_no_match().
  TestTypeName.test_with_name_field: TestTypeName#test_with_name_field().
  TestTypeName.test_without_name_field: TestTypeName#test_without_name_field().
  TestVariableName.test_with_name_field: TestVariableName#test_with_name_field().
  TestVariableName.test_without_name_field: TestVariableName#test_without_name_field().
  TestTypeAnnotation.test_with_type_annotation: TestTypeAnnotation#test_with_type_annotation().
  TestTypeAnnotation.test_without_type_annotation: TestTypeAnnotation#test_without_type_annotation().
  TestWalk.test_walk_single_node: TestWalk#test_walk_single_node().
  TestWalk.test_walk_with_children: TestWalk#test_walk_with_children().
  TestWalk.test_walk_nested: TestWalk#test_walk_nested().
  TestDecodeNodeText.test_bytes_input: TestDecodeNodeText#test_bytes_input().
  TestDecodeNodeText.test_string_input: TestDecodeNodeText#test_string_input().
  TestDecodeNodeText.test_utf8_decode_error: TestDecodeNodeText#test_utf8_decode_error().
  TestModifierWords.test_no_modifiers_field: TestModifierWords#test_no_modifiers_field().
  TestModifierWords.test_with_modifiers_field: TestModifierWords#test_with_modifiers_field().
  TestModifierWords.test_modifiers_as_child: TestModifierWords#test_modifiers_as_child().
  TestModifierWords.test_modifiers_with_non_alpha: TestModifierWords#test_modifiers_with_non_alpha().
  TestClassType.test_protocol_declaration: TestClassType#test_protocol_declaration().
  TestClassType.test_with_declaration_kind_field: TestClassType#test_with_declaration_kind_field().
  TestClassType.test_with_child_type: TestClassType#test_with_child_type().
  TestClassType.test_default_class: TestClassType#test_default_class().
  TestBindingKind.test_let_binding: TestBindingKind#test_let_binding().
  TestBindingKind.test_var_binding: TestBindingKind#test_var_binding().
  TestBindingKind.test_fallback_let: TestBindingKind#test_fallback_let().
  TestBindingKind.test_fallback_var: TestBindingKind#test_fallback_var().
  TestBindingKind.test_fallback_default: TestBindingKind#test_fallback_default().
  TestBaseElementFields.test_fields: TestBaseElementFields#test_fields().
  TestFallbackName.test_format: TestFallbackName#test_format().
  TestFallbackName.test_zero_position: TestFallbackName#test_zero_position().
  TREE_SITTER_SWIFT_AVAILABLE: TREE_SITTER_SWIFT_AVAILABLE.
  TestConstants.test_visibility_modifiers: TestConstants#test_visibility_modifiers().
  TestConstants.test_type_declaration_kinds: TestConstants#test_type_declaration_kinds().
  TestDecodeNodeText.test_none_input: TestDecodeNodeText#test_none_input().
  TestVisibility.test_public: TestVisibility#test_public().
  TestVisibility.test_private: TestVisibility#test_private().
  TestVisibility.test_open: TestVisibility#test_open().
  TestVisibility.test_fileprivate: TestVisibility#test_fileprivate().
  TestVisibility.test_internal_default: TestVisibility#test_internal_default().
  TestVisibility.test_first_visibility_wins: TestVisibility#test_first_visibility_wins().
  TestInheritedTypes.test_with_inheritance: TestInheritedTypes#test_with_inheritance().
  TestInheritedTypes.test_no_inheritance: TestInheritedTypes#test_no_inheritance().
  TestInheritedTypes.test_colon_no_types: TestInheritedTypes#test_colon_no_types().
  TestInheritedTypes.test_single_protocol: TestInheritedTypes#test_single_protocol().
  TestSuperclass.test_class_with_inheritance: TestSuperclass#test_class_with_inheritance().
  TestSuperclass.test_class_no_inheritance: TestSuperclass#test_class_no_inheritance().
  TestSuperclass.test_struct_no_superclass: TestSuperclass#test_struct_no_superclass().
  TestSuperclass.test_enum_no_superclass: TestSuperclass#test_enum_no_superclass().
  TestInterfaces.test_with_superclass: TestInterfaces#test_with_superclass().
  TestInterfaces.test_without_superclass: TestInterfaces#test_without_superclass().
  TestInterfaces.test_empty: TestInterfaces#test_empty().
  TestInterfaces.test_single_with_superclass: TestInterfaces#test_single_with_superclass().
  TestWalkWithRealParser: TestWalkWithRealParser#
  TestWalkWithRealParser.test_walk_real_tree: TestWalkWithRealParser#test_walk_real_tree().
  TestWalkWithRealParser.test_decode_real_node: TestWalkWithRealParser#test_decode_real_node().
  _make_extractor_with_source.get_node_text: _make_extractor_with_source().get_node_text().
  TestConstants: TestConstants#
  TestWalk: TestWalk#
  TestDecodeNodeText: TestDecodeNodeText#
  TestModifierWords: TestModifierWords#
  TestClassType: TestClassType#
  TestBindingKind: TestBindingKind#
  TestVisibility: TestVisibility#
  TestBaseElementFields: TestBaseElementFields#
  TestNamedChildText: TestNamedChildText#
  TestFirstDescendantText: TestFirstDescendantText#
  TestTypeName: TestTypeName#
  TestVariableName: TestVariableName#
  TestTypeAnnotation: TestTypeAnnotation#
  TestInheritedTypes: TestInheritedTypes#
  TestSuperclass: TestSuperclass#
  TestInterfaces: TestInterfaces#
  TestFallbackName: TestFallbackName#
---
# Module: [`tests/unit/languages/test_swift_plugin_nodes.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py)

## Classes
### `TestBaseElementFields`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L242)
- signature: `class TestBaseElementFields:`
- members:
  - `test_fields(self)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L243)
- uses (calls/refs, reference-scoped): [`base_element_fields`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#base_element_fields)  (1 test-only)

### `TestBindingKind`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L196)
- signature: `class TestBindingKind:`
- members:
  - `test_fallback_default(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L215)
  - `test_fallback_let(self)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L207)
  - `test_fallback_var(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L211)
  - `test_let_binding(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L197)
  - `test_var_binding(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L202)
- uses (calls/refs, reference-scoped): [`binding_kind`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#binding_kind)  (1 test-only)

### `TestClassType`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L173)
- signature: `class TestClassType:`
- members:
  - `test_default_class(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L190)
  - `test_protocol_declaration(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L174)
  - `test_with_child_type(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L184)
  - `test_with_declaration_kind_field(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L178)
- uses (calls/refs, reference-scoped): [`class_type`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#class_type)  (1 test-only)

### `TestConstants`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L81)
- signature: `class TestConstants:`
- members:
  - `test_type_declaration_kinds(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L89)
  - `test_visibility_modifiers(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L82)
- uses (calls/refs, reference-scoped): [`TYPE_DECLARATION_KINDS`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#TYPE_DECLARATION_KINDS), [`VISIBILITY_MODIFIERS`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#VISIBILITY_MODIFIERS)

### `TestDecodeNodeText`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L123)
- signature: `class TestDecodeNodeText:`
- members:
  - `test_bytes_input(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L124)
  - `test_none_input(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L132)
  - `test_string_input(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L128)
  - `test_utf8_decode_error(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L137)
- uses (calls/refs, reference-scoped): [`decode_node_text`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#decode_node_text)  (1 test-only)

### `TestFallbackName`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L390)
- signature: `class TestFallbackName:`
- members:
  - `test_format(self)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L391)
  - `test_zero_position(self)` — [`L396`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L396)
- uses (calls/refs, reference-scoped): [`fallback_name`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#fallback_name)  (1 test-only)

### `TestFirstDescendantText`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L271)
- signature: `class TestFirstDescendantText:`
- members:
  - `test_matching_type(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L272)
  - `test_no_match(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L279)
- uses (calls/refs, reference-scoped): [`first_descendant_text`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#first_descendant_text)  (2 test-only)

### `TestInheritedTypes`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L340)
- signature: `class TestInheritedTypes:`
- members:
  - `test_colon_no_types(self)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L350)
  - `test_no_inheritance(self)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L346)
  - `test_single_protocol(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L354)
  - `test_with_inheritance(self)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L341)
- uses (calls/refs, reference-scoped): [`inherited_types`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#inherited_types)

### `TestInterfaces`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L373)
- signature: `class TestInterfaces:`
- members:
  - `test_empty(self)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L382)
  - `test_single_with_superclass(self)` — [`L385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L385)
  - `test_with_superclass(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L374)
  - `test_without_superclass(self)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L378)
- uses (calls/refs, reference-scoped): [`interfaces`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#interfaces)

### `TestModifierWords`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L143)
- signature: `class TestModifierWords:`
- members:
  - `test_modifiers_as_child(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L158)
  - `test_modifiers_with_non_alpha(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L165)
  - `test_no_modifiers_field(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L144)
  - `test_with_modifiers_field(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L150)
- uses (calls/refs, reference-scoped): [`modifier_words`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#modifier_words)  (1 test-only)

### `TestNamedChildText`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L256)
- signature: `class TestNamedChildText:`
- members:
  - `test_fallback_name(self)` — [`L264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L264)
  - `test_finds_matching_descendant(self)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L257)
- uses (calls/refs, reference-scoped): [`named_child_text`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#named_child_text)  (2 test-only)

### `TestSuperclass`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L359)
- signature: `class TestSuperclass:`
- members:
  - `test_class_no_inheritance(self)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L363)
  - `test_class_with_inheritance(self)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L360)
  - `test_enum_no_superclass(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L369)
  - `test_struct_no_superclass(self)` — [`L366`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L366)
- uses (calls/refs, reference-scoped): [`superclass`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#superclass)

### `TestTypeAnnotation`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L324)
- signature: `class TestTypeAnnotation:`
- members:
  - `test_with_type_annotation(self)` — [`L325`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L325)
  - `test_without_type_annotation(self)` — [`L333`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L333)
- uses (calls/refs, reference-scoped): [`type_annotation`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#type_annotation)  (2 test-only)

### `TestTypeName`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L286)
- signature: `class TestTypeName:`
- members:
  - `test_with_name_field(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L287)
  - `test_without_name_field(self)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L296)
- uses (calls/refs, reference-scoped): [`type_name`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#type_name)  (2 test-only)

### `TestVariableName`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L305)
- signature: `class TestVariableName:`
- members:
  - `test_with_name_field(self)` — [`L306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L306)
  - `test_without_name_field(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L315)
- uses (calls/refs, reference-scoped): [`variable_name`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#variable_name)  (2 test-only)

### `TestVisibility`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L220)
- signature: `class TestVisibility:`
- members:
  - `test_fileprivate(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L230)
  - `test_first_visibility_wins(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L238)
  - `test_internal_default(self)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L233)
  - `test_open(self)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L227)
  - `test_private(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L224)
  - `test_public(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L221)
- uses (calls/refs, reference-scoped): [`visibility`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#visibility)

### `TestWalk`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L98)
- signature: `class TestWalk:`
- members:
  - `test_walk_nested(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L115)
  - `test_walk_single_node(self)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L99)
  - `test_walk_with_children(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L105)
- uses (calls/refs, reference-scoped): [`walk`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#walk)  (1 test-only)

### `TestWalkWithRealParser`
- def: [`tests/unit/languages/test_swift_plugin_nodes.py:406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L406)
- signature: `class TestWalkWithRealParser:`
- members:
  - `test_decode_real_node(self)` — [`L415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L415)
  - `test_walk_real_tree(self)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L407)
- uses (calls/refs, reference-scoped): [`decode_node_text`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#decode_node_text), [`walk`](../../../tree_sitter_analyzer/languages/_swift_plugin_nodes.md#walk)  (1 test-only)

## Functions
- `_make_extractor_with_source(source: str)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L60)
- `_make_node(node_type: str = "source_file", text: bytes = b"", children: list | None = None, start_point: tuple[int, int] = (0, 0), end_point: tuple[int, int] = (0, 0), start_byte: int = 0, end_byte: int = 0)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L39)
- `get_node_text(node)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L66)

## Module values
- `TREE_SITTER_SWIFT_AVAILABLE` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_swift_plugin_nodes.py#L34)

