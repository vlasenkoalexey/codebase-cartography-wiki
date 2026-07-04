---
title: 'Module: tests/test_cpp_objc_cross_file_calls.py'
type: catalog
provenance: extracted
module: tests/test_cpp_objc_cross_file_calls.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_cpp_objc_cross_file_calls`/
symbols:
  _write: _write().
  _call_edges: _call_edges().
  test_cpp_instance_member_call_resolves: test_cpp_instance_member_call_resolves().
  test_cpp_pointer_member_call_resolves: test_cpp_pointer_member_call_resolves().
  test_cpp_qualified_member_call_is_extracted: test_cpp_qualified_member_call_is_extracted().
  test_cpp_this_member_call_resolves_to_enclosing_class: test_cpp_this_member_call_resolves_to_enclosing_class().
  test_cpp_godnode_guard_ambiguous_and_unknown_receiver: test_cpp_godnode_guard_ambiguous_and_unknown_receiver().
  test_cpp_resolved_call_survives_build: test_cpp_resolved_call_survives_build().
  test_cpp_unknown_receiver_emits_no_edge: test_cpp_unknown_receiver_emits_no_edge().
  test_objc_instance_message_send_resolves: test_objc_instance_message_send_resolves().
  test_objc_self_message_send_resolves_to_enclosing_class: test_objc_self_message_send_resolves_to_enclosing_class().
  test_objc_godnode_guard_ambiguous_selector: test_objc_godnode_guard_ambiguous_selector().
  test_objc_resolved_calls_survive_build: test_objc_resolved_calls_survive_build().
  _label: _label().
  test_cpp_cross_file_member_call_connects_with_relative_paths: test_cpp_cross_file_member_call_connects_with_relative_paths().
---
# Module: [`tests/test_cpp_objc_cross_file_calls.py`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py)

## Functions
- `_call_edges(result: dict, relations=("calls",))` — [`L29`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L29) — {(source_label, relation, target_label, confidence)} for the given relations.
- `_label(result: dict, nid: str)` — [`L22`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L22)
- `_write(path: Path, text: str)` — [`L16`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L16)
- `test_cpp_cross_file_member_call_connects_with_relative_paths(tmp_path)` — [`L45`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L45) — The headline #1547 fix: a paired class no longer islands — Main.cpp's use of
- `test_cpp_godnode_guard_ambiguous_and_unknown_receiver(tmp_path: Path)` — [`L143`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L143)
- `test_cpp_instance_member_call_resolves(tmp_path: Path)` — [`L91`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L91)
- `test_cpp_pointer_member_call_resolves(tmp_path: Path)` — [`L107`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L107)
- `test_cpp_qualified_member_call_is_extracted(tmp_path: Path)` — [`L119`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L119)
- `test_cpp_resolved_call_survives_build(tmp_path: Path)` — [`L167`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L167)
- `test_cpp_this_member_call_resolves_to_enclosing_class(tmp_path: Path)` — [`L131`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L131)
- `test_cpp_unknown_receiver_emits_no_edge(tmp_path: Path)` — [`L185`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L185)
- `test_objc_godnode_guard_ambiguous_selector(tmp_path: Path)` — [`L227`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L227)
- `test_objc_instance_message_send_resolves(tmp_path: Path)` — [`L199`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L199)
- `test_objc_resolved_calls_survive_build(tmp_path: Path)` — [`L247`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L247)
- `test_objc_self_message_send_resolves_to_enclosing_class(tmp_path: Path)` — [`L214`](../../../../../raw/code/graphify/tests/test_cpp_objc_cross_file_calls.py#L214)

