---
title: 'Module: tests/unit/utils/test_claude_md_frontmatter.py'
type: catalog
provenance: extracted
module: tests/unit/utils/test_claude_md_frontmatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.utils.test_claude_md_frontmatter`/
symbols:
  TestParseIntentionalDesign.test_single_valid_rule: TestParseIntentionalDesign#test_single_valid_rule().
  TestEndToEnd.test_real_claude_md_layout: TestEndToEnd#test_real_claude_md_layout().
  _MODULE_LOGGER: _MODULE_LOGGER.
  TestParseFixtureAllowlist.test_single_entry: TestParseFixtureAllowlist#test_single_entry().
  TestLoadFrontmatter.test_malformed_yaml_returns_empty_dict_and_warns: TestLoadFrontmatter#test_malformed_yaml_returns_empty_dict_and_warns().
  TestLoadFrontmatter.test_frontmatter_is_list_not_dict_warns_and_returns_empty: TestLoadFrontmatter#test_frontmatter_is_list_not_dict_warns_and_returns_empty().
  TestParseIntentionalDesign.test_invalid_action_coerced_to_info_with_warning: TestParseIntentionalDesign#test_invalid_action_coerced_to_info_with_warning().
  TestParseIntentionalDesign.test_all_valid_actions_round_trip: TestParseIntentionalDesign#test_all_valid_actions_round_trip().
  TestParseIntentionalDesign.test_missing_required_field_skips_rule_with_warning: TestParseIntentionalDesign#test_missing_required_field_skips_rule_with_warning().
  TestParseIntentionalDesign.test_entry_is_not_dict_skipped: TestParseIntentionalDesign#test_entry_is_not_dict_skipped().
  TestParseIntentionalDesign.test_files_empty_list_skipped: TestParseIntentionalDesign#test_files_empty_list_skipped().
  TestParseFixtureAllowlist.test_missing_path_skipped_with_warning: TestParseFixtureAllowlist#test_missing_path_skipped_with_warning().
  TestParseFixtureAllowlist.test_entry_is_not_dict_skipped: TestParseFixtureAllowlist#test_entry_is_not_dict_skipped().
  _write_claude_md: _write_claude_md().
  TestLoadFrontmatter.test_no_frontmatter_block_returns_empty_dict: TestLoadFrontmatter#test_no_frontmatter_block_returns_empty_dict().
  TestLoadFrontmatter.test_empty_frontmatter_returns_empty_dict: TestLoadFrontmatter#test_empty_frontmatter_returns_empty_dict().
  TestLoadFrontmatter.test_valid_frontmatter_returns_dict: TestLoadFrontmatter#test_valid_frontmatter_returns_dict().
  TestLoadFrontmatter.test_accepts_str_or_path_project_root: TestLoadFrontmatter#test_accepts_str_or_path_project_root().
  TestParseIntentionalDesign.test_glob_pattern_compiles_and_matches: TestParseIntentionalDesign#test_glob_pattern_compiles_and_matches().
  TestParseIntentionalDesign.test_missing_action_defaults_to_info: TestParseIntentionalDesign#test_missing_action_defaults_to_info().
  TestParseIntentionalDesign.test_symbols_defaults_to_empty_tuple_not_none: TestParseIntentionalDesign#test_symbols_defaults_to_empty_tuple_not_none().
  TestParseIntentionalDesign.test_action_case_normalised_to_upper: TestParseIntentionalDesign#test_action_case_normalised_to_upper().
  TestParseIntentionalDesign.test_rule_is_frozen_dataclass: TestParseIntentionalDesign#test_rule_is_frozen_dataclass().
  TestParseIntentionalDesign.test_section_is_not_list_warns: TestParseIntentionalDesign#test_section_is_not_list_warns().
  TestParseIntentionalDesign.test_files_as_single_string_wrapped_in_list: TestParseIntentionalDesign#test_files_as_single_string_wrapped_in_list().
  TestParseIntentionalDesign.test_symbols_as_single_string_wrapped_in_tuple: TestParseIntentionalDesign#test_symbols_as_single_string_wrapped_in_tuple().
  TestParseFixtureAllowlist.test_missing_note_defaults_to_empty_string: TestParseFixtureAllowlist#test_missing_note_defaults_to_empty_string().
  TestParseFixtureAllowlist.test_entry_is_frozen_dataclass: TestParseFixtureAllowlist#test_entry_is_frozen_dataclass().
  TestParseFixtureAllowlist.test_section_is_not_list_warns: TestParseFixtureAllowlist#test_section_is_not_list_warns().
  TestLoadFrontmatter.test_no_claude_md_returns_empty_dict: TestLoadFrontmatter#test_no_claude_md_returns_empty_dict().
  TestParseIntentionalDesign.test_empty_input_returns_empty_list: TestParseIntentionalDesign#test_empty_input_returns_empty_list().
  TestParseFixtureAllowlist.test_empty_input_returns_empty_list: TestParseFixtureAllowlist#test_empty_input_returns_empty_list().
  TestLoadFrontmatter: TestLoadFrontmatter#
  TestParseIntentionalDesign: TestParseIntentionalDesign#
  TestParseFixtureAllowlist: TestParseFixtureAllowlist#
  TestEndToEnd: TestEndToEnd#
---
# Module: [`tests/unit/utils/test_claude_md_frontmatter.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py)

## Classes
### `TestEndToEnd`
- def: [`tests/unit/utils/test_claude_md_frontmatter.py:394`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L394)
- signature: `class TestEndToEnd:`
- members:
  - `test_real_claude_md_layout(self, tmp_path: Path)` — [`L395`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L395)
- uses (calls/refs, reference-scoped): [`parse_intentional_design`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#parse_intentional_design), [`parse_fixture_allowlist`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#parse_fixture_allowlist), [`load_frontmatter`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#load_frontmatter), [`id`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#IntentionalDesignRule.id), [`path`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#FixtureAllowlistEntry.path), [`file_patterns`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#IntentionalDesignRule.file_patterns)  (1 test-only)

### `TestLoadFrontmatter`
- def: [`tests/unit/utils/test_claude_md_frontmatter.py:55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L55)
- signature: `class TestLoadFrontmatter:`
- members:
  - `test_accepts_str_or_path_project_root(self, tmp_path: Path)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L102)
  - `test_empty_frontmatter_returns_empty_dict(self, tmp_path: Path)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L65)
  - `test_frontmatter_is_list_not_dict_warns_and_returns_empty(self, tmp_path: Path, caplog: pytest.LogCaptureFixture)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L106)
  - `test_malformed_yaml_returns_empty_dict_and_warns(self, tmp_path: Path, caplog: pytest.LogCaptureFixture)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L88)
  - `test_no_claude_md_returns_empty_dict(self, tmp_path: Path)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L56)
  - `test_no_frontmatter_block_returns_empty_dict(self, tmp_path: Path)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L59)
  - `test_valid_frontmatter_returns_dict(self, tmp_path: Path)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L71)
- uses (calls/refs, reference-scoped): [`load_frontmatter`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#load_frontmatter)  (2 test-only)

### `TestParseFixtureAllowlist`
- def: [`tests/unit/utils/test_claude_md_frontmatter.py:330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L330)
- signature: `class TestParseFixtureAllowlist:`
- members:
  - `test_empty_input_returns_empty_list(self)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L331)
  - `test_entry_is_frozen_dataclass(self)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L370)
  - `test_entry_is_not_dict_skipped(self, caplog: pytest.LogCaptureFixture)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L381)
  - `test_missing_note_defaults_to_empty_string(self)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L365)
  - `test_missing_path_skipped_with_warning(self, caplog: pytest.LogCaptureFixture)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L350)
  - `test_section_is_not_list_warns(self, caplog: pytest.LogCaptureFixture)` — [`L376`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L376)
  - `test_single_entry(self)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L334)
- uses (calls/refs, reference-scoped): [`parse_fixture_allowlist`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#parse_fixture_allowlist), [`path`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#FixtureAllowlistEntry.path), [`FixtureAllowlistEntry`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#FixtureAllowlistEntry), [`note`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#FixtureAllowlistEntry.note)  (1 test-only)

### `TestParseIntentionalDesign`
- def: [`tests/unit/utils/test_claude_md_frontmatter.py:122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L122)
- signature: `class TestParseIntentionalDesign:`
- members:
  - `test_action_case_normalised_to_upper(self)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L243)
  - `test_all_valid_actions_round_trip(self, action: str)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L209)
  - `test_empty_input_returns_empty_list(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L123)
  - `test_entry_is_not_dict_skipped(self, caplog: pytest.LogCaptureFixture)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L271)
  - `test_files_as_single_string_wrapped_in_list(self)` — [`L283`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L283)
  - `test_files_empty_list_skipped(self, caplog: pytest.LogCaptureFixture)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L292)
  - `test_glob_pattern_compiles_and_matches(self)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L152)
  - `test_invalid_action_coerced_to_info_with_warning(self, caplog: pytest.LogCaptureFixture)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L180)
  - `test_missing_action_defaults_to_info(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L167)
  - `test_missing_required_field_skips_rule_with_warning(self, caplog: pytest.LogCaptureFixture)` — [`L222`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L222)
  - `test_rule_is_frozen_dataclass(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L256)
  - `test_section_is_not_list_warns(self, caplog: pytest.LogCaptureFixture)` — [`L262`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L262)
  - `test_single_valid_rule(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L127)
  - `test_symbols_as_single_string_wrapped_in_tuple(self)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L310)
  - `test_symbols_defaults_to_empty_tuple_not_none(self)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L239)
- uses (calls/refs, reference-scoped): [`parse_intentional_design`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#parse_intentional_design), [`id`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#IntentionalDesignRule.id), [`IntentionalDesignRule`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#IntentionalDesignRule), [`action`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#IntentionalDesignRule.action), [`file_patterns`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#IntentionalDesignRule.file_patterns), [`VALID_VERDICT_ACTIONS`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#VALID_VERDICT_ACTIONS.VALID_VERDICT_ACTIONS), [`symbols`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#IntentionalDesignRule.symbols), [`raw_globs`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#IntentionalDesignRule.raw_globs), [`note`](../../../tree_sitter_analyzer/utils/claude_md_frontmatter.md#IntentionalDesignRule.note)  (1 test-only)

## Functions
- `_write_claude_md(root: Path, body: str)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L42) — Write ``body`` to ``<root>/CLAUDE.md`` and return the path.

## Module values
- `_MODULE_LOGGER` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/utils/test_claude_md_frontmatter.py#L35)

