---
title: 'Module: tests/integration/platform/test_detector_properties.py'
type: catalog
provenance: extracted
module: tests/integration/platform/test_detector_properties.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.platform.test_detector_properties`/
symbols:
  TestPlatformDetectorProperties.test_platform_detection_accuracy: TestPlatformDetectorProperties#test_platform_detection_accuracy().
  TestPlatformDetectorProperties.test_get_profile_path: TestPlatformDetectorProperties#test_get_profile_path().
  platform_config: platform_config().
  TestPlatformDetectorProperties: TestPlatformDetectorProperties#
---
# Module: [`tests/integration/platform/test_detector_properties.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_detector_properties.py)

## Classes
### `TestPlatformDetectorProperties`
- def: [`tests/integration/platform/test_detector_properties.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_detector_properties.py#L20)
- signature: `class TestPlatformDetectorProperties:`
- members:
  - `test_get_profile_path(self, config)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_detector_properties.py#L54) — Test profile path resolution.
  - `test_platform_detection_accuracy(self, config)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_detector_properties.py#L22) — Property 2: Platform detection accuracy
- uses (calls/refs, reference-scoped): [`detect`](../../../tree_sitter_analyzer/platform_compat/detector.md#PlatformDetector.detect), [`PlatformDetector`](../../../tree_sitter_analyzer/platform_compat/detector.md#PlatformDetector), [`get_profile_path`](../../../tree_sitter_analyzer/platform_compat/detector.md#PlatformDetector.get_profile_path), [`platform_key`](../../../tree_sitter_analyzer/platform_compat/detector.md#PlatformInfo.platform_key), [`PlatformInfo`](../../../tree_sitter_analyzer/platform_compat/detector.md#PlatformInfo), [`os_name`](../../../tree_sitter_analyzer/platform_compat/detector.md#PlatformInfo.os_name), [`python_version`](../../../tree_sitter_analyzer/platform_compat/detector.md#PlatformInfo.python_version), [`os_version`](../../../tree_sitter_analyzer/platform_compat/detector.md#PlatformInfo.os_version)  (1 test-only)

## Functions
- `platform_config(draw)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/platform/test_detector_properties.py#L11) — Generates random platform configurations.

