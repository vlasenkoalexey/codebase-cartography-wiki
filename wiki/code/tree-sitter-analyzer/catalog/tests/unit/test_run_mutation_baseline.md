---
title: 'Module: tests/unit/test_run_mutation_baseline.py'
type: catalog
provenance: extracted
module: tests/unit/test_run_mutation_baseline.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_run_mutation_baseline`/test_
symbols:
  test_run_module_does_not_invoke_uv_while_pyproject_is_swapped: run_module_does_not_invoke_uv_while_pyproject_is_swapped().
  test_resolve_mutmut_command_prefers_current_environment_script: resolve_mutmut_command_prefers_current_environment_script().
  test_resolve_mutmut_command_falls_back_to_path: resolve_mutmut_command_falls_back_to_path().
  test_resolve_mutmut_command_falls_back_to_python_module: resolve_mutmut_command_falls_back_to_python_module().
  test_run_module_rejects_unknown_module: run_module_rejects_unknown_module().
  test_main_defaults_to_ast_diff: main_defaults_to_ast_diff().
  test_run_module_does_not_invoke_uv_while_pyproject_is_swapped.fake_run: run_module_does_not_invoke_uv_while_pyproject_is_swapped().fake_run().
---
# Module: [`tests/unit/test_run_mutation_baseline.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_run_mutation_baseline.py)

## Functions
- `fake_run(cmd, *, cwd=None, capture_output=False)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_run_mutation_baseline.py#L21)
- `test_main_defaults_to_ast_diff(monkeypatch, tmp_path: Path)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_run_mutation_baseline.py#L100)
- `test_resolve_mutmut_command_falls_back_to_path(monkeypatch, tmp_path: Path)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_run_mutation_baseline.py#L61)
- `test_resolve_mutmut_command_falls_back_to_python_module(monkeypatch, tmp_path: Path)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_run_mutation_baseline.py#L77)
- `test_resolve_mutmut_command_prefers_current_environment_script(monkeypatch, tmp_path: Path)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_run_mutation_baseline.py#L44)
- `test_run_module_does_not_invoke_uv_while_pyproject_is_swapped(monkeypatch, tmp_path: Path)` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_run_mutation_baseline.py#L11)
- `test_run_module_rejects_unknown_module(capsys, tmp_path: Path)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_run_mutation_baseline.py#L92)

