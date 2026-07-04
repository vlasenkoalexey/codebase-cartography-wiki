---
title: 'Module: tests/unit/languages/test_yaml_plugin.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_yaml_plugin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_yaml_plugin`/TestYAML
symbols:
  TestYAMLElement.test_yaml_element_defaults: Element#test_yaml_element_defaults().
  TestYAMLPluginAnalysis.test_analyze_simple_yaml: PluginAnalysis#test_analyze_simple_yaml().
  TestYAMLElement.test_create_yaml_element: Element#test_create_yaml_element().
  TestYAMLPluginAnalysis.test_analyze_yaml_with_anchors: PluginAnalysis#test_analyze_yaml_with_anchors().
  TestYAMLPluginAnalysis.test_analyze_multi_document_yaml: PluginAnalysis#test_analyze_multi_document_yaml().
  TestYAMLPluginAnalysis.test_analyze_yaml_with_sequences: PluginAnalysis#test_analyze_yaml_with_sequences().
  TestYAMLPlugin.test_get_supported_element_types: Plugin#test_get_supported_element_types().
  TestYAMLPlugin.test_get_queries: Plugin#test_get_queries().
  TestYAMLElementExtractor.test_extract_empty_functions: ElementExtractor#test_extract_empty_functions().
  TestYAMLElementExtractor.test_extract_empty_classes: ElementExtractor#test_extract_empty_classes().
  TestYAMLElementExtractor: ElementExtractor#
  TestYAMLPluginAnalysis: PluginAnalysis#
  TestYAMLPlugin: Plugin#
  TestYAMLElement: Element#
---
# Module: [`tests/unit/languages/test_yaml_plugin.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py)

## Classes
### `TestYAMLElement`
- def: [`tests/unit/languages/test_yaml_plugin.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L43)
- doc: Tests for YAMLElement class.
- signature: `class TestYAMLElement:`
- members:
  - `test_create_yaml_element(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L46) — Test creating a YAMLElement.
  - `test_yaml_element_defaults(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L64) — Test YAMLElement default values.
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`element_type`](../../../tree_sitter_analyzer/models/base.md#CodeElement.element_type), [`YAMLElement`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement), [`key`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.key), [`document_index`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.document_index), [`value_type`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.value_type), [`value`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.value), [`nesting_level`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.nesting_level), [`alias_target`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.alias_target), [`anchor_name`](../../../tree_sitter_analyzer/languages/yaml_helpers.md#YAMLElement.anchor_name)

### `TestYAMLElementExtractor`
- def: [`tests/unit/languages/test_yaml_plugin.py:81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L81)
- doc: Tests for YAMLElementExtractor class.
- signature: `class TestYAMLElementExtractor:`
- members:
  - `test_extract_empty_classes(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L91) — Test that extract_classes returns empty list.
  - `test_extract_empty_functions(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L84) — Test that extract_functions returns empty list.
- uses (calls/refs, reference-scoped): [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE), [`YAMLElementExtractor`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_classes), [`extract_functions`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLElementExtractor.extract_functions)

### `TestYAMLPlugin`
- def: [`tests/unit/languages/test_yaml_plugin.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L18)
- doc: Tests for YAMLPlugin class.
- signature: `class TestYAMLPlugin:`
- members:
  - `test_get_queries(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L33) — Test that plugin returns queries.
  - `test_get_supported_element_types(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L21) — Test that plugin returns supported element types.
- uses (calls/refs, reference-scoped): [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`get_queries`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.get_queries), [`get_supported_element_types`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.get_supported_element_types)

### `TestYAMLPluginAnalysis`
- def: [`tests/unit/languages/test_yaml_plugin.py:101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L101)
- doc: Integration tests for YAML plugin analysis.
- signature: `class TestYAMLPluginAnalysis:`
- members:
  - `test_analyze_multi_document_yaml(self, tmp_path)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L152) — Test analyzing multi-document YAML.
  - `test_analyze_simple_yaml(self, tmp_path)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L104) — Test analyzing a simple YAML file.
  - `test_analyze_yaml_with_anchors(self, tmp_path)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L125) — Test analyzing YAML with anchors and aliases.
  - `test_analyze_yaml_with_sequences(self, tmp_path)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_yaml_plugin.py#L175) — Test analyzing YAML with sequences.
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`elements`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.elements), [`language`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.language), [`success`](../../../tree_sitter_analyzer/models/result.md#AnalysisResult.success), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`YAMLPlugin`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin), [`analyze_file`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAMLPlugin.analyze_file), [`YAML_AVAILABLE`](../../../tree_sitter_analyzer/languages/yaml_plugin.md#YAML_AVAILABLE)

