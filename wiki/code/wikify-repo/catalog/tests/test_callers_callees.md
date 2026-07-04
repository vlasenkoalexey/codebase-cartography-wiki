---
title: 'Module: tests/test_callers_callees.py'
type: catalog
provenance: extracted
module: tests/test_callers_callees.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `tests.test_callers_callees`/
symbols:
  graph: graph().
  _one: _one().
  INDEX: INDEX.
  test_callees: test_callees().
  test_callers: test_callers().
  test_method_body_scoping: test_method_body_scoping().
  test_importance_rank: test_importance_rank().
  FIXTURE: FIXTURE.
  test_symbols_present: test_symbols_present().
---
# Module: [`tests/test_callers_callees.py`](../../../../../raw/code/wikify-repo/tests/test_callers_callees.py)

## Functions
- `_one(graph, name)` — [`L32`](../../../../../raw/code/wikify-repo/tests/test_callers_callees.py#L32) — Resolve the single in-repo moniker whose terminal descriptor is `name`.
- `graph(tmp_path_factory)` — [`L21`](../../../../../raw/code/wikify-repo/tests/test_callers_callees.py#L21)
- `test_callees(graph)` — [`L45`](../../../../../raw/code/wikify-repo/tests/test_callers_callees.py#L45)
- `test_callers(graph)` — [`L57`](../../../../../raw/code/wikify-repo/tests/test_callers_callees.py#L57)
- `test_importance_rank(graph)` — [`L75`](../../../../../raw/code/wikify-repo/tests/test_callers_callees.py#L75) — Importance = outbound*5 + ref_count*2; compute (2 callees) outranks add.
- `test_method_body_scoping(graph)` — [`L68`](../../../../../raw/code/wikify-repo/tests/test_callers_callees.py#L68) — A reference inside a method body must scope to the method, not the class.
- `test_symbols_present(graph)` — [`L40`](../../../../../raw/code/wikify-repo/tests/test_callers_callees.py#L40)

## Module values
- `FIXTURE` — [`L16`](../../../../../raw/code/wikify-repo/tests/test_callers_callees.py#L16)
- `INDEX` — [`L17`](../../../../../raw/code/wikify-repo/tests/test_callers_callees.py#L17)

