---
title: 'Module: tests/unit/languages/test_yaml_file_extension_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_file_extension_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_file_extension_properties`/
symbols:
  TestYAMLFileExtensionProperties.test_property_7_file_extension_selection_end_to_end_yaml: TestYAMLFileExtensionProperties#test_property_7_file_extension_selection_end_to_end_yaml().
  TestYAMLFileExtensionProperties.test_property_7_file_extension_selection_end_to_end_yml: TestYAMLFileExtensionProperties#test_property_7_file_extension_selection_end_to_end_yml().
  TestYAMLFileExtensionProperties.test_property_7_file_extension_selection_plugin_manager_integration: TestYAMLFileExtensionProperties#test_property_7_file_extension_selection_plugin_manager_integration().
  TestYAMLFileExtensionProperties.test_property_7_file_extension_selection_language_detection: TestYAMLFileExtensionProperties#test_property_7_file_extension_selection_language_detection().
  TestYAMLFileExtensionProperties.test_property_7_file_extension_selection_plugin_returns_yaml: TestYAMLFileExtensionProperties#test_property_7_file_extension_selection_plugin_returns_yaml().
  TestYAMLFileExtensionProperties.test_property_7_file_extension_selection_consistency: TestYAMLFileExtensionProperties#test_property_7_file_extension_selection_consistency().
  TestYAMLFileExtensionProperties.test_property_7_file_extension_selection_both_extensions_equivalent: TestYAMLFileExtensionProperties#test_property_7_file_extension_selection_both_extensions_equivalent().
  filename_strategy: filename_strategy.
  yaml_content_strategy: yaml_content_strategy.
  TestYAMLFileExtensionProperties: TestYAMLFileExtensionProperties#
---
# Module: [`tests/unit/languages/test_yaml_file_extension_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py)

## Classes
### `TestYAMLFileExtensionProperties`
- def: [`tests/unit/languages/test_yaml_file_extension_properties.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py#L47)
- doc: Property-based tests for YAML file extension selection.
- signature: `class TestYAMLFileExtensionProperties:`
- members:
  - `test_property_7_file_extension_selection_both_extensions_equivalent(self, extension: str)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py#L300) — Feature: yaml-language-support, Property 7: File Extension Selection
  - `test_property_7_file_extension_selection_consistency(self, extension: str)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py#L163) — Feature: yaml-language-support, Property 7: File Extension Selection
  - `test_property_7_file_extension_selection_end_to_end_yaml(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py#L204) — Feature: yaml-language-support, Property 7: File Extension Selection
  - `test_property_7_file_extension_selection_end_to_end_yml(self)` — [`L251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py#L251) — Feature: yaml-language-support, Property 7: File Extension Selection
  - `test_property_7_file_extension_selection_language_detection(self, filename: str, extension: str, content: str)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py#L58) — Feature: yaml-language-support, Property 7: File Extension Selection
  - `test_property_7_file_extension_selection_plugin_manager_integration(self, filename: str, extension: str)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py#L125) — Feature: yaml-language-support, Property 7: File Extension Selection
  - `test_property_7_file_extension_selection_plugin_returns_yaml(self, extension: str)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py#L97) — Feature: yaml-language-support, Property 7: File Extension Selection
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`detect_language_from_file`](../../../tree_sitter_analyzer/language_detector.md#detect_language_from_file), [`get_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`analyze_file`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.analyze_file), [`load_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.load_plugins), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`get_file_extensions`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.get_file_extensions)  (2 test-only)

## Module values
- `filename_strategy` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py#L36)
- `yaml_content_strategy` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_file_extension_properties.py#L25)

