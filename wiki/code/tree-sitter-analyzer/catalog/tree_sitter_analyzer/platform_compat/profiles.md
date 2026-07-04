---
title: 'Module: tree_sitter_analyzer/platform_compat/profiles.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/platform_compat/profiles.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.platform_compat.profiles`/
symbols:
  BehaviorProfile: BehaviorProfile#
  ParsingBehavior: ParsingBehavior#
  BehaviorProfile.behaviors: BehaviorProfile#behaviors.
  BehaviorProfile.platform_key: BehaviorProfile#platform_key.
  ProfileCache.get: ProfileCache#get().
  BehaviorProfile.load: BehaviorProfile#load().
  ParsingBehavior.node_type: ParsingBehavior#node_type.
  ProfileCache.stats: ProfileCache#stats().
  PROFILE_SCHEMA_VERSION: PROFILE_SCHEMA_VERSION.
  ParsingBehavior.has_error: ParsingBehavior#has_error.
  BehaviorProfile.adaptation_rules: BehaviorProfile#adaptation_rules.
  ParsingBehavior.construct_id: ParsingBehavior#construct_id.
  ParsingBehavior.element_count: ParsingBehavior#element_count.
  ParsingBehavior.attributes: ParsingBehavior#attributes.
  validate_profile: validate_profile().
  BehaviorProfile.schema_version: BehaviorProfile#schema_version.
  ProfileCache.put: ProfileCache#put().
  ProfileCache.clear: ProfileCache#clear().
  migrate_profile_schema: migrate_profile_schema().
  _validate_profile_minimal: _validate_profile_minimal().
  BehaviorProfile.save: BehaviorProfile#save().
  logger: logger.
  ParsingBehavior.known_issues: ParsingBehavior#known_issues.
  BehaviorProfile.__post_init__: BehaviorProfile#__post_init__().
  ProfileCache: ProfileCache#
  ProfileCache._cache: ProfileCache#_cache.
  ProfileCache._lock: ProfileCache#_lock.
  PROFILE_SCHEMA: PROFILE_SCHEMA.
  ProfileCache._hits: ProfileCache#_hits.
  ProfileCache._misses: ProfileCache#_misses.
  _is_string_list: _is_string_list().
  migrate_to_1_0_0: migrate_to_1_0_0().
  ProfileCache.__init__: ProfileCache#__init__().
---
# Module: [`tree_sitter_analyzer/platform_compat/profiles.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py)

## Classes
### `BehaviorProfile`
- def: [`tree_sitter_analyzer/platform_compat/profiles.py:28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L28)
- doc: Complete behavior profile for a platform.
- signature: `class BehaviorProfile:`
- members:
  - `__post_init__(self)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L36) — Ensure behaviors are ParsingBehavior objects.
  - `load(cls, platform_key: str, base_path: Path | None = None)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L44) — Loads a profile for the given platform key.
  - `save(self, base_path: Path)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L105) — Saves the profile to disk.
  - `adaptation_rules` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L34)
  - `behaviors` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L33)
  - `platform_key` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L32)
  - `schema_version` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L31)
- uses (calls/refs, reference-scoped): [`ParsingBehavior`](profiles.md#ParsingBehavior), [`validate_profile`](profiles.md#validate_profile), [`migrate_profile_schema`](profiles.md#migrate_profile_schema), [`logger`](profiles.md#logger)
- used by: [`compare_profiles`](compare.md#compare_profiles), [`platform_info`](../languages/sql_plugin/plugin.md#SQLPlugin.platform_info), [`record_all`](recorder.md#BehaviorRecorder.record_all), [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/plugin.md#TREE_SITTER_AVAILABLE), [`generate_compatibility_matrix`](report.md#generate_compatibility_matrix), [`handle_sql_platform_info`](../cli/commands/sql_platform_helpers.md#handle_sql_platform_info), [`_load_rules`](adapter.md#CompatibilityAdapter._load_rules), [`get`](profiles.md#ProfileCache.get), [`load_profile_from_file`](compare.md#load_profile_from_file), [`main`](record.md#main), [`_load_profile`](../cli/commands/sql_platform_helpers.md#_load_profile), [`_load_profile_from_path`](report.md#_load_profile_from_path), [`profile`](recorder.md#profile), [`put`](profiles.md#ProfileCache.put), [`handle_record_sql_profile`](../cli/commands/sql_platform_helpers.md#handle_record_sql_profile), [`save_profile`](recorder.md#BehaviorRecorder.save_profile), [`__init__`](adapter.md#CompatibilityAdapter.__init__)  (19 test-only)

### `ParsingBehavior`
- def: [`tree_sitter_analyzer/platform_compat/profiles.py:16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L16)
- doc: Describes how a specific SQL construct parses on a platform.
- signature: `class ParsingBehavior:`
- members:
  - `attributes` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L22)
  - `construct_id` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L19)
  - `element_count` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L21)
  - `has_error` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L23)
  - `known_issues` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L24)
  - `node_type` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L20)
- used by: [`behaviors`](profiles.md#BehaviorProfile.behaviors), [`record_fixture`](recorder.md#BehaviorRecorder.record_fixture), [`generate_compatibility_matrix`](report.md#generate_compatibility_matrix), [`load_profile_from_file`](compare.md#load_profile_from_file), [`load`](profiles.md#BehaviorProfile.load), [`_load_profile`](../cli/commands/sql_platform_helpers.md#_load_profile), [`_load_profile_from_path`](report.md#_load_profile_from_path), [`__post_init__`](profiles.md#BehaviorProfile.__post_init__)  (19 test-only)

### `ProfileCache`
- def: [`tree_sitter_analyzer/platform_compat/profiles.py:252`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L252)
- doc: Thread-safe cache for behavior profiles.
- signature: `class ProfileCache:`
- members:
  - `clear(self)` — [`L273`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L273)
  - `get(self, key: str)` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L261)
  - `put(self, key: str, profile: BehaviorProfile)` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L269)
  - `stats(self)` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L280)
- protocol/private: `__init__`[`L255`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L255), `_cache`[`L256`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L256), `_hits`[`L258`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L258), `_lock`[`L257`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L257), `_misses`[`L259`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L259)
- uses (calls/refs, reference-scoped): [`BehaviorProfile`](profiles.md#BehaviorProfile)
- used by: (5 test-only callers)

## Functions
- `_is_string_list(value: Any)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L226)
- `_validate_profile_minimal(data: dict[str, Any])` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L178) — Validate the profile shape when jsonschema cannot be imported.
- `migrate_profile_schema(data: dict[str, Any])` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L230) — Migrates profile data to the current schema version.
- `migrate_to_1_0_0(data: dict[str, Any])` — [`L242`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L242) — Initial migration to 1.0.0.
- `validate_profile(data: dict[str, Any])` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L155) — Validates profile data against the schema.

## Module values
- `PROFILE_SCHEMA` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L123)
- `PROFILE_SCHEMA_VERSION` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L12)
- `logger` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/profiles.py#L10)

