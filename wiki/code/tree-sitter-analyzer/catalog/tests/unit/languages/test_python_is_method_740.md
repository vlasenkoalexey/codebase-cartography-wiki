---
title: 'Module: tests/unit/languages/test_python_is_method_740.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_is_method_740.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_is_method_740`/
symbols:
  TestPythonIsMethod._get_functions: TestPythonIsMethod#_get_functions().
  _TREE_SITTER_AVAILABLE: _TREE_SITTER_AVAILABLE.
  TestPythonControlFlowMethods._get_functions: TestPythonControlFlowMethods#_get_functions().
  TestPythonParentClass._get_functions: TestPythonParentClass#_get_functions().
  _SOURCE: _SOURCE.
  pytestmark: pytestmark.
  extractor: extractor().
  TestPythonIsMethod.test_parse_file_is_method: TestPythonIsMethod#test_parse_file_is_method().
  TestPythonIsMethod.test_init_is_method: TestPythonIsMethod#test_init_is_method().
  TestPythonIsMethod.test_static_method_is_method: TestPythonIsMethod#test_static_method_is_method().
  TestPythonIsMethod.test_classmethod_is_method: TestPythonIsMethod#test_classmethod_is_method().
  TestPythonIsMethod.test_standalone_function_is_not_method: TestPythonIsMethod#test_standalone_function_is_not_method().
  TestPythonParentClass.test_parse_file_parent_class: TestPythonParentClass#test_parse_file_parent_class().
  TestPythonParentClass.test_init_parent_class: TestPythonParentClass#test_init_parent_class().
  TestPythonParentClass.test_standalone_no_parent_class: TestPythonParentClass#test_standalone_no_parent_class().
  TestPythonControlFlowMethods.test_if_branch_method_is_method: TestPythonControlFlowMethods#test_if_branch_method_is_method().
  TestPythonControlFlowMethods.test_if_branch_method_parent_class: TestPythonControlFlowMethods#test_if_branch_method_parent_class().
  TestPythonControlFlowMethods.test_else_branch_method_is_method: TestPythonControlFlowMethods#test_else_branch_method_is_method().
  TestPythonControlFlowMethods.test_try_block_method_is_method: TestPythonControlFlowMethods#test_try_block_method_is_method().
  _CONDITIONAL_SOURCE: _CONDITIONAL_SOURCE.
  py_parser: py_parser().
  TestPythonIsMethod: TestPythonIsMethod#
  TestPythonParentClass: TestPythonParentClass#
  TestPythonControlFlowMethods: TestPythonControlFlowMethods#
---
# Module: [`tests/unit/languages/test_python_is_method_740.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py)

## Classes
### `TestPythonControlFlowMethods`
- def: [`tests/unit/languages/test_python_is_method_740.py:143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L143)
- doc: Codex P2 on #740: methods inside if/try inside a class must be detected.
- signature: `class TestPythonControlFlowMethods:`
- members:
  - `test_else_branch_method_is_method(self, extractor, py_parser)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L168) — posix_method inside 'else' must be is_method=True.
  - `test_if_branch_method_is_method(self, extractor, py_parser)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L152) — win_method inside 'if sys.platform' must be is_method=True.
  - `test_if_branch_method_parent_class(self, extractor, py_parser)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L160) — win_method must know its parent is Platform.
  - `test_try_block_method_is_method(self, extractor, py_parser)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L174) — try_method inside 'try' block in class body must be is_method=True.
- protocol/private: `_get_functions`[`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L146)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestPythonIsMethod`
- def: [`tests/unit/languages/test_python_is_method_740.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L61)
- doc: is_method must be True for class methods, False for module-level fns.
- signature: `class TestPythonIsMethod:`
- members:
  - `test_classmethod_is_method(self, extractor, py_parser)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L87)
  - `test_init_is_method(self, extractor, py_parser)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L75)
  - `test_parse_file_is_method(self, extractor, py_parser)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L68)
  - `test_standalone_function_is_not_method(self, extractor, py_parser)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L92)
  - `test_static_method_is_method(self, extractor, py_parser)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L80)
- protocol/private: `_get_functions`[`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L64)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestPythonParentClass`
- def: [`tests/unit/languages/test_python_is_method_740.py:100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L100)
- doc: parent_class must be set to the enclosing class name for methods.
- signature: `class TestPythonParentClass:`
- members:
  - `test_init_parent_class(self, extractor, py_parser)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L113)
  - `test_parse_file_parent_class(self, extractor, py_parser)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L107)
  - `test_standalone_no_parent_class(self, extractor, py_parser)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L117)
- protocol/private: `_get_functions`[`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L103)
- uses (calls/refs, reference-scoped): (1 test-only callers)

## Functions
- `extractor()` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L57)
- `py_parser()` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L51)

## Module values
- `_CONDITIONAL_SOURCE` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L124)
- `_SOURCE` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L28)
- `_TREE_SITTER_AVAILABLE` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L15)
- `pytestmark` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_is_method_740.py#L23)

