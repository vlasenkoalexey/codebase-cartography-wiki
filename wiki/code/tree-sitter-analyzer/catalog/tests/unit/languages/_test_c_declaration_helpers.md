---
title: 'Module: tests/unit/languages/_test_c_declaration_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/_test_c_declaration_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages._test_c_declaration_helpers`/
symbols:
  FakeNode: FakeNode#
  FakeNode.text: FakeNode#text.
  FakeNode.children: FakeNode#children.
  _get_node_text: _get_node_text().
  TestExtractFieldDeclaration.test_simple_int_field: TestExtractFieldDeclaration#test_simple_int_field().
  TestExtractVariableDeclaration.test_simple_int_variable: TestExtractVariableDeclaration#test_simple_int_variable().
  TestExtractFieldDeclaration.test_const_field: TestExtractFieldDeclaration#test_const_field().
  TestExtractVariableDeclaration.test_static_variable: TestExtractVariableDeclaration#test_static_variable().
  TestExtractFieldDeclaration.test_pointer_field: TestExtractFieldDeclaration#test_pointer_field().
  TestExtractFieldDeclaration.test_array_field: TestExtractFieldDeclaration#test_array_field().
  TestExtractVariableDeclaration.test_struct_member_skipped: TestExtractVariableDeclaration#test_struct_member_skipped().
  TestExtractVariableDeclaration.test_pointer_variable: TestExtractVariableDeclaration#test_pointer_variable().
  TestExtractVariableDeclaration.test_const_variable: TestExtractVariableDeclaration#test_const_variable().
  TestExtractFieldDeclaration.test_no_type_returns_empty: TestExtractFieldDeclaration#test_no_type_returns_empty().
  TestExtractFieldDeclaration.test_no_names_returns_empty: TestExtractFieldDeclaration#test_no_names_returns_empty().
  TestExtractVariableDeclaration.test_no_type_returns_empty: TestExtractVariableDeclaration#test_no_type_returns_empty().
  FakeNode.start_point: FakeNode#start_point.
  FakeNode.end_point: FakeNode#end_point.
  TestAppendChildNames.test_finds_matching_children: TestAppendChildNames#test_finds_matching_children().
  TestAppendArrayFields.test_appends_field_identifier: TestAppendArrayFields#test_appends_field_identifier().
  TestAppendArrayFields.test_no_type: TestAppendArrayFields#test_no_type().
  TestAppendInitializerFields.test_finds_field_identifier: TestAppendInitializerFields#test_finds_field_identifier().
  TestAppendInitializerFields.test_finds_plain_identifier: TestAppendInitializerFields#test_finds_plain_identifier().
  TestAppendPointerFields.test_appends_and_adds_star: TestAppendPointerFields#test_appends_and_adds_star().
  TestAppendPointerVariables.test_appends_and_adds_star: TestAppendPointerVariables#test_appends_and_adds_star().
  TestFieldParts.test_primitive_type_with_field: TestFieldParts#test_primitive_type_with_field().
  TestFieldParts.test_with_type_qualifier: TestFieldParts#test_with_type_qualifier().
  TestVariableParts.test_primitive_type_with_identifier: TestVariableParts#test_primitive_type_with_identifier().
  TestVariableParts.test_storage_class_specifier: TestVariableParts#test_storage_class_specifier().
  TestVariableParts.test_init_declarator: TestVariableParts#test_init_declarator().
  TestNodeLineRange.test_basic_range: TestNodeLineRange#test_basic_range().
  TestNodeLineRange.test_multiline_range: TestNodeLineRange#test_multiline_range().
  TestAppendModifier.test_appends_non_empty: TestAppendModifier#test_appends_non_empty().
  TestAppendModifier.test_skips_empty: TestAppendModifier#test_skips_empty().
  TestAppendChildNames.test_no_matching_children: TestAppendChildNames#test_no_matching_children().
  TestAppendPointerFields.test_no_field_identifier: TestAppendPointerFields#test_no_field_identifier().
  TestAppendPointerVariables.test_no_identifier: TestAppendPointerVariables#test_no_identifier().
  TestFieldParts.test_empty_children: TestFieldParts#test_empty_children().
  TestExtractFieldDeclaration.test_exception_returns_empty: TestExtractFieldDeclaration#test_exception_returns_empty().
  TestExtractVariableDeclaration.test_exception_returns_empty: TestExtractVariableDeclaration#test_exception_returns_empty().
  FakeNode.child_by_field_name: FakeNode#child_by_field_name().
  FakeNode.fields: FakeNode#fields.
  FakeNode.parent: FakeNode#parent.
  FakeNode.start_byte: FakeNode#start_byte.
  FakeNode.end_byte: FakeNode#end_byte.
  TestNodeLineRange: TestNodeLineRange#
  TestAppendModifier: TestAppendModifier#
  TestAppendChildNames: TestAppendChildNames#
  TestAppendArrayFields: TestAppendArrayFields#
  TestAppendInitializerFields: TestAppendInitializerFields#
  TestAppendPointerFields: TestAppendPointerFields#
  TestAppendPointerVariables: TestAppendPointerVariables#
  TestFieldParts: TestFieldParts#
  TestVariableParts: TestVariableParts#
  TestExtractFieldDeclaration: TestExtractFieldDeclaration#
  TestExtractVariableDeclaration: TestExtractVariableDeclaration#
---
# Module: [`tests/unit/languages/_test_c_declaration_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L24)
- signature: `class FakeNode:`
- members:
  - `child_by_field_name(self, name: str)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L35)
  - `children` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L27)
  - `end_byte` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L32)
  - `end_point` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L30)
  - `fields` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L28)
  - `parent` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L33)
  - `start_byte` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L31)
  - `start_point` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L29)
  - `text` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L26)
- used by: (34 test-only callers)

### `TestAppendArrayFields`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L91)
- signature: `class TestAppendArrayFields:`
- members:
  - `test_appends_field_identifier(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L92)
  - `test_no_type(self)` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L101)
- uses (calls/refs, reference-scoped): [`_append_array_fields`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#_append_array_fields)  (4 test-only)

### `TestAppendChildNames`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L71)
- signature: `class TestAppendChildNames:`
- members:
  - `test_finds_matching_children(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L72)
  - `test_no_matching_children(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L83)
- uses (calls/refs, reference-scoped): [`_append_child_names`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#_append_child_names)  (4 test-only)

### `TestAppendInitializerFields`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L110)
- signature: `class TestAppendInitializerFields:`
- members:
  - `test_finds_field_identifier(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L111)
  - `test_finds_plain_identifier(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L119)
- uses (calls/refs, reference-scoped): [`_append_initializer_fields`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#_append_initializer_fields)  (4 test-only)

### `TestAppendModifier`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L57)
- signature: `class TestAppendModifier:`
- members:
  - `test_appends_non_empty(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L58)
  - `test_skips_empty(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L64)
- uses (calls/refs, reference-scoped): [`_append_modifier`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#_append_modifier)  (3 test-only)

### `TestAppendPointerFields`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L128)
- signature: `class TestAppendPointerFields:`
- members:
  - `test_appends_and_adds_star(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L129)
  - `test_no_field_identifier(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L138)
- uses (calls/refs, reference-scoped): [`_append_pointer_fields`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#_append_pointer_fields)  (4 test-only)

### `TestAppendPointerVariables`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L145)
- signature: `class TestAppendPointerVariables:`
- members:
  - `test_appends_and_adds_star(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L146)
  - `test_no_identifier(self)` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L155)
- uses (calls/refs, reference-scoped): [`_append_pointer_variables`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#_append_pointer_variables)  (4 test-only)

### `TestExtractFieldDeclaration`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L220)
- signature: `class TestExtractFieldDeclaration:`
- members:
  - `test_array_field(self)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L294)
  - `test_const_field(self)` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L238)
  - `test_exception_returns_empty(self)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L311)
  - `test_no_names_returns_empty(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L283)
  - `test_no_type_returns_empty(self)` — [`L272`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L272)
  - `test_pointer_field(self)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L255)
  - `test_simple_int_field(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L221)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`variable_type`](../../../tree_sitter_analyzer/models/base.md#Variable.variable_type), [`is_constant`](../../../tree_sitter_analyzer/models/base.md#Variable.is_constant), [`extract_field_declaration`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#extract_field_declaration), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Variable.modifiers)  (6 test-only)

### `TestExtractVariableDeclaration`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L318)
- signature: `class TestExtractVariableDeclaration:`
- members:
  - `test_const_variable(self)` — [`L386`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L386)
  - `test_exception_returns_empty(self)` — [`L415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L415)
  - `test_no_type_returns_empty(self)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L404)
  - `test_pointer_variable(self)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L369)
  - `test_simple_int_variable(self)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L319)
  - `test_static_variable(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L336)
  - `test_struct_member_skipped(self)` — [`L353`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L353)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`variable_type`](../../../tree_sitter_analyzer/models/base.md#Variable.variable_type), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Variable.visibility), [`is_constant`](../../../tree_sitter_analyzer/models/base.md#Variable.is_constant), [`extract_variable_declaration`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#extract_variable_declaration), [`is_static`](../../../tree_sitter_analyzer/models/base.md#Variable.is_static)  (7 test-only)

### `TestFieldParts`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L162)
- signature: `class TestFieldParts:`
- members:
  - `test_empty_children(self)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L183)
  - `test_primitive_type_with_field(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L163)
  - `test_with_type_qualifier(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L173)
- uses (calls/refs, reference-scoped): [`_field_parts`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#_field_parts)  (4 test-only)

### `TestNodeLineRange`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L43)
- signature: `class TestNodeLineRange:`
- members:
  - `test_basic_range(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L44)
  - `test_multiline_range(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L50)
- uses (calls/refs, reference-scoped): [`_node_line_range`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#_node_line_range)  (3 test-only)

### `TestVariableParts`
- def: [`tests/unit/languages/_test_c_declaration_helpers.py:190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L190)
- signature: `class TestVariableParts:`
- members:
  - `test_init_declarator(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L209)
  - `test_primitive_type_with_identifier(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L191)
  - `test_storage_class_specifier(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L200)
- uses (calls/refs, reference-scoped): [`_variable_parts`](../../../tree_sitter_analyzer/languages/_c_declaration_helpers.md#_variable_parts)  (4 test-only)

## Functions
- `_get_node_text(node: Any)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_declaration_helpers.py#L39)

