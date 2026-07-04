---
title: 'Module: tests/unit/languages/_test_c_function_macro_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/_test_c_function_macro_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages._test_c_function_macro_helpers`/
symbols:
  FakeNode: FakeNode#
  FakeNode.children: FakeNode#children.
  FakeNode.text: FakeNode#text.
  TestExtractMacroFunction.test_basic_macro: TestExtractMacroFunction#test_basic_macro().
  _get_node_text: _get_node_text().
  TestExtractCFunction.test_basic_function: TestExtractCFunction#test_basic_function().
  TestExtractMacroFunction.test_variadic_macro: TestExtractMacroFunction#test_variadic_macro().
  TestExtractMacroFunction.test_line_numbers: TestExtractMacroFunction#test_line_numbers().
  TestExtractCFunction.test_with_modifiers: TestExtractCFunction#test_with_modifiers().
  TestExtractCFunction.test_with_docstring: TestExtractCFunction#test_with_docstring().
  TestExtractMacroFunction.test_no_name_returns_none: TestExtractMacroFunction#test_no_name_returns_none().
  TestExtractCFunction.test_none_signature: TestExtractCFunction#test_none_signature().
  TestMacroFunctionParts.test_identifier_and_params: TestMacroFunctionParts#test_identifier_and_params().
  TestMacroFunctionParts.test_no_params: TestMacroFunctionParts#test_no_params().
  TestAppendMacroParams.test_identifiers: TestAppendMacroParams#test_identifiers().
  TestAppendMacroParams.test_variadic: TestAppendMacroParams#test_variadic().
  TestFunctionDeclaratorInfo.test_name_and_params: TestFunctionDeclaratorInfo#test_name_and_params().
  TestFunctionDeclaratorInfo.test_no_parameter_list: TestFunctionDeclaratorInfo#test_no_parameter_list().
  TestFindFunctionDeclarator.test_finds_nested_declarator: TestFindFunctionDeclarator#test_finds_nested_declarator().
  TestFindFunctionDeclarator.test_no_declarator: TestFindFunctionDeclarator#test_no_declarator().
  TestFindFunctionDeclarator.test_deeply_nested: TestFindFunctionDeclarator#test_deeply_nested().
  TestParseFunctionSignature.test_simple_function: TestParseFunctionSignature#test_simple_function().
  TestParseFunctionSignature.test_static_function: TestParseFunctionSignature#test_static_function().
  TestParseFunctionSignature.test_pointer_return: TestParseFunctionSignature#test_pointer_return().
  TestParseFunctionSignature.test_no_name_returns_none: TestParseFunctionSignature#test_no_name_returns_none().
  TestParseFunctionSignature.test_with_type_qualifier: TestParseFunctionSignature#test_with_type_qualifier().
  FakeNode.start_point: FakeNode#start_point.
  TestExtractCFunction.test_exception_returns_none: TestExtractCFunction#test_exception_returns_none().
  TestMacroFunctionParts.test_no_identifier: TestMacroFunctionParts#test_no_identifier().
  TestAppendMacroParams.test_empty: TestAppendMacroParams#test_empty().
  TestExtractMacroFunction.test_exception_returns_none: TestExtractMacroFunction#test_exception_returns_none().
  TestSignatureAppendModifier.test_appends: TestSignatureAppendModifier#test_appends().
  TestSignatureAppendModifier.test_empty_text_skipped: TestSignatureAppendModifier#test_empty_text_skipped().
  TestParseFunctionSignature.test_exception_returns_none: TestParseFunctionSignature#test_exception_returns_none().
  FakeNode.end_point: FakeNode#end_point.
  FakeNode.child_by_field_name: FakeNode#child_by_field_name().
  TestExtractCFunction.parse_sig: TestExtractCFunction#parse_sig().
  FakeNode.fields: FakeNode#fields.
  FakeNode.parent: FakeNode#parent.
  TestFunctionRawText.test_basic_extraction: TestFunctionRawText#test_basic_extraction().
  TestFunctionRawText.test_single_line: TestFunctionRawText#test_single_line().
  TestFunctionRawText.test_out_of_range_clamped: TestFunctionRawText#test_out_of_range_clamped().
  TestFunctionRawText.test_empty_lines: TestFunctionRawText#test_empty_lines().
  TestPointerReturnType.test_adds_star: TestPointerReturnType#test_adds_star().
  TestPointerReturnType.test_already_has_star: TestPointerReturnType#test_already_has_star().
  TestPointerReturnType.test_double_pointer: TestPointerReturnType#test_double_pointer().
  TestPointerReturnType.test_empty_string: TestPointerReturnType#test_empty_string().
  TestExtractCFunction.calc_complexity: TestExtractCFunction#calc_complexity().
  TestExtractCFunction.get_comment: TestExtractCFunction#get_comment().
  FakeNode.start_byte: FakeNode#start_byte.
  FakeNode.end_byte: FakeNode#end_byte.
  TestFunctionRawText: TestFunctionRawText#
  TestExtractCFunction: TestExtractCFunction#
  TestMacroFunctionParts: TestMacroFunctionParts#
  TestAppendMacroParams: TestAppendMacroParams#
  TestExtractMacroFunction: TestExtractMacroFunction#
  TestPointerReturnType: TestPointerReturnType#
  TestSignatureAppendModifier: TestSignatureAppendModifier#
  TestFunctionDeclaratorInfo: TestFunctionDeclaratorInfo#
  TestFindFunctionDeclarator: TestFindFunctionDeclarator#
  TestParseFunctionSignature: TestParseFunctionSignature#
---
# Module: [`tests/unit/languages/_test_c_function_macro_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L27)
- signature: `class FakeNode:`
- members:
  - `child_by_field_name(self, name: str)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L38)
  - `children` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L30)
  - `end_byte` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L35)
  - `end_point` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L33)
  - `fields` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L31)
  - `parent` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L36)
  - `start_byte` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L34)
  - `start_point` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L32)
  - `text` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L29)
- used by: (29 test-only callers)

### `TestAppendMacroParams`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L178)
- signature: `class TestAppendMacroParams:`
- members:
  - `test_empty(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L197)
  - `test_identifiers(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L179)
  - `test_variadic(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L188)
- uses (calls/refs, reference-scoped): [`_append_macro_params`](../../../tree_sitter_analyzer/languages/_c_macro_helpers.md#_append_macro_params)  (4 test-only)

### `TestExtractCFunction`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L69)
- signature: `class TestExtractCFunction:`
- members:
  - `calc_complexity(n: Any)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L78)
  - `get_comment(line: int)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L80)
  - `parse_sig(n: Any)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L76)
  - `test_basic_function(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L70)
  - `test_exception_returns_none(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L139)
  - `test_none_signature(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L93)
  - `test_with_docstring(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L123)
  - `test_with_modifiers(self)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L107)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`docstring`](../../../tree_sitter_analyzer/models/base.md#CodeElement.docstring), [`extract_c_function`](../../../tree_sitter_analyzer/languages/_c_function_helpers.md#extract_c_function), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Function.modifiers), [`is_static`](../../../tree_sitter_analyzer/models/base.md#Function.is_static)  (4 test-only)

### `TestExtractMacroFunction`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L204)
- signature: `class TestExtractMacroFunction:`
- members:
  - `test_basic_macro(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L205)
  - `test_exception_returns_none(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L269)
  - `test_line_numbers(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L256)
  - `test_no_name_returns_none(self)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L226)
  - `test_variadic_macro(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L237)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`complexity_score`](../../../tree_sitter_analyzer/models/base.md#Function.complexity_score), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`extract_macro_function`](../../../tree_sitter_analyzer/languages/_c_macro_helpers.md#extract_macro_function), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Function.modifiers)  (6 test-only)

### `TestFindFunctionDeclarator`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L321)
- signature: `class TestFindFunctionDeclarator:`
- members:
  - `test_deeply_nested(self)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L338)
  - `test_finds_nested_declarator(self)` — [`L322`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L322)
  - `test_no_declarator(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L330)
- uses (calls/refs, reference-scoped): [`_find_function_declarator`](../../../tree_sitter_analyzer/languages/_c_signature_helpers.md#_find_function_declarator)  (4 test-only)

### `TestFunctionDeclaratorInfo`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L302)
- signature: `class TestFunctionDeclaratorInfo:`
- members:
  - `test_name_and_params(self)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L303)
  - `test_no_parameter_list(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L312)
- uses (calls/refs, reference-scoped): [`_function_declarator_info`](../../../tree_sitter_analyzer/languages/_c_signature_helpers.md#_function_declarator_info)  (4 test-only)

### `TestFunctionRawText`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L46)
- signature: `class TestFunctionRawText:`
- members:
  - `test_basic_extraction(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L47)
  - `test_empty_lines(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L64)
  - `test_out_of_range_clamped(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L58)
  - `test_single_line(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L53)
- uses (calls/refs, reference-scoped): [`_function_raw_text`](../../../tree_sitter_analyzer/languages/_c_function_helpers.md#_function_raw_text)

### `TestMacroFunctionParts`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L151)
- signature: `class TestMacroFunctionParts:`
- members:
  - `test_identifier_and_params(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L152)
  - `test_no_identifier(self)` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L172)
  - `test_no_params(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L164)
- uses (calls/refs, reference-scoped): [`_macro_function_parts`](../../../tree_sitter_analyzer/languages/_c_macro_helpers.md#_macro_function_parts)  (4 test-only)

### `TestParseFunctionSignature`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L348)
- signature: `class TestParseFunctionSignature:`
- members:
  - `test_exception_returns_none(self)` — [`L407`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L407)
  - `test_no_name_returns_none(self)` — [`L388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L388)
  - `test_pointer_return(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L374)
  - `test_simple_function(self)` — [`L349`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L349)
  - `test_static_function(self)` — [`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L362)
  - `test_with_type_qualifier(self)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L395)
- uses (calls/refs, reference-scoped): [`parse_function_signature`](../../../tree_sitter_analyzer/languages/_c_signature_helpers.md#parse_function_signature)  (4 test-only)

### `TestPointerReturnType`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L276)
- signature: `class TestPointerReturnType:`
- members:
  - `test_adds_star(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L277)
  - `test_already_has_star(self)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L280)
  - `test_double_pointer(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L283)
  - `test_empty_string(self)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L286)
- uses (calls/refs, reference-scoped): [`_pointer_return_type`](../../../tree_sitter_analyzer/languages/_c_signature_helpers.md#_pointer_return_type)

### `TestSignatureAppendModifier`
- def: [`tests/unit/languages/_test_c_function_macro_helpers.py:290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L290)
- signature: `class TestSignatureAppendModifier:`
- members:
  - `test_appends(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L291)
  - `test_empty_text_skipped(self)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L296)
- uses (calls/refs, reference-scoped): [`_append_modifier`](../../../tree_sitter_analyzer/languages/_c_signature_helpers.md#_append_modifier)  (3 test-only)

## Functions
- `_get_node_text(node: Any)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_function_macro_helpers.py#L42)

