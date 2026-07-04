---
title: 'Module: tests/test_swift_cross_file_calls.py'
type: catalog
provenance: extracted
module: tests/test_swift_cross_file_calls.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_swift_cross_file_calls`/
symbols:
  _write: _write().
  test_swift_cross_file_member_calls_have_correct_confidence_and_resolve: test_swift_cross_file_member_calls_have_correct_confidence_and_resolve().
  test_swift_cross_file_member_calls_resolve: test_swift_cross_file_member_calls_resolve().
  test_swift_unknown_receiver_emits_no_edge: test_swift_unknown_receiver_emits_no_edge().
  test_deferred_singleton_local_var_resolves: test_deferred_singleton_local_var_resolves().
  _edge_labels: _edge_labels().
  test_swift_ambiguous_type_does_not_over_connect: test_swift_ambiguous_type_does_not_over_connect().
  _issue_fixture: _issue_fixture().
  _label: _label().
---
# Module: [`tests/test_swift_cross_file_calls.py`](../../../../../raw/code/graphify/tests/test_swift_cross_file_calls.py)

## Functions
- `_edge_labels(result: dict, relations=("calls", "references"))` — [`L22`](../../../../../raw/code/graphify/tests/test_swift_cross_file_calls.py#L22) — Return {(source_label, relation, target_label)} for the given relations.
- `_issue_fixture(base: Path)` — [`L31`](../../../../../raw/code/graphify/tests/test_swift_cross_file_calls.py#L31) — The three cross-file patterns from #1356, plus a constructor-in-initializer.
- `_label(result: dict, nid: str)` — [`L15`](../../../../../raw/code/graphify/tests/test_swift_cross_file_calls.py#L15)
- `_write(path: Path, text: str)` — [`L9`](../../../../../raw/code/graphify/tests/test_swift_cross_file_calls.py#L9)
- `test_deferred_singleton_local_var_resolves(tmp_path)` — [`L157`](../../../../../raw/code/graphify/tests/test_swift_cross_file_calls.py#L157) — #1604: `let x = Type.shared` cached into a local var, then `x.method()` on a
- `test_swift_ambiguous_type_does_not_over_connect(tmp_path: Path)` — [`L113`](../../../../../raw/code/graphify/tests/test_swift_cross_file_calls.py#L113)
- `test_swift_cross_file_member_calls_have_correct_confidence_and_resolve(tmp_path: Path)` — [`L73`](../../../../../raw/code/graphify/tests/test_swift_cross_file_calls.py#L73)
- `test_swift_cross_file_member_calls_resolve(tmp_path: Path)` — [`L56`](../../../../../raw/code/graphify/tests/test_swift_cross_file_calls.py#L56)
- `test_swift_unknown_receiver_emits_no_edge(tmp_path: Path)` — [`L139`](../../../../../raw/code/graphify/tests/test_swift_cross_file_calls.py#L139)

