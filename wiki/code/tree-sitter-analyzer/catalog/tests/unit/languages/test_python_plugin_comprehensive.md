---
title: 'Module: tests/unit/languages/test_python_plugin_comprehensive.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_python_plugin_comprehensive.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_python_plugin_comprehensive`/TestPythonPlugin
symbols:
  TestPythonPluginIntegration.test_full_extraction_workflow: Integration#test_full_extraction_workflow().
  TestPythonPluginIntegration.test_error_recovery_integration: Integration#test_error_recovery_integration().
  TestPythonPluginIntegration.test_framework_detection_integration: Integration#test_framework_detection_integration().
  TestPythonPlugin.plugin: '#plugin().'
  TestPythonPlugin.test_plugin_initialization: '#test_plugin_initialization().'
  TestPythonPlugin: '#'
  TestPythonPlugin.test_plugin_extract_functions: '#test_plugin_extract_functions().'
  TestPythonPlugin.test_plugin_extract_classes: '#test_plugin_extract_classes().'
  TestPythonPlugin.test_plugin_extract_variables: '#test_plugin_extract_variables().'
  TestPythonPlugin.test_plugin_extract_imports: '#test_plugin_extract_imports().'
  TestPythonPlugin.test_plugin_with_real_python_code: '#test_plugin_with_real_python_code().'
  TestPythonPluginIntegration: Integration#
---
# Module: [`tests/unit/languages/test_python_plugin_comprehensive.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py)

## Classes
### `TestPythonPlugin`
- def: [`tests/unit/languages/test_python_plugin_comprehensive.py:13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L13)
- doc: Test Python plugin main class
- signature: `class TestPythonPlugin:`
- members:
  - `plugin(self)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L17) — Create a Python plugin instance
  - `test_plugin_extract_classes(self, plugin)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L37) — Test plugin class extraction
  - `test_plugin_extract_functions(self, plugin)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L27) — Test plugin function extraction
  - `test_plugin_extract_imports(self, plugin)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L57) — Test plugin import extraction
  - `test_plugin_extract_variables(self, plugin)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L47) — Test plugin variable extraction
  - `test_plugin_initialization(self, plugin)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L21) — Test plugin initialization
  - `test_plugin_with_real_python_code(self, plugin)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L67) — Test plugin with realistic Python code
- uses (calls/refs, reference-scoped): [`PythonElementExtractor`](../../../tree_sitter_analyzer/languages/python_plugin/extractor.md#PythonElementExtractor), [`PythonPlugin`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin)

### `TestPythonPluginIntegration`
- def: [`tests/unit/languages/test_python_plugin_comprehensive.py:134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L134)
- doc: Integration tests for Python plugin
- signature: `class TestPythonPluginIntegration:`
- members:
  - `test_error_recovery_integration(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L326) — Test error recovery in integration scenario
  - `test_framework_detection_integration(self)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L301) — Test framework detection in integration scenario
  - `test_full_extraction_workflow(self)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_python_plugin_comprehensive.py#L137) — Test complete extraction workflow
- uses (calls/refs, reference-scoped): [`extract_functions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_functions), [`extract_classes`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_classes), [`extract_variables`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_variables), [`extract_imports`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_imports), [`PythonPlugin`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin), [`create_extractor`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.create_extractor), [`extractor`](../../../tree_sitter_analyzer/languages/python_plugin/plugin.md#PythonPlugin.extractor)

