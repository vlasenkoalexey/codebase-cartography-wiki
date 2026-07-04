---
title: 'Module: tests/test_rationale.py'
type: catalog
provenance: extracted
module: tests/test_rationale.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_rationale`/
symbols:
  _write_py: _write_py().
  test_decorated_method_node_id_is_class_qualified: test_decorated_method_node_id_is_class_qualified().
  test_module_docstring_extracted: test_module_docstring_extracted().
  test_function_docstring_extracted: test_function_docstring_extracted().
  test_class_docstring_extracted: test_class_docstring_extracted().
  test_rationale_comment_extracted: test_rationale_comment_extracted().
  test_rationale_for_edges_present: test_rationale_for_edges_present().
  test_short_docstring_ignored: test_short_docstring_ignored().
  test_rationale_confidence_is_extracted: test_rationale_confidence_is_extracted().
  test_alembic_module_docstring_suppressed: test_alembic_module_docstring_suppressed().
  test_alembic_function_docstrings_still_extracted: test_alembic_function_docstrings_still_extracted().
  test_non_migration_revision_var_not_suppressed: test_non_migration_revision_var_not_suppressed().
  test_django_migration_module_docstring_suppressed: test_django_migration_module_docstring_suppressed().
  test_generated_file_module_docstring_suppressed: test_generated_file_module_docstring_suppressed().
---
# Module: [`tests/test_rationale.py`](../../../../../raw/code/graphify/tests/test_rationale.py)

## Functions
- `_write_py(tmp_path: Path, code: str)` — [`L9`](../../../../../raw/code/graphify/tests/test_rationale.py#L9)
- `test_alembic_function_docstrings_still_extracted(tmp_path)` — [`L116`](../../../../../raw/code/graphify/tests/test_rationale.py#L116) — Function docstrings inside upgrade/downgrade should still be captured.
- `test_alembic_module_docstring_suppressed(tmp_path)` — [`L93`](../../../../../raw/code/graphify/tests/test_rationale.py#L93)
- `test_class_docstring_extracted(tmp_path)` — [`L37`](../../../../../raw/code/graphify/tests/test_rationale.py#L37)
- `test_decorated_method_node_id_is_class_qualified(tmp_path)` — [`L178`](../../../../../raw/code/graphify/tests/test_rationale.py#L178) — Regression for #1050: @property / @staticmethod / @classmethod methods
- `test_django_migration_module_docstring_suppressed(tmp_path)` — [`L151`](../../../../../raw/code/graphify/tests/test_rationale.py#L151)
- `test_function_docstring_extracted(tmp_path)` — [`L26`](../../../../../raw/code/graphify/tests/test_rationale.py#L26)
- `test_generated_file_module_docstring_suppressed(tmp_path)` — [`L165`](../../../../../raw/code/graphify/tests/test_rationale.py#L165)
- `test_module_docstring_extracted(tmp_path)` — [`L15`](../../../../../raw/code/graphify/tests/test_rationale.py#L15)
- `test_non_migration_revision_var_not_suppressed(tmp_path)` — [`L138`](../../../../../raw/code/graphify/tests/test_rationale.py#L138) — A file with a `revision` variable but no Alembic markers keeps its docstring.
- `test_rationale_comment_extracted(tmp_path)` — [`L48`](../../../../../raw/code/graphify/tests/test_rationale.py#L48)
- `test_rationale_confidence_is_extracted(tmp_path)` — [`L83`](../../../../../raw/code/graphify/tests/test_rationale.py#L83)
- `test_rationale_for_edges_present(tmp_path)` — [`L59`](../../../../../raw/code/graphify/tests/test_rationale.py#L59)
- `test_short_docstring_ignored(tmp_path)` — [`L71`](../../../../../raw/code/graphify/tests/test_rationale.py#L71) — Trivial docstrings under 20 chars should not become rationale nodes.

