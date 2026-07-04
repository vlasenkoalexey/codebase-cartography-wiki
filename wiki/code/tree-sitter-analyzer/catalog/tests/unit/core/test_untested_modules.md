---
title: 'Module: tests/unit/core/test_untested_modules.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_untested_modules.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_untested_modules`/Test
symbols:
  TestConstants.test_element_types: Constants#test_element_types().
  TestEngineManager.test_reset: EngineManager#test_reset().
  TestConstants.test_is_element_of_type: Constants#test_is_element_of_type().
  TestEngineManager.test_singleton_same_root: EngineManager#test_singleton_same_root().
  TestEngineManager.test_different_roots: EngineManager#test_different_roots().
  TestCLIArgumentValidator.test_validate_no_conflicts: CLIArgumentValidator#test_validate_no_conflicts().
  TestCLIArgumentValidator.test_validate_table_and_query_key_conflict: CLIArgumentValidator#test_validate_table_and_query_key_conflict().
  TestOutputFormatValidator.test_no_conflict_passes: OutputFormatValidator#test_no_conflict_passes().
  TestOutputFormatValidator.test_mutual_exclusion_raises: OutputFormatValidator#test_mutual_exclusion_raises().
  TestOutputFormatValidator.test_single_format_passes: OutputFormatValidator#test_single_format_passes().
  TestOutputFormatValidator.test_format_params: OutputFormatValidator#test_format_params().
  TestCLIArgumentValidator.test_init: CLIArgumentValidator#test_init().
  TestConstants.test_sql_element_types: Constants#test_sql_element_types().
  TestConstants.test_mapping: Constants#test_mapping().
  TestOutputFormatValidator.test_init: OutputFormatValidator#test_init().
  TestCLIArgumentValidator: CLIArgumentValidator#
  TestConstants: Constants#
  TestEngineManager: EngineManager#
  TestOutputFormatValidator: OutputFormatValidator#
---
# Module: [`tests/unit/core/test_untested_modules.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py)

## Classes
### `TestCLIArgumentValidator`
- def: [`tests/unit/core/test_untested_modules.py:22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L22)
- signature: `class TestCLIArgumentValidator:`
- members:
  - `test_init(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L23)
  - `test_validate_no_conflicts(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L26)
  - `test_validate_table_and_query_key_conflict(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L33)
- uses (calls/refs, reference-scoped): [`validate_arguments`](../../../tree_sitter_analyzer/cli/argument_validator.md#CLIArgumentValidator.validate_arguments), [`CLIArgumentValidator`](../../../tree_sitter_analyzer/cli/argument_validator.md#CLIArgumentValidator)

### `TestConstants`
- def: [`tests/unit/core/test_untested_modules.py:43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L43)
- signature: `class TestConstants:`
- members:
  - `test_element_types(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L44)
  - `test_is_element_of_type(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L66)
  - `test_mapping(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L53)
  - `test_sql_element_types(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L50)
- uses (calls/refs, reference-scoped): [`ELEMENT_TYPE_CLASS`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_CLASS), [`ELEMENT_TYPE_FUNCTION`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_FUNCTION), [`is_element_of_type`](../../../tree_sitter_analyzer/constants.md#is_element_of_type), [`ELEMENT_TYPE_VARIABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_VARIABLE), [`ELEMENT_TYPE_IMPORT`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_IMPORT), [`ELEMENT_TYPE_MAPPING`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_MAPPING), [`ELEMENT_TYPE_SQL_TABLE`](../../../tree_sitter_analyzer/constants.md#ELEMENT_TYPE_SQL_TABLE)

### `TestEngineManager`
- def: [`tests/unit/core/test_untested_modules.py:73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L73)
- signature: `class TestEngineManager:`
- members:
  - `test_different_roots(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L80)
  - `test_reset(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L86)
  - `test_singleton_same_root(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L74)
- uses (calls/refs, reference-scoped): [`EngineManager`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager), [`get_instance`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager.get_instance), [`reset_instances`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager.reset_instances), [`_instances`](../../../tree_sitter_analyzer/core/engine_manager.md#EngineManager._instances)

### `TestOutputFormatValidator`
- def: [`tests/unit/core/test_untested_modules.py:94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L94)
- signature: `class TestOutputFormatValidator:`
- members:
  - `test_format_params(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L113)
  - `test_init(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L95)
  - `test_mutual_exclusion_raises(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L102)
  - `test_no_conflict_passes(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L98)
  - `test_single_format_passes(self)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_untested_modules.py#L109)
- uses (calls/refs, reference-scoped): [`OutputFormatValidator`](../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator), [`validate_output_format_exclusion`](../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator.validate_output_format_exclusion), [`OUTPUT_FORMAT_PARAMS`](../../../tree_sitter_analyzer/mcp/tools/output_format_validator.md#OutputFormatValidator.OUTPUT_FORMAT_PARAMS)

