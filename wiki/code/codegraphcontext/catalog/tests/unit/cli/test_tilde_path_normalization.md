---
title: 'Module: tests/unit/cli/test_tilde_path_normalization.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_tilde_path_normalization.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.cli.test_tilde_path_normalization`/
symbols:
  _set_home_env: _set_home_env().
  test_normalize_config_path_expands_home_and_makes_absolute: test_normalize_config_path_expands_home_and_makes_absolute().
  test_validate_config_value_accepts_tilde_path_without_relative_tilde_dir: test_validate_config_value_accepts_tilde_path_without_relative_tilde_dir().
  test_configure_mcp_client_writes_expanded_paths: test_configure_mcp_client_writes_expanded_paths().
---
# Module: [`tests/unit/cli/test_tilde_path_normalization.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_tilde_path_normalization.py)

## Functions
- `_set_home_env(monkeypatch, tmp_path)` — [`L9`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_tilde_path_normalization.py#L9) — Set HOME (and USERPROFILE on Windows) so os.path.expanduser('~') resolves to tmp_path.
- `test_configure_mcp_client_writes_expanded_paths(tmp_path, monkeypatch)` — [`L31`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_tilde_path_normalization.py#L31)
- `test_normalize_config_path_expands_home_and_makes_absolute(tmp_path, monkeypatch)` — [`L16`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_tilde_path_normalization.py#L16)
- `test_validate_config_value_accepts_tilde_path_without_relative_tilde_dir(tmp_path, monkeypatch)` — [`L22`](../../../../../../../raw/code/codegraphcontext/tests/unit/cli/test_tilde_path_normalization.py#L22)

