---
title: 'Module: tests/unit/test_external_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_external_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_external_method_resolution`/
symbols:
  _index: _index().
  test_lazy_context_construction_populates_external_methods: test_lazy_context_construction_populates_external_methods().
  _resolution_for: _resolution_for().
  test_mock_method_classifies_as_external: test_mock_method_classifies_as_external().
  test_pytest_raises_classifies_as_external: test_pytest_raises_classifies_as_external().
  test_project_method_shadows_external_name: test_project_method_shadows_external_name().
  test_ambiguous_project_method_stays_unknown_not_external: test_ambiguous_project_method_stays_unknown_not_external().
  test_cross_language_js_symbol_does_not_suppress_external: test_cross_language_js_symbol_does_not_suppress_external().
---
# Module: [`tests/unit/test_external_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_external_method_resolution.py)

## Functions
- `_index(tmp_path: Path, files: dict[str, str])` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_external_method_resolution.py#L24)
- `_resolution_for(db_path: str, callee_name: str)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_external_method_resolution.py#L38)
- `test_ambiguous_project_method_stays_unknown_not_external(tmp_path: Path)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_external_method_resolution.py#L130) — Two project classes define a name that also appears in the external table.
- `test_cross_language_js_symbol_does_not_suppress_external(tmp_path: Path)` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_external_method_resolution.py#L160) — A JS file defining ``readouterr`` must NOT make a Python pytest-capfd call
- `test_lazy_context_construction_populates_external_methods(tmp_path: Path)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_external_method_resolution.py#L189) — The public lazy ResolverContext(project_root=, cache=) must populate
- `test_mock_method_classifies_as_external(tmp_path: Path)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_external_method_resolution.py#L52) — ``obj.assert_called_once_with(...)`` with no project def → not unknown.
- `test_project_method_shadows_external_name(tmp_path: Path)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_external_method_resolution.py#L104) — A project class defining ``assert_called_once`` wins over the external table.
- `test_pytest_raises_classifies_as_external(tmp_path: Path)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_external_method_resolution.py#L85) — ``pytest.raises(...)`` bare name → external, not unknown.

