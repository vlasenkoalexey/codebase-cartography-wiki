---
title: 'Module: tests/unit/test_java_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_java_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_java_method_resolution`/
symbols:
  _index: _index().
  _resolution_for: _resolution_for().
  test_java_stdlib_method_classifies_as_stdlib: test_java_stdlib_method_classifies_as_stdlib().
  test_java_optional_method_classifies_as_stdlib: test_java_optional_method_classifies_as_stdlib().
  test_java_project_method_shadows_stdlib_name: test_java_project_method_shadows_stdlib_name().
  test_java_ambiguous_project_method_stays_unknown: test_java_ambiguous_project_method_stays_unknown().
  test_cross_language_python_table_does_not_classify_java_caller: test_cross_language_python_table_does_not_classify_java_caller().
  test_java_dropped_generic_method_stays_unknown: test_java_dropped_generic_method_stays_unknown().
  test_java_interface_method_stays_unknown: test_java_interface_method_stays_unknown().
  test_java_production_verify_stays_unknown: test_java_production_verify_stays_unknown().
  test_java_external_method_classifies_as_external: test_java_external_method_classifies_as_external().
  test_java_project_method_shadows_external_name: test_java_project_method_shadows_external_name().
  test_cross_language_python_external_does_not_classify_java_caller: test_cross_language_python_external_does_not_classify_java_caller().
  test_java_external_import_receiver_not_stdlib: test_java_external_import_receiver_not_stdlib().
  test_java_external_static_import_not_stdlib: test_java_external_static_import_not_stdlib().
  test_java_project_fqn_receiver_wins_over_imported_tail: test_java_project_fqn_receiver_wins_over_imported_tail().
---
# Module: [`tests/unit/test_java_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py)

## Functions
- `_index(tmp_path: Path, files: dict[str, str])` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L26) — Index a mixed-language project rooted at ``tmp_path``.
- `_resolution_for(db_path: str, callee_name: str)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L45)
- `test_cross_language_python_external_does_not_classify_java_caller(tmp_path: Path)` — [`L358`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L358) — A Java ``obj.assert_called_once()`` must NOT be classified external from
- `test_cross_language_python_table_does_not_classify_java_caller(tmp_path: Path)` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L171) — CRITICAL cross-language gate: a Java ``str.substring(1)`` must still
- `test_java_ambiguous_project_method_stays_unknown(tmp_path: Path)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L141) — Two Java classes define ``substring`` → a bare ``substring()`` stays
- `test_java_dropped_generic_method_stays_unknown(tmp_path: Path)` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L202) — Codex P2 #326 regression lock: a Java ``cache.get(k)`` with no project
- `test_java_external_import_receiver_not_stdlib(tmp_path: Path)` — [`L388`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L388) — ``StringUtils.substring(s, 1)`` with ``import
- `test_java_external_method_classifies_as_external(tmp_path: Path)` — [`L306`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L306) — A Java test ``assertEquals(a, b)`` with no project ``assertEquals`` →
- `test_java_external_static_import_not_stdlib(tmp_path: Path)` — [`L421`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L421) — ``substring(s, 1)`` with ``import static
- `test_java_interface_method_stays_unknown(tmp_path: Path)` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L236) — Review P1 regression lock: ``flux.stream()`` must stay UNKNOWN, never
- `test_java_optional_method_classifies_as_stdlib(tmp_path: Path)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L90) — ``opt.orElseThrow()`` with no project ``orElseThrow`` → stdlib. Covers the
- `test_java_production_verify_stays_unknown(tmp_path: Path)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L270) — Review P1 regression lock: ``signature.verify(sig)`` must stay UNKNOWN,
- `test_java_project_fqn_receiver_wins_over_imported_tail(tmp_path: Path)` — [`L451`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L451) — An explicit project FQN receiver must resolve PROJECT even when its simple
- `test_java_project_method_shadows_external_name(tmp_path: Path)` — [`L332`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L332) — A Java class defining ``assertEquals`` → ``c.assertEquals()`` resolves
- `test_java_project_method_shadows_stdlib_name(tmp_path: Path)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L115) — A Java class defining ``substring`` → ``box.substring()`` resolves
- `test_java_stdlib_method_classifies_as_stdlib(tmp_path: Path)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_java_method_resolution.py#L62) — ``s.substring(1)`` with no project ``substring`` → stdlib, not unknown.

