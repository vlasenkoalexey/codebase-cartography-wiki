---
title: 'Module: tests/unit/tools/test_graph_builder_perf_fixes.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_graph_builder_perf_fixes.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_graph_builder_perf_fixes`/
symbols:
  _make_graph_builder: _make_graph_builder().
  _FakeResult: _FakeResult#
  _RecordingSession.calls: _RecordingSession#calls.
  _RecordingSession: _RecordingSession#
  TestDeleteRepositoryFromGraph._make_repo_exists_session: TestDeleteRepositoryFromGraph#_make_repo_exists_session().
  TestCreateAllFunctionCallsV3._run: TestCreateAllFunctionCallsV3#_run().
  _RecordingSession.run: _RecordingSession#run().
  _DeleteRepoSession.run: _DeleteRepoSession#run().
  TestDeleteRepositoryFromGraph.test_deletion_queries_use_forward_slash_paths: TestDeleteRepositoryFromGraph#test_deletion_queries_use_forward_slash_paths().
  TestAddFileToGraph.test_writes_use_unwind: TestAddFileToGraph#test_writes_use_unwind().
  TestAddFileToGraph.test_class_function_contains_uses_class_context_line: TestAddFileToGraph#test_class_function_contains_uses_class_context_line().
  TestAddFileToGraph.test_non_javascript_import_rows_are_schema_complete: TestAddFileToGraph#test_non_javascript_import_rows_are_schema_complete().
  TestAddFileToGraph.test_import_module_metadata_preserves_existing_node_values: TestAddFileToGraph#test_import_module_metadata_preserves_existing_node_values().
  TestAddFileToGraph.test_duplicate_import_metadata_uses_stable_canonical_order: TestAddFileToGraph#test_duplicate_import_metadata_uses_stable_canonical_order().
  TestDeleteRepositoryFromGraph.test_finds_repo_with_unix_path: TestDeleteRepositoryFromGraph#test_finds_repo_with_unix_path().
  TestDeleteRelationshipHelpers.test_delete_relationship_links_runs_query: TestDeleteRelationshipHelpers#test_delete_relationship_links_runs_query().
  TestDeleteRelationshipHelpers.test_delete_outgoing_calls_from_files: TestDeleteRelationshipHelpers#test_delete_outgoing_calls_from_files().
  TestDeleteRelationshipHelpers.test_delete_outgoing_calls_passes_paths: TestDeleteRelationshipHelpers#test_delete_outgoing_calls_passes_paths().
  TestDeleteRelationshipHelpers.test_delete_inherits_for_files: TestDeleteRelationshipHelpers#test_delete_inherits_for_files().
  TestResolveFunctionCall._call: TestResolveFunctionCall#_call().
  TestCreateAllFunctionCallsV3.test_uses_merge_for_calls_rel_on_kuzudb: TestCreateAllFunctionCallsV3#test_uses_merge_for_calls_rel_on_kuzudb().
  TestCreateAllFunctionCallsV3.test_uses_merge_for_calls_rel_on_falkordb: TestCreateAllFunctionCallsV3#test_uses_merge_for_calls_rel_on_falkordb().
  TestCreateAllFunctionCallsV3.test_function_call_batch_normalization_preserves_falsy_filters: TestCreateAllFunctionCallsV3#test_function_call_batch_normalization_preserves_falsy_filters().
  TestDeleteRepositoryFromGraph.test_returns_false_when_repo_not_found: TestDeleteRepositoryFromGraph#test_returns_false_when_repo_not_found().
  TestDeleteRepositoryFromGraph.test_purges_dangling_pathless_modules: TestDeleteRepositoryFromGraph#test_purges_dangling_pathless_modules().
  TestDeleteRepositoryFromGraph.test_deletes_relationships_before_nodes: TestDeleteRepositoryFromGraph#test_deletes_relationships_before_nodes().
  TestDeleteRepositoryFromGraph.test_uses_starts_with_prefix_for_scope: TestDeleteRepositoryFromGraph#test_uses_starts_with_prefix_for_scope().
  TestDeleteRepositoryFromGraph.test_batched_delete_uses_limit: TestDeleteRepositoryFromGraph#test_batched_delete_uses_limit().
  TestDeleteRepositoryFromGraph.test_deletes_repository_node_itself: TestDeleteRepositoryFromGraph#test_deletes_repository_node_itself().
  TestDeleteRepositoryFromGraph.test_purges_labels_discovered_dynamically: TestDeleteRepositoryFromGraph#test_purges_labels_discovered_dynamically().
  TestDeleteRepositoryFromGraph.test_calls_db_labels_after_existence_check: TestDeleteRepositoryFromGraph#test_calls_db_labels_after_existence_check().
  TestDeleteRepositoryFromGraph.test_finds_repo_stored_with_backslash_path: TestDeleteRepositoryFromGraph#test_finds_repo_stored_with_backslash_path().
  _RecordingSession._call_idx: _RecordingSession#_call_idx.
  _DeleteRepoSession: _DeleteRepoSession#
  TestResolveFunctionCall.test_returns_none_for_builtin: TestResolveFunctionCall#test_returns_none_for_builtin().
  TestResolveFunctionCall.test_resolves_local_function_call: TestResolveFunctionCall#test_resolves_local_function_call().
  TestResolveFunctionCall.test_resolves_self_method_call: TestResolveFunctionCall#test_resolves_self_method_call().
  TestResolveFunctionCall.test_resolves_via_imports_map: TestResolveFunctionCall#test_resolves_via_imports_map().
  TestResolveFunctionCall.test_resolves_aliased_import_to_original_symbol: TestResolveFunctionCall#test_resolves_aliased_import_to_original_symbol().
  TestResolveFunctionCall.test_skip_external_suppresses_unresolved: TestResolveFunctionCall#test_skip_external_suppresses_unresolved().
  TestResolveFunctionCall.test_skip_external_false_still_returns_something: TestResolveFunctionCall#test_skip_external_false_still_returns_something().
  TestResolveFunctionCall.test_file_type_returned_when_no_caller_context: TestResolveFunctionCall#test_file_type_returned_when_no_caller_context().
  TestCreateAllFunctionCallsV3.test_file_class_lookup_supplemented_from_file_data: TestCreateAllFunctionCallsV3#test_file_class_lookup_supplemented_from_file_data().
  TestDeleteRepositoryFromGraph.test_returns_true_when_repo_found: TestDeleteRepositoryFromGraph#test_returns_true_when_repo_found().
  _RecordingSession._responses: _RecordingSession#_responses.
  _RecordingSession.__init__: _RecordingSession#__init__().
  _FakeResult._rows: _FakeResult#_rows.
  TestDeleteRepositoryFromGraph._DEFAULT_DB_LABELS: TestDeleteRepositoryFromGraph#_DEFAULT_DB_LABELS.
  _FakeResult.single: _FakeResult#single().
  _FakeResult.__iter__: _FakeResult#__iter__().
  _FakeDriver.__init__: _FakeDriver#__init__().
  _FakeDriver.session: _FakeDriver#session().
  _FakeDBManager.get_backend_type: _FakeDBManager#get_backend_type().
  TestCreateAllFunctionCallsV3.test_uses_unwind_queries: TestCreateAllFunctionCallsV3#test_uses_unwind_queries().
  TestCreateAllFunctionCallsV3.test_uses_create_for_calls_rel_on_neo4j: TestCreateAllFunctionCallsV3#test_uses_create_for_calls_rel_on_neo4j().
  TestCreateAllFunctionCallsV3.test_calls_rel_identity_excludes_mutable_metadata: TestCreateAllFunctionCallsV3#test_calls_rel_identity_excludes_mutable_metadata().
  TestCreateAllFunctionCallsV3.test_function_call_writes_use_precise_target_filters: TestCreateAllFunctionCallsV3#test_function_call_writes_use_precise_target_filters().
  TestCreateAllFunctionCallsV3.test_empty_file_data_writes_nothing: TestCreateAllFunctionCallsV3#test_empty_file_data_writes_nothing().
  TestCreateAllFunctionCallsV3.test_label_specific_queries_used: TestCreateAllFunctionCallsV3#test_label_specific_queries_used().
  _DeleteRepoSession.__init__: _DeleteRepoSession#__init__().
  TestWriteOrmMappingsDatasourceName.test_orm_batch_sets_datasource_name_on_existing_node: TestWriteOrmMappingsDatasourceName#test_orm_batch_sets_datasource_name_on_existing_node().
  _FakeDriver: _FakeDriver#
  _DeleteRepoSession._labels: _DeleteRepoSession#_labels.
  _FakeDriver._session: _FakeDriver#_session.
  _FakeDBManager: _FakeDBManager#
  _FakeDBManager._backend: _FakeDBManager#_backend.
  TestWriteOrmMappingsDatasourceName._make_writer: TestWriteOrmMappingsDatasourceName#_make_writer().
  _FakeResult.__init__: _FakeResult#__init__().
  _RecordingSession.__enter__: _RecordingSession#__enter__().
  _RecordingSession.__exit__: _RecordingSession#__exit__().
  _FakeDBManager.__init__: _FakeDBManager#__init__().
  TestResolveFunctionCall: TestResolveFunctionCall#
  TestCreateAllFunctionCallsV3: TestCreateAllFunctionCallsV3#
  TestAddFileToGraph: TestAddFileToGraph#
  TestAddFileToGraph.test_accepts_repo_path_str_kwarg: TestAddFileToGraph#test_accepts_repo_path_str_kwarg().
  TestAddFileToGraph.test_repo_path_str_is_optional: TestAddFileToGraph#test_repo_path_str_is_optional().
  TestDeleteRepositoryFromGraph: TestDeleteRepositoryFromGraph#
  TestDeleteRelationshipHelpers: TestDeleteRelationshipHelpers#
  TestGraphBuilderMethodsExist: TestGraphBuilderMethodsExist#
  TestGraphBuilderMethodsExist.test_resolve_function_call_exists: TestGraphBuilderMethodsExist#test_resolve_function_call_exists().
  TestGraphBuilderMethodsExist.test_create_all_function_calls_exists: TestGraphBuilderMethodsExist#test_create_all_function_calls_exists().
  TestGraphBuilderMethodsExist.test_delete_outgoing_calls_from_files_exists: TestGraphBuilderMethodsExist#test_delete_outgoing_calls_from_files_exists().
  TestGraphBuilderMethodsExist.test_delete_inherits_for_files_exists: TestGraphBuilderMethodsExist#test_delete_inherits_for_files_exists().
  TestGraphBuilderMethodsExist.test_get_caller_file_paths_exists: TestGraphBuilderMethodsExist#test_get_caller_file_paths_exists().
  TestGraphBuilderMethodsExist.test_get_inheritance_neighbor_paths_exists: TestGraphBuilderMethodsExist#test_get_inheritance_neighbor_paths_exists().
  TestGraphBuilderMethodsExist.test_get_repo_class_lookup_exists: TestGraphBuilderMethodsExist#test_get_repo_class_lookup_exists().
  TestCliHelpersContainsFix: TestCliHelpersContainsFix#
  TestCliHelpersContainsFix.test_index_helper_uses_variable_length_contains: TestCliHelpersContainsFix#test_index_helper_uses_variable_length_contains().
  TestCliHelpersContainsFix.test_index_helper_does_not_use_fixed_contains_only: TestCliHelpersContainsFix#test_index_helper_does_not_use_fixed_contains_only().
  TestWatcherMemoryClear: TestWatcherMemoryClear#
  TestWatcherMemoryClear.test_initial_scan_clears_all_file_data: TestWatcherMemoryClear#test_initial_scan_clears_all_file_data().
  TestWatcherMemoryClear.test_all_file_data_is_empty_after_initial_scan: TestWatcherMemoryClear#test_all_file_data_is_empty_after_initial_scan().
  TestWatcherIncrementalHandleModification: TestWatcherIncrementalHandleModification#
  TestWatcherIncrementalHandleModification.test_handle_modification_calls_delete_outgoing: TestWatcherIncrementalHandleModification#test_handle_modification_calls_delete_outgoing().
  TestWatcherIncrementalHandleModification.test_handle_modification_skips_delete_when_no_callers: TestWatcherIncrementalHandleModification#test_handle_modification_skips_delete_when_no_callers().
  TestWatcherIncrementalHandleModification.test_handle_modification_calls_create_all_function_calls: TestWatcherIncrementalHandleModification#test_handle_modification_calls_create_all_function_calls().
  TestWriteOrmMappingsDatasourceName: TestWriteOrmMappingsDatasourceName#
  TestWriteOrmMappingsDatasourceName.test_on_match_set_present_in_write_orm_mappings: TestWriteOrmMappingsDatasourceName#test_on_match_set_present_in_write_orm_mappings().
---
# Module: [`tests/unit/tools/test_graph_builder_perf_fixes.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py)

## Classes
### `TestAddFileToGraph`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:473`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L473)
- doc: Tests for the batched add_file_to_graph method (Change 7).
- signature: `class TestAddFileToGraph:`
- members:
  - `test_accepts_repo_path_str_kwarg(self)` — [`L476`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L476) — Should accept the new repo_path_str parameter without error.
  - `test_class_function_contains_uses_class_context_line(self)` — [`L507`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L507) — Same-named nested classes in one file should not all own every method.
  - `test_duplicate_import_metadata_uses_stable_canonical_order(self)` — [`L626`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L626) — Shared Rust module nodes should prefer stable, descriptive import metadata.
  - `test_import_module_metadata_preserves_existing_node_values(self)` — [`L593`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L593) — Repeated imports of the same module should not overwrite node metadata.
  - `test_non_javascript_import_rows_are_schema_complete(self)` — [`L552`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L552) — Imports without full_import_name/source parity should not break Kuzu UNWIND.
  - `test_repo_path_str_is_optional(self)` — [`L482`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L482) — repo_path_str should have a default value (None).
  - `test_writes_use_unwind(self)` — [`L489`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L489) — Node writes should use UNWIND (not individual per-item MERGE).
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestCliHelpersContainsFix`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:995`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L995)
- doc: Change 3: \[:CONTAINS\] -&gt; \[:CONTAINS*\] in indexed path query.
- signature: `class TestCliHelpersContainsFix:`
- members:
  - `test_index_helper_does_not_use_fixed_contains_only(self)` — [`L1006`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1006) — Make sure the old single-hop [:CONTAINS] without * is not used for the indexed check.
  - `test_index_helper_uses_variable_length_contains(self)` — [`L998`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L998)

### `TestCreateAllFunctionCallsV3`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:228`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L228)
- doc: Tests for the V3 _create_all_function_calls method (Change 2).
- signature: `class TestCreateAllFunctionCallsV3:`
- members:
  - `test_calls_rel_identity_excludes_mutable_metadata(self)` — [`L335`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L335) — CALLS confidence/tier should be written via SET, not baked into the
  - `test_empty_file_data_writes_nothing(self)` — [`L421`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L421)
  - `test_file_class_lookup_supplemented_from_file_data(self)` — [`L426`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L426) — External file_class_lookup is supplemented with classes from all_file_data.
  - `test_function_call_batch_normalization_preserves_falsy_filters(self)` — [`L392`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L392) — Valid call rows are passed through to the driver batch as-is.
  - `test_function_call_writes_use_precise_target_filters(self)` — [`L364`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L364) — CALLS writes should use target line/context hints when resolution provides them.
  - `test_label_specific_queries_used(self)` — [`L445`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L445) — Queries should reference specific labels like Function, Class, File — not generic nodes.
  - `test_uses_create_for_calls_rel_on_neo4j(self)` — [`L263`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L263) — CALLS relationships should use CREATE on Neo4j — MERGE lock overhead
  - `test_uses_merge_for_calls_rel_on_falkordb(self)` — [`L311`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L311) — CALLS relationships should keep MERGE on FalkorDB.
  - `test_uses_merge_for_calls_rel_on_kuzudb(self)` — [`L286`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L286) — CALLS relationships should keep MERGE on KuzuDB — its UNWIND fallback
  - `test_uses_unwind_queries(self)` — [`L244`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L244) — All DB writes should use UNWIND (not individual MERGE per call).
- protocol/private: `_run`[`L231`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L231)
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestDeleteRelationshipHelpers`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:918`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L918)
- doc: Tests for the relationship-deletion helpers (Changes 5/6).
- signature: `class TestDeleteRelationshipHelpers:`
- members:
  - `test_delete_inherits_for_files(self)` — [`L945`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L945)
  - `test_delete_outgoing_calls_from_files(self)` — [`L927`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L927)
  - `test_delete_outgoing_calls_passes_paths(self)` — [`L936`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L936)
  - `test_delete_relationship_links_runs_query(self)` — [`L921`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L921)
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestDeleteRepositoryFromGraph`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:713`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L713)
- doc: Tests for delete_repository_from_graph (batched, rels-first, orphan purge).
- signature: `class TestDeleteRepositoryFromGraph:`
- members:
  - `_make_repo_exists_session(self, extra_responses=None, db_labels=None)` — [`L723`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L723) — Session that reports the repo exists (cnt=1), then zero-counts to stop loops.
  - `test_batched_delete_uses_limit(self)` — [`L792`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L792) — Deletion should use LIMIT to batch and avoid cartesian explosion.
  - `test_calls_db_labels_after_existence_check(self)` — [`L839`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L839) — Label discovery should happen exactly once, after the repo
  - `test_deletes_relationships_before_nodes(self)` — [`L765`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L765) — CALLS/INHERITS/IMPORTS/INCLUDES deletion must appear before Function/Class/File node deletion.
  - `test_deletes_repository_node_itself(self)` — [`L801`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L801)
  - `test_deletion_queries_use_forward_slash_paths(self)` — [`L890`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L890) — All deletion queries must use forward-slash normalised paths so that
  - `test_finds_repo_stored_with_backslash_path(self)` — [`L879`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L879) — Fallback should find a Repository stored with Windows backslash paths.
  - `test_finds_repo_with_unix_path(self)` — [`L864`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L864) — A Unix path supplied to delete_repository_from_graph should resolve
  - `test_purges_dangling_pathless_modules(self)` — [`L753`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L753) — Pathless Module nodes (C #includes) must be removed after repo delete.
  - `test_purges_labels_discovered_dynamically(self)` — [`L809`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L809) — Should DETACH DELETE every label that `CALL db.labels()` reports,
  - `test_returns_false_when_repo_not_found(self)` — [`L737`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L737)
  - `test_returns_true_when_repo_found(self)` — [`L747`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L747)
  - `test_uses_starts_with_prefix_for_scope(self)` — [`L783`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L783) — Queries should scope deletion to the repository path prefix.
- protocol/private: `_DEFAULT_DB_LABELS`[`L721`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L721)
- uses (calls/refs, reference-scoped): (5 test-only callers)

### `TestGraphBuilderMethodsExist`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:959`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L959)
- doc: Smoke tests confirming all new/changed methods are present.
- signature: `class TestGraphBuilderMethodsExist:`
- members:
  - `test_create_all_function_calls_exists(self)` — [`L966`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L966)
  - `test_delete_inherits_for_files_exists(self)` — [`L974`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L974)
  - `test_delete_outgoing_calls_from_files_exists(self)` — [`L970`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L970)
  - `test_get_caller_file_paths_exists(self)` — [`L978`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L978)
  - `test_get_inheritance_neighbor_paths_exists(self)` — [`L982`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L982)
  - `test_get_repo_class_lookup_exists(self)` — [`L986`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L986)
  - `test_resolve_function_call_exists(self)` — [`L962`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L962)

### `TestResolveFunctionCall`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:100`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L100)
- doc: Tests for the _resolve_function_call helper (Change 2).
- signature: `class TestResolveFunctionCall:`
- members:
  - `test_file_type_returned_when_no_caller_context(self)` — [`L210`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L210)
  - `test_resolves_aliased_import_to_original_symbol(self)` — [`L161`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L161)
  - `test_resolves_local_function_call(self)` — [`L119`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L119)
  - `test_resolves_self_method_call(self)` — [`L134`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L134)
  - `test_resolves_via_imports_map(self)` — [`L147`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L147)
  - `test_returns_none_for_builtin(self)` — [`L114`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L114)
  - `test_skip_external_false_still_returns_something(self)` — [`L197`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L197) — skip_external=False should NOT suppress unresolved calls.
  - `test_skip_external_suppresses_unresolved(self)` — [`L184`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L184) — When skip_external=True, calls that cannot be resolved should return None.
- protocol/private: `_call`[`L103`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L103)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestWatcherIncrementalHandleModification`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:1057`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1057)
- doc: Change 5/6: _handle_modification uses incremental O(k) relinking.
- signature: `class TestWatcherIncrementalHandleModification:`
- members:
  - `test_handle_modification_calls_create_all_function_calls(self)` — [`L1108`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1108) — After relinking, link_function_calls must be called for the subset.
  - `test_handle_modification_calls_delete_outgoing(self)` — [`L1060`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1060) — When callers exist, delete_outgoing_calls_from_files must be called.
  - `test_handle_modification_skips_delete_when_no_callers(self)` — [`L1084`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1084) — When no callers exist, delete_outgoing_calls_from_files must NOT be called.

### `TestWatcherMemoryClear`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:1019`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1019)
- doc: Change 4: all_file_data.clear() after the linking pass in _initial_scan.
- signature: `class TestWatcherMemoryClear:`
- members:
  - `test_all_file_data_is_empty_after_initial_scan(self)` — [`L1029`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1029) — Simulate _initial_scan: after the call, self.all_file_data must be empty.
  - `test_initial_scan_clears_all_file_data(self)` — [`L1022`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1022)

### `TestWriteOrmMappingsDatasourceName`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:1133`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1133)
- doc: Regression test for bug: DbTable.datasource_name is null when write_query_links
- signature: `class TestWriteOrmMappingsDatasourceName:`
- members:
  - `test_on_match_set_present_in_write_orm_mappings(self)` — [`L1151`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1151) — write_orm_mappings Cypher must include ON MATCH SET so datasource_name
  - `test_orm_batch_sets_datasource_name_on_existing_node(self)` — [`L1165`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1165) — write_orm_mappings must emit an ON MATCH SET clause that populates
- protocol/private: `_make_writer`[`L1139`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L1139)

### `_DeleteRepoSession`  ·  implements/extends _RecordingSession
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:686`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L686)
- doc: RecordingSession that intercepts label-discovery queries and
- signature: `class _DeleteRepoSession(_RecordingSession):`
- members:
  - `run(self, query: str, **kwargs)` — [`L699`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L699)
- protocol/private: `__init__`[`L695`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L695), `_labels`[`L697`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L697)
- uses (calls/refs, reference-scoped): (6 test-only callers)
- used by: (5 test-only callers)

### `_FakeDBManager`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:70`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L70)
- doc: Minimal stub that satisfies GraphWriter's backend detection.
- signature: `class _FakeDBManager:`
- members:
  - `get_backend_type(self)` — [`L76`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L76)
- protocol/private: `__init__`[`L73`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L73), `_backend`[`L74`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L74)
- used by: (1 test-only callers)

### `_FakeDriver`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:62`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L62)
- signature: `class _FakeDriver:`
- members:
  - `session(self)` — [`L66`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L66)
- protocol/private: `__init__`[`L63`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L63), `_session`[`L64`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L64)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `_FakeResult`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:26`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L26)
- signature: `class _FakeResult:`
- members:
  - `single(self)` — [`L30`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L30)
- protocol/private: `__init__`[`L27`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L27), `__iter__`[`L33`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L33), `_rows`[`L28`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L28)
- used by: (17 test-only callers)

### `_RecordingSession`
- def: [`tests/unit/tools/test_graph_builder_perf_fixes.py:37`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L37)
- doc: Records every (query, kwargs) pair passed to .run().
- signature: `class _RecordingSession:`
- members:
  - `run(self, query: str, **kwargs)` — [`L45`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L45)
  - `calls` — [`L41`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L41)
- protocol/private: `__enter__`[`L55`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L55), `__exit__`[`L58`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L58), `__init__`[`L40`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L40), `_call_idx`[`L43`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L43), `_responses`[`L42`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L42)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (29 test-only callers)

## Functions
- `_make_graph_builder(session: Optional[_RecordingSession] = None, backend: str = "neo4j")` — [`L80`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_graph_builder_perf_fixes.py#L80) — Return a GraphBuilder with a fake driver. Skips full __init__ setup.

