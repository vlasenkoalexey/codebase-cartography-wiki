---
title: 'Module: tests/test_incremental.py'
type: catalog
provenance: extracted
module: tests/test_incremental.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_incremental`/
symbols:
  _run: _run().
  test_manifest_written_after_extract: test_manifest_written_after_extract().
  test_incremental_mode_detected_via_manifest: test_incremental_mode_detected_via_manifest().
  test_no_incremental_without_manifest: test_no_incremental_without_manifest().
  test_update_prunes_a_removed_imports_edge: test_update_prunes_a_removed_imports_edge().
  _make_docs_corpus: _make_docs_corpus().
  test_extract_no_cluster_incremental_noop_preserves_existing_graph: test_extract_no_cluster_incremental_noop_preserves_existing_graph().
  _edges: _edges().
  PYTHON: PYTHON.
  _LLM_ENV_KEYS: _LLM_ENV_KEYS.
---
# Module: [`tests/test_incremental.py`](../../../../../raw/code/graphify/tests/test_incremental.py)

## Functions
- `_edges(graph_json: Path)` — [`L101`](../../../../../raw/code/graphify/tests/test_incremental.py#L101)
- `_make_docs_corpus(tmp_path: Path)` — [`L35`](../../../../../raw/code/graphify/tests/test_incremental.py#L35)
- `_run(args: list[str], cwd: Path)` — [`L24`](../../../../../raw/code/graphify/tests/test_incremental.py#L24)
- `test_extract_no_cluster_incremental_noop_preserves_existing_graph(tmp_path)` — [`L77`](../../../../../raw/code/graphify/tests/test_incremental.py#L77) — #1347: no-op incremental no-cluster extract must not overwrite graph.json.
- `test_incremental_mode_detected_via_manifest(tmp_path)` — [`L54`](../../../../../raw/code/graphify/tests/test_incremental.py#L54) — If manifest.json + graph.json exist, incremental mode message is shown.
- `test_manifest_written_after_extract(tmp_path)` — [`L43`](../../../../../raw/code/graphify/tests/test_incremental.py#L43) — After a full extract run, manifest.json must exist (or run fails before writing it).
- `test_no_incremental_without_manifest(tmp_path)` — [`L66`](../../../../../raw/code/graphify/tests/test_incremental.py#L66) — Without manifest.json, full scan message is shown (not incremental).
- `test_update_prunes_a_removed_imports_edge(tmp_path)` — [`L106`](../../../../../raw/code/graphify/tests/test_incremental.py#L106) — #1521: when an import is deleted from a file, `graphify update` must prune

## Module values
- `PYTHON` — [`L11`](../../../../../raw/code/graphify/tests/test_incremental.py#L11)
- `_LLM_ENV_KEYS` — [`L17`](../../../../../raw/code/graphify/tests/test_incremental.py#L17)

