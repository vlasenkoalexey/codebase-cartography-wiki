---
title: 'Module: tests/unit/test_stdlib_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_stdlib_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_stdlib_method_resolution`/
symbols:
  test_prebuilt_context_without_file_languages_keeps_python_tiers: test_prebuilt_context_without_file_languages_keeps_python_tiers().
  _index: _index().
  test_lazy_context_construction_fires_stdlib_method: test_lazy_context_construction_fires_stdlib_method().
  _resolution_for: _resolution_for().
  test_stdlib_method_name_classifies_as_stdlib: test_stdlib_method_name_classifies_as_stdlib().
  test_project_method_shadows_stdlib_name: test_project_method_shadows_stdlib_name().
  test_ambiguous_project_method_stays_unknown: test_ambiguous_project_method_stays_unknown().
  test_cross_language_symbol_does_not_suppress_stdlib: test_cross_language_symbol_does_not_suppress_stdlib().
  test_genuinely_unknown_name_stays_unknown: test_genuinely_unknown_name_stays_unknown().
---
# Module: [`tests/unit/test_stdlib_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_stdlib_method_resolution.py)

## Functions
- `_index(tmp_path: Path, files: dict[str, str])` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_stdlib_method_resolution.py#L17)
- `_resolution_for(db_path: str, callee_name: str)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_stdlib_method_resolution.py#L31)
- `test_ambiguous_project_method_stays_unknown(tmp_path: Path)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_stdlib_method_resolution.py#L93) — Two classes define ``get`` → an unqualifiable ``get()`` stays unknown,
- `test_cross_language_symbol_does_not_suppress_stdlib(tmp_path: Path)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_stdlib_method_resolution.py#L120) — Codex P2 #319: a JS file defining ``split`` must NOT make a Python
- `test_genuinely_unknown_name_stays_unknown(tmp_path: Path)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_stdlib_method_resolution.py#L158) — A name that is neither project nor stdlib stays unknown.
- `test_lazy_context_construction_fires_stdlib_method(tmp_path: Path)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_stdlib_method_resolution.py#L138) — Codex P2 #319: the public lazy form ResolverContext(project_root=, cache=)
- `test_prebuilt_context_without_file_languages_keeps_python_tiers()` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_stdlib_method_resolution.py#L170) — Codex P2 #326 regression lock: a pre-built ResolverContext constructed
- `test_project_method_shadows_stdlib_name(tmp_path: Path)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_stdlib_method_resolution.py#L69) — A project class defining ``split`` → ``split()`` resolves to project,
- `test_stdlib_method_name_classifies_as_stdlib(tmp_path: Path)` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_stdlib_method_resolution.py#L45) — ``p.write_text(...)`` with no project ``write_text`` → stdlib, not unknown.

