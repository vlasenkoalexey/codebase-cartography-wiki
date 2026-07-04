---
title: 'Module: tests/integration/platform/test_integration_properties.py'
type: catalog
provenance: extracted
module: tests/integration/platform/test_integration_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.platform.test_integration_properties`/TestIntegrationProperties#
symbols:
  TestIntegrationProperties.test_output_schema_consistency: test_output_schema_consistency().
  TestIntegrationProperties.test_diagnostic_logging: test_diagnostic_logging().
  TestIntegrationProperties.test_graceful_degradation: test_graceful_degradation().
  TestIntegrationProperties.side_effect: side_effect().
  TestIntegrationProperties: ''
---
# Module: [`tests/integration/platform/test_integration_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_integration_properties.py)

## Classes
### `TestIntegrationProperties`
- def: [`tests/integration/platform/test_integration_properties.py:8`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_integration_properties.py#L8)
- signature: `class TestIntegrationProperties:`
- members:
  - `side_effect(node, elements)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_integration_properties.py#L45)
  - `test_diagnostic_logging(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_integration_properties.py#L76) — Property 11: Comprehensive diagnostic logging
  - `test_graceful_degradation(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_integration_properties.py#L142) — Property 13: Language isolation (Graceful degradation)
  - `test_output_schema_consistency(self)` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_integration_properties.py#L9) — Property 5: Output schema consistency
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLElementType`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType), [`SQLElement`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement), [`SQLPlugin`](../../../tree_sitter_analyzer/languages/sql_plugin/plugin.md#SQLPlugin), [`extract_sql_elements`](../../../tree_sitter_analyzer/languages/sql_plugin/extractor.md#SQLElementExtractor.extract_sql_elements), [`SQLElementExtractor`](../../../tree_sitter_analyzer/languages/sql_plugin/extractor.md#SQLElementExtractor), [`TABLE`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType.TABLE), [`CompatibilityAdapter`](../../../tree_sitter_analyzer/platform_compat/adapter.md#CompatibilityAdapter), [`sql_element_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.sql_element_type), [`set_adapter`](../../../tree_sitter_analyzer/languages/sql_plugin/extractor.md#SQLElementExtractor.set_adapter), [`extractor`](../../../tree_sitter_analyzer/languages/sql_plugin/plugin.md#SQLPlugin.extractor), [`platform_info`](../../../tree_sitter_analyzer/plugins/base.md#ElementExtractor.platform_info), [`diagnostic_mode`](../../../tree_sitter_analyzer/languages/sql_plugin/extractor.md#SQLElementExtractor.diagnostic_mode), [`element_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.element_type)

