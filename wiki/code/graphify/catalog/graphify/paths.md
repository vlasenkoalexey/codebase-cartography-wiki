---
title: 'Module: graphify/paths.py'
type: catalog
provenance: extracted
module: graphify/paths.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.paths`/
symbols:
  GRAPHIFY_OUT: GRAPHIFY_OUT.
  disambiguate_ambiguous_candidates: disambiguate_ambiguous_candidates().
  default_graph_json: default_graph_json().
  GRAPHIFY_OUT_NAME: GRAPHIFY_OUT_NAME.
  _is_test_path: _is_test_path().
  out_path: out_path().
  _path_proximity_winner: _path_proximity_winner().
  _TEST_DIR_SEGMENTS: _TEST_DIR_SEGMENTS.
  _TEST_FILENAME_PATTERNS: _TEST_FILENAME_PATTERNS.
  _path_proximity_winner._common_prefix_len: _path_proximity_winner()._common_prefix_len().
---
# Module: [`graphify/paths.py`](../../../../../raw/code/graphify/graphify/paths.py)

## Functions
- `_common_prefix_len(f: str)` — [`L130`](../../../../../raw/code/graphify/graphify/paths.py#L130) — documented in [graphify-paths](../../concepts/graphify-paths.md)
- `_is_test_path(path: str)` — [`L55`](../../../../../raw/code/graphify/graphify/paths.py#L55) — Classify a source path as a test path (case-insensitive, segment-aware). — documented in [graphify-paths](../../concepts/graphify-paths.md)
- `_path_proximity_winner(call_site_file: str, candidate_files: dict[str, str])` — [`L91`](../../../../../raw/code/graphify/graphify/paths.py#L91) — Pick the candidate whose source file is closest to the call site. — documented in [graphify-paths](../../concepts/graphify-paths.md)
- `default_graph_json()` — [`L227`](../../../../../raw/code/graphify/graphify/paths.py#L227) — Default ``graph.json`` path under the configured output dir. — documented in [graphify-build](../../concepts/graphify-build.md)
- `disambiguate_ambiguous_candidates(candidates: list[str], candidate_files: dict[str, str], call_site_file: str)` — [`L153`](../../../../../raw/code/graphify/graphify/paths.py#L153) — Resolve an ambiguous bare-name call to one candidate, or ``None``. — documented in [graphify-paths](../../concepts/graphify-paths.md)
- `out_path(*parts: str)` — [`L218`](../../../../../raw/code/graphify/graphify/paths.py#L218) — A path inside the configured output dir, e.g. ``out_path("cache")``. — documented in [graphify-paths](../../concepts/graphify-paths.md)

## Module values
- `GRAPHIFY_OUT` — [`L23`](../../../../../raw/code/graphify/graphify/paths.py#L23) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `GRAPHIFY_OUT_NAME` — [`L215`](../../../../../raw/code/graphify/graphify/paths.py#L215) — documented in [graphify-callflow_html](../../concepts/graphify-callflow_html.md)
- `_TEST_DIR_SEGMENTS` — [`L29`](../../../../../raw/code/graphify/graphify/paths.py#L29) — documented in [graphify-paths](../../concepts/graphify-paths.md)
- `_TEST_FILENAME_PATTERNS` — [`L39`](../../../../../raw/code/graphify/graphify/paths.py#L39) — documented in [graphify-paths](../../concepts/graphify-paths.md)

