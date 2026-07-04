---
title: 'Module: graphify/scip_ingest.py'
type: catalog
provenance: extracted
module: graphify/scip_ingest.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.scip_ingest`/
symbols:
  ingest_scip_json: ingest_scip_json().
  _emit_relationships: _emit_relationships().
  _emit_symbol_node: _emit_symbol_node().
  _make_scip_node_id: _make_scip_node_id().
  _scip_kind_to_file_type: _scip_kind_to_file_type().
  _coerce_str: _coerce_str().
  _build_scip_metadata: _build_scip_metadata().
  _scip_relation_for: _scip_relation_for().
  _is_true: _is_true().
  _first_occurrence_line: _first_occurrence_line().
  _resolve_relationship_target: _resolve_relationship_target().
---
# Module: [`graphify/scip_ingest.py`](../../../../../raw/code/graphify/graphify/scip_ingest.py)

## Functions
- `_build_scip_metadata(symbol_id: str, kind: str, description: str)` — [`L355`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L355) — Build metadata for a SCIP node. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `_coerce_str(value: object, default: str)` — [`L321`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L321) — Return ``value`` if it is a string, else the ``default`` (also a string). — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `_emit_relationships(record: dict[str, Any], per_doc_index: dict[tuple[str, str], str], global_index: dict[str, list[str]], nodes: list[dict[str, Any]], edges: list[dict[str, Any]], seen_node_ids: set[str], seen_edges: set[tuple[str, str, str, str | None]])` — [`L169`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L169) — Append edges (and stub nodes when needed) for a symbol's relationships. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `_emit_symbol_node(record: dict[str, Any], nodes: list[dict[str, Any]], seen_node_ids: set[str])` — [`L132`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L132) — Append the canonical node for a SCIP symbol record. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `_first_occurrence_line(occurrences: object)` — [`L300`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L300) — Read the 1-based line number from the first occurrence range, defensively.
- `_is_true(value: object)` — [`L276`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L276) — Return True only when value is exactly the boolean True.
- `_make_scip_node_id(symbol: str, source_file: str)` — [`L330`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L330) — Derive a stable Graphify node ID from a SCIP symbol identifier. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `_resolve_relationship_target(target_symbol: str, source_doc_path: str, per_doc_index: dict[tuple[str, str], str], global_index: dict[str, list[str]])` — [`L251`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L251) — Resolve a SCIP relationship target to an emitted node id, or None.
- `_scip_kind_to_file_type(kind: str)` — [`L347`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L347) — Map SCIP symbol kind to a Graphify file_type. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `_scip_relation_for(rel: dict[str, Any])` — [`L285`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L285) — Pick the Graphify relation tag for a SCIP relationship dict. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `ingest_scip_json(doc: object, source_file: str = "", language: str = "python")` — [`L42`](../../../../../raw/code/graphify/graphify/scip_ingest.py#L42) — Convert a SCIP-style JSON document into Graphify nodes and edges. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)

