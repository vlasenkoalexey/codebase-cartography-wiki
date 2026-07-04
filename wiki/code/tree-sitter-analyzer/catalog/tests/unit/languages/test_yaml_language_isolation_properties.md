---
title: 'Module: tests/unit/languages/test_yaml_language_isolation_properties.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_language_isolation_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_language_isolation_properties`/
symbols:
  TestYAMLLanguageIsolationProperties.test_property_8_language_isolation_multiple_yaml_analyses: TestYAMLLanguageIsolationProperties#test_property_8_language_isolation_multiple_yaml_analyses().
  TestYAMLLanguageIsolationProperties.test_property_8_language_isolation_concurrent_analysis: TestYAMLLanguageIsolationProperties#test_property_8_language_isolation_concurrent_analysis().
  TestYAMLLanguageIsolationProperties.test_property_8_language_isolation_plugin_manager: TestYAMLLanguageIsolationProperties#test_property_8_language_isolation_plugin_manager().
  TestYAMLLanguageIsolationProperties.test_property_8_language_isolation_plugin_state: TestYAMLLanguageIsolationProperties#test_property_8_language_isolation_plugin_state().
  TestYAMLLanguageIsolationProperties.test_property_8_language_isolation_supported_element_types: TestYAMLLanguageIsolationProperties#test_property_8_language_isolation_supported_element_types().
  TestYAMLLanguageIsolationProperties.test_property_8_language_isolation_file_extensions: TestYAMLLanguageIsolationProperties#test_property_8_language_isolation_file_extensions().
  TestYAMLLanguageIsolationProperties.test_property_8_language_isolation_language_detection: TestYAMLLanguageIsolationProperties#test_property_8_language_isolation_language_detection().
  yaml_code_strategy: yaml_code_strategy.
  _assert_no_yaml_type_overlap: _assert_no_yaml_type_overlap().
  java_code_strategy: java_code_strategy.
  python_code_strategy: python_code_strategy.
  _YAML_SPECIFIC_TYPES: _YAML_SPECIFIC_TYPES.
  _create_temp_files: _create_temp_files().
  javascript_code_strategy: javascript_code_strategy.
  TestYAMLLanguageIsolationProperties: TestYAMLLanguageIsolationProperties#
---
# Module: [`tests/unit/languages/test_yaml_language_isolation_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py)

## Classes
### `TestYAMLLanguageIsolationProperties`
- def: [`tests/unit/languages/test_yaml_language_isolation_properties.py:98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L98)
- doc: Property-based tests for YAML language isolation.
- signature: `class TestYAMLLanguageIsolationProperties:`
- members:
  - `test_property_8_language_isolation_concurrent_analysis(self)` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L213) — Feature: yaml-language-support, Property 8: Language Isolation
  - `test_property_8_language_isolation_file_extensions(self, yaml_code: str)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L168) — Feature: yaml-language-support, Property 8: Language Isolation
  - `test_property_8_language_isolation_language_detection(self, yaml_code: str)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L301) — Feature: yaml-language-support, Property 8: Language Isolation
  - `test_property_8_language_isolation_multiple_yaml_analyses(self)` — [`L394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L394) — Feature: yaml-language-support, Property 8: Language Isolation
  - `test_property_8_language_isolation_plugin_manager(self, java_code: str, python_code: str, yaml_code: str)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L107) — Feature: yaml-language-support, Property 8: Language Isolation
  - `test_property_8_language_isolation_plugin_state(self, yaml_code: str)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L340) — Feature: yaml-language-support, Property 8: Language Isolation
  - `test_property_8_language_isolation_supported_element_types(self, yaml_code: str)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L476) — Feature: yaml-language-support, Property 8: Language Isolation
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`file_path`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.file_path), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`PluginManager`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager), [`detect_language_from_file`](../../../tree_sitter_analyzer/language_detector.md#detect_language_from_file), [`get_plugin`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_plugin), [`get_language_name`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_language_name), [`analyze_file`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.analyze_file), [`get_file_extensions`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_file_extensions), [`create_extractor`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.create_extractor), [`load_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.load_plugins), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`get_all_plugins`](../../../tree_sitter_analyzer/plugins/manager.md#PluginManager.get_all_plugins), [`get_supported_element_types`](../../../tree_sitter_analyzer/plugins/base.md#LanguagePlugin.get_supported_element_types)  (5 test-only)

## Functions
- `_assert_no_yaml_type_overlap(language: str, plugin)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L89) — Assert plugin doesn't claim YAML-specific element types; also checks language_name.
- `_create_temp_files(specs: dict)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L79) — Create temp files from {lang: (ext, content)} specs. Returns {lang: path}.

## Module values
- `_YAML_SPECIFIC_TYPES` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L76)
- `java_code_strategy` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L25)
- `javascript_code_strategy` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L47)
- `python_code_strategy` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L35)
- `yaml_code_strategy` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_language_isolation_properties.py#L62)

