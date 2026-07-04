---
title: 'Module: tests/integration/_test_phase7_unicode_security_helpers.py'
type: catalog
provenance: extracted
module: tests/integration/_test_phase7_unicode_security_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration._test_phase7_unicode_security_helpers`/
symbols:
  collect_unicode_attack_results: collect_unicode_attack_results().
  _run_unicode_attack: _run_unicode_attack().
  assert_unicode_attacks_handled_safely: assert_unicode_attacks_handled_safely().
---
# Module: [`tests/integration/_test_phase7_unicode_security_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_unicode_security_helpers.py)

## Functions
- `_run_unicode_attack(list_tool: ListFilesTool, attack_string: str, secure_test_project: str)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_unicode_security_helpers.py#L34)
- `assert_unicode_attacks_handled_safely(unicode_results: list[dict[str, Any]])` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_unicode_security_helpers.py#L21) — Assert and report Unicode attack handling expectations.
- `collect_unicode_attack_results(list_tool: ListFilesTool, unicode_attacks: Iterable[str], secure_test_project: str)` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/_test_phase7_unicode_security_helpers.py#L9) — Run Unicode attack patterns through the list-files path boundary.

