---
title: 'Module: tests/unit/core/test_file_output_search_content.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_file_output_search_content.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_file_output_search_content`/
symbols:
  test_search_content_with_output_file_and_suppress_output: test_search_content_with_output_file_and_suppress_output().
  test_search_content_output_file_without_suppress_output: test_search_content_output_file_without_suppress_output().
  test_search_content_large_results_token_optimization: test_search_content_large_results_token_optimization().
  test_search_content_validation_with_new_parameters: test_search_content_validation_with_new_parameters().
  _make_multi_file_rg_output: _make_multi_file_rg_output().
  _make_rg_match_line: _make_rg_match_line().
  _patch_rg_tools: _patch_rg_tools().
  test_search_content_with_output_file_and_suppress_output.mock_run_command: test_search_content_with_output_file_and_suppress_output().mock_run_command().
  test_search_content_output_file_without_suppress_output.mock_run_command: test_search_content_output_file_without_suppress_output().mock_run_command().
  test_search_content_large_results_token_optimization.mock_run_command: test_search_content_large_results_token_optimization().mock_run_command().
---
# Module: [`tests/unit/core/test_file_output_search_content.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py)

## Functions
- `_make_multi_file_rg_output(tmp_path, n_files: int, n_functions: int)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py#L41) — Build ripgrep JSON output with n_files × n_functions function matches.
- `_make_rg_match_line(file_path, line_text: str, function_name: str, start: int, end: int, line_number: int = 1, offset: int = 0)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py#L15) — Build one ripgrep JSON match line.
- `_patch_rg_tools(monkeypatch, mock_run_command)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py#L59) — Monkeypatch fd_rg_utils so tests don't invoke real ripgrep.
- `mock_run_command(cmd, **kwargs)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py#L87)
- `mock_run_command(cmd, **kwargs)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py#L134)
- `mock_run_command(cmd, **kwargs)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py#L171)
- `test_search_content_large_results_token_optimization(monkeypatch, tmp_path)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py#L161)
- `test_search_content_output_file_without_suppress_output(monkeypatch, tmp_path)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py#L121)
- `test_search_content_validation_with_new_parameters(tmp_path)` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py#L203)
- `test_search_content_with_output_file_and_suppress_output(monkeypatch, tmp_path)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_file_output_search_content.py#L72)

