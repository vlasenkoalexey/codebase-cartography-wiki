---
title: 'Module: tests/unit/mcp/test_mcp_find_and_grep_p1.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_find_and_grep_p1.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_find_and_grep_p1`/
symbols:
  test_tools_timeout_handling: test_tools_timeout_handling().
  test_tools_with_empty_results: test_tools_with_empty_results().
  test_find_and_grep_exec_composed: test_find_and_grep_exec_composed().
  test_find_and_grep_multiline_case_insensitive: test_find_and_grep_multiline_case_insensitive().
  test_find_and_grep_count_only_matches: test_find_and_grep_count_only_matches().
  test_find_and_grep_optimize_paths: test_find_and_grep_optimize_paths().
  test_find_and_grep_error_handling: test_find_and_grep_error_handling().
  test_find_and_grep_file_discovery_parameters: test_find_and_grep_file_discovery_parameters().
  test_find_and_grep_content_search_parameters: test_find_and_grep_content_search_parameters().
  test_find_and_grep_with_file_sorting: test_find_and_grep_with_file_sorting().
  test_find_and_grep_summary_only_mode: test_find_and_grep_summary_only_mode().
  test_find_and_grep_validation_requires_roots_and_query: test_find_and_grep_validation_requires_roots_and_query().
  _mock_find_and_grep_json_run: _mock_find_and_grep_json_run().
  _mock_find_and_grep_json_run.fake_run: _mock_find_and_grep_json_run().fake_run().
  test_find_and_grep_exec_composed.fake_run: test_find_and_grep_exec_composed().fake_run().
  test_find_and_grep_multiline_case_insensitive.fake_run: test_find_and_grep_multiline_case_insensitive().fake_run().
  test_find_and_grep_count_only_matches.fake_run: test_find_and_grep_count_only_matches().fake_run().
  test_find_and_grep_error_handling.fake_run: test_find_and_grep_error_handling().fake_run().
  test_find_and_grep_file_discovery_parameters.fake_run: test_find_and_grep_file_discovery_parameters().fake_run().
  test_find_and_grep_content_search_parameters.fake_run: test_find_and_grep_content_search_parameters().fake_run().
  test_find_and_grep_with_file_sorting.fake_run: test_find_and_grep_with_file_sorting().fake_run().
  test_find_and_grep_summary_only_mode.fake_run: test_find_and_grep_summary_only_mode().fake_run().
  test_tools_timeout_handling.fake_timeout_run: test_tools_timeout_handling().fake_timeout_run().
  test_tools_with_empty_results.fake_empty_run: test_tools_with_empty_results().fake_empty_run().
  mock_external_commands: mock_external_commands().
---
# Module: [`tests/unit/mcp/test_mcp_find_and_grep_p1.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py)

## Functions
- `_mock_find_and_grep_json_run(monkeypatch, file_path, line_text, match_text)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L19) — Mock fd then rg JSON output for a single matched file.
- `fake_empty_run(cmd, input_data=None, timeout_ms=None)` — [`L497`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L497)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L31)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L79)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L127)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L175)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L245)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L271)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L323`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L323)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L381)
- `fake_run(cmd, input_data=None, timeout_ms=None)` — [`L420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L420)
- `fake_timeout_run(cmd, input_data=None, timeout_ms=None)` — [`L460`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L460)
- `mock_external_commands(monkeypatch)` — [`L11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L11) — Auto-mock external command availability checks for all tests in this module.
- `test_find_and_grep_content_search_parameters(monkeypatch, tmp_path)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L317) — Test FindAndGrepTool with comprehensive content search parameters.
- `test_find_and_grep_count_only_matches(monkeypatch, tmp_path)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L157) — Test find_and_grep tool with count_only_matches option.
- `test_find_and_grep_error_handling(monkeypatch, tmp_path)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L241) — Test FindAndGrepTool error handling when fd command fails.
- `test_find_and_grep_exec_composed(monkeypatch, tmp_path)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L63) — Test FindAndGrepTool execution combining file discovery (fd) and content search (rg).
- `test_find_and_grep_file_discovery_parameters(monkeypatch, tmp_path)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L265) — Test FindAndGrepTool with comprehensive file discovery parameters.
- `test_find_and_grep_multiline_case_insensitive(monkeypatch, tmp_path)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L105) — Test FindAndGrepTool with multiline regex patterns and case-insensitive matching.
- `test_find_and_grep_optimize_paths(monkeypatch, tmp_path)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L207) — Test FindAndGrepTool with path optimization enabled.
- `test_find_and_grep_summary_only_mode(monkeypatch, tmp_path)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L414) — Test FindAndGrepTool with summary_only output format.
- `test_find_and_grep_validation_requires_roots_and_query(tmp_path)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L46) — ``query`` is always required; ``roots`` is required only when no
- `test_find_and_grep_with_file_sorting(monkeypatch, tmp_path)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L369) — Test FindAndGrepTool with file sorting options.
- `test_tools_timeout_handling(monkeypatch, tmp_path)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L452) — Test timeout handling for all tools.
- `test_tools_with_empty_results(monkeypatch, tmp_path)` — [`L483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_find_and_grep_p1.py#L483) — Test all tools with empty results.

