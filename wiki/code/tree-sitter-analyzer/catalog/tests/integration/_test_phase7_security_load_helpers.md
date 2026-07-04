---
title: 'Module: tests/integration/_test_phase7_security_load_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/_test_phase7_security_load_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration._test_phase7_security_load_helpers`/
symbols:
  _build_security_under_load_tasks: _build_security_under_load_tasks().
  collect_security_under_load_results: collect_security_under_load_results().
  _classify_security_under_load_results: _classify_security_under_load_results().
  _classify_security_under_load_result: _classify_security_under_load_result().
---
# Module: [`tests/integration/_test_phase7_security_load_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_load_helpers.py)

## Functions
- `_build_security_under_load_tasks(secure_test_project: str)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_load_helpers.py#L30)
- `_classify_security_under_load_result(attack_type: str, result: Any, successful_attacks: list[dict[str, str]], blocked_attacks: list[dict[str, str]])` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_load_helpers.py#L77)
- `_classify_security_under_load_results(concurrent_attacks: list[tuple[str, Any]], results: list[Any])` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_load_helpers.py#L55)
- `collect_security_under_load_results(secure_test_project: str)` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_security_load_helpers.py#L11) — Run mixed security load and classify attack outcomes.

