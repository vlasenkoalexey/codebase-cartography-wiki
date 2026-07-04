---
title: 'Module: tree_sitter_analyzer/platform_compat/recorder.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/platform_compat/recorder.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.platform_compat.recorder`/
symbols:
  BehaviorRecorder.record_all: BehaviorRecorder#record_all().
  BehaviorRecorder.record_fixture: BehaviorRecorder#record_fixture().
  profile: profile.
  BehaviorRecorder: BehaviorRecorder#
  BehaviorRecorder.platform_info: BehaviorRecorder#platform_info.
  BehaviorRecorder.save_profile: BehaviorRecorder#save_profile().
  _inspect_node_for_recorder: _inspect_node_for_recorder().
  BehaviorRecorder.parser: BehaviorRecorder#parser.
  BehaviorRecorder.analyze_ast: BehaviorRecorder#analyze_ast().
  recorder: recorder.
  BehaviorRecorder.language: BehaviorRecorder#language.
  _RECORDER_DEFINITION_TYPES._RECORDER_DEFINITION_TYPES: _RECORDER_DEFINITION_TYPES._RECORDER_DEFINITION_TYPES.
  logger: logger.
  BehaviorRecorder.__init__: BehaviorRecorder#__init__().
---
# Module: [`tree_sitter_analyzer/platform_compat/recorder.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py)

## Classes
### `BehaviorRecorder`
- def: [`tree_sitter_analyzer/platform_compat/recorder.py:59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L59)
- doc: Records SQL parsing behavior on the current platform.
- signature: `class BehaviorRecorder:`
- members:
  - `analyze_ast(self, node: Any)` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L112) — Analyzes the AST to extract characteristics.
  - `record_all(self)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L67) — Records behavior for all fixtures.
  - `record_fixture(self, fixture: SQLTestFixture)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L87) — Records behavior for a single fixture.
  - `save_profile(self, profile: BehaviorProfile, base_path: Path)` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L156) — Saves the recorded profile to disk.
  - `language` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L63)
  - `parser` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L64)
  - `platform_info` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L65)
- protocol/private: `__init__`[`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L62)
- uses (calls/refs, reference-scoped): [`BehaviorProfile`](profiles.md#BehaviorProfile), [`ParsingBehavior`](profiles.md#ParsingBehavior), [`ALL_FIXTURES`](fixtures.md#ALL_FIXTURES), [`behaviors`](profiles.md#BehaviorProfile.behaviors), [`platform_key`](profiles.md#BehaviorProfile.platform_key), [`detect`](detector.md#PlatformDetector.detect), [`id`](fixtures.md#SQLTestFixture.id), [`node_type`](profiles.md#ParsingBehavior.node_type), [`SQLTestFixture`](fixtures.md#SQLTestFixture), [`PROFILE_SCHEMA_VERSION`](profiles.md#PROFILE_SCHEMA_VERSION), [`adaptation_rules`](profiles.md#BehaviorProfile.adaptation_rules), [`has_error`](profiles.md#ParsingBehavior.has_error), [`PlatformDetector`](detector.md#PlatformDetector), [`attributes`](profiles.md#ParsingBehavior.attributes), [`construct_id`](profiles.md#ParsingBehavior.construct_id), [`element_count`](profiles.md#ParsingBehavior.element_count), [`sql`](fixtures.md#SQLTestFixture.sql), [`schema_version`](profiles.md#BehaviorProfile.schema_version), [`platform_key`](detector.md#PlatformInfo.platform_key), [`save`](profiles.md#BehaviorProfile.save), [`known_issues`](profiles.md#ParsingBehavior.known_issues), [`_inspect_node_for_recorder`](recorder.md#_inspect_node_for_recorder)
- used by: [`main`](record.md#main), [`profile`](recorder.md#profile), [`handle_record_sql_profile`](../cli/commands/sql_platform_helpers.md#handle_record_sql_profile), [`recorder`](recorder.md#recorder)  (3 test-only)

## Functions
- `_inspect_node_for_recorder(node: Any, attributes: set[str], element_count: int, has_error: bool)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L31) — Apply per-node accounting for the BehaviorRecorder cursor walk.

## Module values
- `_RECORDER_DEFINITION_TYPES` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L19)
- `logger` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L16)
- `profile` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L170)
- `recorder` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/recorder.py#L169)

