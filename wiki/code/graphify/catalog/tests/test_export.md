---
title: 'Module: tests/test_export.py'
type: catalog
provenance: extracted
module: tests/test_export.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_export`/
symbols:
  make_graph: make_graph().
  test_to_html_annotated_node_gets_learning_status_and_ring: test_to_html_annotated_node_gets_learning_status_and_ring().
  test_to_html_contested_stale_node_gets_dashed_desaturated_ring: test_to_html_contested_stale_node_gets_dashed_desaturated_ring().
  test_obsidian_canvas_filenames_agree: test_obsidian_canvas_filenames_agree().
  test_to_json_creates_file: test_to_json_creates_file().
  test_to_json_valid_json: test_to_json_valid_json().
  test_to_json_nodes_have_community: test_to_json_nodes_have_community().
  test_to_graphml_creates_file: test_to_graphml_creates_file().
  test_to_graphml_valid_xml: test_to_graphml_valid_xml().
  test_to_graphml_has_community_attribute: test_to_graphml_has_community_attribute().
  test_to_graphml_tolerates_none_attribute_values: test_to_graphml_tolerates_none_attribute_values().
  test_to_html_creates_file: test_to_html_creates_file().
  test_to_html_contains_visjs: test_to_html_contains_visjs().
  test_to_html_pins_visjs_version_with_sri: test_to_html_pins_visjs_version_with_sri().
  test_to_html_contains_search: test_to_html_contains_search().
  test_to_html_contains_legend_with_labels: test_to_html_contains_legend_with_labels().
  test_to_html_contains_nodes_and_edges: test_to_html_contains_nodes_and_edges().
  test_to_html_member_counts_accepted: test_to_html_member_counts_accepted().
  test_to_html_unannotated_identical_to_pre_feature: test_to_html_unannotated_identical_to_pre_feature().
  test_to_canvas_file_paths_relative_to_vault: test_to_canvas_file_paths_relative_to_vault().
  test_to_obsidian_never_emits_punctuation_only_filenames: test_to_obsidian_never_emits_punctuation_only_filenames().
  test_to_canvas_never_emits_punctuation_only_filenames: test_to_canvas_never_emits_punctuation_only_filenames().
  test_to_obsidian_case_only_distinct_labels_dont_overwrite: test_to_obsidian_case_only_distinct_labels_dont_overwrite().
  test_to_obsidian_generated_suffix_doesnt_overwrite_literal: test_to_obsidian_generated_suffix_doesnt_overwrite_literal().
  test_to_canvas_case_only_distinct_labels_get_distinct_files: test_to_canvas_case_only_distinct_labels_get_distinct_files().
  _case_collision_graph: _case_collision_graph().
  test_to_cypher_creates_file: test_to_cypher_creates_file().
  test_to_cypher_contains_merge_statements: test_to_cypher_contains_merge_statements().
  test_to_canvas_no_communities_still_populates: test_to_canvas_no_communities_still_populates().
  test_to_canvas_node_grid_matches_box_columns: test_to_canvas_node_grid_matches_box_columns().
  test_to_obsidian_preserves_existing_user_notes_and_obsidian_config: test_to_obsidian_preserves_existing_user_notes_and_obsidian_config().
  test_to_obsidian_empty_dir_writes_full_vault: test_to_obsidian_empty_dir_writes_full_vault().
  test_to_obsidian_rerun_updates_own_notes_but_not_user_files: test_to_obsidian_rerun_updates_own_notes_but_not_user_files().
  test_to_obsidian_community_notes_case_collision: test_to_obsidian_community_notes_case_collision().
  _punct_graph: _punct_graph().
  _two_node_graph: _two_node_graph().
  test_backup_no_graph_json: test_backup_no_graph_json().
  test_backup_no_markers: test_backup_no_markers().
  test_backup_semantic_marker: test_backup_semantic_marker().
  test_backup_curated_labels: test_backup_curated_labels().
  test_backup_default_labels_only: test_backup_default_labels_only().
  test_backup_same_day_no_accumulation: test_backup_same_day_no_accumulation().
  test_backup_same_day_changed_content: test_backup_same_day_changed_content().
  test_backup_env_disable: test_backup_env_disable().
  _vis_nodes_from_html: _vis_nodes_from_html().
  FIXTURES: FIXTURES.
---
# Module: [`tests/test_export.py`](../../../../../raw/code/graphify/tests/test_export.py)

## Functions
- `_case_collision_graph()` — [`L423`](../../../../../raw/code/graphify/tests/test_export.py#L423) — Two nodes whose labels differ only by case - on macOS/APFS and Windows/NTFS
- `_punct_graph(label: str)` — [`L328`](../../../../../raw/code/graphify/tests/test_export.py#L328) — A 2-node graph where one node's label is all-punctuation (e.g. a `@/*`
- `_two_node_graph()` — [`L371`](../../../../../raw/code/graphify/tests/test_export.py#L371)
- `_vis_nodes_from_html(content: str)` — [`L187`](../../../../../raw/code/graphify/tests/test_export.py#L187) — Extract the RAW_NODES JSON array embedded in the generated HTML.
- `make_graph()` — [`L12`](../../../../../raw/code/graphify/tests/test_export.py#L12)
- `test_backup_curated_labels(tmp_path)` — [`L554`](../../../../../raw/code/graphify/tests/test_export.py#L554) — graph.json + non-default label in .graphify_labels.json → backup taken.
- `test_backup_default_labels_only(tmp_path)` — [`L564`](../../../../../raw/code/graphify/tests/test_export.py#L564) — All-default labels → no backup (not curated).
- `test_backup_env_disable(tmp_path, monkeypatch)` — [`L599`](../../../../../raw/code/graphify/tests/test_export.py#L599) — GRAPHIFY_NO_BACKUP=1 disables backup entirely.
- `test_backup_no_graph_json(tmp_path)` — [`L527`](../../../../../raw/code/graphify/tests/test_export.py#L527) — No graph.json → no backup.
- `test_backup_no_markers(tmp_path)` — [`L533`](../../../../../raw/code/graphify/tests/test_export.py#L533) — graph.json present but no sentinel and no curated labels → no backup.
- `test_backup_same_day_changed_content(tmp_path)` — [`L586`](../../../../../raw/code/graphify/tests/test_export.py#L586) — Changed graph.json on same day overwrites the existing backup in place.
- `test_backup_same_day_no_accumulation(tmp_path)` — [`L573`](../../../../../raw/code/graphify/tests/test_export.py#L573) — Same content on same day returns existing backup dir without re-copying.
- `test_backup_semantic_marker(tmp_path)` — [`L540`](../../../../../raw/code/graphify/tests/test_export.py#L540) — graph.json + .graphify_semantic_marker → backup taken.
- `test_obsidian_canvas_filenames_agree()` — [`L488`](../../../../../raw/code/graphify/tests/test_export.py#L488) — The CLI calls to_obsidian and to_canvas separately with no shared map, so — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_to_canvas_case_only_distinct_labels_get_distinct_files()` — [`L474`](../../../../../raw/code/graphify/tests/test_export.py#L474) — Canvas file-node references for case-only-distinct labels must be distinct
- `test_to_canvas_file_paths_relative_to_vault()` — [`L256`](../../../../../raw/code/graphify/tests/test_export.py#L256) — Node file paths in canvas must be vault-root-relative (just fname.md), not hardcoded.
- `test_to_canvas_never_emits_punctuation_only_filenames()` — [`L355`](../../../../../raw/code/graphify/tests/test_export.py#L355) — #1409: same guard on the canvas exporter's file-node names.
- `test_to_canvas_no_communities_still_populates()` — [`L271`](../../../../../raw/code/graphify/tests/test_export.py#L271) — #1324: empty communities (e.g. --no-cluster builds) on a populated graph
- `test_to_canvas_node_grid_matches_box_columns()` — [`L284`](../../../../../raw/code/graphify/tests/test_export.py#L284) — #1452: a community's node cards are laid out in the same ceil(sqrt(n))-column
- `test_to_cypher_contains_merge_statements()` — [`L50`](../../../../../raw/code/graphify/tests/test_export.py#L50)
- `test_to_cypher_creates_file()` — [`L43`](../../../../../raw/code/graphify/tests/test_export.py#L43)
- `test_to_graphml_creates_file()` — [`L58`](../../../../../raw/code/graphify/tests/test_export.py#L58)
- `test_to_graphml_has_community_attribute()` — [`L76`](../../../../../raw/code/graphify/tests/test_export.py#L76)
- `test_to_graphml_tolerates_none_attribute_values()` — [`L85`](../../../../../raw/code/graphify/tests/test_export.py#L85) — nx.write_graphml raises ValueError on a None attribute value; to_graphml
- `test_to_graphml_valid_xml()` — [`L66`](../../../../../raw/code/graphify/tests/test_export.py#L66)
- `test_to_html_annotated_node_gets_learning_status_and_ring()` — [`L194`](../../../../../raw/code/graphify/tests/test_export.py#L194) — A node with an overlay entry gets learning_status + learning_stale fields,
- `test_to_html_contains_legend_with_labels()` — [`L155`](../../../../../raw/code/graphify/tests/test_export.py#L155)
- `test_to_html_contains_nodes_and_edges()` — [`L165`](../../../../../raw/code/graphify/tests/test_export.py#L165)
- `test_to_html_contains_search()` — [`L146`](../../../../../raw/code/graphify/tests/test_export.py#L146)
- `test_to_html_contains_visjs()` — [`L110`](../../../../../raw/code/graphify/tests/test_export.py#L110) — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_to_html_contested_stale_node_gets_dashed_desaturated_ring()` — [`L220`](../../../../../raw/code/graphify/tests/test_export.py#L220)
- `test_to_html_creates_file()` — [`L102`](../../../../../raw/code/graphify/tests/test_export.py#L102)
- `test_to_html_member_counts_accepted()` — [`L176`](../../../../../raw/code/graphify/tests/test_export.py#L176) — to_html accepts member_counts without raising.
- `test_to_html_pins_visjs_version_with_sri()` — [`L120`](../../../../../raw/code/graphify/tests/test_export.py#L120) — vis-network script tag must use a pinned versioned URL with a sha384
- `test_to_html_unannotated_identical_to_pre_feature()` — [`L239`](../../../../../raw/code/graphify/tests/test_export.py#L239) — With no overlay, the HTML is byte-identical whether learning_overlay is — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_to_json_creates_file()` — [`L15`](../../../../../raw/code/graphify/tests/test_export.py#L15)
- `test_to_json_nodes_have_community()` — [`L33`](../../../../../raw/code/graphify/tests/test_export.py#L33) — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_to_json_valid_json()` — [`L23`](../../../../../raw/code/graphify/tests/test_export.py#L23) — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_to_obsidian_case_only_distinct_labels_dont_overwrite()` — [`L435`](../../../../../raw/code/graphify/tests/test_export.py#L435) — Both notes must survive as separate files. On a case-insensitive filesystem — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_to_obsidian_community_notes_case_collision()` — [`L504`](../../../../../raw/code/graphify/tests/test_export.py#L504) — Two community labels differing only by case must each get their own
- `test_to_obsidian_empty_dir_writes_full_vault()` — [`L397`](../../../../../raw/code/graphify/tests/test_export.py#L397) — No regression: a fresh/empty dir still gets every note + .obsidian/graph.json.
- `test_to_obsidian_generated_suffix_doesnt_overwrite_literal()` — [`L452`](../../../../../raw/code/graphify/tests/test_export.py#L452) — A generated `_1` suffix must not collide with a node whose literal label is — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_to_obsidian_never_emits_punctuation_only_filenames()` — [`L340`](../../../../../raw/code/graphify/tests/test_export.py#L340) — #1409: an all-punctuation label (e.g. `@/*`) must not produce a `@.md`-style — documented in [graphify-export](../../concepts/graphify-export.md)
- `test_to_obsidian_preserves_existing_user_notes_and_obsidian_config()` — [`L380`](../../../../../raw/code/graphify/tests/test_export.py#L380) — #1506: exporting into an existing vault must not overwrite a user's note that
- `test_to_obsidian_rerun_updates_own_notes_but_not_user_files()` — [`L408`](../../../../../raw/code/graphify/tests/test_export.py#L408) — A re-run overwrites graphify's own prior notes (via the manifest) but leaves a

## Module values
- `FIXTURES` — [`L10`](../../../../../raw/code/graphify/tests/test_export.py#L10)

