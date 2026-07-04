---
title: 'Module: tests/unit/test_knowledge_graph.py'
type: catalog
provenance: extracted
module: tests/unit/test_knowledge_graph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_knowledge_graph`/
symbols:
  test_builder_edge_and_markdown_caps_cover_relationship_boundaries: test_builder_edge_and_markdown_caps_cover_relationship_boundaries().
  test_graphology_export_supports_package_focus_and_empty_graph: test_graphology_export_supports_package_focus_and_empty_graph().
  test_ladybug_store_writes_snapshot_when_optional_dependency_exists: test_ladybug_store_writes_snapshot_when_optional_dependency_exists().
  test_knowledge_graph_tool_exports_graphology: test_knowledge_graph_tool_exports_graphology().
  test_knowledge_graph_tool_exports_html_viewer: test_knowledge_graph_tool_exports_html_viewer().
  test_graphology_export_filters_docs_lod_exactly: test_graphology_export_filters_docs_lod_exactly().
  test_json_store_round_trips_snapshot: test_json_store_round_trips_snapshot().
  test_knowledge_graph_tool_exports_raw_and_summary: test_knowledge_graph_tool_exports_raw_and_summary().
  test_builder_respects_caps_and_skips_bad_markdown_refs: test_builder_respects_caps_and_skips_bad_markdown_refs().
  test_builder_private_edge_and_value_boundaries: test_builder_private_edge_and_value_boundaries().
  test_builder_projects_ast_cache_and_markdown_links: test_builder_projects_ast_cache_and_markdown_links().
  test_ladybug_store_reports_missing_optional_dependency: test_ladybug_store_reports_missing_optional_dependency().
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeBuilder.build: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeBuilder#build().
  test_cli_knowledge_graph_import_and_special_command_paths: test_cli_knowledge_graph_import_and_special_command_paths().
  test_knowledge_index_tool_builds_json_and_hybrid_error: test_knowledge_index_tool_builds_json_and_hybrid_error().
  test_knowledge_index_tool_validation_rejects_bad_values: test_knowledge_index_tool_validation_rejects_bad_values().
  test_knowledge_index_tool_requires_project_root: test_knowledge_index_tool_requires_project_root().
  test_knowledge_index_tool_status_is_readable: test_knowledge_index_tool_status_is_readable().
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeLadybugStore.write: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeLadybugStore#write().
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeLadybugSuccessStore.write: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeLadybugSuccessStore#write().
  test_knowledge_index_prepare_index_build_and_update: test_knowledge_index_prepare_index_build_and_update().
  test_knowledge_graph_tool_validation_rejects_bad_values: test_knowledge_graph_tool_validation_rejects_bad_values().
  test_knowledge_graph_tool_requires_project_root: test_knowledge_graph_tool_requires_project_root().
  test_knowledge_graph_tool_reports_missing_sidecar: test_knowledge_graph_tool_reports_missing_sidecar().
  test_html_viewer_embeds_graphology_payload_safely: test_html_viewer_embeds_graphology_payload_safely().
  test_compact_sync_report_drops_per_file_payloads: test_compact_sync_report_drops_per_file_payloads().
  test_builder_respects_caps_and_skips_bad_markdown_refs._raise_os_error: test_builder_respects_caps_and_skips_bad_markdown_refs()._raise_os_error().
  test_ladybug_store_reports_missing_optional_dependency._missing_ladybug: test_ladybug_store_reports_missing_optional_dependency()._missing_ladybug().
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeBuilder: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeBuilder#
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeLadybugStore: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeLadybugStore#
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeLadybugSuccessStore: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeLadybugSuccessStore#
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeBuilder.__init__: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeBuilder#__init__().
  FakeBuilder.project_root: FakeBuilder#project_root.
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeLadybugStore.__init__: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeLadybugStore#__init__().
  FakeLadybugStore.project_root: FakeLadybugStore#project_root.
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeLadybugStore.status: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeLadybugStore#status().
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeLadybugSuccessStore.__init__: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeLadybugSuccessStore#__init__().
  FakeLadybugSuccessStore.project_root: FakeLadybugSuccessStore#project_root.
  test_knowledge_index_tool_builds_json_and_hybrid_error.FakeLadybugSuccessStore.status: test_knowledge_index_tool_builds_json_and_hybrid_error().FakeLadybugSuccessStore#status().
---
# Module: [`tests/unit/test_knowledge_graph.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py)

## Classes
### `FakeBuilder`
- def: [`tests/unit/test_knowledge_graph.py:513`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L513)
- signature: `class FakeBuilder:`
- members:
  - `build(self, **kwargs: Any)` — [`L517`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L517)
  - `project_root` — [`L515`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L515)
- protocol/private: `__init__`[`L514`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L514)
- uses (calls/refs, reference-scoped): [`KnowledgeNode`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeNode), [`id`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeNode.id), [`kind`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeNode.kind), [`label`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeNode.label), [`KnowledgeGraphSnapshot`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeGraphSnapshot), [`file_path`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeNode.file_path), [`stats`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeGraphSnapshot.stats), [`edges`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeGraphSnapshot.edges), [`nodes`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeGraphSnapshot.nodes)
- used by: (1 test-only callers)

### `FakeLadybugStore`
- def: [`tests/unit/test_knowledge_graph.py:531`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L531)
- signature: `class FakeLadybugStore:`
- members:
  - `status(self)` — [`L535`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L535)
  - `write(self, snapshot: KnowledgeGraphSnapshot)` — [`L538`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L538)
  - `project_root` — [`L533`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L533)
- protocol/private: `__init__`[`L532`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L532)
- uses (calls/refs, reference-scoped): [`KnowledgeGraphSnapshot`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeGraphSnapshot), [`LadybugUnavailableError`](../../tree_sitter_analyzer/knowledge_graph/stores.md#LadybugUnavailableError)
- used by: (1 test-only callers)

### `FakeLadybugSuccessStore`
- def: [`tests/unit/test_knowledge_graph.py:541`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L541)
- signature: `class FakeLadybugSuccessStore:`
- members:
  - `status(self)` — [`L545`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L545)
  - `write(self, snapshot: KnowledgeGraphSnapshot)` — [`L548`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L548)
  - `project_root` — [`L543`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L543)
- protocol/private: `__init__`[`L542`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L542)
- uses (calls/refs, reference-scoped): [`KnowledgeGraphSnapshot`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeGraphSnapshot), [`nodes`](../../tree_sitter_analyzer/knowledge_graph/models.md#KnowledgeGraphSnapshot.nodes)
- used by: (1 test-only callers)

## Functions
- `_missing_ladybug(name: str)` — [`L428`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L428)
- `_raise_os_error(*args: Any, **kwargs: Any)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L110)
- `test_builder_edge_and_markdown_caps_cover_relationship_boundaries(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L178)
- `test_builder_private_edge_and_value_boundaries()` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L122)
- `test_builder_projects_ast_cache_and_markdown_links(tmp_path: Path)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L47)
- `test_builder_respects_caps_and_skips_bad_markdown_refs(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L76)
- `test_cli_knowledge_graph_import_and_special_command_paths(monkeypatch: pytest.MonkeyPatch)` — [`L740`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L740)
- `test_compact_sync_report_drops_per_file_payloads()` — [`L725`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L725)
- `test_graphology_export_filters_docs_lod_exactly()` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L265)
- `test_graphology_export_supports_package_focus_and_empty_graph()` — [`L311`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L311)
- `test_html_viewer_embeds_graphology_payload_safely()` — [`L392`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L392)
- `test_json_store_round_trips_snapshot(tmp_path: Path)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L244)
- `test_knowledge_graph_tool_exports_graphology(tmp_path: Path)` — [`L636`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L636)
- `test_knowledge_graph_tool_exports_html_viewer(tmp_path: Path)` — [`L688`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L688)
- `test_knowledge_graph_tool_exports_raw_and_summary(tmp_path: Path)` — [`L669`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L669)
- `test_knowledge_graph_tool_reports_missing_sidecar(tmp_path: Path)` — [`L625`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L625)
- `test_knowledge_graph_tool_requires_project_root()` — [`L615`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L615)
- `test_knowledge_graph_tool_validation_rejects_bad_values(tmp_path: Path)` — [`L605`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L605)
- `test_knowledge_index_prepare_index_build_and_update(tmp_path: Path)` — [`L593`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L593)
- `test_knowledge_index_tool_builds_json_and_hybrid_error(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L510`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L510)
- `test_knowledge_index_tool_requires_project_root()` — [`L486`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L486)
- `test_knowledge_index_tool_status_is_readable(tmp_path: Path)` — [`L496`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L496)
- `test_knowledge_index_tool_validation_rejects_bad_values(tmp_path: Path)` — [`L476`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L476)
- `test_ladybug_store_reports_missing_optional_dependency(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L420`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L420)
- `test_ladybug_store_writes_snapshot_when_optional_dependency_exists(tmp_path: Path)` — [`L447`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_knowledge_graph.py#L447)

