---
title: 'Module: tests/unit/test_constraint_dsl.py'
type: catalog
provenance: extracted
module: tests/unit/test_constraint_dsl.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_constraint_dsl`/
symbols:
  TestEvaluator.test_duplicate_pk_violations_deduplicated: TestEvaluator#test_duplicate_pk_violations_deduplicated().
  TestEvaluator.test_violation_detected_mcp_to_cli: TestEvaluator#test_violation_detected_mcp_to_cli().
  TestEvaluator.test_real_violation_not_filtered_when_import_present: TestEvaluator#test_real_violation_not_filtered_when_import_present().
  _build_call_edges_db: _build_call_edges_db().
  _stage_constraints_file: _stage_constraints_file().
  TestConstraintParser.test_parse_valid_yaml: TestConstraintParser#test_parse_valid_yaml().
  TestEvaluator.test_phantom_bare_name_resolution_skipped_when_no_import: TestEvaluator#test_phantom_bare_name_resolution_skipped_when_no_import().
  TestEvaluator.test_exception_suppresses_violation: TestEvaluator#test_exception_suppresses_violation().
  TestEvaluator.test_eval_perf_on_synthetic_edges_under_500ms: TestEvaluator#test_eval_perf_on_synthetic_edges_under_500ms().
  TestConstraintParser.test_parse_invalid_yaml_raises: TestConstraintParser#test_parse_invalid_yaml_raises().
  TestConstraintParser.test_parse_unknown_top_level_key_raises: TestConstraintParser#test_parse_unknown_top_level_key_raises().
  TestConstraintParser.test_parse_unknown_per_rule_key_warns_and_skips: TestConstraintParser#test_parse_unknown_per_rule_key_warns_and_skips().
  TestConstraintParser.test_missing_config_returns_empty_constraints: TestConstraintParser#test_missing_config_returns_empty_constraints().
  TestGlobMatching.test_glob_matches_recursive: TestGlobMatching#test_glob_matches_recursive().
  _populate_ast_imports: _populate_ast_imports().
  FIXTURES: FIXTURES.
  TestConstraintParser: TestConstraintParser#
  TestGlobMatching: TestGlobMatching#
  TestEvaluator: TestEvaluator#
---
# Module: [`tests/unit/test_constraint_dsl.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py)

## Classes
### `TestConstraintParser`
- def: [`tests/unit/test_constraint_dsl.py:193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L193)
- doc: Cover the YAML-to-Constraint pipeline end to end.
- signature: `class TestConstraintParser:`
- members:
  - `test_missing_config_returns_empty_constraints(self, tmp_path: Path)` — [`L302`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L302) — A repo with no constraints.yml is a valid state, not an error.
  - `test_parse_invalid_yaml_raises(self, tmp_path: Path)` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L228) — Unclosed flow sequence → ConstraintParseError with line context.
  - `test_parse_unknown_per_rule_key_warns_and_skips(self, tmp_path: Path, caplog: pytest.LogCaptureFixture)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L265) — Forward-compat: unknown per-rule keys are warn-and-skip, NOT fatal.
  - `test_parse_unknown_top_level_key_raises(self, tmp_path: Path)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L248) — ``rulez:`` instead of ``constraints:`` is fatal and names the typo.
  - `test_parse_valid_yaml(self, tmp_path: Path)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L196) — Three rules, three severities, exceptions preserved on rule 2.
- uses (calls/refs, reference-scoped): [`load_constraints`](../../tree_sitter_analyzer/constraints/parser.md#load_constraints), [`ConstraintParseError`](../../tree_sitter_analyzer/constraints/parser.md#ConstraintParseError), [`id`](../../tree_sitter_analyzer/constraints/schema.md#Constraint.id), [`exceptions`](../../tree_sitter_analyzer/constraints/schema.md#Constraint.exceptions), [`severity`](../../tree_sitter_analyzer/constraints/schema.md#Constraint.severity)  (1 test-only)

### `TestEvaluator`
- def: [`tests/unit/test_constraint_dsl.py:358`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L358)
- doc: Synthesize an ast_call_edges row and verify the evaluator's verdict.
- signature: `class TestEvaluator:`
- members:
  - `test_duplicate_pk_violations_deduplicated(self, tmp_path: Path)` — [`L541`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L541) — evaluate() dedupes violations that share the same PK.
  - `test_eval_perf_on_synthetic_edges_under_500ms(self, tmp_path: Path)` — [`L443`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L443) — 50k edges × 5 rules in <500 ms.
  - `test_exception_suppresses_violation(self, tmp_path: Path)` — [`L403`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L403) — An edge whose caller is in ``exceptions:`` produces zero violations.
  - `test_phantom_bare_name_resolution_skipped_when_no_import(self, tmp_path: Path)` — [`L649`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L649) — Regression #780: bare-name callee resolved to forbidden module is
  - `test_real_violation_not_filtered_when_import_present(self, tmp_path: Path)` — [`L706`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L706) — Regression #780: a genuine cross-boundary call IS flagged when the
  - `test_violation_detected_mcp_to_cli(self, tmp_path: Path)` — [`L361`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L361) — A real edge that crosses a forbidden boundary → 1 error violation.
- uses (calls/refs, reference-scoped): [`EdgeKind`](../../tree_sitter_analyzer/graph/edge_store.md#EdgeKind), [`symbol_node`](../../tree_sitter_analyzer/graph/edge_store.md#symbol_node), [`CALLS`](../../tree_sitter_analyzer/graph/edge_store.md#EdgeKind.CALLS), [`load_constraints`](../../tree_sitter_analyzer/constraints/parser.md#load_constraints), [`evaluate`](../../tree_sitter_analyzer/constraints/evaluator.md#evaluate), [`EDGE_STORE_SCHEMA`](../../tree_sitter_analyzer/graph/edge_store.md#EDGE_STORE_SCHEMA), [`caller_file`](../../tree_sitter_analyzer/constraints/schema.md#Violation.caller_file), [`rule_id`](../../tree_sitter_analyzer/constraints/schema.md#Violation.rule_id), [`callee_file`](../../tree_sitter_analyzer/constraints/schema.md#Violation.callee_file), [`caller_line`](../../tree_sitter_analyzer/constraints/schema.md#Violation.caller_line), [`callee_name`](../../tree_sitter_analyzer/constraints/schema.md#Violation.callee_name), [`severity`](../../tree_sitter_analyzer/constraints/schema.md#Violation.severity)  (3 test-only)

### `TestGlobMatching`
- def: [`tests/unit/test_constraint_dsl.py:320`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L320)
- doc: Pin the recursive `**` semantics — easy to get wrong.
- signature: `class TestGlobMatching:`
- members:
  - `test_glob_matches_recursive(self)` — [`L323`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L323) — ``**`` descends into arbitrary subdirectories.
- uses (calls/refs, reference-scoped): [`match_glob`](../../tree_sitter_analyzer/constraints/parser.md#match_glob)

## Functions
- `_build_call_edges_db(db_path: Path, rows: list[tuple[str, str, int, str, str, str]])` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L73) — Create a minimal sqlite db with the unified ``edges`` schema.
- `_populate_ast_imports(db_path: Path, rows: list[tuple[str, str]])` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L152) — Insert rows into ``ast_imports`` in the given DB.
- `_stage_constraints_file(tmp_path: Path, fixture_name: str)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L58) — Copy a fixture into ``<tmp_path>/architectural-constraints.yml``.

## Module values
- `FIXTURES` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_constraint_dsl.py#L50)

