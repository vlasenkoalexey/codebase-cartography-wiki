---
title: 'Module: tests/integration/platform/test_profiles_properties.py'
type: catalog
provenance: extracted
module: tests/integration/platform/test_profiles_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.platform.test_profiles_properties`/
symbols:
  parsing_behavior_strategy: parsing_behavior_strategy().
  behavior_profile_strategy: behavior_profile_strategy().
  TestProfileProperties.test_profile_persistence_correctness: TestProfileProperties#test_profile_persistence_correctness().
  TestProfileProperties.test_profile_loading_correctness: TestProfileProperties#test_profile_loading_correctness().
  TestProfileProperties: TestProfileProperties#
---
# Module: [`tests/integration/platform/test_profiles_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_profiles_properties.py)

## Classes
### `TestProfileProperties`
- def: [`tests/integration/platform/test_profiles_properties.py:39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_profiles_properties.py#L39)
- signature: `class TestProfileProperties:`
- members:
  - `test_profile_loading_correctness(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_profiles_properties.py#L68) — Property 3: Profile loading correctness
  - `test_profile_persistence_correctness(self, profile)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_profiles_properties.py#L42) — Property 8: Profile persistence correctness
- uses (calls/refs, reference-scoped): [`BehaviorProfile`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile), [`behaviors`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.behaviors), [`platform_key`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.platform_key), [`load`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.load), [`adaptation_rules`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.adaptation_rules), [`schema_version`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.schema_version)  (1 test-only)

## Functions
- `behavior_profile_strategy(draw)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_profiles_properties.py#L28)
- `parsing_behavior_strategy(draw)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_profiles_properties.py#L16)

