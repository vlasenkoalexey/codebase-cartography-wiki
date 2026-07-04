---
title: 'Module: tree_sitter_analyzer/platform_compat/detector.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/platform_compat/detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.platform_compat.detector`/Platform
symbols:
  PlatformDetector.detect: Detector#detect().
  PlatformDetector: Detector#
  PlatformDetector.get_profile_path: Detector#get_profile_path().
  PlatformInfo.platform_key: Info#platform_key.
  PlatformInfo: Info#
  PlatformInfo.os_name: Info#os_name.
  PlatformInfo.python_version: Info#python_version.
  PlatformInfo.os_version: Info#os_version.
---
# Module: [`tree_sitter_analyzer/platform_compat/detector.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/detector.py)

## Classes
### `PlatformDetector`
- def: [`tree_sitter_analyzer/platform_compat/detector.py:17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/detector.py#L17)
- members:
  - `detect()` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/detector.py#L21) — Detects the current platform information.
  - `get_profile_path(base_path: Path, platform_info: PlatformInfo | None = None)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/detector.py#L46) — Resolves the path to the profile file for the given platform.
- uses (calls/refs, reference-scoped): [`platform_key`](detector.md#PlatformInfo.platform_key), [`PlatformInfo`](detector.md#PlatformInfo), [`os_name`](detector.md#PlatformInfo.os_name), [`python_version`](detector.md#PlatformInfo.python_version), [`os_version`](detector.md#PlatformInfo.os_version)
- used by: [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`platform_info`](../languages/sql_plugin/plugin.md#SQLPlugin.platform_info), [`version`](../mcp/server.md#TreeSitterAnalyzerMCPServer.version), [`handle_sql_platform_info`](../cli/commands/sql_platform_helpers.md#handle_sql_platform_info), [`platform_info`](recorder.md#BehaviorRecorder.platform_info)  (2 test-only)

### `PlatformInfo`
- def: [`tree_sitter_analyzer/platform_compat/detector.py:8`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/detector.py#L8)
- doc: Platform identification information.
- signature: `class PlatformInfo:`
- members:
  - `os_name` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/detector.py#L11)
  - `os_version` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/detector.py#L12)
  - `platform_key` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/detector.py#L14)
  - `python_version` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/detector.py#L13)
- used by: [`platform_info`](../languages/sql_plugin/plugin.md#SQLPlugin.platform_info), [`record_all`](recorder.md#BehaviorRecorder.record_all), [`handle_sql_platform_info`](../cli/commands/sql_platform_helpers.md#handle_sql_platform_info), [`detect`](detector.md#PlatformDetector.detect), [`get_profile_path`](detector.md#PlatformDetector.get_profile_path), [`platform_info`](../plugins/base.md#ElementExtractor.platform_info)  (2 test-only)

