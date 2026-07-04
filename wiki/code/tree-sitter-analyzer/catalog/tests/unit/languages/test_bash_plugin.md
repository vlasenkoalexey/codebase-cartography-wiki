---
title: 'Module: tests/unit/languages/test_bash_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_bash_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_bash_plugin`/
symbols:
  TestBashExtraction.test_extracts_function_definition: TestBashExtraction#test_extracts_function_definition().
  TestBashExtraction.test_extracts_control_flow_expression: TestBashExtraction#test_extracts_control_flow_expression().
  _parse: _parse().
  TestBashPluginMetadata.test_language_name: TestBashPluginMetadata#test_language_name().
  TestBashPluginMetadata.test_file_extensions: TestBashPluginMetadata#test_file_extensions().
  TestBashPluginMetadata.test_is_applicable: TestBashPluginMetadata#test_is_applicable().
  TestBashExtraction: TestBashExtraction#
  TestBashPluginMetadata: TestBashPluginMetadata#
---
# Module: [`tests/unit/languages/test_bash_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_plugin.py)

## Classes
### `TestBashExtraction`
- def: [`tests/unit/languages/test_bash_plugin.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_plugin.py#L19)
- signature: `class TestBashExtraction:`
- members:
  - `test_extracts_control_flow_expression(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_plugin.py#L29)
  - `test_extracts_function_definition(self)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_plugin.py#L20)
- uses (calls/refs, reference-scoped): [`extract_elements`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_elements), [`create_extractor`](../../../tree_sitter_analyzer/languages/bash_plugin.md#BashPlugin.create_extractor), [`extract_expressions`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.extract_expressions)  (1 test-only)

### `TestBashPluginMetadata`
- def: [`tests/unit/languages/test_bash_plugin.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_plugin.py#L38)
- signature: `class TestBashPluginMetadata:`
- members:
  - `test_file_extensions(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_plugin.py#L42)
  - `test_is_applicable(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_plugin.py#L45)
  - `test_language_name(self)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_plugin.py#L39)
- uses (calls/refs, reference-scoped): [`BashPlugin`](../../../tree_sitter_analyzer/languages/bash_plugin.md#BashPlugin), [`get_language_name`](../../../tree_sitter_analyzer/languages/bash_plugin.md#BashPlugin.get_language_name), [`is_applicable`](../../../tree_sitter_analyzer/languages/bash_plugin.md#BashPlugin.is_applicable), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/bash_plugin.md#BashPlugin.get_file_extensions)

## Functions
- `_parse(code: str)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_bash_plugin.py#L10)

