---
title: 'Module: graphify/multigraph_compat.py'
type: catalog
provenance: extracted
module: graphify/multigraph_compat.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.multigraph_compat`/
symbols:
  probe_multigraph_capabilities: probe_multigraph_capabilities().
  MultigraphCapabilityResult.error_message: MultigraphCapabilityResult#error_message().
  require_multigraph_capabilities: require_multigraph_capabilities().
  CapabilityCheck: CapabilityCheck#
  MultigraphCapabilityResult.ok: MultigraphCapabilityResult#ok().
  MultigraphCapabilityResult.failed: MultigraphCapabilityResult#failed().
  _check: _check().
  MultigraphCapabilityResult.checks: MultigraphCapabilityResult#checks.
  MultigraphCapabilityResult: MultigraphCapabilityResult#
  MultigraphCapabilityResult.python_version: MultigraphCapabilityResult#python_version.
  MultigraphCapabilityResult.networkx_version: MultigraphCapabilityResult#networkx_version.
  _probe_keyed_parallel_edges: _probe_keyed_parallel_edges().
  _probe_node_link_round_trip: _probe_node_link_round_trip().
  _probe_to_undirected_preserves_multigraph_type: _probe_to_undirected_preserves_multigraph_type().
  _build_probe_graph: _build_probe_graph().
  CapabilityCheck.name: CapabilityCheck#name.
  CapabilityCheck.ok: CapabilityCheck#ok.
  CapabilityCheck.detail: CapabilityCheck#detail.
  _probe_duplicate_key_overwrite_semantics: _probe_duplicate_key_overwrite_semantics().
  _probe_reserved_key_attr_rejected: _probe_reserved_key_attr_rejected().
  _probe_remove_edges_from_two_tuple_semantics: _probe_remove_edges_from_two_tuple_semantics().
---
# Module: [`graphify/multigraph_compat.py`](../../../../../raw/code/graphify/graphify/multigraph_compat.py)

## Classes
### `CapabilityCheck`
- def: [`graphify/multigraph_compat.py:25`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L25) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- signature: `class CapabilityCheck:`
- members:
  - `detail` — [`L28`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L28) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
  - `name` — [`L26`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L26) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
  - `ok` — [`L27`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L27) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- used by: [`error_message`](multigraph_compat.md#MultigraphCapabilityResult.error_message), [`ok`](multigraph_compat.md#MultigraphCapabilityResult.ok), [`_check`](multigraph_compat.md#_check), [`failed`](multigraph_compat.md#MultigraphCapabilityResult.failed), [`checks`](multigraph_compat.md#MultigraphCapabilityResult.checks)  (2 test-only)

### `MultigraphCapabilityResult`
- def: [`graphify/multigraph_compat.py:32`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L32) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- signature: `class MultigraphCapabilityResult:`
- members:
  - `error_message(self)` — [`L45`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L45) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
  - `failed(self)` — [`L42`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L42) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
  - `ok(self)` — [`L38`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L38) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
  - `checks` — [`L35`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L35) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
  - `networkx_version` — [`L34`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L34) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
  - `python_version` — [`L33`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L33) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- uses (calls/refs, reference-scoped): [`CapabilityCheck`](multigraph_compat.md#CapabilityCheck), [`name`](multigraph_compat.md#CapabilityCheck.name), [`ok`](multigraph_compat.md#CapabilityCheck.ok), [`detail`](multigraph_compat.md#CapabilityCheck.detail)
- used by: [`probe_multigraph_capabilities`](multigraph_compat.md#probe_multigraph_capabilities), [`require_multigraph_capabilities`](multigraph_compat.md#require_multigraph_capabilities)  (3 test-only)

## Functions
- `_build_probe_graph()` — [`L73`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L73) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- `_check(name: str, func: Callable[[], bool | str])` — [`L61`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L61) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- `_probe_duplicate_key_overwrite_semantics()` — [`L126`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L126) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- `_probe_keyed_parallel_edges()` — [`L82`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L82) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- `_probe_node_link_round_trip()` — [`L95`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L95) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- `_probe_remove_edges_from_two_tuple_semantics()` — [`L161`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L161) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- `_probe_reserved_key_attr_rejected()` — [`L138`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L138) — Verify the Python language guarantee that NetworkX add_edge inherits. — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- `_probe_to_undirected_preserves_multigraph_type()` — [`L172`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L172) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- `probe_multigraph_capabilities()` — [`L184`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L184) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)
- `require_multigraph_capabilities()` — [`L208`](../../../../../raw/code/graphify/graphify/multigraph_compat.py#L208) — documented in [graphify-multigraph_compat](../../concepts/graphify-multigraph_compat.md)

