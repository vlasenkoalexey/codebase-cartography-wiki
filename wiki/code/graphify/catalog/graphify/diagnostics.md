---
title: 'Module: graphify/diagnostics.py'
type: catalog
provenance: extracted
module: graphify/diagnostics.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.diagnostics`/
symbols:
  diagnose_extraction: diagnose_extraction().
  diagnose_file: diagnose_file().
  scan_producer_suppression_sites: scan_producer_suppression_sites().
  _safe_text: _safe_text().
  _read_json_file: _read_json_file().
  format_diagnostic_report: format_diagnostic_report().
  _variant_group_count: _variant_group_count().
  format_diagnostic_json: format_diagnostic_json().
  _canonical_edge: _canonical_edge().
  _tuple_arity_from_annotation: _tuple_arity_from_annotation().
  _count_extra: _count_extra().
  _SUPPRESSION_DECL_RE: _SUPPRESSION_DECL_RE.
  _TYPE_TUPLE_RE: _TYPE_TUPLE_RE.
  _edge_list: _edge_list().
  _node_ids: _node_ids().
  _exact_signature: _exact_signature().
---
# Module: [`graphify/diagnostics.py`](../../../../../raw/code/graphify/graphify/diagnostics.py)

## Functions
- `_canonical_edge(edge: Any)` — [`L45`](../../../../../raw/code/graphify/graphify/diagnostics.py#L45)
- `_count_extra(counter: Counter[Any])` — [`L90`](../../../../../raw/code/graphify/graphify/diagnostics.py#L90)
- `_edge_list(extraction: dict[str, Any])` — [`L27`](../../../../../raw/code/graphify/graphify/diagnostics.py#L27)
- `_exact_signature(edge: Any)` — [`L71`](../../../../../raw/code/graphify/graphify/diagnostics.py#L71)
- `_node_ids(extraction: dict[str, Any])` — [`L34`](../../../../../raw/code/graphify/graphify/diagnostics.py#L34)
- `_read_json_file(path: str | Path)` — [`L271`](../../../../../raw/code/graphify/graphify/diagnostics.py#L271) — Read a JSON graph after applying Graphify's graph-load size cap. — documented in [graphify-security](../../concepts/graphify-security.md)
- `_safe_text(value: Any)` — [`L19`](../../../../../raw/code/graphify/graphify/diagnostics.py#L19)
- `_tuple_arity_from_annotation(line: str)` — [`L112`](../../../../../raw/code/graphify/graphify/diagnostics.py#L112)
- `_variant_group_count(grouped_edges: dict[tuple[str, str], list[dict[str, str]]], field: str, *, relation_sensitive: bool = False)` — [`L94`](../../../../../raw/code/graphify/graphify/diagnostics.py#L94)
- `diagnose_extraction(extraction: dict[str, Any], *, directed: bool = True, root: str | Path | None = None, max_examples: int = 5, extract_path: str | Path | None = None)` — [`L156`](../../../../../raw/code/graphify/graphify/diagnostics.py#L156) — Summarize same-endpoint edge-collapse risk for one JSON graph/extraction dict. — documented in [graphify-build](../../concepts/graphify-build.md)
- `diagnose_file(path: str | Path, *, directed: bool | None = None, root: str | Path | None = None, max_examples: int = 5, extract_path: str | Path | None = None)` — [`L289`](../../../../../raw/code/graphify/graphify/diagnostics.py#L289) — Diagnose a graph/extraction JSON file without mutating it.
- `format_diagnostic_json(summary: dict[str, Any])` — [`L321`](../../../../../raw/code/graphify/graphify/diagnostics.py#L321)
- `format_diagnostic_report(summary: dict[str, Any])` — [`L339`](../../../../../raw/code/graphify/graphify/diagnostics.py#L339)
- `scan_producer_suppression_sites(path: str | Path)` — [`L122`](../../../../../raw/code/graphify/graphify/diagnostics.py#L122) — Find likely `seen_*` producer-suppression sets in an extractor file.

## Module values
- `_SUPPRESSION_DECL_RE` — [`L15`](../../../../../raw/code/graphify/graphify/diagnostics.py#L15)
- `_TYPE_TUPLE_RE` — [`L16`](../../../../../raw/code/graphify/graphify/diagnostics.py#L16)

