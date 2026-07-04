---
title: 'Module: tests/unit/mcp/test_mcp_fd_rg_utils.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_mcp_fd_rg_utils.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_mcp_fd_rg_utils`/
symbols:
  test_fd_rg_utils_edge_cases: test_fd_rg_utils_edge_cases().
  test_fd_67_performance_large_dataset: test_fd_67_performance_large_dataset().
  test_fd_68_command_timeout_handling: test_fd_68_command_timeout_handling().
  test_fd_69_invalid_regex_handling: test_fd_69_invalid_regex_handling().
  test_fd_70_memory_usage_optimization: test_fd_70_memory_usage_optimization().
  test_fd_71_cross_platform_compatibility: test_fd_71_cross_platform_compatibility().
  test_fd_72_edge_case_patterns: test_fd_72_edge_case_patterns().
  test_fd_73_concurrent_execution_safety: test_fd_73_concurrent_execution_safety().
  test_fd_74_resource_cleanup: test_fd_74_resource_cleanup().
  test_fd_85_invalid_utf8_handling: test_fd_85_invalid_utf8_handling().
  test_fd_87_single_and_multithreaded_execution: test_fd_87_single_and_multithreaded_execution().
  test_fd_88_number_parsing_errors: test_fd_88_number_parsing_errors().
  test_fd_89_opposing_parameters: test_fd_89_opposing_parameters().
  test_fd_90_error_if_hidden_not_set_and_pattern_starts_with_dot: test_fd_90_error_if_hidden_not_set_and_pattern_starts_with_dot().
  test_fd_91_invalid_cwd: test_fd_91_invalid_cwd().
  test_parse_rg_count_output: test_parse_rg_count_output().
  test_build_rg_command_with_count_only: test_build_rg_command_with_count_only().
  test_summarize_search_results: test_summarize_search_results().
  test_build_fd_command: test_build_fd_command().
  test_parse_rg_count_output_edge_cases: test_parse_rg_count_output_edge_cases().
  test_summarize_search_results_edge_cases: test_summarize_search_results_edge_cases().
  test_fd_67_performance_large_dataset.fake_run: test_fd_67_performance_large_dataset().fake_run().
  test_fd_68_command_timeout_handling.fake_run: test_fd_68_command_timeout_handling().fake_run().
  test_fd_69_invalid_regex_handling.fake_run: test_fd_69_invalid_regex_handling().fake_run().
  test_fd_70_memory_usage_optimization.fake_run: test_fd_70_memory_usage_optimization().fake_run().
  test_fd_71_cross_platform_compatibility.fake_run: test_fd_71_cross_platform_compatibility().fake_run().
  test_fd_72_edge_case_patterns.fake_run: test_fd_72_edge_case_patterns().fake_run().
  test_fd_73_concurrent_execution_safety.fake_run: test_fd_73_concurrent_execution_safety().fake_run().
  test_fd_74_resource_cleanup.fake_run: test_fd_74_resource_cleanup().fake_run().
  test_fd_85_invalid_utf8_handling.fake_run: test_fd_85_invalid_utf8_handling().fake_run().
  test_fd_87_single_and_multithreaded_execution.fake_run: test_fd_87_single_and_multithreaded_execution().fake_run().
  test_fd_88_number_parsing_errors.fake_run: test_fd_88_number_parsing_errors().fake_run().
  test_fd_89_opposing_parameters.fake_run: test_fd_89_opposing_parameters().fake_run().
  test_fd_90_error_if_hidden_not_set_and_pattern_starts_with_dot.fake_run: test_fd_90_error_if_hidden_not_set_and_pattern_starts_with_dot().fake_run().
  mock_external_commands: mock_external_commands().
  DummyProc: DummyProc#
  DummyProc.__init__: DummyProc#__init__().
  DummyProc.rc: DummyProc#rc.
  DummyProc.stdout: DummyProc#stdout.
  DummyProc.stderr: DummyProc#stderr.
---
# Module: [`tests/unit/mcp/test_mcp_fd_rg_utils.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py)

## Classes
### `DummyProc`
- def: [`tests/unit/mcp/test_mcp_fd_rg_utils.py:16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L16)
- signature: `class DummyProc:`
- members:
  - `rc` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L18)
  - `stderr` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L20)
  - `stdout` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L19)
- protocol/private: `__init__`[`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L17)

## Functions
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L305)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L331`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L331)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L358)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L387`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L387)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L415`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L415)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L449`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L449)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L484`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L484)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L511`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L511)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L538`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L538)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L567`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L567)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L592`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L592)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L628`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L628)
- `fake_run(cmd, cwd=None, timeout=None, timeout_ms=None)` — [`L657`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L657)
- `mock_external_commands(monkeypatch)` — [`L7`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L7) — Auto-mock external command availability checks for all tests in this module.
- `test_build_fd_command()` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L142) — Test building fd command with various options.
- `test_build_rg_command_with_count_only()` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L45) — Test building ripgrep command with count_only_matches option.
- `test_fd_67_performance_large_dataset(tmp_path, monkeypatch)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L294) — Test performance with large dataset - corresponds to fd's performance tests.
- `test_fd_68_command_timeout_handling(tmp_path, monkeypatch)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L324) — Test command timeout handling - corresponds to fd's timeout tests.
- `test_fd_69_invalid_regex_handling(tmp_path, monkeypatch)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L351) — Test invalid regex handling - corresponds to fd's regex error tests.
- `test_fd_70_memory_usage_optimization(tmp_path, monkeypatch)` — [`L378`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L378) — Test memory usage optimization - corresponds to fd's memory tests.
- `test_fd_71_cross_platform_compatibility(tmp_path, monkeypatch)` — [`L406`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L406) — Test cross-platform compatibility - corresponds to fd's platform tests.
- `test_fd_72_edge_case_patterns(tmp_path, monkeypatch)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L439) — Test edge case patterns - corresponds to fd's edge case tests.
- `test_fd_73_concurrent_execution_safety(tmp_path, monkeypatch)` — [`L476`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L476) — Test concurrent execution safety - corresponds to fd's concurrency tests.
- `test_fd_74_resource_cleanup(tmp_path, monkeypatch)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L504) — Test resource cleanup - corresponds to fd's cleanup tests.
- `test_fd_85_invalid_utf8_handling(tmp_path, monkeypatch)` — [`L530`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L530) — Test invalid UTF-8 filename handling - corresponds to fd's test_invalid_utf8.
- `test_fd_87_single_and_multithreaded_execution(tmp_path, monkeypatch)` — [`L559`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L559) — Test single and multithreaded execution - corresponds to fd's test_single_and_multithreaded_execution.
- `test_fd_88_number_parsing_errors(tmp_path, monkeypatch)` — [`L588`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L588) — Test number parsing errors - corresponds to fd's test_number_parsing_errors.
- `test_fd_89_opposing_parameters(tmp_path, monkeypatch)` — [`L621`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L621) — Test opposing parameters - corresponds to fd's test_opposing.
- `test_fd_90_error_if_hidden_not_set_and_pattern_starts_with_dot(tmp_path, monkeypatch)` — [`L647`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L647) — Test error for hidden pattern without hidden flag - corresponds to fd's test_error_if_hidden_not_set_and_pattern_starts_with_dot.
- `test_fd_91_invalid_cwd(tmp_path, monkeypatch)` — [`L690`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L690) — Test invalid current working directory - corresponds to fd's test_invalid_cwd.
- `test_fd_rg_utils_edge_cases()` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L266) — Test edge cases in fd_rg_utils functions.
- `test_parse_rg_count_output()` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L24) — Test parsing ripgrep --count-matches output.
- `test_parse_rg_count_output_edge_cases()` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L211) — Test parsing ripgrep count output with edge cases.
- `test_summarize_search_results()` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L107) — Test summarizing search results for context reduction.
- `test_summarize_search_results_edge_cases()` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_mcp_fd_rg_utils.py#L243) — Test summarizing search results with edge cases.

