---
title: 'Module: tests/test_ruby_resolution.py'
type: catalog
provenance: extracted
module: tests/test_ruby_resolution.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_ruby_resolution`/
symbols:
  _write: _write().
  test_resolution_is_type_based_not_name_luck: test_resolution_is_type_based_not_name_luck().
  test_resolves_member_call_by_type: test_resolves_member_call_by_type().
  test_class_new_creates_instantiation_edge: test_class_new_creates_instantiation_edge().
  _has_call_edge: _has_call_edge().
  test_member_call_captures_receiver: test_member_call_captures_receiver().
  test_local_binding_gives_receiver_a_type: test_local_binding_gives_receiver_a_type().
  test_no_false_positive_when_type_unknown: test_no_false_positive_when_type_unknown().
  test_plain_module_gets_a_node_with_methods: test_plain_module_gets_a_node_with_methods().
  test_nested_modules_each_get_a_node: test_nested_modules_each_get_a_node().
  test_struct_new_constant_creates_class_with_methods: test_struct_new_constant_creates_class_with_methods().
  test_class_new_constant_creates_class_and_inherits: test_class_new_constant_creates_class_and_inherits().
  test_ambiguous_binding_yields_no_type: test_ambiguous_binding_yields_no_type().
  test_data_define_constant_creates_class: test_data_define_constant_creates_class().
  test_constant_receiver_singleton_call_resolves: test_constant_receiver_singleton_call_resolves().
  test_constant_receiver_module_function_call_resolves: test_constant_receiver_module_function_call_resolves().
  test_constant_receiver_unknown_class_method_falls_back_to_class: test_constant_receiver_unknown_class_method_falls_back_to_class().
  test_ambiguous_constant_receiver_emits_no_edge: test_ambiguous_constant_receiver_emits_no_edge().
  _find_raw_call: _find_raw_call().
  _method_edges: _method_edges().
  MAIN_RB: MAIN_RB.
  _node_labels: _node_labels().
  _labels: _labels().
  HELPER_RB: HELPER_RB.
  _raw_calls: _raw_calls().
  WORKER_RB: WORKER_RB.
---
# Module: [`tests/test_ruby_resolution.py`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py)

## Functions
- `_find_raw_call(result: dict, callee: str)` — [`L35`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L35)
- `_has_call_edge(graph: dict, src_label_sub: str, tgt_label_sub: str)` — [`L46`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L46) — Return the `calls` edge whose source/target labels contain the given
- `_labels(nodes: list[dict])` — [`L42`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L42)
- `_method_edges(result: dict)` — [`L205`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L205)
- `_node_labels(result: dict)` — [`L201`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L201)
- `_raw_calls(result: dict)` — [`L31`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L31)
- `_write(tmp_path: Path, name: str, body: str)` — [`L25`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L25)
- `test_ambiguous_binding_yields_no_type(tmp_path: Path)` — [`L113`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L113)
- `test_ambiguous_constant_receiver_emits_no_edge(tmp_path: Path)` — [`L285`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L285) — Two classes named `Processor` => ambiguous receiver => bail (no wrong edge).
- `test_class_new_constant_creates_class_and_inherits(tmp_path: Path)` — [`L239`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L239) — #1640 shape 3: `Foo = Class.new(Super)` — node + inherits edge.
- `test_class_new_creates_instantiation_edge(tmp_path: Path)` — [`L188`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L188) — `p = Processor.new` should link the caller to the Processor class.
- `test_constant_receiver_module_function_call_resolves(tmp_path: Path)` — [`L263`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L263) — #1634 + #1640: `TaxCalculator.rate_for` resolves across files to a
- `test_constant_receiver_singleton_call_resolves(tmp_path: Path)` — [`L254`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L254) — #1634: `Processor.call` (def self.call) resolves to the singleton method.
- `test_constant_receiver_unknown_class_method_falls_back_to_class(tmp_path: Path)` — [`L274`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L274) — #1634: `Model.where` (no `where` def, e.g. ActiveRecord) still links to the
- `test_data_define_constant_creates_class(tmp_path: Path)` — [`L249`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L249)
- `test_local_binding_gives_receiver_a_type(tmp_path: Path)` — [`L105`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L105)
- `test_member_call_captures_receiver(tmp_path: Path)` — [`L97`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L97)
- `test_nested_modules_each_get_a_node(tmp_path: Path)` — [`L222`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L222) — #1640 shape 1, nested.
- `test_no_false_positive_when_type_unknown(tmp_path: Path)` — [`L169`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L169) — A member call on a receiver with no known type must NOT be resolved.
- `test_plain_module_gets_a_node_with_methods(tmp_path: Path)` — [`L213`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L213) — #1640 shape 1: `module Foo` must get a node and own its methods.
- `test_resolution_is_type_based_not_name_luck(tmp_path: Path)` — [`L143`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L143) — The differentiator: adding an unrelated Worker#run must NOT break the edge.
- `test_resolves_member_call_by_type(tmp_path: Path)` — [`L134`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L134)
- `test_struct_new_constant_creates_class_with_methods(tmp_path: Path)` — [`L231`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L231) — #1640 shape 2: `Foo = Struct.new(...) do ... end`.

## Module values
- `HELPER_RB` — [`L60`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L60)
- `MAIN_RB` — [`L72`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L72)
- `WORKER_RB` — [`L85`](../../../../../raw/code/graphify/tests/test_ruby_resolution.py#L85)

