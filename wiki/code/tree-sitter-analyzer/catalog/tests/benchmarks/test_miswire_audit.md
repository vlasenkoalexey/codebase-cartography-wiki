---
title: 'Module: tests/benchmarks/test_miswire_audit.py'
type: catalog
provenance: extracted
module: tests/benchmarks/test_miswire_audit.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.benchmarks.test_miswire_audit`/
symbols:
  test_audit_flags_name_only_miswire_but_tsa_does_not: test_audit_flags_name_only_miswire_but_tsa_does_not().
  test_genuine_collisions_exclude_builtins: test_genuine_collisions_exclude_builtins().
  test_symbols_json_fallback_when_no_ast_symbol_rows: test_symbols_json_fallback_when_no_ast_symbol_rows().
  test_render_terminal_and_card_are_honest: test_render_terminal_and_card_are_honest().
  test_no_fts5_renders_clear_unavailable_message_not_misleading_zero: test_no_fts5_renders_clear_unavailable_message_not_misleading_zero().
  test_audit_clean_repo_reports_zero_for_both: test_audit_clean_repo_reports_zero_for_both().
  _planted_polyglot: _planted_polyglot().
  test_js_builtins_excluded_from_genuine: test_js_builtins_excluded_from_genuine().
  pytestmark: pytestmark.
---
# Module: [`tests/benchmarks/test_miswire_audit.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_miswire_audit.py)

## Functions
- `_planted_polyglot()` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_miswire_audit.py#L21) — A tiny repo with a same-name collision: a Python `sorted()` caller and a
- `test_audit_clean_repo_reports_zero_for_both()` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_miswire_audit.py#L50) — A single-language repo with no cross-language collisions -> 0 and 0.
- `test_audit_flags_name_only_miswire_but_tsa_does_not()` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_miswire_audit.py#L32)
- `test_genuine_collisions_exclude_builtins()` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_miswire_audit.py#L117) — RFC-0011 open Q1 (skeptic-resistance): the GENUINE count excludes the
- `test_js_builtins_excluded_from_genuine()` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_miswire_audit.py#L152) — Codex #377 P2: a language WITHOUT a builtin set would count its own
- `test_no_fts5_renders_clear_unavailable_message_not_misleading_zero()` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_miswire_audit.py#L106) — Codex #369 L158: on no-FTS5 builds TSA writes no call edges; the audit must
- `test_render_terminal_and_card_are_honest()` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_miswire_audit.py#L64) — The output must NOT claim the name-only number is CodeGraph's exact count
- `test_symbols_json_fallback_when_no_ast_symbol_rows()` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_miswire_audit.py#L82) — Codex #369 L74: on no-FTS5 builds ast_symbol_rows is absent; the audit

## Module values
- `pytestmark` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/benchmarks/test_miswire_audit.py#L18)

