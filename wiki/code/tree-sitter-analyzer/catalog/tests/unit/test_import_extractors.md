---
title: 'Module: tests/unit/test_import_extractors.py'
type: catalog
provenance: extracted
module: tests/unit/test_import_extractors.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_import_extractors`/
symbols:
  MockNode: MockNode#
  MockNode.start_byte: MockNode#start_byte.
  MockNode.end_byte: MockNode#end_byte.
  MockNode.children: MockNode#children().
  TestExtractJsImports.test_require_call_extracts: TestExtractJsImports#test_require_call_extracts().
  TestWalkImports.test_ruby_dispatch: TestWalkImports#test_ruby_dispatch().
  TestExtractRubyImports.test_require_extracts_gem: TestExtractRubyImports#test_require_extracts_gem().
  TestExtractRubyImports.test_require_relative_extracts: TestExtractRubyImports#test_require_relative_extracts().
  TestExtractRubyImports.test_require_skips_stdlib: TestExtractRubyImports#test_require_skips_stdlib().
  TestNodeText.test_extracts_text_by_byte_range: TestNodeText#test_extracts_text_by_byte_range().
  TestNodeText.test_returns_empty_for_mismatched_range: TestNodeText#test_returns_empty_for_mismatched_range().
  TestNodeText.test_returns_empty_for_none_range: TestNodeText#test_returns_empty_for_none_range().
  TestExtractPythonImportSimple.test_skips_stdlib: TestExtractPythonImportSimple#test_skips_stdlib().
  TestExtractJsImports.test_import_statement_extracts_module: TestExtractJsImports#test_import_statement_extracts_module().
  TestExtractGoImports.test_skips_stdlib: TestExtractGoImports#test_skips_stdlib().
  TestExtractGoImports.test_extracts_third_party: TestExtractGoImports#test_extracts_third_party().
  TestExtractRustImports.test_skips_std_crate: TestExtractRustImports#test_skips_std_crate().
  TestExtractRustImports.test_extracts_crate_local: TestExtractRustImports#test_extracts_crate_local().
  TestExtractCppImports.test_local_include: TestExtractCppImports#test_local_include().
  TestExtractCppImports.test_system_include: TestExtractCppImports#test_system_include().
  TestExtractJavaImports.test_skips_java_stdlib: TestExtractJavaImports#test_skips_java_stdlib().
  TestExtractJavaImports.test_extracts_third_party: TestExtractJavaImports#test_extracts_third_party().
  TestExtractJavaImports.test_static_import: TestExtractJavaImports#test_static_import().
  TestExtractJavaImports.test_wildcard_import: TestExtractJavaImports#test_wildcard_import().
  TestWalkImports.test_kotlin_dispatch: TestWalkImports#test_kotlin_dispatch().
  TestWalkImports.test_php_dispatch: TestWalkImports#test_php_dispatch().
  TestExtractCSharpImports.test_extracts_third_party: TestExtractCSharpImports#test_extracts_third_party().
  TestExtractKotlinImports.test_skips_kotlin_stdlib: TestExtractKotlinImports#test_skips_kotlin_stdlib().
  TestExtractKotlinImports.test_extracts_third_party: TestExtractKotlinImports#test_extracts_third_party().
  TestExtractKotlinImports.test_wildcard_import: TestExtractKotlinImports#test_wildcard_import().
  TestExtractSwiftImports.test_skips_stdlib_foundation: TestExtractSwiftImports#test_skips_stdlib_foundation().
  TestExtractSwiftImports.test_extracts_custom_framework: TestExtractSwiftImports#test_extracts_custom_framework().
  TestExtractPhpImports.test_extracts_use_declaration: TestExtractPhpImports#test_extracts_use_declaration().
  TestExtractPhpImports.test_function_use: TestExtractPhpImports#test_function_use().
  TestExtractPhpImports.test_aliased_use: TestExtractPhpImports#test_aliased_use().
  TestExtractPythonImportSimple.test_extracts_third_party: TestExtractPythonImportSimple#test_extracts_third_party().
  TestExtractPythonImportFrom.test_skips_stdlib_from_import: TestExtractPythonImportFrom#test_skips_stdlib_from_import().
  TestExtractPythonImports.test_import_statement_dispatches: TestExtractPythonImports#test_import_statement_dispatches().
  TestWalkImports.test_csharp_dispatch: TestWalkImports#test_csharp_dispatch().
  TestWalkImports.test_swift_dispatch: TestWalkImports#test_swift_dispatch().
  TestExtractCSharpImports.test_skips_stdlib_system: TestExtractCSharpImports#test_skips_stdlib_system().
  MockNode._fields: MockNode#_fields.
  MockNode.__repr__: MockNode#__repr__().
  TestExtractPythonImportFrom.test_no_module_name_returns_early: TestExtractPythonImportFrom#test_no_module_name_returns_early().
  TestExtractPythonImports.test_non_import_node_skipped: TestExtractPythonImports#test_non_import_node_skipped().
  TestExtractGoImports.test_non_import_declaration_skipped: TestExtractGoImports#test_non_import_declaration_skipped().
  TestExtractRustImports.test_non_use_declaration_skipped: TestExtractRustImports#test_non_use_declaration_skipped().
  TestExtractCppImports.test_non_include_skipped: TestExtractCppImports#test_non_include_skipped().
  TestWalkImports.test_unsupported_language_no_error: TestWalkImports#test_unsupported_language_no_error().
  TestWalkImports.test_walks_children_recursively: TestWalkImports#test_walks_children_recursively().
  TestExtractCSharpImports.test_non_using_directive_skipped: TestExtractCSharpImports#test_non_using_directive_skipped().
  TestExtractKotlinImports.test_non_import_skipped: TestExtractKotlinImports#test_non_import_skipped().
  TestExtractSwiftImports.test_non_import_skipped: TestExtractSwiftImports#test_non_import_skipped().
  TestExtractRubyImports.test_non_call_skipped: TestExtractRubyImports#test_non_call_skipped().
  TestExtractPhpImports.test_non_use_skipped: TestExtractPhpImports#test_non_use_skipped().
  MockNode.type: MockNode#type().
  MockNode.child_by_field_name: MockNode#child_by_field_name().
  TestParseRustUsePath.test_simple_use: TestParseRustUsePath#test_simple_use().
  TestParseRustUsePath.test_crate_prefixed: TestParseRustUsePath#test_crate_prefixed().
  TestParseRustUsePath.test_super_prefixed: TestParseRustUsePath#test_super_prefixed().
  TestParseRustUsePath.test_group_import_strips_braces: TestParseRustUsePath#test_group_import_strips_braces().
  TestParseRustUsePath.test_std_crate_still_parsed: TestParseRustUsePath#test_std_crate_still_parsed().
  TestParseRustUsePath.test_empty_returns_none: TestParseRustUsePath#test_empty_returns_none().
  MockNode._type: MockNode#_type.
  MockNode._text: MockNode#_text.
  MockNode._children: MockNode#_children.
  MockNode.__init__: MockNode#__init__().
  TestNodeText: TestNodeText#
  TestParseRustUsePath: TestParseRustUsePath#
  TestExtractPythonImportSimple: TestExtractPythonImportSimple#
  TestExtractPythonImportFrom: TestExtractPythonImportFrom#
  TestExtractPythonImports: TestExtractPythonImports#
  TestExtractJsImports: TestExtractJsImports#
  TestExtractGoImports: TestExtractGoImports#
  TestExtractRustImports: TestExtractRustImports#
  TestExtractCppImports: TestExtractCppImports#
  TestExtractJavaImports: TestExtractJavaImports#
  TestWalkImports: TestWalkImports#
  TestExtractCSharpImports: TestExtractCSharpImports#
  TestExtractKotlinImports: TestExtractKotlinImports#
  TestExtractSwiftImports: TestExtractSwiftImports#
  TestExtractRubyImports: TestExtractRubyImports#
  TestExtractPhpImports: TestExtractPhpImports#
---
# Module: [`tests/unit/test_import_extractors.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py)

## Classes
### `MockNode`
- def: [`tests/unit/test_import_extractors.py:28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L28)
- signature: `class MockNode:`
- members:
  - `child_by_field_name(self, name: str)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L45)
  - `children(self)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L42)
  - `type(self)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L38)
  - `end_byte` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L35)
  - `start_byte` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L34)
- protocol/private: `__init__`[`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L29), `__repr__`[`L48`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L48), `_children`[`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L32), `_fields`[`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L33), `_text`[`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L31), `_type`[`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L30)
- used by: (49 test-only callers)

### `TestExtractCSharpImports`
- def: [`tests/unit/test_import_extractors.py:459`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L459)
- signature: `class TestExtractCSharpImports:`
- members:
  - `test_extracts_third_party(self)` — [`L468`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L468)
  - `test_non_using_directive_skipped(self)` — [`L483`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L483)
  - `test_skips_stdlib_system(self)` — [`L460`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L460)
- uses (calls/refs, reference-scoped): [`_extract_csharp_imports`](../../tree_sitter_analyzer/import_extractors/_other_langs.md#_extract_csharp_imports)  (4 test-only)

### `TestExtractCppImports`
- def: [`tests/unit/test_import_extractors.py:306`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L306)
- signature: `class TestExtractCppImports:`
- members:
  - `test_local_include(self)` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L307)
  - `test_non_include_skipped(self)` — [`L336`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L336)
  - `test_system_include(self)` — [`L322`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L322)
- uses (calls/refs, reference-scoped): [`_extract_cpp_imports`](../../tree_sitter_analyzer/import_extractors/_cpp.md#_extract_cpp_imports)  (3 test-only)

### `TestExtractGoImports`
- def: [`tests/unit/test_import_extractors.py:227`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L227)
- signature: `class TestExtractGoImports:`
- members:
  - `test_extracts_third_party(self)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L244)
  - `test_non_import_declaration_skipped(self)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L264)
  - `test_skips_stdlib(self)` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L228)
- uses (calls/refs, reference-scoped): [`_extract_go_imports`](../../tree_sitter_analyzer/import_extractors/_go.md#_extract_go_imports)  (3 test-only)

### `TestExtractJavaImports`
- def: [`tests/unit/test_import_extractors.py:348`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L348)
- signature: `class TestExtractJavaImports:`
- members:
  - `test_extracts_third_party(self)` — [`L357`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L357)
  - `test_skips_java_stdlib(self)` — [`L349`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L349)
  - `test_static_import(self)` — [`L366`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L366)
  - `test_wildcard_import(self)` — [`L374`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L374)
- uses (calls/refs, reference-scoped): [`_extract_java_imports`](../../tree_sitter_analyzer/import_extractors/_java.md#_extract_java_imports)  (3 test-only)

### `TestExtractJsImports`
- def: [`tests/unit/test_import_extractors.py:189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L189)
- signature: `class TestExtractJsImports:`
- members:
  - `test_import_statement_extracts_module(self)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L190)
  - `test_require_call_extracts(self)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L203)
- uses (calls/refs, reference-scoped): [`_extract_js_imports`](../../tree_sitter_analyzer/import_extractors/_javascript.md#_extract_js_imports)  (4 test-only)

### `TestExtractKotlinImports`
- def: [`tests/unit/test_import_extractors.py:495`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L495)
- signature: `class TestExtractKotlinImports:`
- members:
  - `test_extracts_third_party(self)` — [`L504`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L504)
  - `test_non_import_skipped(self)` — [`L523`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L523)
  - `test_skips_kotlin_stdlib(self)` — [`L496`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L496)
  - `test_wildcard_import(self)` — [`L514`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L514)
- uses (calls/refs, reference-scoped): [`_extract_kotlin_imports`](../../tree_sitter_analyzer/import_extractors/_other_langs.md#_extract_kotlin_imports)  (3 test-only)

### `TestExtractPhpImports`
- def: [`tests/unit/test_import_extractors.py:626`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L626)
- signature: `class TestExtractPhpImports:`
- members:
  - `test_aliased_use(self)` — [`L645`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L645)
  - `test_extracts_use_declaration(self)` — [`L627`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L627)
  - `test_function_use(self)` — [`L637`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L637)
  - `test_non_use_skipped(self)` — [`L654`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L654)
- uses (calls/refs, reference-scoped): [`_extract_php_imports`](../../tree_sitter_analyzer/import_extractors/_other_langs.md#_extract_php_imports)  (3 test-only)

### `TestExtractPythonImportFrom`
- def: [`tests/unit/test_import_extractors.py:139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L139)
- signature: `class TestExtractPythonImportFrom:`
- members:
  - `test_no_module_name_returns_early(self)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L152)
  - `test_skips_stdlib_from_import(self)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L140)
- uses (calls/refs, reference-scoped): [`extract_python_import_from`](../../tree_sitter_analyzer/import_extractors/_python.md#extract_python_import_from)  (2 test-only)

### `TestExtractPythonImportSimple`
- def: [`tests/unit/test_import_extractors.py:110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L110)
- signature: `class TestExtractPythonImportSimple:`
- members:
  - `test_extracts_third_party(self)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L124)
  - `test_skips_stdlib(self)` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L111)
- uses (calls/refs, reference-scoped): [`extract_python_import_simple`](../../tree_sitter_analyzer/import_extractors/_python.md#extract_python_import_simple)  (4 test-only)

### `TestExtractPythonImports`
- def: [`tests/unit/test_import_extractors.py:164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L164)
- signature: `class TestExtractPythonImports:`
- members:
  - `test_import_statement_dispatches(self)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L165)
  - `test_non_import_node_skipped(self)` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L177)
- uses (calls/refs, reference-scoped): [`_extract_python_imports`](../../tree_sitter_analyzer/import_extractors/_python.md#_extract_python_imports)  (2 test-only)

### `TestExtractRubyImports`
- def: [`tests/unit/test_import_extractors.py:568`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L568)
- signature: `class TestExtractRubyImports:`
- members:
  - `test_non_call_skipped(self)` — [`L614`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L614)
  - `test_require_extracts_gem(self)` — [`L569`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L569)
  - `test_require_relative_extracts(self)` — [`L585`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L585)
  - `test_require_skips_stdlib(self)` — [`L600`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L600)
- uses (calls/refs, reference-scoped): [`_extract_ruby_imports`](../../tree_sitter_analyzer/import_extractors/_other_langs.md#_extract_ruby_imports)  (4 test-only)

### `TestExtractRustImports`
- def: [`tests/unit/test_import_extractors.py:276`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L276)
- signature: `class TestExtractRustImports:`
- members:
  - `test_extracts_crate_local(self)` — [`L285`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L285)
  - `test_non_use_declaration_skipped(self)` — [`L294`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L294)
  - `test_skips_std_crate(self)` — [`L277`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L277)
- uses (calls/refs, reference-scoped): [`_extract_rust_imports`](../../tree_sitter_analyzer/import_extractors/_rust.md#_extract_rust_imports)  (3 test-only)

### `TestExtractSwiftImports`
- def: [`tests/unit/test_import_extractors.py:535`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L535)
- signature: `class TestExtractSwiftImports:`
- members:
  - `test_extracts_custom_framework(self)` — [`L545`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L545)
  - `test_non_import_skipped(self)` — [`L556`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L556)
  - `test_skips_stdlib_foundation(self)` — [`L536`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L536)
- uses (calls/refs, reference-scoped): [`_extract_swift_imports`](../../tree_sitter_analyzer/import_extractors/_other_langs.md#_extract_swift_imports)  (3 test-only)

### `TestNodeText`
- def: [`tests/unit/test_import_extractors.py:57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L57)
- signature: `class TestNodeText:`
- members:
  - `test_extracts_text_by_byte_range(self)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L58)
  - `test_returns_empty_for_mismatched_range(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L65)
  - `test_returns_empty_for_none_range(self)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L71)
- uses (calls/refs, reference-scoped): [`_node_text`](../../tree_sitter_analyzer/import_extractors/_shared.md#_node_text)  (3 test-only)

### `TestParseRustUsePath`
- def: [`tests/unit/test_import_extractors.py:83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L83)
- signature: `class TestParseRustUsePath:`
- members:
  - `test_crate_prefixed(self)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L87)
  - `test_empty_returns_none(self)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L100)
  - `test_group_import_strips_braces(self)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L93)
  - `test_simple_use(self)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L84)
  - `test_std_crate_still_parsed(self)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L96)
  - `test_super_prefixed(self)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L90)
- uses (calls/refs, reference-scoped): [`_parse_rust_use_path`](../../tree_sitter_analyzer/import_extractors/_rust.md#_parse_rust_use_path)

### `TestWalkImports`
- def: [`tests/unit/test_import_extractors.py:389`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L389)
- signature: `class TestWalkImports:`
- members:
  - `test_csharp_dispatch(self)` — [`L402`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L402)
  - `test_kotlin_dispatch(self)` — [`L411`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L411)
  - `test_php_dispatch(self)` — [`L444`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L444)
  - `test_ruby_dispatch(self)` — [`L429`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L429)
  - `test_swift_dispatch(self)` — [`L420`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L420)
  - `test_unsupported_language_no_error(self)` — [`L390`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L390)
  - `test_walks_children_recursively(self)` — [`L396`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_import_extractors.py#L396)
- uses (calls/refs, reference-scoped): [`walk_imports`](../../tree_sitter_analyzer/import_extractors/__init__.md#walk_imports)  (5 test-only)

