---
title: 'Module: tests/unit/languages/test_is_constructor_531.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_is_constructor_531.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_is_constructor_531`/
symbols:
  TestCppIsConstructor.functions: TestCppIsConstructor#functions().
  TestPythonIsConstructor.functions: TestPythonIsConstructor#functions().
  TestRubyIsConstructor.functions: TestRubyIsConstructor#functions().
  TestPhpIsConstructor.functions: TestPhpIsConstructor#functions().
  TestScalaIsConstructor.functions: TestScalaIsConstructor#functions().
  TestDecoratedPythonConstructor.test_decorated_init_is_constructor: TestDecoratedPythonConstructor#test_decorated_init_is_constructor().
  TestCppHeaderConstructorDeclaration.test_header_declaration_is_constructor: TestCppHeaderConstructorDeclaration#test_header_declaration_is_constructor().
  _CPP_SRC: _CPP_SRC.
  TestPythonIsConstructor.extractor: TestPythonIsConstructor#extractor().
  _PYTHON_SRC: _PYTHON_SRC.
  _RUBY_SRC: _RUBY_SRC.
  _PHP_SRC: _PHP_SRC.
  _SCALA_SRC: _SCALA_SRC.
  TestPythonIsConstructor: TestPythonIsConstructor#
  TestPythonIsConstructor.test_init_in_class_is_constructor_true: TestPythonIsConstructor#test_init_in_class_is_constructor_true().
  TestPythonIsConstructor.test_regular_method_is_constructor_false: TestPythonIsConstructor#test_regular_method_is_constructor_false().
  TestPythonIsConstructor.test_module_level_init_is_constructor_false: TestPythonIsConstructor#test_module_level_init_is_constructor_false().
  TestRubyIsConstructor: TestRubyIsConstructor#
  TestRubyIsConstructor.test_initialize_is_constructor_true: TestRubyIsConstructor#test_initialize_is_constructor_true().
  TestRubyIsConstructor.test_regular_method_is_constructor_false: TestRubyIsConstructor#test_regular_method_is_constructor_false().
  TestPhpIsConstructor: TestPhpIsConstructor#
  TestPhpIsConstructor.test_construct_is_constructor_true: TestPhpIsConstructor#test_construct_is_constructor_true().
  TestPhpIsConstructor.test_regular_method_is_constructor_false: TestPhpIsConstructor#test_regular_method_is_constructor_false().
  TestScalaIsConstructor: TestScalaIsConstructor#
  TestScalaIsConstructor.test_def_this_is_constructor_true: TestScalaIsConstructor#test_def_this_is_constructor_true().
  TestScalaIsConstructor.test_regular_method_is_constructor_false: TestScalaIsConstructor#test_regular_method_is_constructor_false().
  TestCppIsConstructor: TestCppIsConstructor#
  TestCppIsConstructor.test_constructor_is_constructor_true: TestCppIsConstructor#test_constructor_is_constructor_true().
  TestCppIsConstructor.test_destructor_is_constructor_false: TestCppIsConstructor#test_destructor_is_constructor_false().
  TestCppIsConstructor.test_regular_method_is_constructor_false: TestCppIsConstructor#test_regular_method_is_constructor_false().
  TestCppIsConstructor.test_global_function_is_constructor_false: TestCppIsConstructor#test_global_function_is_constructor_false().
  TestDecoratedPythonConstructor: TestDecoratedPythonConstructor#
  TestCppHeaderConstructorDeclaration: TestCppHeaderConstructorDeclaration#
---
# Module: [`tests/unit/languages/test_is_constructor_531.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py)

## Classes
### `TestCppHeaderConstructorDeclaration`
- def: [`tests/unit/languages/test_is_constructor_531.py:278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L278)
- doc: Codex P2 on #567: body-less constructor declarations in headers go
- signature: `class TestCppHeaderConstructorDeclaration:`
- members:
  - `test_header_declaration_is_constructor(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L282)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`CppElementExtractor`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor), [`extract_functions`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_functions), [`is_constructor`](../../../tree_sitter_analyzer/models/base.md#Function.is_constructor)

### `TestCppIsConstructor`
- def: [`tests/unit/languages/test_is_constructor_531.py:218`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L218)
- doc: Constructor (name == class name) → True; destructor → False; regular → False.
- signature: `class TestCppIsConstructor:`
- members:
  - `functions(self)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L222)
  - `test_constructor_is_constructor_true(self, functions)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L232)
  - `test_destructor_is_constructor_false(self, functions)` — [`L236`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L236)
  - `test_global_function_is_constructor_false(self, functions)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L244)
  - `test_regular_method_is_constructor_false(self, functions)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L240)
- uses (calls/refs, reference-scoped): [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`CppPlugin`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin), [`create_cpp_parser`](../../../tree_sitter_analyzer/languages/_cpp_plugin_analysis_helpers.md#create_cpp_parser), [`create_extractor`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin.create_extractor), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppPlugin.get_tree_sitter_language)  (1 test-only)

### `TestDecoratedPythonConstructor`
- def: [`tests/unit/languages/test_is_constructor_531.py:249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L249)
- doc: Codex P2 on #567: decorated_definition sits between the function and
- signature: `class TestDecoratedPythonConstructor:`
- members:
  - `test_decorated_init_is_constructor(self)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L253)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor), [`is_constructor`](../../../tree_sitter_analyzer/models/base.md#Function.is_constructor), [`extract_functions`](../../../tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.md#PythonFunctionExtractionMixin.extract_functions)

### `TestPhpIsConstructor`
- def: [`tests/unit/languages/test_is_constructor_531.py:146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L146)
- doc: __construct → True; regular method → False; standalone function → None/False.
- signature: `class TestPhpIsConstructor:`
- members:
  - `functions(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L150)
  - `test_construct_is_constructor_true(self, functions)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L159)
  - `test_regular_method_is_constructor_false(self, functions)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L163)
- uses (calls/refs, reference-scoped): [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`PHPPlugin`](../../../tree_sitter_analyzer/languages/php_plugin.md#PHPPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/php_plugin.md#PHPPlugin.create_extractor), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/php_plugin.md#PHPPlugin.get_tree_sitter_language)  (1 test-only)

### `TestPythonIsConstructor`
- def: [`tests/unit/languages/test_is_constructor_531.py:52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L52)
- doc: __init__ inside a class → True; outside → False.
- signature: `class TestPythonIsConstructor:`
- members:
  - `extractor(self)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L56)
  - `functions(self, extractor: PythonElementExtractor)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L60)
  - `test_init_in_class_is_constructor_true(self, functions)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L68)
  - `test_module_level_init_is_constructor_false(self, functions)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L78)
  - `test_regular_method_is_constructor_false(self, functions)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L74)
- uses (calls/refs, reference-scoped): [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor), [`PythonPlugin`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.get_tree_sitter_language), [`extract_functions`](../../../tree_sitter_analyzer/languages/python_plugin/_function_extractor_mixin.md#PythonFunctionExtractionMixin.extract_functions)  (1 test-only)

### `TestRubyIsConstructor`
- def: [`tests/unit/languages/test_is_constructor_531.py:104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L104)
- doc: initialize → True; regular method → False.
- signature: `class TestRubyIsConstructor:`
- members:
  - `functions(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L108)
  - `test_initialize_is_constructor_true(self, functions)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L117)
  - `test_regular_method_is_constructor_false(self, functions)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L121)
- uses (calls/refs, reference-scoped): [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`RubyPlugin`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.create_extractor), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/ruby_plugin.md#RubyPlugin.get_tree_sitter_language)  (1 test-only)

### `TestScalaIsConstructor`
- def: [`tests/unit/languages/test_is_constructor_531.py:180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L180)
- doc: def this(...) → True; regular method → False.
- signature: `class TestScalaIsConstructor:`
- members:
  - `functions(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L184)
  - `test_def_this_is_constructor_true(self, functions)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L193)
  - `test_regular_method_is_constructor_false(self, functions)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L197)
- uses (calls/refs, reference-scoped): [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`ScalaPlugin`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaPlugin), [`get_tree_sitter_language`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaPlugin.get_tree_sitter_language), [`create_extractor`](../../../tree_sitter_analyzer/languages/scala_plugin.md#ScalaPlugin.create_extractor)  (1 test-only)

## Module values
- `_CPP_SRC` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L206)
- `_PHP_SRC` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L130)
- `_PYTHON_SRC` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L37)
- `_RUBY_SRC` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L90)
- `_SCALA_SRC` — [`L172`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_is_constructor_531.py#L172)

