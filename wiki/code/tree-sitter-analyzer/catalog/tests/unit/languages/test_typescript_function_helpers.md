---
title: 'Module: tests/unit/languages/test_typescript_function_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_typescript_function_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_typescript_function_helpers`/
symbols:
  FakeNode: FakeNode#
  TestExtractFunction.test_basic_function_extraction: TestExtractFunction#test_basic_function_extraction().
  TestExtractArrowFunction.test_basic_arrow_with_variable_declarator: TestExtractArrowFunction#test_basic_arrow_with_variable_declarator().
  TestExtractMethod.test_basic_method: TestExtractMethod#test_basic_method().
  TestExtractMethodSignature.test_basic_method_signature: TestExtractMethodSignature#test_basic_method_signature().
  FakeNode.start_point: FakeNode#start_point.
  FakeNode.end_point: FakeNode#end_point.
  FakeNode.children: FakeNode#children.
  TestExtractMethod.test_static_constructor_method: TestExtractMethod#test_static_constructor_method().
  TestExtractGeneratorFunction.test_basic_generator: TestExtractGeneratorFunction#test_basic_generator().
  TestExtractArrowFunction.test_anonymous_arrow_no_parent: TestExtractArrowFunction#test_anonymous_arrow_no_parent().
  TestExtractArrowFunction.test_arrow_async_detection: TestExtractArrowFunction#test_arrow_async_detection().
  TestExtractArrowFunction.test_arrow_no_return_type_defaults_to_any: TestExtractArrowFunction#test_arrow_no_return_type_defaults_to_any().
  TestExtractArrowFunction.test_arrow_parent_not_variable_declarator: TestExtractArrowFunction#test_arrow_parent_not_variable_declarator().
  TestExtractArrowFunction.test_arrow_with_type_annotation_child: TestExtractArrowFunction#test_arrow_with_type_annotation_child().
  TestExtractArrowFunction.test_arrow_parent_no_identifier_child: TestExtractArrowFunction#test_arrow_parent_no_identifier_child().
  TestExtractFunction.test_async_function: TestExtractFunction#test_async_function().
  TestExtractFunction.test_none_return_type_defaults_to_any: TestExtractFunction#test_none_return_type_defaults_to_any().
  TestExtractFunction.test_generator_function_flag: TestExtractFunction#test_generator_function_flag().
  TestExtractArrowFunction.test_arrow_with_single_identifier_param: TestExtractArrowFunction#test_arrow_with_single_identifier_param().
  TestExtractMethod.test_method_none_return_type_defaults_any: TestExtractMethod#test_method_none_return_type_defaults_any().
  TestExtractMethodSignature.test_none_return_type_defaults_any: TestExtractMethodSignature#test_none_return_type_defaults_any().
  TestExtractGeneratorFunction.test_generator_async_flag: TestExtractGeneratorFunction#test_generator_async_flag().
  TestExtractGeneratorFunction.test_generator_none_return_type_defaults_generator: TestExtractGeneratorFunction#test_generator_none_return_type_defaults_generator().
  _make_function_sig: _make_function_sig().
  TestExtractFunction.test_content_lines_boundary_clamping: TestExtractFunction#test_content_lines_boundary_clamping().
  _make_method_sig: _make_method_sig().
  FakeNode.parent: FakeNode#parent.
  TestExtractFunction.test_none_name_returns_none: TestExtractFunction#test_none_name_returns_none().
  TestExtractMethod.test_none_method_name: TestExtractMethod#test_none_method_name().
  TestExtractMethodSignature.test_none_name_returns_none: TestExtractMethodSignature#test_none_name_returns_none().
  TestExtractGeneratorFunction.test_generator_none_name: TestExtractGeneratorFunction#test_generator_none_name().
  TestExtractFunction.test_none_signature_returns_none: TestExtractFunction#test_none_signature_returns_none().
  TestExtractFunction.test_exception_returns_none: TestExtractFunction#test_exception_returns_none().
  TestExtractMethod.test_none_method_signature: TestExtractMethod#test_none_method_signature().
  TestExtractMethod.test_method_exception_returns_none: TestExtractMethod#test_method_exception_returns_none().
  TestExtractMethodSignature.test_none_signature_returns_none: TestExtractMethodSignature#test_none_signature_returns_none().
  TestExtractMethodSignature.test_exception_returns_none: TestExtractMethodSignature#test_exception_returns_none().
  TestExtractGeneratorFunction.test_generator_none_signature: TestExtractGeneratorFunction#test_generator_none_signature().
  TestExtractGeneratorFunction.test_generator_exception_returns_none: TestExtractGeneratorFunction#test_generator_exception_returns_none().
  TestExtractArrowFunction.test_arrow_exception_returns_none: TestExtractArrowFunction#test_arrow_exception_returns_none().
  TestExtractArrowFunction.get_text: TestExtractArrowFunction#get_text().
  FakeNode.child_by_field_name: FakeNode#child_by_field_name().
  TestExtractFunction: TestExtractFunction#
  TestExtractArrowFunction: TestExtractArrowFunction#
  TestExtractMethod: TestExtractMethod#
  TestExtractMethodSignature: TestExtractMethodSignature#
  TestExtractGeneratorFunction: TestExtractGeneratorFunction#
---
# Module: [`tests/unit/languages/test_typescript_function_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/test_typescript_function_helpers.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L23)
- signature: `class FakeNode:`
- members:
  - `child_by_field_name(self, name: str)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L30)
  - `children` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L27)
  - `end_point` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L26)
  - `parent` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L28)
  - `start_point` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L25)
- used by: (30 test-only callers)

### `TestExtractArrowFunction`
- def: [`tests/unit/languages/test_typescript_function_helpers.py:202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L202)
- signature: `class TestExtractArrowFunction:`
- members:
  - `get_text(n)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L219)
  - `test_anonymous_arrow_no_parent(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L240)
  - `test_arrow_async_detection(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L282)
  - `test_arrow_exception_returns_none(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L326)
  - `test_arrow_no_return_type_defaults_to_any(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L304)
  - `test_arrow_parent_no_identifier_child(self)` — [`L383`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L383)
  - `test_arrow_parent_not_variable_declarator(self)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L340)
  - `test_arrow_with_single_identifier_param(self)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L260)
  - `test_arrow_with_type_annotation_child(self)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L360)
  - `test_basic_arrow_with_variable_declarator(self)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L203)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`extract_arrow_function`](../../../tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.md#extract_arrow_function), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`is_async`](../../../tree_sitter_analyzer/models/base.md#Function.is_async), [`is_arrow`](../../../tree_sitter_analyzer/models/base.md#Function.is_arrow)  (5 test-only)

### `TestExtractFunction`
- def: [`tests/unit/languages/test_typescript_function_helpers.py:78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L78)
- signature: `class TestExtractFunction:`
- members:
  - `test_async_function(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L113)
  - `test_basic_function_extraction(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L79)
  - `test_content_lines_boundary_clamping(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L175)
  - `test_exception_returns_none(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L163)
  - `test_generator_function_flag(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L188)
  - `test_none_name_returns_none(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L138)
  - `test_none_return_type_defaults_to_any(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L150)
  - `test_none_signature_returns_none(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L126)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`complexity_score`](../../../tree_sitter_analyzer/models/base.md#Function.complexity_score), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`extract_function`](../../../tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.md#extract_function), [`docstring`](../../../tree_sitter_analyzer/models/base.md#CodeElement.docstring), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`is_async`](../../../tree_sitter_analyzer/models/base.md#Function.is_async), [`is_arrow`](../../../tree_sitter_analyzer/models/base.md#Function.is_arrow), [`framework_type`](../../../tree_sitter_analyzer/models/base.md#Function.framework_type), [`is_generator`](../../../tree_sitter_analyzer/models/base.md#Function.is_generator)  (4 test-only)

### `TestExtractGeneratorFunction`
- def: [`tests/unit/languages/test_typescript_function_helpers.py:554`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L554)
- signature: `class TestExtractGeneratorFunction:`
- members:
  - `test_basic_generator(self)` — [`L555`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L555)
  - `test_generator_async_flag(self)` — [`L608`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L608)
  - `test_generator_exception_returns_none(self)` — [`L594`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L594)
  - `test_generator_none_name(self)` — [`L582`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L582)
  - `test_generator_none_return_type_defaults_generator(self)` — [`L621`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L621)
  - `test_generator_none_signature(self)` — [`L570`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L570)
- uses (calls/refs, reference-scoped): [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`extract_generator_function`](../../../tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.md#extract_generator_function), [`docstring`](../../../tree_sitter_analyzer/models/base.md#CodeElement.docstring), [`is_async`](../../../tree_sitter_analyzer/models/base.md#Function.is_async), [`is_generator`](../../../tree_sitter_analyzer/models/base.md#Function.is_generator)  (4 test-only)

### `TestExtractMethod`
- def: [`tests/unit/languages/test_typescript_function_helpers.py:404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L404)
- signature: `class TestExtractMethod:`
- members:
  - `test_basic_method(self)` — [`L405`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L405)
  - `test_method_exception_returns_none(self)` — [`L462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L462)
  - `test_method_none_return_type_defaults_any(self)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L476)
  - `test_none_method_name(self)` — [`L450`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L450)
  - `test_none_method_signature(self)` — [`L438`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L438)
  - `test_static_constructor_method(self)` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L421)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`extract_method`](../../../tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.md#extract_method), [`docstring`](../../../tree_sitter_analyzer/models/base.md#CodeElement.docstring), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`is_static`](../../../tree_sitter_analyzer/models/base.md#Function.is_static), [`is_constructor`](../../../tree_sitter_analyzer/models/base.md#Function.is_constructor)  (4 test-only)

### `TestExtractMethodSignature`
- def: [`tests/unit/languages/test_typescript_function_helpers.py:490`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L490)
- signature: `class TestExtractMethodSignature:`
- members:
  - `test_basic_method_signature(self)` — [`L491`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L491)
  - `test_exception_returns_none(self)` — [`L528`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L528)
  - `test_none_name_returns_none(self)` — [`L517`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L517)
  - `test_none_return_type_defaults_any(self)` — [`L541`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L541)
  - `test_none_signature_returns_none(self)` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L506)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`complexity_score`](../../../tree_sitter_analyzer/models/base.md#Function.complexity_score), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`extract_method_signature`](../../../tree_sitter_analyzer/languages/typescript_plugin/_function_helpers.md#extract_method_signature), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`is_arrow`](../../../tree_sitter_analyzer/models/base.md#Function.is_arrow)  (4 test-only)

## Functions
- `_make_function_sig(name: str | None = "myFunc", parameters: list[str] | None = None, is_async: bool = False, is_generator: bool = False, return_type: str | None = "void", generics: list[str] | None = None)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L34)
- `_make_method_sig(name: str | None = "myMethod", parameters: list[str] | None = None, is_async: bool = False, is_static: bool = False, is_getter: bool = False, is_setter: bool = False, is_constructor: bool = False, return_type: str | None = "void", visibility: str = "public", generics: list[str] | None = None)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_function_helpers.py#L52)

