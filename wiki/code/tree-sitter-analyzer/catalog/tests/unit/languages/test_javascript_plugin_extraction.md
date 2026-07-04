---
title: 'Module: tests/unit/languages/test_javascript_plugin_extraction.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_javascript_plugin_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_javascript_plugin_extraction`/
symbols:
  TestExtractGeneratorFunction.test_generator_extraction: TestExtractGeneratorFunction#test_generator_extraction().
  TestExtractImportInfoEnhanced.test_valid_import: TestExtractImportInfoEnhanced#test_valid_import().
  TestExtractPropertyOptimized.test_property_with_value: TestExtractPropertyOptimized#test_property_with_value().
  extractor: extractor().
  plugin: plugin().
  TestExecuteQueryStrategy: TestExecuteQueryStrategy#
  TestExecuteQueryStrategy.test_none_query_key: TestExecuteQueryStrategy#test_none_query_key().
  TestExecuteQueryStrategy.test_invalid_query_key: TestExecuteQueryStrategy#test_invalid_query_key().
  TestGetElementCategories: TestGetElementCategories#
  TestGetElementCategories.test_returns_dict: TestGetElementCategories#test_returns_dict().
  TestDetectFileCharacteristics: TestDetectFileCharacteristics#
  TestDetectFileCharacteristics.test_angular_detection: TestDetectFileCharacteristics#test_angular_detection().
  TestDetectFileCharacteristics.test_react_detection: TestDetectFileCharacteristics#test_react_detection().
  TestDetectFileCharacteristics.test_vue_detection: TestDetectFileCharacteristics#test_vue_detection().
  TestFindParentClassName: TestFindParentClassName#
  TestFindParentClassName.test_finds_class_declaration: TestFindParentClassName#test_finds_class_declaration().
  TestFindParentClassName.test_no_parent: TestFindParentClassName#test_no_parent().
  TestFindParentClassName.test_class_without_identifier: TestFindParentClassName#test_class_without_identifier().
  TestIsReactComponent: TestIsReactComponent#
  TestIsReactComponent.test_react_component: TestIsReactComponent#test_react_component().
  TestIsReactComponent.test_not_react_framework: TestIsReactComponent#test_not_react_framework().
  TestIsExportedClass: TestIsExportedClass#
  TestIsExportedClass.test_exported: TestIsExportedClass#test_exported().
  TestIsExportedClass.test_not_exported: TestIsExportedClass#test_not_exported().
  TestExtractExportInfo: TestExtractExportInfo#
  TestExtractExportInfo.test_valid_export: TestExtractExportInfo#test_valid_export().
  TestExtractExportInfo.test_unparseable_export: TestExtractExportInfo#test_unparseable_export().
  TestExtractElementsExtractor: TestExtractElementsExtractor#
  TestExtractElementsExtractor.test_extract_elements_combines_all: TestExtractElementsExtractor#test_extract_elements_combines_all().
  TestExtractElementsExtractor.test_extract_elements_handles_error: TestExtractElementsExtractor#test_extract_elements_handles_error().
  TestExtractGeneratorFunction: TestExtractGeneratorFunction#
  TestExtractGeneratorFunction.test_generator_no_signature: TestExtractGeneratorFunction#test_generator_no_signature().
  TestExtractGeneratorFunction.test_generator_exception: TestExtractGeneratorFunction#test_generator_exception().
  TestExtractPropertyOptimized: TestExtractPropertyOptimized#
  TestExtractPropertyOptimized.test_property_no_name: TestExtractPropertyOptimized#test_property_no_name().
  TestExtractPropertyOptimized.test_property_exception: TestExtractPropertyOptimized#test_property_exception().
  TestExtractImportInfoEnhanced: TestExtractImportInfoEnhanced#
  TestExtractImportInfoEnhanced.test_unparseable_import: TestExtractImportInfoEnhanced#test_unparseable_import().
  TestExtractImportNames: TestExtractImportNames#
  TestExtractImportNames.test_default_import_name: TestExtractImportNames#test_default_import_name().
  TestExtractImportNames.test_named_imports: TestExtractImportNames#test_named_imports().
  TestPluginCapabilities: TestPluginCapabilities#
  TestPluginCapabilities.test_get_plugin_info: TestPluginCapabilities#test_get_plugin_info().
  TestPluginCapabilities.test_get_supported_queries: TestPluginCapabilities#test_get_supported_queries().
  TestPluginCapabilities.test_get_element_categories_coverage: TestPluginCapabilities#test_get_element_categories_coverage().
  TestGetNodeTextMultiLine: TestGetNodeTextMultiLine#
  TestGetNodeTextMultiLine.test_multiline_node_fallback: TestGetNodeTextMultiLine#test_multiline_node_fallback().
  TestPrivateMethodNameExtraction: TestPrivateMethodNameExtraction#
  TestPrivateMethodNameExtraction.test_private_method_name_is_not_empty: TestPrivateMethodNameExtraction#test_private_method_name_is_not_empty().
---
# Module: [`tests/unit/languages/test_javascript_plugin_extraction.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py)

## Classes
### `TestDetectFileCharacteristics`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L47)
- signature: `class TestDetectFileCharacteristics:`
- members:
  - `test_angular_detection(self, extractor)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L48)
  - `test_react_detection(self, extractor)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L54)
  - `test_vue_detection(self, extractor)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L60)

### `TestExecuteQueryStrategy`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L27)
- signature: `class TestExecuteQueryStrategy:`
- members:
  - `test_invalid_query_key(self, plugin)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L32)
  - `test_none_query_key(self, plugin)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L28)

### `TestExtractElementsExtractor`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L167)
- signature: `class TestExtractElementsExtractor:`
- members:
  - `test_extract_elements_combines_all(self, extractor)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L168)
  - `test_extract_elements_handles_error(self, extractor)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L185)

### `TestExtractExportInfo`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L133)
- signature: `class TestExtractExportInfo:`
- members:
  - `test_unparseable_export(self, extractor)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L151)
  - `test_valid_export(self, extractor)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L134)

### `TestExtractGeneratorFunction`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L198)
- signature: `class TestExtractGeneratorFunction:`
- members:
  - `test_generator_exception(self, extractor)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L246)
  - `test_generator_extraction(self, extractor)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L199)
  - `test_generator_no_signature(self, extractor)` — [`L233`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L233)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`Function`](../../../tree_sitter_analyzer/models/base.md#Function), [`is_generator`](../../../tree_sitter_analyzer/models/base.md#Function.is_generator)

### `TestExtractImportInfoEnhanced`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L323)
- signature: `class TestExtractImportInfoEnhanced:`
- members:
  - `test_unparseable_import(self, extractor)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L344)
  - `test_valid_import(self, extractor)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L324)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`Import`](../../../tree_sitter_analyzer/models/base.md#Import), [`module_path`](../../../tree_sitter_analyzer/models/base.md#Import.module_path)

### `TestExtractImportNames`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L360)
- signature: `class TestExtractImportNames:`
- members:
  - `test_default_import_name(self, extractor)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L361)
  - `test_named_imports(self, extractor)` — [`L380`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L380)

### `TestExtractPropertyOptimized`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L260)
- signature: `class TestExtractPropertyOptimized:`
- members:
  - `test_property_exception(self, extractor)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L313)
  - `test_property_no_name(self, extractor)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L302)
  - `test_property_with_value(self, extractor)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L261)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`Variable`](../../../tree_sitter_analyzer/models/base.md#Variable)

### `TestFindParentClassName`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L67)
- signature: `class TestFindParentClassName:`
- members:
  - `test_class_without_identifier(self, extractor)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L92)
  - `test_finds_class_declaration(self, extractor)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L68)
  - `test_no_parent(self, extractor)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L86)

### `TestGetElementCategories`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L37)
- signature: `class TestGetElementCategories:`
- members:
  - `test_returns_dict(self, plugin)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L38)

### `TestGetNodeTextMultiLine`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L436)
- signature: `class TestGetNodeTextMultiLine:`
- members:
  - `test_multiline_node_fallback(self, extractor)` — [`L437`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L437)

### `TestIsExportedClass`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L123)
- signature: `class TestIsExportedClass:`
- members:
  - `test_exported(self, extractor)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L124)
  - `test_not_exported(self, extractor)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L128)

### `TestIsReactComponent`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L105)
- signature: `class TestIsReactComponent:`
- members:
  - `test_not_react_framework(self, extractor)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L117)
  - `test_react_component(self, extractor)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L106)

### `TestPluginCapabilities`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:413`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L413)
- signature: `class TestPluginCapabilities:`
- members:
  - `test_get_element_categories_coverage(self, plugin)` — [`L426`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L426)
  - `test_get_plugin_info(self, plugin)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L414)
  - `test_get_supported_queries(self, plugin)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L420)

### `TestPrivateMethodNameExtraction`
- def: [`tests/unit/languages/test_javascript_plugin_extraction.py:465`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L465)
- doc: Private class fields (#name) must produce a non-empty name — not ''.
- signature: `class TestPrivateMethodNameExtraction:`
- members:
  - `test_private_method_name_is_not_empty(self, plugin)` — [`L468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L468) — #logActivity must be extracted as 'logActivity', not empty string.

## Functions
- `extractor()` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L18)
- `plugin()` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_javascript_plugin_extraction.py#L23)

