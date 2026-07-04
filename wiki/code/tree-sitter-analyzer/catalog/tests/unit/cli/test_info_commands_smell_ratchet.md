---
title: 'Module: tests/unit/cli/test_info_commands_smell_ratchet.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_info_commands_smell_ratchet.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_info_commands_smell_ratchet`/
symbols:
  code_patterns_result: code_patterns_result().
  TARGET: TARGET.
  test_info_commands_total_smell_ratchet: test_info_commands_total_smell_ratchet().
  test_info_commands_critical_smell_ratchet: test_info_commands_critical_smell_ratchet().
  test_info_commands_warning_smell_ratchet: test_info_commands_warning_smell_ratchet().
  PROJECT_ROOT: PROJECT_ROOT.
  MAX_TOTAL_PATTERNS: MAX_TOTAL_PATTERNS.
  MAX_CRITICAL: MAX_CRITICAL.
  MAX_WARNING: MAX_WARNING.
---
# Module: [`tests/unit/cli/test_info_commands_smell_ratchet.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands_smell_ratchet.py)

## Functions
- `code_patterns_result()` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands_smell_ratchet.py#L42) — Invoke ``--code-patterns`` once for all assertions in this module.
- `test_info_commands_critical_smell_ratchet(code_patterns_result: dict[str, object])` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands_smell_ratchet.py#L78) — No critical smells (deep_nesting depth ≥ 8, god_class, etc.).
- `test_info_commands_total_smell_ratchet(code_patterns_result: dict[str, object])` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands_smell_ratchet.py#L65) — info_commands.py must never grow beyond ``MAX_TOTAL_PATTERNS`` smells.
- `test_info_commands_warning_smell_ratchet(code_patterns_result: dict[str, object])` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands_smell_ratchet.py#L90) — At most ``MAX_WARNING`` warning-level smells.

## Module values
- `MAX_CRITICAL` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands_smell_ratchet.py#L37)
- `MAX_TOTAL_PATTERNS` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands_smell_ratchet.py#L36)
- `MAX_WARNING` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands_smell_ratchet.py#L38)
- `PROJECT_ROOT` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands_smell_ratchet.py#L29)
- `TARGET` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands_smell_ratchet.py#L30)

