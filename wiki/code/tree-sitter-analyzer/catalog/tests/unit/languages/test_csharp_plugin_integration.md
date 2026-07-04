---
title: 'Module: tests/unit/languages/test_csharp_plugin_integration.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_csharp_plugin_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_csharp_plugin_integration`/
symbols:
  TestCSharpIntegration.test_full_extraction_workflow: TestCSharpIntegration#test_full_extraction_workflow().
  TestCSharpPluginAnalyzeFile.test_analyze_file_with_temp_file: TestCSharpPluginAnalyzeFile#test_analyze_file_with_temp_file().
  TestCSharpIntegration.test_record_type_extraction: TestCSharpIntegration#test_record_type_extraction().
  TestCSharpIntegration.test_struct_extraction: TestCSharpIntegration#test_struct_extraction().
  TestCSharpIntegration.test_enum_extraction: TestCSharpIntegration#test_enum_extraction().
  COMPLEX_CLASS_CODE: COMPLEX_CLASS_CODE.
  get_tree_for_code: get_tree_for_code().
  TestCSharpPluginAnalyzeFile.test_analyze_file_nonexistent: TestCSharpPluginAnalyzeFile#test_analyze_file_nonexistent().
  TestCSharpIntegration.test_plugin_loads_successfully: TestCSharpIntegration#test_plugin_loads_successfully().
  TestCSharpIntegration.test_cs_file_extension_recognized: TestCSharpIntegration#test_cs_file_extension_recognized().
  TestCSharpIntegration.test_analyze_sample_file: TestCSharpIntegration#test_analyze_sample_file().
  SIMPLE_CLASS_CODE: SIMPLE_CLASS_CODE.
  INTERFACE_CODE: INTERFACE_CODE.
  ASYNC_METHOD_CODE: ASYNC_METHOD_CODE.
  PROPERTY_VARIATIONS_CODE: PROPERTY_VARIATIONS_CODE.
  CONTROL_FLOW_CODE: CONTROL_FLOW_CODE.
  TestCSharpPluginAnalyzeFile: TestCSharpPluginAnalyzeFile#
  TestCSharpIntegration: TestCSharpIntegration#
---
# Module: [`tests/unit/languages/test_csharp_plugin_integration.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py)

## Classes
### `TestCSharpIntegration`
- def: [`tests/unit/languages/test_csharp_plugin_integration.py:290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L290)
- doc: Integration tests for C# plugin.
- signature: `class TestCSharpIntegration:`
- members:
  - `test_analyze_sample_file(self)` — [`L359`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L359) — Test analysis of example C# file.
  - `test_cs_file_extension_recognized(self)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L299) — Test that .cs file extension is recognized.
  - `test_enum_extraction(self)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L344) — Test extraction of C# enum.
  - `test_full_extraction_workflow(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L305) — Test complete extraction workflow.
  - `test_plugin_loads_successfully(self)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L293) — Test that C# plugin loads successfully.
  - `test_record_type_extraction(self)` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L321) — Test extraction of C# record type.
  - `test_struct_extraction(self)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L334) — Test extraction of C# struct.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`extractor`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.extractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_classes), [`extract_functions`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_functions), [`extract_variables`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_variables), [`extract_imports`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpElementExtractor.extract_imports), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.get_file_extensions), [`get_language_name`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.get_language_name)  (2 test-only)

### `TestCSharpPluginAnalyzeFile`
- def: [`tests/unit/languages/test_csharp_plugin_integration.py:265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L265)
- doc: Test analyze_file method.
- signature: `class TestCSharpPluginAnalyzeFile:`
- members:
  - `test_analyze_file_nonexistent(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L269) — Test analyzing nonexistent file.
  - `test_analyze_file_with_temp_file(self, tmp_path)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L276) — Test analyzing a temporary C# file.
- uses (calls/refs, reference-scoped): [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`CSharpPlugin`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin), [`error_message`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.error_message), [`analyze_file`](../../../tree_sitter_analyzer/languages/csharp_plugin.md#CSharpPlugin.analyze_file)  (1 test-only)

## Functions
- `get_tree_for_code(code: str, plugin: CSharpPlugin)` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L252) — Helper to parse C# code and return tree.

## Module values
- `ASYNC_METHOD_CODE` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L52)
- `COMPLEX_CLASS_CODE` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L77)
- `CONTROL_FLOW_CODE` — [`L195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L195)
- `INTERFACE_CODE` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L38)
- `PROPERTY_VARIATIONS_CODE` — [`L155`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L155)
- `SIMPLE_CLASS_CODE` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_csharp_plugin_integration.py#L13)

