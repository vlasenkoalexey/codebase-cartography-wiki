---
title: 'Module: tests/unit/core/test_skip_external_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_skip_external_resolution.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.core.test_skip_external_resolution`/
symbols:
  isolated_config: isolated_config().
  TestSkipExternalResolutionConfig: TestSkipExternalResolutionConfig#
  TestSkipExternalResolutionConfig.test_config_exists_in_descriptions: TestSkipExternalResolutionConfig#test_config_exists_in_descriptions().
  TestSkipExternalResolutionConfig.test_config_has_validator: TestSkipExternalResolutionConfig#test_config_has_validator().
  TestSkipExternalResolutionConfig.test_validator_accepts_true: TestSkipExternalResolutionConfig#test_validator_accepts_true().
  TestSkipExternalResolutionConfig.test_validator_accepts_false: TestSkipExternalResolutionConfig#test_validator_accepts_false().
  TestSkipExternalResolutionConfig.test_validator_rejects_invalid_values: TestSkipExternalResolutionConfig#test_validator_rejects_invalid_values().
  TestSkipExternalResolutionConfig.test_default_value_is_false: TestSkipExternalResolutionConfig#test_default_value_is_false().
  TestSkipExternalResolutionConfig.test_set_and_get_config_value: TestSkipExternalResolutionConfig#test_set_and_get_config_value().
  TestSkipExternalResolutionConfig.test_environment_variable_override: TestSkipExternalResolutionConfig#test_environment_variable_override().
  TestSkipExternalResolutionBehavior: TestSkipExternalResolutionBehavior#
  TestSkipExternalResolutionBehavior.test_graph_builder_uses_config_value: TestSkipExternalResolutionBehavior#test_graph_builder_uses_config_value().
  TestSkipExternalResolutionBehavior.test_skip_external_logic_exists_in_code: TestSkipExternalResolutionBehavior#test_skip_external_logic_exists_in_code().
  TestBackwardCompatibility: TestBackwardCompatibility#
  TestBackwardCompatibility.test_default_behavior_unchanged: TestBackwardCompatibility#test_default_behavior_unchanged().
  TestBackwardCompatibility.test_existing_configs_not_affected: TestBackwardCompatibility#test_existing_configs_not_affected().
  TestSkipExternalResolutionE2E: TestSkipExternalResolutionE2E#
  TestSkipExternalResolutionE2E.test_indexing_with_skip_external_enabled: TestSkipExternalResolutionE2E#test_indexing_with_skip_external_enabled().
  TestSkipExternalResolutionE2E.test_performance_improvement: TestSkipExternalResolutionE2E#test_performance_improvement().
---
# Module: [`tests/unit/core/test_skip_external_resolution.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py)

## Classes
### `TestBackwardCompatibility`
- def: [`tests/unit/core/test_skip_external_resolution.py:128`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L128)
- doc: Test that existing behavior is preserved when config is not set.
- signature: `class TestBackwardCompatibility:`
- members:
  - `test_default_behavior_unchanged(self)` — [`L131`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L131) — Test that default behavior matches original (warnings + attempts).
  - `test_existing_configs_not_affected(self)` — [`L139`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L139) — Test that other configuration options still work.

### `TestSkipExternalResolutionBehavior`
- def: [`tests/unit/core/test_skip_external_resolution.py:98`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L98)
- doc: Test the behavior of SKIP_EXTERNAL_RESOLUTION in graph_builder.py
- signature: `class TestSkipExternalResolutionBehavior:`
- members:
  - `test_graph_builder_uses_config_value(self)` — [`L106`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L106) — Test that GraphBuilder imports and can call get_config_value.
  - `test_skip_external_logic_exists_in_code(self)` — [`L117`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L117) — Test that the skip_external logic is present in resolution layer.

### `TestSkipExternalResolutionConfig`
- def: [`tests/unit/core/test_skip_external_resolution.py:36`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L36)
- doc: Test the SKIP_EXTERNAL_RESOLUTION configuration cli option.
- signature: `class TestSkipExternalResolutionConfig:`
- members:
  - `test_config_exists_in_descriptions(self)` — [`L39`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L39) — Test that SKIP_EXTERNAL_RESOLUTION has a description.
  - `test_config_has_validator(self)` — [`L45`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L45) — Test that SKIP_EXTERNAL_RESOLUTION has valid values list.
  - `test_default_value_is_false(self)` — [`L71`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L71) — Test that default value is 'false' for backward compatibility.
  - `test_environment_variable_override(self)` — [`L87`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L87) — Test that environment variable SKIP_EXTERNAL_RESOLUTION works.
  - `test_set_and_get_config_value(self)` — [`L77`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L77) — Test setting and getting the configuration value.
  - `test_validator_accepts_false(self)` — [`L57`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L57) — Test that validator list includes 'false'.
  - `test_validator_accepts_true(self)` — [`L52`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L52) — Test that validator list includes 'true'.
  - `test_validator_rejects_invalid_values(self)` — [`L62`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L62) — Test that validator list does not include invalid values.

### `TestSkipExternalResolutionE2E`
- def: [`tests/unit/core/test_skip_external_resolution.py:151`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L151)
- doc: End-to-end tests for SKIP_EXTERNAL_RESOLUTION (requires Neo4j).
- signature: `class TestSkipExternalResolutionE2E:`
- members:
  - `test_indexing_with_skip_external_enabled(self)` — [`L154`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L154) — Test full indexing cycle with SKIP_EXTERNAL_RESOLUTION=true.
  - `test_performance_improvement(self)` — [`L161`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L161) — Test that indexing is faster with SKIP_EXTERNAL_RESOLUTION=true.

## Functions
- `isolated_config(tmp_path, monkeypatch)` — [`L22`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_skip_external_resolution.py#L22) — Use an isolated HOME so config tests do not leak across the suite.

