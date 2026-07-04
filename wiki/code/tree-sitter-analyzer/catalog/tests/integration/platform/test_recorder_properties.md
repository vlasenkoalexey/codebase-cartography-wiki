---
title: 'Module: tests/integration/platform/test_recorder_properties.py'
type: catalog
provenance: extracted
module: tests/integration/platform/test_recorder_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.platform.test_recorder_properties`/TestRecorderProperties#
symbols:
  TestRecorderProperties.test_profile_content_completeness: test_profile_content_completeness().
  TestRecorderProperties.test_recording_completeness: test_recording_completeness().
  TestRecorderProperties.test_profile_persistence_integration: test_profile_persistence_integration().
  TestRecorderProperties: ''
---
# Module: [`tests/integration/platform/test_recorder_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_recorder_properties.py)

## Classes
### `TestRecorderProperties`
- def: [`tests/integration/platform/test_recorder_properties.py:8`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_recorder_properties.py#L8)
- signature: `class TestRecorderProperties:`
- members:
  - `test_profile_content_completeness(self)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_recorder_properties.py#L25) — Property 7: Profile content completeness
  - `test_profile_persistence_integration(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_recorder_properties.py#L45) — Property 8: Profile persistence correctness (Integration)
  - `test_recording_completeness(self)` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_recorder_properties.py#L9) — Property 6: Behavior recording completeness
- uses (calls/refs, reference-scoped): [`ALL_FIXTURES`](../../../tree_sitter_analyzer/platform_compat/fixtures.md#ALL_FIXTURES), [`record_all`](../../../tree_sitter_analyzer/platform_compat/recorder.md#BehaviorRecorder.record_all), [`behaviors`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.behaviors), [`platform_key`](../../../tree_sitter_analyzer/platform_compat/profiles.md#BehaviorProfile.platform_key), [`id`](../../../tree_sitter_analyzer/platform_compat/fixtures.md#SQLTestFixture.id), [`node_type`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior.node_type), [`has_error`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior.has_error), [`attributes`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior.attributes), [`construct_id`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior.construct_id), [`element_count`](../../../tree_sitter_analyzer/platform_compat/profiles.md#ParsingBehavior.element_count), [`BehaviorRecorder`](../../../tree_sitter_analyzer/platform_compat/recorder.md#BehaviorRecorder), [`save_profile`](../../../tree_sitter_analyzer/platform_compat/recorder.md#BehaviorRecorder.save_profile)

