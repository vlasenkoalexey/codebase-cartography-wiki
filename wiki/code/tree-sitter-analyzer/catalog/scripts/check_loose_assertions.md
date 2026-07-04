---
title: 'Module: scripts/check_loose_assertions.py'
type: catalog
provenance: extracted
module: scripts/check_loose_assertions.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.check_loose_assertions`/
symbols:
  check_file: check_file().
  format_baseline_json: format_baseline_json().
  _check_added_ranges: _check_added_ranges().
  main: main().
  Violation: Violation#
  baseline_violations: baseline_violations().
  _assert_has_concrete_behavior: _assert_has_concrete_behavior().
  format_baseline_table: format_baseline_table().
  _none_compare_subject: _none_compare_subject().
  check_diff: check_diff().
  check_staged: check_staged().
  Violation.lineno: Violation#lineno.
  count_baseline_legacy: count_baseline_legacy().
  _assert_has_none_tautology: _assert_has_none_tautology().
  _assert_is_placeholder_candidate: _assert_is_placeholder_candidate().
  _find_loose_compares: _find_loose_compares().
  _is_int_literal: _is_int_literal().
  _is_loose_compare: _is_loose_compare().
  _is_placeholder_compare: _is_placeholder_compare().
  _is_none_tautology: _is_none_tautology().
  _loose_operator: _loose_operator().
  _asserts_by_function: _asserts_by_function().
  _segment_is_exempt: _segment_is_exempt().
  _added_line_ranges: _added_line_ranges().
  _added_line_ranges_staged: _added_line_ranges_staged().
  PROPERTY_FILE_RE: PROPERTY_FILE_RE.
  Violation.path: Violation#path.
  count_baseline: count_baseline().
  Violation.snippet: Violation#snippet.
  Violation.end_lineno: Violation#end_lineno.
  _parse_added_line_ranges: _parse_added_line_ranges().
  _repo_relative: _repo_relative().
  EXEMPTION_RE: EXEMPTION_RE.
  _PLACEHOLDER_OPERATOR: _PLACEHOLDER_OPERATOR.
  _TAUTOLOGY_OPERATOR: _TAUTOLOGY_OPERATOR.
  Violation.operator: Violation#operator.
  Violation.category: Violation#category.
  _is_none_literal: _is_none_literal().
  _expr_key: _expr_key().
  _assert_has_eq_compare: _assert_has_eq_compare().
  _category_for_path: _category_for_path().
  _LOOSE_OPS: _LOOSE_OPS.
---
# Module: [`scripts/check_loose_assertions.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py)

## Classes
### `Violation`  ·  implements/extends NamedTuple
- def: [`scripts/check_loose_assertions.py:70`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L70)
- signature: `class Violation(NamedTuple):`
- members:
  - `category` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L76)
  - `end_lineno` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L74)
  - `lineno` — [`L72`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L72)
  - `operator` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L75)
  - `path` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L71)
  - `snippet` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L73)
- used by: [`check_file`](check_loose_assertions.md#check_file), [`format_baseline_json`](check_loose_assertions.md#format_baseline_json), [`_check_added_ranges`](check_loose_assertions.md#_check_added_ranges), [`baseline_violations`](check_loose_assertions.md#baseline_violations), [`format_baseline_table`](check_loose_assertions.md#format_baseline_table)

## Functions
- `_added_line_ranges(base_ref: str)` — [`L345`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L345) — Map changed test file (new path) → set of ADDED line numbers.
- `_added_line_ranges_staged()` — [`L374`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L374) — Map staged test file (new path) -> set of ADDED line numbers.
- `_assert_has_concrete_behavior(assert_node: ast.Assert)` — [`L167`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L167) — Return True when an assert checks behavior, not only a weak shape.
- `_assert_has_eq_compare(assert_node: ast.Assert)` — [`L178`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L178) — Return True if the assert's test contains any == comparison.
- `_assert_has_none_tautology(assert_node: ast.Assert)` — [`L155`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L155) — Return True if the assert contains a None-check tautology.
- `_assert_is_placeholder_candidate(assert_node: ast.Assert)` — [`L160`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L160) — Return True when an assert is only an existence check.
- `_asserts_by_function(tree: ast.AST)` — [`L224`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L224) — Map assert node ids to whether their function has concrete assertions.
- `_category_for_path(path: Path)` — [`L210`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L210) — Best-effort triage category for baseline queueing.
- `_check_added_ranges(added: dict[str, set[int]], source_label: str)` — [`L434`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L434) — Run assertion-quality checks against already parsed added line ranges.
- `_expr_key(node: ast.expr)` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L94) — Return a stable structural key for comparing simple expressions.
- `_find_loose_compares(assert_node: ast.Assert)` — [`L191`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L191) — Return all Compare nodes inside the assert that are loose bounds.
- `_is_int_literal(node: ast.expr)` — [`L84`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L84) — Return True for integer constant literals (0, 1, 2, …).
- `_is_loose_compare(compare: ast.Compare)` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L99) — Return True if the Compare contains a >= / > check against an int.
- `_is_none_literal(node: ast.expr)` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L89) — Return True for the None singleton literal.
- `_is_none_tautology(expr: ast.expr)` — [`L136`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L136) — Return True for ``x is not None or x is None`` style tautologies.
- `_is_placeholder_compare(compare: ast.Compare)` — [`L131`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L131) — Return True for the placeholder shape ``expr is not None``.
- `_loose_operator(compare: ast.Compare)` — [`L200`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L200) — Return the first loose operator in *compare* as source-like text.
- `_none_compare_subject(compare: ast.Compare, op_type: type[ast.cmpop])` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L120) — Return the expression key for ``expr is/is not None`` comparisons.
- `_parse_added_line_ranges(diff_text: str)` — [`L395`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L395) — Parse ``git diff -U0`` output into added line numbers.
- `_repo_relative(path: str, project_root: Path)` — [`L484`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L484)
- `_segment_is_exempt(source_lines: list[str], lineno: int, end_lineno: int)` — [`L246`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L246) — Return True if the exemption marker appears in the assert's source lines.
- `baseline_violations(tests_dir: Path)` — [`L474`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L474) — Return all baseline weak assertions under *tests_dir* using AST rules.
- `check_diff(base_ref: str)` — [`L419`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L419) — Run diff-scoped check.  Returns exit code (0 = OK, 1 = violations).
- `check_file(path: Path)` — [`L263`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L263) — Return Violation entries for every weak assert in the file.
- `check_staged()` — [`L429`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L429) — Run staged diff check. Returns exit code (0 = OK, 1 = violations).
- `count_baseline(tests_dir: Path)` — [`L469`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L469) — Count all weak assertions under *tests_dir* using AST rules.
- `count_baseline_legacy(tests_dir: Path)` — [`L519`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L519) — Compatibility alias retained for older callers.
- `format_baseline_json(violations: list[Violation], project_root: Path)` — [`L492`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L492) — Format violations as stable machine-readable JSON.
- `format_baseline_table(violations: list[Violation], project_root: Path)` — [`L509`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L509) — Format violations as a short human-readable summary table.
- `main(argv: list[str] | None = None)` — [`L534`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L534)

## Module values
- `EXEMPTION_RE` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L56)
- `PROPERTY_FILE_RE` — [`L57`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L57)
- `_LOOSE_OPS` — [`L60`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L60)
- `_PLACEHOLDER_OPERATOR` — [`L61`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L61)
- `_TAUTOLOGY_OPERATOR` — [`L62`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_loose_assertions.py#L62)

