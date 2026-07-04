---
title: 'Module: graphify/extractors/csharp.py'
type: catalog
provenance: extracted
module: graphify/extractors/csharp.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.extractors.csharp`/_
symbols:
  _resolve_csharp_type_references: resolve_csharp_type_references().
  _resolve_csharp_type_references._scopes_for: resolve_csharp_type_references()._scopes_for().
  _resolve_cross_file_csharp_imports: resolve_cross_file_csharp_imports().
  _resolve_csharp_type_references._resolve_alias: resolve_csharp_type_references()._resolve_alias().
  _resolve_csharp_type_references._resolve_label: resolve_csharp_type_references()._resolve_label().
  _resolve_csharp_type_references._resolve_qualified: resolve_csharp_type_references()._resolve_qualified().
  _resolve_csharp_type_references._dangling_stub_id: resolve_csharp_type_references()._dangling_stub_id().
  _resolve_csharp_type_references._using_in_scope: resolve_csharp_type_references()._using_in_scope().
  _resolve_csharp_type_references._metadata: resolve_csharp_type_references()._metadata().
  _resolve_csharp_type_references._namespace: resolve_csharp_type_references()._namespace().
  _resolve_csharp_type_references._scope_chain: resolve_csharp_type_references()._scope_chain().
  _resolve_csharp_type_references._is_csharp_relevant_target: resolve_csharp_type_references()._is_csharp_relevant_target().
  _resolve_csharp_type_references._label_for_type_ref_target: resolve_csharp_type_references()._label_for_type_ref_target().
  _strip_trailing_csharp_generic_args: strip_trailing_csharp_generic_args().
  _resolve_csharp_type_references._is_cs_file: resolve_csharp_type_references()._is_cs_file().
  _resolve_csharp_type_references._append_unique: resolve_csharp_type_references()._append_unique().
  _resolve_csharp_type_references._is_placeholder: resolve_csharp_type_references()._is_placeholder().
  _build_csharp_type_def_index: build_csharp_type_def_index().
---
# Module: [`graphify/extractors/csharp.py`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py)

## Functions
- `_append_unique(items: list[str], value: str)` — [`L178`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L178)
- `_build_csharp_type_def_index(all_nodes: list[dict])` — [`L19`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L19) — Return deterministic ``(namespace, name) -> node_id`` C# type definitions.
- `_dangling_stub_id(label: str, current_target: object)` — [`L321`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L321)
- `_is_cs_file(value: object)` — [`L167`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L167)
- `_is_csharp_relevant_target(node: dict)` — [`L302`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L302)
- `_is_placeholder(node: dict | None)` — [`L299`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L299)
- `_label_for_type_ref_target(target_node: dict, source_file: str)` — [`L308`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L308)
- `_metadata(value: object)` — [`L170`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L170)
- `_namespace(node: dict | None)` — [`L173`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L173)
- `_resolve_alias(label: str, source_node: dict, source_file: str)` — [`L250`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L250)
- `_resolve_cross_file_csharp_imports(per_file: list[dict], paths: list[Path], all_nodes: list[dict], all_edges: list[dict])` — [`L77`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L77) — Re-point resolvable C# ``using`` import edges to canonical internal nodes.
- `_resolve_csharp_type_references(per_file: list[dict], paths: list[Path], all_nodes: list[dict], all_edges: list[dict])` — [`L152`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L152) — Arbitrate all C# ``inherits``/``implements``/``references`` targets. — documented in [graphify-extract](../../../concepts/graphify-extract.md)
- `_resolve_label(label: str, source_node: dict, source_file: str)` — [`L267`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L267)
- `_resolve_qualified(label: str, qualifier: object, source_node: dict, source_file: str)` — [`L277`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L277)
- `_scope_chain(node: dict)` — [`L232`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L232)
- `_scopes_for(source_node: dict, source_file: str)` — [`L241`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L241)
- `_strip_trailing_csharp_generic_args(target_fqn: str)` — [`L61`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L61)
- `_using_in_scope(scope_kind: str, scope_id: str | None, source_node: dict)` — [`L236`](../../../../../../raw/code/graphify/graphify/extractors/csharp.py#L236)

