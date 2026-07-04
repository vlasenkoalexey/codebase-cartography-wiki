---
title: 'Module: tests/test_cli_export.py'
type: catalog
provenance: extracted
module: tests/test_cli_export.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_cli_export`/
symbols:
  _make_graph: _make_graph().
  _run: _run().
  test_export_html_creates_file: test_export_html_creates_file().
  test_export_html_no_viz_removes_file: test_export_html_no_viz_removes_file().
  test_export_obsidian_creates_vault: test_export_obsidian_creates_vault().
  test_export_obsidian_custom_dir: test_export_obsidian_custom_dir().
  test_export_wiki_creates_articles: test_export_wiki_creates_articles().
  test_export_wiki_accepts_edges_only_graph_json: test_export_wiki_accepts_edges_only_graph_json().
  test_export_graphml_creates_file: test_export_graphml_creates_file().
  test_export_neo4j_creates_cypher: test_export_neo4j_creates_cypher().
  test_export_falkordb_creates_cypher: test_export_falkordb_creates_cypher().
  test_query_returns_output: test_query_returns_output().
  test_query_dfs_flag: test_query_dfs_flag().
  test_query_budget_flag: test_query_budget_flag().
  test_query_uses_graphify_out_env: test_query_uses_graphify_out_env().
  test_path_runs_without_error: test_path_runs_without_error().
  test_path_uses_graphify_out_env: test_path_uses_graphify_out_env().
  test_explain_runs_without_error: test_explain_runs_without_error().
  test_explain_uses_graphify_out_env: test_explain_uses_graphify_out_env().
  test_cluster_only_creates_output_dir_when_missing: test_cluster_only_creates_output_dir_when_missing().
  test_cluster_only_persists_analysis_sidecar: test_cluster_only_persists_analysis_sidecar().
  test_cluster_only_remaps_labels_to_previous_cids: test_cluster_only_remaps_labels_to_previous_cids().
  test_export_html_falls_back_to_node_community_attribute: test_export_html_falls_back_to_node_community_attribute().
  test_export_html_fallback_recovers_multiple_communities: test_export_html_fallback_recovers_multiple_communities().
  test_export_html_no_community_data_at_all_still_succeeds: test_export_html_no_community_data_at_all_still_succeeds().
  test_export_html_error_without_graph: test_export_html_error_without_graph().
  test_query_missing_graph_fails: test_query_missing_graph_fails().
  test_extract_writes_to_graphify_out_env: test_extract_writes_to_graphify_out_env().
  test_path_missing_graph_fails: test_path_missing_graph_fails().
  test_explain_missing_graph_fails: test_explain_missing_graph_fails().
  test_export_unknown_format_fails: test_export_unknown_format_fails().
  test_update_no_cluster_writes_raw_graph: test_update_no_cluster_writes_raw_graph().
  PYTHON: PYTHON.
  FIXTURES: FIXTURES.
---
# Module: [`tests/test_cli_export.py`](../../../../../raw/code/graphify/tests/test_cli_export.py)

## Functions
- `_make_graph(tmp_path: Path)` — [`L29`](../../../../../raw/code/graphify/tests/test_cli_export.py#L29) — Build a minimal graph.json + analysis/labels files in tmp_path/graphify-out/.
- `_run(args: list[str], cwd: Path, env: dict[str, str] | None = None)` — [`L19`](../../../../../raw/code/graphify/tests/test_cli_export.py#L19)
- `test_cluster_only_creates_output_dir_when_missing(tmp_path)` — [`L303`](../../../../../raw/code/graphify/tests/test_cli_export.py#L303) — cluster-only must not crash with FileNotFoundError when graphify-out/ is absent (#934).
- `test_cluster_only_persists_analysis_sidecar(tmp_path)` — [`L326`](../../../../../raw/code/graphify/tests/test_cli_export.py#L326) — cluster-only must refresh .graphify_analysis.json alongside graph.json.
- `test_cluster_only_remaps_labels_to_previous_cids(tmp_path)` — [`L356`](../../../../../raw/code/graphify/tests/test_cli_export.py#L356) — cluster-only must invoke remap_communities_to_previous so the existing
- `test_explain_missing_graph_fails(tmp_path)` — [`L263`](../../../../../raw/code/graphify/tests/test_cli_export.py#L263)
- `test_explain_runs_without_error(tmp_path)` — [`L257`](../../../../../raw/code/graphify/tests/test_cli_export.py#L257)
- `test_explain_uses_graphify_out_env(tmp_path)` — [`L268`](../../../../../raw/code/graphify/tests/test_cli_export.py#L268)
- `test_export_falkordb_creates_cypher(tmp_path)` — [`L159`](../../../../../raw/code/graphify/tests/test_cli_export.py#L159)
- `test_export_graphml_creates_file(tmp_path)` — [`L133`](../../../../../raw/code/graphify/tests/test_cli_export.py#L133)
- `test_export_html_creates_file(tmp_path)` — [`L64`](../../../../../raw/code/graphify/tests/test_cli_export.py#L64)
- `test_export_html_error_without_graph(tmp_path)` — [`L81`](../../../../../raw/code/graphify/tests/test_cli_export.py#L81)
- `test_export_html_fallback_recovers_multiple_communities(tmp_path)` — [`L437`](../../../../../raw/code/graphify/tests/test_cli_export.py#L437) — Stronger assertion: the reconstructed `communities` dict should have the
- `test_export_html_falls_back_to_node_community_attribute(tmp_path)` — [`L416`](../../../../../raw/code/graphify/tests/test_cli_export.py#L416) — When .graphify_analysis.json is absent, export html should reconstruct
- `test_export_html_no_community_data_at_all_still_succeeds(tmp_path)` — [`L466`](../../../../../raw/code/graphify/tests/test_cli_export.py#L466) — If a graph.json was somehow written without any per-node `community`
- `test_export_html_no_viz_removes_file(tmp_path)` — [`L73`](../../../../../raw/code/graphify/tests/test_cli_export.py#L73)
- `test_export_neo4j_creates_cypher(tmp_path)` — [`L146`](../../../../../raw/code/graphify/tests/test_cli_export.py#L146)
- `test_export_obsidian_creates_vault(tmp_path)` — [`L88`](../../../../../raw/code/graphify/tests/test_cli_export.py#L88)
- `test_export_obsidian_custom_dir(tmp_path)` — [`L98`](../../../../../raw/code/graphify/tests/test_cli_export.py#L98)
- `test_export_unknown_format_fails(tmp_path)` — [`L282`](../../../../../raw/code/graphify/tests/test_cli_export.py#L282)
- `test_export_wiki_accepts_edges_only_graph_json(tmp_path)` — [`L118`](../../../../../raw/code/graphify/tests/test_cli_export.py#L118)
- `test_export_wiki_creates_articles(tmp_path)` — [`L109`](../../../../../raw/code/graphify/tests/test_cli_export.py#L109)
- `test_extract_writes_to_graphify_out_env(tmp_path)` — [`L209`](../../../../../raw/code/graphify/tests/test_cli_export.py#L209) — #1423: `graphify extract` honours GRAPHIFY_OUT for where it WRITES, not only
- `test_path_missing_graph_fails(tmp_path)` — [`L238`](../../../../../raw/code/graphify/tests/test_cli_export.py#L238)
- `test_path_runs_without_error(tmp_path)` — [`L231`](../../../../../raw/code/graphify/tests/test_cli_export.py#L231)
- `test_path_uses_graphify_out_env(tmp_path)` — [`L243`](../../../../../raw/code/graphify/tests/test_cli_export.py#L243)
- `test_query_budget_flag(tmp_path)` — [`L185`](../../../../../raw/code/graphify/tests/test_cli_export.py#L185)
- `test_query_dfs_flag(tmp_path)` — [`L179`](../../../../../raw/code/graphify/tests/test_cli_export.py#L179)
- `test_query_missing_graph_fails(tmp_path)` — [`L191`](../../../../../raw/code/graphify/tests/test_cli_export.py#L191)
- `test_query_returns_output(tmp_path)` — [`L172`](../../../../../raw/code/graphify/tests/test_cli_export.py#L172)
- `test_query_uses_graphify_out_env(tmp_path)` — [`L196`](../../../../../raw/code/graphify/tests/test_cli_export.py#L196)
- `test_update_no_cluster_writes_raw_graph(tmp_path)` — [`L287`](../../../../../raw/code/graphify/tests/test_cli_export.py#L287)

## Module values
- `FIXTURES` — [`L16`](../../../../../raw/code/graphify/tests/test_cli_export.py#L16)
- `PYTHON` — [`L15`](../../../../../raw/code/graphify/tests/test_cli_export.py#L15)

