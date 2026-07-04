---
title: 'Module: tests/integration/platform/test_adapter_properties.py'
type: catalog
provenance: extracted
module: tests/integration/platform/test_adapter_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.platform.test_adapter_properties`/TestAdapterProperties#
symbols:
  TestAdapterProperties.test_function_name_normalization: test_function_name_normalization().
  TestAdapterProperties.test_trigger_name_normalization: test_trigger_name_normalization().
  TestAdapterProperties.test_phantom_element_removal: test_phantom_element_removal().
  TestAdapterProperties.test_adaptation_idempotence: test_adaptation_idempotence().
  TestAdapterProperties.test_view_recovery: test_view_recovery().
  TestAdapterProperties: ''
---
# Module: [`tests/integration/platform/test_adapter_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_adapter_properties.py)

## Classes
### `TestAdapterProperties`
- def: [`tests/integration/platform/test_adapter_properties.py:14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_adapter_properties.py#L14)
- signature: `class TestAdapterProperties:`
- members:
  - `test_adaptation_idempotence(self)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_adapter_properties.py#L114) — Property 15: Adaptation rule idempotence
  - `test_function_name_normalization(self, name)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_adapter_properties.py#L16) — Property 4: Transformation normalization (function names)
  - `test_phantom_element_removal(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_adapter_properties.py#L73) — Property 4: Transformation normalization (phantom removal)
  - `test_trigger_name_normalization(self, name)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_adapter_properties.py#L44) — Property 4: Transformation normalization (trigger names)
  - `test_view_recovery(self, name)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_adapter_properties.py#L99) — Property 4: Transformation normalization (view recovery)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLElementType`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType), [`SQLFunction`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction), [`SQLTrigger`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger), [`SQLView`](../../../tree_sitter_analyzer/models/sql_models.md#SQLView), [`generate_elements`](../../../tree_sitter_analyzer/platform_compat/adapter.md#RecoverViewsFromErrorsRule.generate_elements), [`sql_element_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger.sql_element_type), [`TRIGGER`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType.TRIGGER), [`apply`](../../../tree_sitter_analyzer/platform_compat/adapter.md#RemovePhantomTriggersRule.apply), [`sql_element_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction.sql_element_type), [`CompatibilityAdapter`](../../../tree_sitter_analyzer/platform_compat/adapter.md#CompatibilityAdapter), [`FUNCTION`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType.FUNCTION), [`apply`](../../../tree_sitter_analyzer/platform_compat/adapter.md#FixFunctionNameKeywordsRule.apply), [`apply`](../../../tree_sitter_analyzer/platform_compat/adapter.md#FixTriggerNameDescriptionRule.apply), [`adapt_elements`](../../../tree_sitter_analyzer/platform_compat/adapter.md#CompatibilityAdapter.adapt_elements), [`FixFunctionNameKeywordsRule`](../../../tree_sitter_analyzer/platform_compat/adapter.md#FixFunctionNameKeywordsRule), [`FixTriggerNameDescriptionRule`](../../../tree_sitter_analyzer/platform_compat/adapter.md#FixTriggerNameDescriptionRule), [`RecoverViewsFromErrorsRule`](../../../tree_sitter_analyzer/platform_compat/adapter.md#RecoverViewsFromErrorsRule), [`RemovePhantomTriggersRule`](../../../tree_sitter_analyzer/platform_compat/adapter.md#RemovePhantomTriggersRule)

