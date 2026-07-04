---
title: 'Module: tests/unit/test_ast_path.py'
type: catalog
provenance: extracted
module: tests/unit/test_ast_path.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ast_path`/
symbols:
  TestPathAtLine.test_line_inside_method: TestPathAtLine#test_line_inside_method().
  TestPathAtLine.test_line_at_class_def: TestPathAtLine#test_line_at_class_def().
  TestPathAtLine.test_line_at_standalone_function: TestPathAtLine#test_line_at_standalone_function().
  TestPathAtLine.test_line_in_init: TestPathAtLine#test_line_in_init().
  TestPathAtLine.test_java_line_in_method: TestPathAtLine#test_java_line_in_method().
  TestScopeAt.test_scope_inside_method: TestScopeAt#test_scope_inside_method().
  TestScopeAt.test_scope_inside_class_not_method: TestScopeAt#test_scope_inside_class_not_method().
  TestScopeAt.test_scope_at_standalone: TestScopeAt#test_scope_at_standalone().
  TestOutline.test_python_outline: TestOutline#test_python_outline().
  TestOutline.test_outline_max_depth: TestOutline#test_outline_max_depth().
  TestOutline.test_java_outline: TestOutline#test_java_outline().
  TestToDict.test_node_to_dict: TestToDict#test_node_to_dict().
  TestEdgeCases.test_empty_file: TestEdgeCases#test_empty_file().
  TestEdgeCases.test_comment_only_file: TestEdgeCases#test_comment_only_file().
  TestPathAtLine.test_line_out_of_range: TestPathAtLine#test_line_out_of_range().
  TestToDict.test_result_to_dict: TestToDict#test_result_to_dict().
  TestPathAtLine.test_file_not_found: TestPathAtLine#test_file_not_found().
  python_file: python_file().
  java_file: java_file().
  _PYTHON_SAMPLE: _PYTHON_SAMPLE.
  _JAVA_SAMPLE: _JAVA_SAMPLE.
  TestPathAtLine: TestPathAtLine#
  TestScopeAt: TestScopeAt#
  TestOutline: TestOutline#
  TestToDict: TestToDict#
  TestEdgeCases: TestEdgeCases#
---
# Module: [`tests/unit/test_ast_path.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py)

## Classes
### `TestEdgeCases`
- def: [`tests/unit/test_ast_path.py:184`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L184)
- signature: `class TestEdgeCases:`
- members:
  - `test_comment_only_file(self, tmp_path)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L193)
  - `test_empty_file(self, tmp_path)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L185)
- uses (calls/refs, reference-scoped): [`path_at_line`](../../tree_sitter_analyzer/ast_path.md#ASTPathNavigator.path_at_line), [`ASTPathNavigator`](../../tree_sitter_analyzer/ast_path.md#ASTPathNavigator), [`path`](../../tree_sitter_analyzer/ast_path.md#ASTPathResult.path), [`target_line`](../../tree_sitter_analyzer/ast_path.md#ASTPathResult.target_line)

### `TestOutline`
- def: [`tests/unit/test_ast_path.py:140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L140)
- signature: `class TestOutline:`
- members:
  - `test_java_outline(self, java_file)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L155)
  - `test_outline_max_depth(self, python_file)` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L148)
  - `test_python_outline(self, python_file)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L141)
- uses (calls/refs, reference-scoped): [`name`](../../tree_sitter_analyzer/ast_path.md#ASTNode.name), [`outline`](../../tree_sitter_analyzer/ast_path.md#ASTPathNavigator.outline), [`ASTPathNavigator`](../../tree_sitter_analyzer/ast_path.md#ASTPathNavigator), [`path`](../../tree_sitter_analyzer/ast_path.md#ASTPathResult.path)

### `TestPathAtLine`
- def: [`tests/unit/test_ast_path.py:73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L73)
- signature: `class TestPathAtLine:`
- members:
  - `test_file_not_found(self)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L113)
  - `test_java_line_in_method(self, java_file)` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L106)
  - `test_line_at_class_def(self, python_file)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L82)
  - `test_line_at_standalone_function(self, python_file)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L88)
  - `test_line_in_init(self, python_file)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L95)
  - `test_line_inside_method(self, python_file)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L74)
  - `test_line_out_of_range(self, python_file)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L101)
- uses (calls/refs, reference-scoped): [`path_at_line`](../../tree_sitter_analyzer/ast_path.md#ASTPathNavigator.path_at_line), [`name`](../../tree_sitter_analyzer/ast_path.md#ASTNode.name), [`ASTPathNavigator`](../../tree_sitter_analyzer/ast_path.md#ASTPathNavigator), [`path`](../../tree_sitter_analyzer/ast_path.md#ASTPathResult.path), [`target_line`](../../tree_sitter_analyzer/ast_path.md#ASTPathResult.target_line)

### `TestScopeAt`
- def: [`tests/unit/test_ast_path.py:119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L119)
- signature: `class TestScopeAt:`
- members:
  - `test_scope_at_standalone(self, python_file)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L132)
  - `test_scope_inside_class_not_method(self, python_file)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L126)
  - `test_scope_inside_method(self, python_file)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L120)
- uses (calls/refs, reference-scoped): [`name`](../../tree_sitter_analyzer/ast_path.md#ASTNode.name), [`ASTPathNavigator`](../../tree_sitter_analyzer/ast_path.md#ASTPathNavigator), [`scope_at`](../../tree_sitter_analyzer/ast_path.md#ASTPathNavigator.scope_at), [`enclosing_scope`](../../tree_sitter_analyzer/ast_path.md#ASTPathResult.enclosing_scope)

### `TestToDict`
- def: [`tests/unit/test_ast_path.py:162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L162)
- signature: `class TestToDict:`
- members:
  - `test_node_to_dict(self, python_file)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L174)
  - `test_result_to_dict(self, python_file)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L163)
- uses (calls/refs, reference-scoped): [`path_at_line`](../../tree_sitter_analyzer/ast_path.md#ASTPathNavigator.path_at_line), [`ASTPathNavigator`](../../tree_sitter_analyzer/ast_path.md#ASTPathNavigator), [`to_dict`](../../tree_sitter_analyzer/ast_path.md#ASTPathResult.to_dict), [`to_dict`](../../tree_sitter_analyzer/ast_path.md#ASTNode.to_dict), [`path`](../../tree_sitter_analyzer/ast_path.md#ASTPathResult.path)

## Functions
- `java_file(tmp_path)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L67)
- `python_file(tmp_path)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L60)

## Module values
- `_JAVA_SAMPLE` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L38)
- `_PYTHON_SAMPLE` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_path.py#L8)

