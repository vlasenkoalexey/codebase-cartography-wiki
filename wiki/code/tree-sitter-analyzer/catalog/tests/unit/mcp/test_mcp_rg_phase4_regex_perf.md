---
title: 'Module: tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_rg_phase4_regex_perf`/
symbols:
  test_rg_45_large_output_truncation: test_rg_45_large_output_truncation().
  test_rg_51_group_by_file_structure: test_rg_51_group_by_file_structure().
  test_rg_52_summary_counts_consistent: test_rg_52_summary_counts_consistent().
  test_rg_46_word_mode_does_not_match_substrings: test_rg_46_word_mode_does_not_match_substrings().
  test_rg_47_fixed_strings_escapes_regex: test_rg_47_fixed_strings_escapes_regex().
  test_rg_50_count_parsing_robust_to_bad_lines: test_rg_50_count_parsing_robust_to_bad_lines().
  test_rg_53_files_mode_uses_parent_dirs: test_rg_53_files_mode_uses_parent_dirs().
  test_rg_54_no_json_non_match_events: test_rg_54_no_json_non_match_events().
  test_rg_55_hidden_files_not_included_by_default: test_rg_55_hidden_files_not_included_by_default().
  test_rg_48_encoding_invalid_is_string_validated: test_rg_48_encoding_invalid_is_string_validated().
  test_rg_49_include_exclude_not_strings: test_rg_49_include_exclude_not_strings().
  test_rg_51_group_by_file_structure.jline: test_rg_51_group_by_file_structure().jline().
  test_rg_52_summary_counts_consistent.jline: test_rg_52_summary_counts_consistent().jline().
  test_rg_44_regex_specials_and_flags: test_rg_44_regex_specials_and_flags().
  test_rg_45_large_output_truncation.jline: test_rg_45_large_output_truncation().jline().
  test_rg_45_large_output_truncation.fake_run: test_rg_45_large_output_truncation().fake_run().
  test_rg_46_word_mode_does_not_match_substrings.fake_run: test_rg_46_word_mode_does_not_match_substrings().fake_run().
  test_rg_47_fixed_strings_escapes_regex.fake_run: test_rg_47_fixed_strings_escapes_regex().fake_run().
  test_rg_50_count_parsing_robust_to_bad_lines.fake_run: test_rg_50_count_parsing_robust_to_bad_lines().fake_run().
  test_rg_51_group_by_file_structure.fake_run: test_rg_51_group_by_file_structure().fake_run().
  test_rg_52_summary_counts_consistent.fake_run: test_rg_52_summary_counts_consistent().fake_run().
  test_rg_53_files_mode_uses_parent_dirs.fake_run: test_rg_53_files_mode_uses_parent_dirs().fake_run().
  test_rg_54_no_json_non_match_events.fake_run: test_rg_54_no_json_non_match_events().fake_run().
  test_rg_55_hidden_files_not_included_by_default.fake_run: test_rg_55_hidden_files_not_included_by_default().fake_run().
  mock_external_commands: mock_external_commands().
---
# Module: [`tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py)

## Functions
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L71)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L107)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L143)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L187)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L225)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L263)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L300`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L300)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L350`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L350)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L381)
- `jline(idx: int)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L53)
- `jline(path: str, line: int)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L207)
- `jline(path: str)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L245)
- `mock_external_commands(monkeypatch)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L10) — Auto-mock external command availability checks for all tests in this module.
- `test_rg_44_regex_specials_and_flags(tmp_path)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L19)
- `test_rg_45_large_output_truncation(monkeypatch, tmp_path)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L49)
- `test_rg_46_word_mode_does_not_match_substrings(monkeypatch, tmp_path)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L94)
- `test_rg_47_fixed_strings_escapes_regex(monkeypatch, tmp_path)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L125)
- `test_rg_48_encoding_invalid_is_string_validated(tmp_path)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L159)
- `test_rg_49_include_exclude_not_strings(tmp_path)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L169)
- `test_rg_50_count_parsing_robust_to_bad_lines(monkeypatch, tmp_path)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L183)
- `test_rg_51_group_by_file_structure(monkeypatch, tmp_path)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L204)
- `test_rg_52_summary_counts_consistent(monkeypatch, tmp_path)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L242)
- `test_rg_53_files_mode_uses_parent_dirs(monkeypatch, tmp_path)` — [`L280`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L280)
- `test_rg_54_no_json_non_match_events(monkeypatch, tmp_path)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L331)
- `test_rg_55_hidden_files_not_included_by_default(monkeypatch, tmp_path)` — [`L363`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_rg_phase4_regex_perf.py#L363)

