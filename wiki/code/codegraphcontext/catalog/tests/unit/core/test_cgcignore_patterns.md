---
title: 'Module: tests/unit/core/test_cgcignore_patterns.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_cgcignore_patterns.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.core.test_cgcignore_patterns`/
symbols:
  query_files_for_repo: query_files_for_repo().
  index_repo: index_repo().
  get_unique_test_dir: get_unique_test_dir().
  setup_test_dir: setup_test_dir().
  test_tc12_default_filtering_without_cgcignore: test_tc12_default_filtering_without_cgcignore().
  test_tc13_cgcignore_adds_new_rules: test_tc13_cgcignore_adds_new_rules().
  test_tc14_cgcignore_ignores_comments: test_tc14_cgcignore_ignores_comments().
  test_tc15_cgcignore_ignores_empty_lines: test_tc15_cgcignore_ignores_empty_lines().
  test_tc16_merge_default_and_user_patterns: test_tc16_merge_default_and_user_patterns().
  test_tc17_expected_output_validation: test_tc17_expected_output_validation().
  test_tc18_cgcignore_discovery_nested: test_tc18_cgcignore_discovery_nested().
  test_tc19_nested_filtering_merged: test_tc19_nested_filtering_merged().
  test_tc20_combined_filtering_real_scenario: test_tc20_combined_filtering_real_scenario().
  test_tc21_cgcignore_auto_created_when_not_exists: test_tc21_cgcignore_auto_created_when_not_exists().
  test_tc23_cgcignore_auto_created_with_default_content: test_tc23_cgcignore_auto_created_with_default_content().
  run: run().
  clean_before_integration_test: clean_before_integration_test().
  CGC_CMD: CGC_CMD.
  clean_db_completely: clean_db_completely().
  query_all_repos: query_all_repos().
  delete_repo_from_db: delete_repo_from_db().
  query_all_files: query_all_files().
  TEST_HOME: TEST_HOME.
  BASE_TEST_DIR: BASE_TEST_DIR.
  _test_env: _test_env().
  _is_neo4j_reachable: _is_neo4j_reachable().
  extract_file_names: extract_file_names().
  test_tc01_default_ignore_patterns_exists: test_tc01_default_ignore_patterns_exists().
  test_tc02_validate_pattern_format: test_tc02_validate_pattern_format().
  test_tc03_media_patterns_included: test_tc03_media_patterns_included().
  test_tc04_archive_patterns_included: test_tc04_archive_patterns_included().
  test_tc05_pathspec_creation: test_tc05_pathspec_creation().
  test_tc06_match_media_files: test_tc06_match_media_files().
  test_tc07_match_video_audio_files: test_tc07_match_video_audio_files().
  test_tc08_do_not_match_source_files: test_tc08_do_not_match_source_files().
  test_tc09_do_not_match_config_files: test_tc09_do_not_match_config_files().
  test_tc10_do_not_match_extensionless_files: test_tc10_do_not_match_extensionless_files().
  test_tc11_match_files_in_subdirectories: test_tc11_match_files_in_subdirectories().
  test_tc22_empty_array_plus_default_patterns: test_tc22_empty_array_plus_default_patterns().
---
# Module: [`tests/unit/core/test_cgcignore_patterns.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py)

## Functions
- `_is_neo4j_reachable(host: str = "localhost", port: int = 7687, timeout: float = 1)` — [`L47`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L47) — Return True when a local Neo4j bolt endpoint is reachable.
- `_test_env()` — [`L24`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L24) — Run shell-based CGC tests against the current interpreter in an isolated HOME.
- `clean_before_integration_test(request)` — [`L207`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L207) — Prepare DB only for integration-style cases that require live cgc DB access.
- `clean_db_completely()` — [`L62`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L62) — Completely clean the database
- `delete_repo_from_db(repo_path: Path)` — [`L68`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L68) — Delete specific repository from database
- `extract_file_names(output)` — [`L110`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L110) — Extract file names from JSON output
- `get_unique_test_dir()` — [`L36`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L36) — Generate unique test directory
- `index_repo(test_dir: Path)` — [`L76`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L76) — Index the test repository
- `query_all_files()` — [`L83`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L83) — Query ALL files in database for debugging
- `query_all_repos()` — [`L89`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L89) — Query ALL repositories in database for debugging
- `query_files_for_repo(test_dir: Path)` — [`L95`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L95) — Query files ONLY from specific test repository
- `run(cmd)` — [`L41`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L41) — Run command and return output
- `setup_test_dir(test_dir: Path)` — [`L55`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L55) — Create clean test directory
- `test_tc01_default_ignore_patterns_exists()` — [`L132`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L132) — Verify DEFAULT_IGNORE_PATTERNS list exists and is not empty
- `test_tc02_validate_pattern_format()` — [`L138`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L138) — Verify patterns are either glob extensions (*.foo) or gitignore-style directory names (name/)
- `test_tc03_media_patterns_included()` — [`L144`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L144) — Verify media patterns (*.png, *.jpg, *.mp4) are included in defaults
- `test_tc04_archive_patterns_included()` — [`L151`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L151) — Verify archive patterns (*.zip, *.tar, *.gz) are included in defaults
- `test_tc05_pathspec_creation()` — [`L157`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L157) — Verify PathSpec object is created successfully from default patterns
- `test_tc06_match_media_files()` — [`L163`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L163) — Verify image files (png, jpg, jpeg) are matched for ignoring
- `test_tc07_match_video_audio_files()` — [`L170`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L170) — Verify video/audio files (mp4, mp3) are matched for ignoring
- `test_tc08_do_not_match_source_files()` — [`L176`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L176) — Verify source files (.py, .js) are NOT matched for ignoring
- `test_tc09_do_not_match_config_files()` — [`L182`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L182) — Verify config files (.json, .yaml, .md, .txt) are NOT matched for ignoring
- `test_tc10_do_not_match_extensionless_files()` — [`L190`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L190) — Verify extensionless files (Makefile) are NOT matched for ignoring
- `test_tc11_match_files_in_subdirectories()` — [`L196`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L196) — Verify media files in subdirectories are also matched for ignoring
- `test_tc12_default_filtering_without_cgcignore()` — [`L227`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L227) — Verify default patterns apply when .cgcignore file does not exist.
- `test_tc13_cgcignore_adds_new_rules()` — [`L250`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L250) — Verify user can add new ignore rules via .cgcignore (e.g., *.txt)
- `test_tc14_cgcignore_ignores_comments()` — [`L270`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L270) — Verify comments (#) in .cgcignore are properly ignored
- `test_tc15_cgcignore_ignores_empty_lines()` — [`L291`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L291) — Verify empty lines in .cgcignore are properly ignored
- `test_tc16_merge_default_and_user_patterns()` — [`L313`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L313) — Verify default and user patterns are merged and both apply
- `test_tc17_expected_output_validation()` — [`L331`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L331) — Verify expected output matches in a mixed repository.
- `test_tc18_cgcignore_discovery_nested()` — [`L358`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L358) — Verify .cgcignore is discovered and applied in nested directories
- `test_tc19_nested_filtering_merged()` — [`L379`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L379) — Verify merged patterns correctly apply to nested files.
- `test_tc20_combined_filtering_real_scenario()` — [`L406`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L406) — Verify real-world scenario with DEFAULT + .cgcignore combined filtering.
- `test_tc21_cgcignore_auto_created_when_not_exists()` — [`L450`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L450) — Verify .cgcignore file is auto-created when it does not exist:
- `test_tc22_empty_array_plus_default_patterns()` — [`L529`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L529) — Verify merge logic: empty array + default patterns = default patterns only
- `test_tc23_cgcignore_auto_created_with_default_content()` — [`L568`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L568) — Verify auto-created .cgcignore file contains default patterns:

## Module values
- `BASE_TEST_DIR` — [`L19`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L19)
- `CGC_CMD` — [`L21`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L21)
- `TEST_HOME` — [`L20`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_cgcignore_patterns.py#L20)

