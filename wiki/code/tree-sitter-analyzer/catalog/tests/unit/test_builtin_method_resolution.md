---
title: 'Module: tests/unit/test_builtin_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_builtin_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_builtin_method_resolution`/
symbols:
  _index: _index().
  test_lazy_context_construction_populates_builtin_methods: test_lazy_context_construction_populates_builtin_methods().
  _resolution_for: _resolution_for().
  test_monkeypatch_setattr_classifies_as_builtin: test_monkeypatch_setattr_classifies_as_builtin().
  test_getattr_with_qualifier_classifies_as_builtin: test_getattr_with_qualifier_classifies_as_builtin().
  test_project_method_named_setattr_shadows_builtin: test_project_method_named_setattr_shadows_builtin().
  test_ambiguous_project_setattr_stays_unknown_not_builtin: test_ambiguous_project_setattr_stays_unknown_not_builtin().
  test_cross_language_js_symbol_does_not_suppress_builtin_method: test_cross_language_js_symbol_does_not_suppress_builtin_method().
  test_js_caller_setattr_stays_unknown_not_python_builtin: test_js_caller_setattr_stays_unknown_not_python_builtin().
---
# Module: [`tests/unit/test_builtin_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_method_resolution.py)

## Functions
- `_index(tmp_path: Path, files: dict[str, str])` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_method_resolution.py#L25)
- `_resolution_for(db_path: str, callee_name: str)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_method_resolution.py#L39)
- `test_ambiguous_project_setattr_stays_unknown_not_builtin(tmp_path: Path)` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_method_resolution.py#L134) — Two project classes define ``setattr`` — ambiguous; stays unknown, not builtin.
- `test_cross_language_js_symbol_does_not_suppress_builtin_method(tmp_path: Path)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_method_resolution.py#L165) — A JS file defining ``setattr`` must NOT make a Python monkeypatch.setattr
- `test_getattr_with_qualifier_classifies_as_builtin(tmp_path: Path)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_method_resolution.py#L83) — ``obj.getattr(...)`` with no project def → builtin.
- `test_js_caller_setattr_stays_unknown_not_python_builtin(tmp_path: Path)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_method_resolution.py#L194) — A JavaScript caller using ``obj.setattr()`` must NOT be classified as
- `test_lazy_context_construction_populates_builtin_methods(tmp_path: Path)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_method_resolution.py#L225) — The public lazy ResolverContext(project_root=, cache=) must populate
- `test_monkeypatch_setattr_classifies_as_builtin(tmp_path: Path)` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_method_resolution.py#L53) — ``monkeypatch.setattr(obj, 'attr', val)`` with no project def → builtin.
- `test_project_method_named_setattr_shadows_builtin(tmp_path: Path)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_builtin_method_resolution.py#L105) — A project class defining ``setattr`` wins over the builtin_method table.

