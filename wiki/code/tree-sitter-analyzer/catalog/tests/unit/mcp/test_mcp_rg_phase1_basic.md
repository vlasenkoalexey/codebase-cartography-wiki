---
title: 'Module: tests/unit/mcp/test_mcp_rg_phase1_basic.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_rg_phase1_basic.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_rg_phase1_basic`/
symbols:
  _build_rg: _build_rg().
  test_rg_09_search_content_exec_roots_basic_match_parsing: test_rg_09_search_content_exec_roots_basic_match_parsing().
  test_rg_10_search_content_exec_files_list_uses_parent_dirs: test_rg_10_search_content_exec_files_list_uses_parent_dirs().
  test_rg_07_build_cmd_globs_include_exclude: test_rg_07_build_cmd_globs_include_exclude().
  test_rg_07_build_cmd_globs_include_exclude.has_pair: test_rg_07_build_cmd_globs_include_exclude().has_pair().
  test_rg_01_build_cmd_default_smart_case: test_rg_01_build_cmd_default_smart_case().
  test_rg_02_build_cmd_case_insensitive: test_rg_02_build_cmd_case_insensitive().
  test_rg_03_build_cmd_case_sensitive: test_rg_03_build_cmd_case_sensitive().
  test_rg_04_build_cmd_fixed_strings_flag: test_rg_04_build_cmd_fixed_strings_flag().
  test_rg_05_build_cmd_word_boundaries: test_rg_05_build_cmd_word_boundaries().
  test_rg_06_build_cmd_multiline: test_rg_06_build_cmd_multiline().
  test_rg_08_build_cmd_hidden_and_no_ignore: test_rg_08_build_cmd_hidden_and_no_ignore().
  test_rg_09_search_content_exec_roots_basic_match_parsing.fake_run: test_rg_09_search_content_exec_roots_basic_match_parsing().fake_run().
  test_rg_10_search_content_exec_files_list_uses_parent_dirs.fake_run: test_rg_10_search_content_exec_files_list_uses_parent_dirs().fake_run().
  mock_external_commands: mock_external_commands().
---
# Module: [`tests/unit/mcp/test_mcp_rg_phase1_basic.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py)

## Functions
- `_build_rg(query: str, tmp_path: object, *, case: str = "smart", fixed_strings: bool = False, word: bool = False, multiline: bool = False, include_globs=None, exclude_globs=None, follow_symlinks: bool = False, hidden: bool = False, no_ignore: bool = False, max_filesize=None, context_before=None, context_after=None, encoding=None, max_count=None, timeout_ms=None, files_from=None, count_only_matches: bool = False)` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L9) — Call build_rg_command with sensible defaults; only vary what the test cares about.
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L160)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L200)
- `has_pair(flag: str, value: str)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L120)
- `mock_external_commands(monkeypatch)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L56) — Auto-mock external command availability checks for all tests in this module.
- `test_rg_01_build_cmd_default_smart_case(tmp_path)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L65) — Default build: --json, smart case (-S), default max-filesize.
- `test_rg_02_build_cmd_case_insensitive(tmp_path)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L78)
- `test_rg_03_build_cmd_case_sensitive(tmp_path)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L86)
- `test_rg_04_build_cmd_fixed_strings_flag(tmp_path)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L94)
- `test_rg_05_build_cmd_word_boundaries(tmp_path)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L100)
- `test_rg_06_build_cmd_multiline(tmp_path)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L106)
- `test_rg_07_build_cmd_globs_include_exclude(tmp_path)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L112)
- `test_rg_08_build_cmd_hidden_and_no_ignore(tmp_path)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L133)
- `test_rg_09_search_content_exec_roots_basic_match_parsing(monkeypatch, tmp_path)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L143)
- `test_rg_10_search_content_exec_files_list_uses_parent_dirs(monkeypatch, tmp_path)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase1_basic.py#L181)

