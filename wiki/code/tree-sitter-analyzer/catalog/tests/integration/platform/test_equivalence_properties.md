---
title: 'Module: tests/integration/platform/test_equivalence_properties.py'
type: catalog
provenance: extracted
module: tests/integration/platform/test_equivalence_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.platform.test_equivalence_properties`/TestEquivalenceProperties#
symbols:
  TestEquivalenceProperties.get_windows_elements: get_windows_elements().
  TestEquivalenceProperties.get_macos_elements: get_macos_elements().
  TestEquivalenceProperties.get_linux_elements: get_linux_elements().
  TestEquivalenceProperties.test_cross_platform_equivalence: test_cross_platform_equivalence().
  TestEquivalenceProperties.run_adaptation: run_adaptation().
  TestEquivalenceProperties.get_names: get_names().
  TestEquivalenceProperties: ''
---
# Module: [`tests/integration/platform/test_equivalence_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_equivalence_properties.py)

## Classes
### `TestEquivalenceProperties`
- def: [`tests/integration/platform/test_equivalence_properties.py:8`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_equivalence_properties.py#L8)
- signature: `class TestEquivalenceProperties:`
- members:
  - `get_linux_elements()` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_equivalence_properties.py#L123) — documented in [tree_sitter_analyzer-models-sql_models](../../../../concepts/tree_sitter_analyzer-models-sql_models.md)
  - `get_macos_elements()` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_equivalence_properties.py#L99) — documented in [tree_sitter_analyzer-models-sql_models](../../../../concepts/tree_sitter_analyzer-models-sql_models.md)
  - `get_names(elements)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_equivalence_properties.py#L181)
  - `get_windows_elements()` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_equivalence_properties.py#L75) — documented in [tree_sitter_analyzer-models-sql_models](../../../../concepts/tree_sitter_analyzer-models-sql_models.md)
  - `run_adaptation(profile, raw_elements)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_equivalence_properties.py#L65)
  - `test_cross_platform_equivalence(self)` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_equivalence_properties.py#L9) — Property 1: Cross-platform parsing equivalence — documented in [tree_sitter_analyzer-models-sql_models](../../../../concepts/tree_sitter_analyzer-models-sql_models.md)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`raw_text`](../../../tree_sitter_analyzer/models/base.md#CodeElement.raw_text), [`SQLElementType`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType), [`BehaviorProfile`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile), [`SQLFunction`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction), [`SQLTrigger`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger), [`parameters`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElement.parameters), [`behaviors`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.behaviors), [`platform_key`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.platform_key), [`sql_element_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger.sql_element_type), [`PROFILE_SCHEMA_VERSION`](../../../tree_sitter_analyzer/platform_compat/profiles.md#PROFILE_SCHEMA_VERSION), [`TRIGGER`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType.TRIGGER), [`adaptation_rules`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.adaptation_rules), [`table_name`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger.table_name), [`trigger_timing`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger.trigger_timing), [`schema_version`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.schema_version), [`sql_element_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction.sql_element_type), [`trigger_event`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger.trigger_event), [`CompatibilityAdapter`](../../../tree_sitter_analyzer/platform_compat/adapter.md#CompatibilityAdapter), [`FUNCTION`](../../../tree_sitter_analyzer/models/sql_models.md#SQLElementType.FUNCTION), [`adapt_elements`](../../../tree_sitter_analyzer/platform_compat/adapter.md#CompatibilityAdapter.adapt_elements), [`element_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLTrigger.element_type), [`element_type`](../../../tree_sitter_analyzer/models/sql_models.md#SQLFunction.element_type)

