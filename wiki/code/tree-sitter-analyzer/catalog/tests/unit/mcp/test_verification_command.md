---
title: 'Module: tests/unit/mcp/test_verification_command.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_verification_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_verification_command`/test_
symbols:
  test_detect_default_test_command_falls_back_to_pytest: detect_default_test_command_falls_back_to_pytest().
  test_detect_default_test_command_uses_package_json_test_script: detect_default_test_command_uses_package_json_test_script().
  test_detect_default_test_command_prefers_node_lockfile_manager: detect_default_test_command_prefers_node_lockfile_manager().
  test_detect_default_test_command_uses_go_test: detect_default_test_command_uses_go_test().
  test_detect_default_test_command_uses_cargo_test: detect_default_test_command_uses_cargo_test().
  test_build_test_command_targets_supported_runners: build_test_command_targets_supported_runners().
  test_build_test_command_falls_back_for_untargetable_runners: build_test_command_falls_back_for_untargetable_runners().
---
# Module: [`tests/unit/mcp/test_verification_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_verification_command.py)

## Functions
- `test_build_test_command_falls_back_for_untargetable_runners()` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_verification_command.py#L76) — Untargeted runners should keep the safe full-project default command.
- `test_build_test_command_targets_supported_runners()` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_verification_command.py#L65) — Supported runners should receive direct test path arguments.
- `test_detect_default_test_command_falls_back_to_pytest(tmp_path)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_verification_command.py#L10) — Unknown or Python-style projects should keep the repo's pytest contract.
- `test_detect_default_test_command_prefers_node_lockfile_manager(tmp_path)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_verification_command.py#L31) — Node package manager lockfiles should make commands copy-pasteable.
- `test_detect_default_test_command_uses_cargo_test(tmp_path)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_verification_command.py#L55) — Rust projects should surface cargo test as the default command.
- `test_detect_default_test_command_uses_go_test(tmp_path)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_verification_command.py#L45) — Go projects should not be sent into pytest.
- `test_detect_default_test_command_uses_package_json_test_script(tmp_path)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_verification_command.py#L18) — Node projects should expose their package test script to agents.

