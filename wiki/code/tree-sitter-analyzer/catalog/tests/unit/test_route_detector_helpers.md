---
title: 'Module: tests/unit/test_route_detector_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/test_route_detector_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_route_detector_helpers`/Test
symbols:
  TestUnquote.test_double_quoted: Unquote#test_double_quoted().
  TestUnquote.test_single_quoted: Unquote#test_single_quoted().
  TestUnquote.test_no_quotes: Unquote#test_no_quotes().
  TestUnquote.test_single_char_quoted: Unquote#test_single_char_quoted().
  TestUnquote.test_mismatched_quotes: Unquote#test_mismatched_quotes().
  TestUnquote.test_whitespace_around_quotes: Unquote#test_whitespace_around_quotes().
  TestUnquote.test_empty_string: Unquote#test_empty_string().
  TestUnquoteJavaString.test_double_quoted: UnquoteJavaString#test_double_quoted().
  TestUnquoteJavaString.test_not_quoted: UnquoteJavaString#test_not_quoted().
  TestUnquoteJavaString.test_single_quoted_not_stripped: UnquoteJavaString#test_single_quoted_not_stripped().
  TestUnquoteJavaString.test_empty_string: UnquoteJavaString#test_empty_string().
  TestUnquoteJavaString.test_whitespace_around: UnquoteJavaString#test_whitespace_around().
  TestParseMethodsList.test_multiple_methods: ParseMethodsList#test_multiple_methods().
  TestParseMethodsList.test_single_method: ParseMethodsList#test_single_method().
  TestParseMethodsList.test_no_methods: ParseMethodsList#test_no_methods().
  TestParseMethodsList.test_empty_string: ParseMethodsList#test_empty_string().
  TestParseMethodsList.test_double_quoted_methods: ParseMethodsList#test_double_quoted_methods().
  TestExtractDjangoHandler.test_dotted_path: ExtractDjangoHandler#test_dotted_path().
  TestExtractDjangoHandler.test_views_prefix: ExtractDjangoHandler#test_views_prefix().
  TestExtractDjangoHandler.test_dot_prefix: ExtractDjangoHandler#test_dot_prefix().
  TestExtractDjangoHandler.test_quoted_string: ExtractDjangoHandler#test_quoted_string().
  TestExtractDjangoHandler.test_single_quoted_string: ExtractDjangoHandler#test_single_quoted_string().
  TestExtractDjangoHandler.test_simple_name_no_dot: ExtractDjangoHandler#test_simple_name_no_dot().
  TestExtractTemplateString.test_string_child: ExtractTemplateString#test_string_child().
  TestExtractTemplateString.test_template_string_child: ExtractTemplateString#test_template_string_child().
  TestExtractTemplateString.test_fallback_backtick_text: ExtractTemplateString#test_fallback_backtick_text().
  TestExtractTemplateString.test_fallback_plain_text: ExtractTemplateString#test_fallback_plain_text().
  TestExtractAnnotationValue.test_parenthesized_string_literal: ExtractAnnotationValue#test_parenthesized_string_literal().
  TestExtractAnnotationValue.test_parenthesized_non_string: ExtractAnnotationValue#test_parenthesized_non_string().
  TestExtractAnnotationValue.test_arguments_field_string_literal: ExtractAnnotationValue#test_arguments_field_string_literal().
  TestExtractAnnotationValue.test_arguments_field_string_type: ExtractAnnotationValue#test_arguments_field_string_type().
  TestExtractAnnotationValue.test_no_paren_no_args: ExtractAnnotationValue#test_no_paren_no_args().
  TestFunctionNameAfterDecorator.test_function_definition_with_name: FunctionNameAfterDecorator#test_function_definition_with_name().
  TestFunctionNameAfterDecorator.test_identifier_child: FunctionNameAfterDecorator#test_identifier_child().
  TestFunctionNameAfterDecorator.test_no_parent: FunctionNameAfterDecorator#test_no_parent().
  TestFunctionNameAfterDecorator.test_no_matching_child: FunctionNameAfterDecorator#test_no_matching_child().
  TestMethodAfterAnnotation.test_method_declaration_with_identifier: MethodAfterAnnotation#test_method_declaration_with_identifier().
  TestMethodAfterAnnotation.test_no_parent: MethodAfterAnnotation#test_no_parent().
  TestMethodAfterAnnotation.test_no_method_declaration: MethodAfterAnnotation#test_no_method_declaration().
  TestFindKeyword.test_finds_keyword: FindKeyword#test_finds_keyword().
  TestFindKeyword.test_keyword_not_found: FindKeyword#test_keyword_not_found().
  TestFindKeyword.test_no_keyword_arguments: FindKeyword#test_no_keyword_arguments().
  TestExtractJsHandler.test_identifier_handler: ExtractJsHandler#test_identifier_handler().
  TestExtractJsHandler.test_arrow_function_handler: ExtractJsHandler#test_arrow_function_handler().
  TestExtractJsHandler.test_function_expression_handler: ExtractJsHandler#test_function_expression_handler().
  TestExtractJsHandler.test_call_expression_handler: ExtractJsHandler#test_call_expression_handler().
  TestExtractJsHandler.test_string_handler: ExtractJsHandler#test_string_handler().
  TestExtractJsHandler.test_single_arg_fallback: ExtractJsHandler#test_single_arg_fallback().
  TestExtractJsHandler.test_empty_args: ExtractJsHandler#test_empty_args().
  TestWalk.test_walk_single_node: Walk#test_walk_single_node().
  TestUnquote: Unquote#
  TestUnquoteJavaString: UnquoteJavaString#
  TestParseMethodsList: ParseMethodsList#
  TestExtractDjangoHandler: ExtractDjangoHandler#
  TestExtractTemplateString: ExtractTemplateString#
  TestExtractAnnotationValue: ExtractAnnotationValue#
  TestFunctionNameAfterDecorator: FunctionNameAfterDecorator#
  TestMethodAfterAnnotation: MethodAfterAnnotation#
  TestFindKeyword: FindKeyword#
  TestExtractJsHandler: ExtractJsHandler#
  TestWalk: Walk#
---
# Module: [`tests/unit/test_route_detector_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py)

## Classes
### `TestExtractAnnotationValue`
- def: [`tests/unit/test_route_detector_helpers.py:145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L145)
- signature: `class TestExtractAnnotationValue:`
- members:
  - `test_arguments_field_string_literal(self)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L168)
  - `test_arguments_field_string_type(self)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L179)
  - `test_no_paren_no_args(self)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L190)
  - `test_parenthesized_non_string(self)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L157)
  - `test_parenthesized_string_literal(self)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L146)
- uses (calls/refs, reference-scoped): [`extract_annotation_value`](../../tree_sitter_analyzer/_route_detector_helpers.md#extract_annotation_value)

### `TestExtractDjangoHandler`
- def: [`tests/unit/test_route_detector_helpers.py:89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L89)
- signature: `class TestExtractDjangoHandler:`
- members:
  - `test_dot_prefix(self)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L96)
  - `test_dotted_path(self)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L90)
  - `test_quoted_string(self)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L99)
  - `test_simple_name_no_dot(self)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L105)
  - `test_single_quoted_string(self)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L102)
  - `test_views_prefix(self)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L93)
- uses (calls/refs, reference-scoped): [`extract_django_handler`](../../tree_sitter_analyzer/_route_detector_helpers.md#extract_django_handler)

### `TestExtractJsHandler`
- def: [`tests/unit/test_route_detector_helpers.py:328`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L328)
- signature: `class TestExtractJsHandler:`
- members:
  - `test_arrow_function_handler(self)` — [`L342`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L342)
  - `test_call_expression_handler(self)` — [`L366`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L366)
  - `test_empty_args(self)` — [`L402`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L402)
  - `test_function_expression_handler(self)` — [`L354`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L354)
  - `test_identifier_handler(self)` — [`L329`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L329)
  - `test_single_arg_fallback(self)` — [`L393`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L393)
  - `test_string_handler(self)` — [`L380`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L380)
- uses (calls/refs, reference-scoped): [`extract_js_handler`](../../tree_sitter_analyzer/_route_detector_helpers.md#extract_js_handler)

### `TestExtractTemplateString`
- def: [`tests/unit/test_route_detector_helpers.py:112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L112)
- signature: `class TestExtractTemplateString:`
- members:
  - `test_fallback_backtick_text(self)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L129)
  - `test_fallback_plain_text(self)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L135)
  - `test_string_child(self)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L113)
  - `test_template_string_child(self)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L121)
- uses (calls/refs, reference-scoped): [`extract_template_string`](../../tree_sitter_analyzer/_route_detector_helpers.md#extract_template_string)

### `TestFindKeyword`
- def: [`tests/unit/test_route_detector_helpers.py:289`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L289)
- signature: `class TestFindKeyword:`
- members:
  - `test_finds_keyword(self)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L290)
  - `test_keyword_not_found(self)` — [`L305`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L305)
  - `test_no_keyword_arguments(self)` — [`L319`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L319)
- uses (calls/refs, reference-scoped): [`find_keyword`](../../tree_sitter_analyzer/_route_detector_helpers.md#find_keyword)

### `TestFunctionNameAfterDecorator`
- def: [`tests/unit/test_route_detector_helpers.py:200`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L200)
- signature: `class TestFunctionNameAfterDecorator:`
- members:
  - `test_function_definition_with_name(self)` — [`L201`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L201)
  - `test_identifier_child(self)` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L216)
  - `test_no_matching_child(self)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L234)
  - `test_no_parent(self)` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L229)
- uses (calls/refs, reference-scoped): [`function_name_after_decorator`](../../tree_sitter_analyzer/_route_detector_helpers.md#function_name_after_decorator)

### `TestMethodAfterAnnotation`
- def: [`tests/unit/test_route_detector_helpers.py:250`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L250)
- signature: `class TestMethodAfterAnnotation:`
- members:
  - `test_method_declaration_with_identifier(self)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L251)
  - `test_no_method_declaration(self)` — [`L273`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L273)
  - `test_no_parent(self)` — [`L268`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L268)
- uses (calls/refs, reference-scoped): [`method_after_annotation`](../../tree_sitter_analyzer/_route_detector_helpers.md#method_after_annotation)

### `TestParseMethodsList`
- def: [`tests/unit/test_route_detector_helpers.py:69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L69)
- signature: `class TestParseMethodsList:`
- members:
  - `test_double_quoted_methods(self)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L82)
  - `test_empty_string(self)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L79)
  - `test_multiple_methods(self)` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L70)
  - `test_no_methods(self)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L76)
  - `test_single_method(self)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L73)
- uses (calls/refs, reference-scoped): [`parse_methods_list`](../../tree_sitter_analyzer/_route_detector_helpers.md#parse_methods_list)

### `TestUnquote`
- def: [`tests/unit/test_route_detector_helpers.py:22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L22)
- signature: `class TestUnquote:`
- members:
  - `test_double_quoted(self)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L23)
  - `test_empty_string(self)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L42)
  - `test_mismatched_quotes(self)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L36)
  - `test_no_quotes(self)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L29)
  - `test_single_char_quoted(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L32)
  - `test_single_quoted(self)` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L26)
  - `test_whitespace_around_quotes(self)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L39)
- uses (calls/refs, reference-scoped): [`unquote`](../../tree_sitter_analyzer/_route_detector_helpers.md#unquote)

### `TestUnquoteJavaString`
- def: [`tests/unit/test_route_detector_helpers.py:49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L49)
- signature: `class TestUnquoteJavaString:`
- members:
  - `test_double_quoted(self)` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L50)
  - `test_empty_string(self)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L59)
  - `test_not_quoted(self)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L53)
  - `test_single_quoted_not_stripped(self)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L56)
  - `test_whitespace_around(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L62)
- uses (calls/refs, reference-scoped): [`unquote_java_string`](../../tree_sitter_analyzer/_route_detector_helpers.md#unquote_java_string)

### `TestWalk`
- def: [`tests/unit/test_route_detector_helpers.py:411`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L411)
- signature: `class TestWalk:`
- members:
  - `test_walk_single_node(self)` — [`L412`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_route_detector_helpers.py#L412) — walk should yield the root node at minimum.
- uses (calls/refs, reference-scoped): [`walk`](../../tree_sitter_analyzer/_route_detector_helpers.md#walk)

