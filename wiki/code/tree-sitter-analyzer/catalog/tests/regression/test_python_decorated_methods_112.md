---
title: 'Module: tests/regression/test_python_decorated_methods_112.py'
type: catalog
provenance: extracted
module: tests/regression/test_python_decorated_methods_112.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.regression.test_python_decorated_methods_112`/TestPythonDecoratedMethodsRegression#
symbols:
  TestPythonDecoratedMethodsRegression._analyze_file: _analyze_file().
  TestPythonDecoratedMethodsRegression.plugin: plugin().
  TestPythonDecoratedMethodsRegression.test_normal_methods_count: test_normal_methods_count().
  TestPythonDecoratedMethodsRegression.test_classmethod_detection: test_classmethod_detection().
  TestPythonDecoratedMethodsRegression.test_staticmethod_detection: test_staticmethod_detection().
  TestPythonDecoratedMethodsRegression.test_mixed_methods_count: test_mixed_methods_count().
  TestPythonDecoratedMethodsRegression.test_property_detection: test_property_detection().
  TestPythonDecoratedMethodsRegression.test_no_methods_dropped: test_no_methods_dropped().
  TestPythonDecoratedMethodsRegression._create_mock_request: _create_mock_request().
  TestPythonDecoratedMethodsRegression: ''
  TestPythonDecoratedMethodsRegression.test_code: test_code().
---
# Module: [`tests/regression/test_python_decorated_methods_112.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py)

## Classes
### `TestPythonDecoratedMethodsRegression`
- def: [`tests/regression/test_python_decorated_methods_112.py:26`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L26)
- doc: 回归测试：确保装饰的方法（@classmethod, @staticmethod）被正确提取
- signature: `class TestPythonDecoratedMethodsRegression:`
- members:
  - `_analyze_file(self, plugin, file_path: str)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L43) — 分析文件并返回结果
  - `_create_mock_request(self, file_path: str)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L34) — 创建 mock AnalysisRequest
  - `plugin(self)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L30) — 创建 Python 插件实例
  - `test_classmethod_detection(self, plugin, test_code)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L117) — 测试 @classmethod 装饰的方法被正确提取
  - `test_code(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L49) — 测试代码：包含各种装饰器的类
  - `test_mixed_methods_count(self, plugin, test_code)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L192) — 测试混合方法类（普通 + classmethod + staticmethod）
  - `test_no_methods_dropped(self, plugin, test_code)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L251) — 综合测试：确保所有方法都被提取，没有遗漏
  - `test_normal_methods_count(self, plugin, test_code)` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L88) — 测试普通方法被正确提取
  - `test_property_detection(self, plugin, test_code)` — [`L222`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L222) — 测试 @property 装饰的方法被正确提取
  - `test_staticmethod_detection(self, plugin, test_code)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_python_decorated_methods_112.py#L155) — 测试 @staticmethod 装饰的方法被正确提取
- uses (calls/refs, reference-scoped): [`PythonPlugin`](../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin)

