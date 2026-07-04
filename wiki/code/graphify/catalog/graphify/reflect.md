---
title: 'Module: graphify/reflect.py'
type: catalog
provenance: extracted
module: graphify/reflect.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.reflect`/
symbols:
  aggregate_lessons: aggregate_lessons().
  reflect: reflect().
  load_learning_overlay: load_learning_overlay().
  render_lessons_md: render_lessons_md().
  parse_memory_doc: parse_memory_doc().
  load_memory_docs: load_memory_docs().
  build_learning_overlay._add: build_learning_overlay()._add().
  build_learning_overlay: build_learning_overlay().
  LEARNING_SIDECAR_NAME: LEARNING_SIDECAR_NAME.
  lessons_fresh: lessons_fresh().
  write_learning_sidecar: write_learning_sidecar().
  _code_fingerprint: _code_fingerprint().
  _is_stale: _is_stale().
  _empty_bucket: _empty_bucket().
  _finalize_sources: _finalize_sources().
  _resolve_source_path: _resolve_source_path().
  _dedupe_by_question: _dedupe_by_question().
  _doc_community: _doc_community().
  _decay: _decay().
  render_lessons_md._topic_key: render_lessons_md()._topic_key().
  _provenance_for: _provenance_for().
  _UNCATEGORIZED: _UNCATEGORIZED.
  _DEFAULT_MIN_CORROBORATION: _DEFAULT_MIN_CORROBORATION.
  _DEFAULT_HALF_LIFE_DAYS: _DEFAULT_HALF_LIFE_DAYS.
  _yaml_unescape: _yaml_unescape().
  _render_bucket: _render_bucket().
  _content_hash: _content_hash().
  _LEARNING_SCHEMA_VERSION: _LEARNING_SCHEMA_VERSION.
  _PROVENANCE_CAP: _PROVENANCE_CAP.
  _SCORE_NDIGITS: _SCORE_NDIGITS.
  _SCALAR_RE: _SCALAR_RE.
  _LIST_RE: _LIST_RE.
  _DQ_ITEM_RE: _DQ_ITEM_RE.
  _load_node_community: _load_node_community().
  _load_known_nodes: _load_known_nodes().
  _parse_dt: _parse_dt().
  _record_node: _record_node().
  _build_id_label_maps: _build_id_label_maps().
  _resolve_canonical_id: _resolve_canonical_id().
---
# Module: [`graphify/reflect.py`](../../../../../raw/code/graphify/graphify/reflect.py)

## Functions
- `_add(entry_src: dict[str, Any], status: str)` — [`L781`](../../../../../raw/code/graphify/graphify/reflect.py#L781) — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `_build_id_label_maps(graph_path: Path)` — [`L622`](../../../../../raw/code/graphify/graphify/reflect.py#L622) — From graph.json build:
- `_code_fingerprint(node: dict[str, Any] | None, graph_path: Path)` — [`L728`](../../../../../raw/code/graphify/graphify/reflect.py#L728) — Content hash of the node's ``source_file``, or '' if unavailable.
- `_content_hash(path: Path)` — [`L717`](../../../../../raw/code/graphify/graphify/reflect.py#L717) — SHA256 of file CONTENT only (no path mixed in), so the fingerprint is
- `_decay(date_str: str, now: datetime, half_life_days: float)` — [`L275`](../../../../../raw/code/graphify/graphify/reflect.py#L275) — Time-decay weight in (0, 1]: halves every ``half_life_days``. — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `_dedupe_by_question(items: list[dict[str, Any]])` — [`L350`](../../../../../raw/code/graphify/graphify/reflect.py#L350) — Collapse repeated questions to one entry. Docs are processed oldest-first, so — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `_doc_community(nodes: list[str], node_community: dict[str, str] | None)` — [`L240`](../../../../../raw/code/graphify/graphify/reflect.py#L240) — The community a doc belongs to: the plurality community of its source nodes. — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `_empty_bucket()` — [`L291`](../../../../../raw/code/graphify/graphify/reflect.py#L291) — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `_finalize_sources(bucket: dict[str, Any], min_corroboration: int)` — [`L327`](../../../../../raw/code/graphify/graphify/reflect.py#L327) — Split a bucket's scored nodes into preferred / tentative / contested lists. — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `_is_stale(entry: dict[str, Any], graph_path: Path)` — [`L868`](../../../../../raw/code/graphify/graphify/reflect.py#L868) — True if the node's source file changed (or vanished) since the fingerprint — documented in [graphify-export](../../concepts/graphify-export.md)
- `_load_known_nodes(graph_path: Path)` — [`L211`](../../../../../raw/code/graphify/graphify/reflect.py#L211) — The set of node ids AND labels in the current graph, or None if unavailable.
- `_load_node_community(graph_path: Path, analysis_path: Path, labels_path: Path)` — [`L162`](../../../../../raw/code/graphify/graphify/reflect.py#L162) — Build a lookup from node id AND node label -> community label, or None if the
- `_parse_dt(date_str: str)` — [`L262`](../../../../../raw/code/graphify/graphify/reflect.py#L262) — Parse an ISO date/datetime to an aware UTC datetime, or None if unparseable.
- `_provenance_for(node: str, prov_map: dict[str, list], fallback_outcome: str)` — [`L741`](../../../../../raw/code/graphify/graphify/reflect.py#L741) — Most-recent-first, capped provenance entries for a node.
- `_record_node(bucket: dict[str, Any], node: str, sign: int, weight: float, date: str, *, outcome: str | None = None, question: str = "")` — [`L310`](../../../../../raw/code/graphify/graphify/reflect.py#L310)
- `_render_bucket(out: list[str], data: dict[str, Any], k: int)` — [`L444`](../../../../../raw/code/graphify/graphify/reflect.py#L444)
- `_resolve_canonical_id(cited: str, id_set: dict[str, str], label_to_ids: dict[str, list[str]])` — [`L652`](../../../../../raw/code/graphify/graphify/reflect.py#L652) — Resolve a cited node (a label OR an id) to a single canonical node id.
- `_resolve_source_path(src: str, graph_path: Path)` — [`L668`](../../../../../raw/code/graphify/graphify/reflect.py#L668) — Locate a node's ``source_file`` on disk, returning an existing file or None.
- `_topic_key(label: str)` — [`L514`](../../../../../raw/code/graphify/graphify/reflect.py#L514) — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `_yaml_unescape(s: str)` — [`L71`](../../../../../raw/code/graphify/graphify/reflect.py#L71) — Reverse the double-quoted escaping that ingest._yaml_str applies.
- `aggregate_lessons(docs: list[dict[str, Any]], node_community: dict[str, str] | None = None, *, now: datetime | None = None, half_life_days: float = _DEFAULT_HALF_LIFE_DAYS, min_corroboration: int = _DEFAULT_MIN_CORROBORATION, known_nodes: set[str] | None = None)` — [`L364`](../../../../../raw/code/graphify/graphify/reflect.py#L364) — Aggregate parsed memory docs into a deterministic lessons structure. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `build_learning_overlay(agg: dict[str, Any], graph_path: Path, *, now: datetime | None = None)` — [`L758`](../../../../../raw/code/graphify/graphify/reflect.py#L758) — Project the reflect aggregate into the sidecar's ``{version, generated_at, — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `lessons_fresh(out_path: Path, memory_dir: Path, graph_path: Path | None = None, analysis_path: Path | None = None, labels_path: Path | None = None)` — [`L527`](../../../../../raw/code/graphify/graphify/reflect.py#L527) — True if ``out_path`` exists and is at least as new as every input that
- `load_learning_overlay(graph_path: Path)` — [`L840`](../../../../../raw/code/graphify/graphify/reflect.py#L840) — Load the sidecar next to ``graph_path`` and return ``{node_id -> entry}`` — documented in [graphify-export](../../concepts/graphify-export.md)
- `load_memory_docs(memory_dir: Path)` — [`L133`](../../../../../raw/code/graphify/graphify/reflect.py#L133) — Parse every memory doc under ``memory_dir``, sorted by date then filename. — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `parse_memory_doc(text: str)` — [`L104`](../../../../../raw/code/graphify/graphify/reflect.py#L104) — Parse the frontmatter of a memory doc into a dict, or None if it has none. — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `reflect(memory_dir: Path, out_path: Path, graph_path: Path | None = None, analysis_path: Path | None = None, labels_path: Path | None = None, *, now: datetime | None = None, half_life_days: float = _DEFAULT_HALF_LIFE_DAYS, min_corroboration: int = _DEFAULT_MIN_CORROBORATION)` — [`L564`](../../../../../raw/code/graphify/graphify/reflect.py#L564) — Scan ``memory_dir``, write the lessons doc to ``out_path``, return (path, agg). — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `render_lessons_md(agg: dict[str, Any])` — [`L489`](../../../../../raw/code/graphify/graphify/reflect.py#L489) — Render the aggregate into the deterministic LESSONS.md markdown body. — documented in [graphify-reflect](../../concepts/graphify-reflect.md)
- `write_learning_sidecar(agg: dict[str, Any], graph_path: Path, *, now: datetime | None = None)` — [`L824`](../../../../../raw/code/graphify/graphify/reflect.py#L824) — Write ``.graphify_learning.json`` next to ``graph_path`` deterministically. — documented in [graphify-reflect](../../concepts/graphify-reflect.md)

## Module values
- `LEARNING_SIDECAR_NAME` — [`L46`](../../../../../raw/code/graphify/graphify/reflect.py#L46) — documented in [graphify-export](../../concepts/graphify-export.md)
- `_DEFAULT_HALF_LIFE_DAYS` — [`L51`](../../../../../raw/code/graphify/graphify/reflect.py#L51)
- `_DEFAULT_MIN_CORROBORATION` — [`L52`](../../../../../raw/code/graphify/graphify/reflect.py#L52)
- `_DQ_ITEM_RE` — [`L68`](../../../../../raw/code/graphify/graphify/reflect.py#L68)
- `_LEARNING_SCHEMA_VERSION` — [`L47`](../../../../../raw/code/graphify/graphify/reflect.py#L47)
- `_LIST_RE` — [`L67`](../../../../../raw/code/graphify/graphify/reflect.py#L67)
- `_PROVENANCE_CAP` — [`L48`](../../../../../raw/code/graphify/graphify/reflect.py#L48)
- `_SCALAR_RE` — [`L66`](../../../../../raw/code/graphify/graphify/reflect.py#L66)
- `_SCORE_NDIGITS` — [`L56`](../../../../../raw/code/graphify/graphify/reflect.py#L56)
- `_UNCATEGORIZED` — [`L40`](../../../../../raw/code/graphify/graphify/reflect.py#L40)

