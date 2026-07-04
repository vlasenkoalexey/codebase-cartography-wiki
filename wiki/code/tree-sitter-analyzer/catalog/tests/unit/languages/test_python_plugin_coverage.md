---
title: 'Module: tests/unit/languages/test_python_plugin_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_plugin_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_plugin_coverage`/TestPython
symbols:
  TestPythonPlugin.plugin: Plugin#plugin().
  TestPythonElementExtractor.extractor: ElementExtractor#extractor().
  TestPythonPlugin: Plugin#
  TestPythonPlugin.test_plugin_properties: Plugin#test_plugin_properties().
  TestPythonPlugin.test_is_applicable_method: Plugin#test_is_applicable_method().
  TestPythonElementExtractor: ElementExtractor#
  TestPythonElementExtractor.test_extract_methods_return_lists: ElementExtractor#test_extract_methods_return_lists().
  TestPythonElementExtractor.test_extract_without_language: ElementExtractor#test_extract_without_language().
---
# Module: [`tests/unit/languages/test_python_plugin_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage.py)

## Classes
### `TestPythonElementExtractor`
- def: [`tests/unit/languages/test_python_plugin_coverage.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage.py#L43)
- doc: PythonElementExtractorの基本テストクラス
- signature: `class TestPythonElementExtractor:`
- members:
  - `extractor(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage.py#L47) — Extractorインスタンスを提供
  - `test_extract_methods_return_lists(self, extractor)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage.py#L51) — 抽出メソッドがリストを返すことを確認
  - `test_extract_without_language(self, extractor)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage.py#L67) — 言語なしでの抽出テスト
- uses (calls/refs, reference-scoped): [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor)

### `TestPythonPlugin`
- def: [`tests/unit/languages/test_python_plugin_coverage.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage.py#L18)
- doc: PythonPluginの基本テストクラス
- signature: `class TestPythonPlugin:`
- members:
  - `plugin(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage.py#L22) — Pluginインスタンスを提供
  - `test_is_applicable_method(self, plugin)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage.py#L32) — is_applicableメソッドテスト
  - `test_plugin_properties(self, plugin)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_coverage.py#L26) — プラグインプロパティテスト
- uses (calls/refs, reference-scoped): [`PythonPlugin`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin)

