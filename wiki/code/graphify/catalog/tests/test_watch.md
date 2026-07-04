---
title: 'Module: tests/test_watch.py'
type: catalog
provenance: extracted
module: tests/test_watch.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_watch`/
symbols:
  _shrink_payload: _shrink_payload().
  test_rebuild_code_evicts_removed_symbol_from_surviving_file: test_rebuild_code_evicts_removed_symbol_from_surviving_file().
  test_watch_loads_graphifyignore_once: test_watch_loads_graphifyignore_once().
  test_rebuild_code_merges_pending_on_acquire: test_rebuild_code_merges_pending_on_acquire().
  test_rebuild_code_full_corpus_skips_pending_queue: test_rebuild_code_full_corpus_skips_pending_queue().
  test_queue_and_drain_pending_round_trip: test_queue_and_drain_pending_round_trip().
  test_rebuild_code_queues_on_lock_contention: test_rebuild_code_queues_on_lock_contention().
  test_rebuild_code_drains_late_arrivals: test_rebuild_code_drains_late_arrivals().
  test_watch_raises_without_watchdog: test_watch_raises_without_watchdog().
  test_rebuild_code_prunes_final_deleted_file: test_rebuild_code_prunes_final_deleted_file().
  test_rebuild_code_prunes_renamed_source_not_listed_by_hook: test_rebuild_code_prunes_renamed_source_not_listed_by_hook().
  test_rebuild_code_preupgrade_marker_less_node_one_cycle_lag: test_rebuild_code_preupgrade_marker_less_node_one_cycle_lag().
  test_rebuild_code_is_idempotent_when_cluster_ids_flap: test_rebuild_code_is_idempotent_when_cluster_ids_flap().
  test_rebuild_code_skips_cluster_when_topology_unchanged: test_rebuild_code_skips_cluster_when_topology_unchanged().
  test_watch_handler_honors_graphifyignore: test_watch_handler_honors_graphifyignore().
  test_check_shrink_blocks_silent_shrink: test_check_shrink_blocks_silent_shrink().
  test_check_shrink_allows_force_override: test_check_shrink_allows_force_override().
  test_check_shrink_allows_explicit_deletions: test_check_shrink_allows_explicit_deletions().
  test_check_shrink_allows_no_existing_data: test_check_shrink_allows_no_existing_data().
  test_check_shrink_allows_growth: test_check_shrink_allows_growth().
  test_check_shrink_unlinks_tmp_on_refuse: test_check_shrink_unlinks_tmp_on_refuse().
  test_check_shrink_keeps_tmp_when_deletions_declared: test_check_shrink_keeps_tmp_when_deletions_declared().
  test_drain_pending_dedupes_and_skips_blank_lines: test_drain_pending_dedupes_and_skips_blank_lines().
  test_queue_pending_noop_on_empty_list: test_queue_pending_noop_on_empty_list().
  test_rebuild_code_drains_late_arrivals.fake_inner: test_rebuild_code_drains_late_arrivals().fake_inner().
  test_rebuild_code_preupgrade_marker_less_node_one_cycle_lag.labels: test_rebuild_code_preupgrade_marker_less_node_one_cycle_lag().labels().
  test_notify_only_creates_flag: test_notify_only_creates_flag().
  test_notify_only_creates_flag_dir: test_notify_only_creates_flag_dir().
  test_notify_only_idempotent: test_notify_only_idempotent().
  test_watched_extensions_includes_code: test_watched_extensions_includes_code().
  test_watched_extensions_includes_docs: test_watched_extensions_includes_docs().
  test_watched_extensions_includes_images: test_watched_extensions_includes_images().
  test_watched_extensions_excludes_noise: test_watched_extensions_excludes_noise().
  test_check_update_no_flag_returns_true: test_check_update_no_flag_returns_true().
  test_check_update_with_flag_returns_true_and_prints: test_check_update_with_flag_returns_true_and_prints().
  test_check_update_does_not_clear_flag: test_check_update_does_not_clear_flag().
  test_rebuild_lock_writes_pid_with_newline: test_rebuild_lock_writes_pid_with_newline().
  test_rebuild_lock_removed_after_release: test_rebuild_lock_removed_after_release().
  test_rebuild_lock_does_not_accumulate_pids_across_runs: test_rebuild_lock_does_not_accumulate_pids_across_runs().
  test_graphify_root_preserves_relative_when_invoked_with_relative_path: test_graphify_root_preserves_relative_when_invoked_with_relative_path().
  test_graphify_root_preserves_absolute_when_user_supplied: test_graphify_root_preserves_absolute_when_user_supplied().
  test_rebuild_code_evicts_nodes_from_deleted_files: test_rebuild_code_evicts_nodes_from_deleted_files().
  test_rebuild_code_normalizes_preserved_source_paths: test_rebuild_code_normalizes_preserved_source_paths().
  test_rebuild_code_prunes_renamed_ast_backed_document: test_rebuild_code_prunes_renamed_ast_backed_document().
  test_rebuild_lock_non_blocking_does_not_clobber_holder: test_rebuild_lock_non_blocking_does_not_clobber_holder().
  test_check_shrink_allows_shrink_within_rebuilt_sources: test_check_shrink_allows_shrink_within_rebuilt_sources().
  test_check_shrink_blocks_shrink_outside_rebuilt_sources: test_check_shrink_blocks_shrink_outside_rebuilt_sources().
  test_rebuild_code_prunes_deleted_file_nodes: test_rebuild_code_prunes_deleted_file_nodes().
  test_rebuild_code_accepts_repo_relative_changed_path_for_subdir_root: test_rebuild_code_accepts_repo_relative_changed_path_for_subdir_root().
  test_rebuild_code_subdir_preserves_outside_ast_nodes: test_rebuild_code_subdir_preserves_outside_ast_nodes().
  test_rebuild_code_subdir_survives_absolute_to_relative_invocation: test_rebuild_code_subdir_survives_absolute_to_relative_invocation().
  test_rebuild_code_prunes_legacy_watch_relative_subdir_source: test_rebuild_code_prunes_legacy_watch_relative_subdir_source().
  test_rebuild_code_does_not_update_root_marker_when_write_is_refused: test_rebuild_code_does_not_update_root_marker_when_write_is_refused().
  test_rebuild_code_incremental_rename_preserves_symlink_source_path: test_rebuild_code_incremental_rename_preserves_symlink_source_path().
  test_merge_changed_paths_dedupes_in_order: test_merge_changed_paths_dedupes_in_order().
  _add_unrelated_semantic_pair: _add_unrelated_semantic_pair().
  test_rebuild_code_evicts_removed_symbol_from_surviving_file.labels: test_rebuild_code_evicts_removed_symbol_from_surviving_file().labels().
  test_rebuild_code_evicts_removed_symbol_from_surviving_file.id_for: test_rebuild_code_evicts_removed_symbol_from_surviving_file().id_for().
  test_rebuild_code_evicts_removed_symbol_from_surviving_file.edges: test_rebuild_code_evicts_removed_symbol_from_surviving_file().edges().
  _watchdog_available: _watchdog_available().
  test_watch_raises_without_watchdog.mock_import: test_watch_raises_without_watchdog().mock_import().
  test_rebuild_code_is_idempotent_when_cluster_ids_flap.flaky_cluster: test_rebuild_code_is_idempotent_when_cluster_ids_flap().flaky_cluster().
  test_rebuild_code_skips_cluster_when_topology_unchanged.cluster_once: test_rebuild_code_skips_cluster_when_topology_unchanged().cluster_once().
  test_watch_loads_graphifyignore_once.counting_loader: test_watch_loads_graphifyignore_once().counting_loader().
  test_rebuild_code_merges_pending_on_acquire.recording_inner: test_rebuild_code_merges_pending_on_acquire().recording_inner().
  test_rebuild_code_full_corpus_skips_pending_queue.fake_inner: test_rebuild_code_full_corpus_skips_pending_queue().fake_inner().
---
# Module: [`tests/test_watch.py`](../../../../../raw/code/graphify/tests/test_watch.py)

## Functions
- `_add_unrelated_semantic_pair(graph_path)` — [`L210`](../../../../../raw/code/graphify/tests/test_watch.py#L210)
- `_shrink_payload(n: int)` — [`L666`](../../../../../raw/code/graphify/tests/test_watch.py#L666) — Build a minimal graph-data dict with *n* placeholder nodes.
- `_watchdog_available()` — [`L574`](../../../../../raw/code/graphify/tests/test_watch.py#L574)
- `cluster_once(G)` — [`L557`](../../../../../raw/code/graphify/tests/test_watch.py#L557)
- `counting_loader(root)` — [`L644`](../../../../../raw/code/graphify/tests/test_watch.py#L644)
- `edges(d)` — [`L398`](../../../../../raw/code/graphify/tests/test_watch.py#L398)
- `fake_inner(watch_path, **kwargs)` — [`L1243`](../../../../../raw/code/graphify/tests/test_watch.py#L1243)
- `fake_inner(watch_path, **kwargs)` — [`L1284`](../../../../../raw/code/graphify/tests/test_watch.py#L1284)
- `flaky_cluster(G)` — [`L524`](../../../../../raw/code/graphify/tests/test_watch.py#L524)
- `id_for(d, label)` — [`L395`](../../../../../raw/code/graphify/tests/test_watch.py#L395)
- `labels(d)` — [`L392`](../../../../../raw/code/graphify/tests/test_watch.py#L392)
- `labels(d)` — [`L459`](../../../../../raw/code/graphify/tests/test_watch.py#L459)
- `mock_import(name, *args, **kwargs)` — [`L93`](../../../../../raw/code/graphify/tests/test_watch.py#L93)
- `recording_inner(watch_path, **kwargs)` — [`L1206`](../../../../../raw/code/graphify/tests/test_watch.py#L1206)
- `test_check_shrink_allows_explicit_deletions(capsys)` — [`L694`](../../../../../raw/code/graphify/tests/test_watch.py#L694) — Caller declared deletions → shrink is expected → guard skipped silently.
- `test_check_shrink_allows_force_override()` — [`L684`](../../../../../raw/code/graphify/tests/test_watch.py#L684) — force=True bypasses the guard regardless of node delta.
- `test_check_shrink_allows_growth()` — [`L747`](../../../../../raw/code/graphify/tests/test_watch.py#L747) — new > existing is always fine.
- `test_check_shrink_allows_no_existing_data()` — [`L707`](../../../../../raw/code/graphify/tests/test_watch.py#L707) — First-run case: no existing graph → guard inert.
- `test_check_shrink_allows_shrink_within_rebuilt_sources(capsys)` — [`L717`](../../../../../raw/code/graphify/tests/test_watch.py#L717) — #1116: a symbol removed from a re-extracted file is a legitimate shrink —
- `test_check_shrink_blocks_shrink_outside_rebuilt_sources(capsys)` — [`L734`](../../../../../raw/code/graphify/tests/test_watch.py#L734) — The guard's real job is intact: a node lost from a file we did NOT re-extract
- `test_check_shrink_blocks_silent_shrink(capsys)` — [`L671`](../../../../../raw/code/graphify/tests/test_watch.py#L671) — Default case: smaller new graph + no force + no declared deletions = refuse.
- `test_check_shrink_keeps_tmp_when_deletions_declared(tmp_path)` — [`L771`](../../../../../raw/code/graphify/tests/test_watch.py#L771) — Mirror of the above: if the caller declared deletions, the tmp file is NOT unlinked
- `test_check_shrink_unlinks_tmp_on_refuse(tmp_path)` — [`L757`](../../../../../raw/code/graphify/tests/test_watch.py#L757) — When refusing, the temp graph file gets cleaned up so it can't leak across runs.
- `test_check_update_does_not_clear_flag(tmp_path)` — [`L79`](../../../../../raw/code/graphify/tests/test_watch.py#L79) — check_update never removes the needs_update flag (clearing is LLM's job).
- `test_check_update_no_flag_returns_true(tmp_path)` — [`L61`](../../../../../raw/code/graphify/tests/test_watch.py#L61) — check_update returns True and is silent when needs_update flag is absent.
- `test_check_update_with_flag_returns_true_and_prints(tmp_path, capsys)` — [`L67`](../../../../../raw/code/graphify/tests/test_watch.py#L67) — check_update returns True and prints notification when flag exists.
- `test_drain_pending_dedupes_and_skips_blank_lines(tmp_path)` — [`L1130`](../../../../../raw/code/graphify/tests/test_watch.py#L1130) — Repeated appends across concurrent contenders must dedupe; partial
- `test_graphify_root_preserves_absolute_when_user_supplied(tmp_path)` — [`L163`](../../../../../raw/code/graphify/tests/test_watch.py#L163) — When the caller supplies an absolute path, ``.graphify_root`` stores
- `test_graphify_root_preserves_relative_when_invoked_with_relative_path(tmp_path, monkeypatch)` — [`L144`](../../../../../raw/code/graphify/tests/test_watch.py#L144) — #777: ``.graphify_root`` stores the user-supplied path (``.``), not the
- `test_merge_changed_paths_dedupes_in_order()` — [`L1301`](../../../../../raw/code/graphify/tests/test_watch.py#L1301) — _merge_changed_paths preserves first-seen order and drops dupes.
- `test_notify_only_creates_flag(tmp_path)` — [`L15`](../../../../../raw/code/graphify/tests/test_watch.py#L15)
- `test_notify_only_creates_flag_dir(tmp_path)` — [`L21`](../../../../../raw/code/graphify/tests/test_watch.py#L21)
- `test_notify_only_idempotent(tmp_path)` — [`L27`](../../../../../raw/code/graphify/tests/test_watch.py#L27)
- `test_queue_and_drain_pending_round_trip(tmp_path)` — [`L1107`](../../../../../raw/code/graphify/tests/test_watch.py#L1107) — _queue_pending writes one path per line; _drain_pending reads + unlinks
- `test_queue_pending_noop_on_empty_list(tmp_path)` — [`L1146`](../../../../../raw/code/graphify/tests/test_watch.py#L1146) — Empty change set must not create an empty .pending_changes file.
- `test_rebuild_code_accepts_repo_relative_changed_path_for_subdir_root(tmp_path)` — [`L851`](../../../../../raw/code/graphify/tests/test_watch.py#L851) — #1348: git-hook paths are repo-root-relative even when the graph root is a subdir.
- `test_rebuild_code_does_not_update_root_marker_when_write_is_refused(tmp_path, monkeypatch)` — [`L1029`](../../../../../raw/code/graphify/tests/test_watch.py#L1029) — A rejected candidate keeps the marker paired with the existing graph.
- `test_rebuild_code_drains_late_arrivals(tmp_path, monkeypatch)` — [`L1231`](../../../../../raw/code/graphify/tests/test_watch.py#L1231) — #1059: after the primary rebuild, the lock-holder must loop and drain
- `test_rebuild_code_evicts_nodes_from_deleted_files(tmp_path)` — [`L179`](../../../../../raw/code/graphify/tests/test_watch.py#L179) — #1007: graphify update (_rebuild_code with no changed_paths) must remove
- `test_rebuild_code_evicts_removed_symbol_from_surviving_file(tmp_path)` — [`L371`](../../../../../raw/code/graphify/tests/test_watch.py#L371) — #1116: graphify update (_rebuild_code with no changed_paths) must prune a
- `test_rebuild_code_full_corpus_skips_pending_queue(tmp_path, monkeypatch)` — [`L1268`](../../../../../raw/code/graphify/tests/test_watch.py#L1268) — #1059: changed_paths=None means a full-corpus rebuild — the queue
- `test_rebuild_code_incremental_rename_preserves_symlink_source_path(tmp_path)` — [`L1056`](../../../../../raw/code/graphify/tests/test_watch.py#L1056) — Changed files under followed symlinks retain their watched lexical path.
- `test_rebuild_code_is_idempotent_when_cluster_ids_flap(tmp_path, monkeypatch)` — [`L515`](../../../../../raw/code/graphify/tests/test_watch.py#L515)
- `test_rebuild_code_merges_pending_on_acquire(tmp_path, monkeypatch)` — [`L1191`](../../../../../raw/code/graphify/tests/test_watch.py#L1191) — #1059: the process that acquires the lock must drain .pending_changes
- `test_rebuild_code_normalizes_preserved_source_paths(tmp_path)` — [`L314`](../../../../../raw/code/graphify/tests/test_watch.py#L314) — An incremental rebuild must not treat ./foo.py as a deleted live source.
- `test_rebuild_code_preupgrade_marker_less_node_one_cycle_lag(tmp_path)` — [`L441`](../../../../../raw/code/graphify/tests/test_watch.py#L441) — #1118 backward-compat: a graph.json built before #1116 has no `_origin`
- `test_rebuild_code_prunes_deleted_file_nodes(tmp_path)` — [`L792`](../../../../../raw/code/graphify/tests/test_watch.py#L792) — End-to-end probe of the post-commit-delete bug fix.
- `test_rebuild_code_prunes_final_deleted_file(tmp_path, changed_paths)` — [`L234`](../../../../../raw/code/graphify/tests/test_watch.py#L234) — Deleting the final code file must reconcile the existing graph.
- `test_rebuild_code_prunes_legacy_watch_relative_subdir_source(tmp_path)` — [`L992`](../../../../../raw/code/graphify/tests/test_watch.py#L992) — Pre-rebase subdirectory graphs stored source_file relative to watch_root.
- `test_rebuild_code_prunes_renamed_ast_backed_document(tmp_path)` — [`L345`](../../../../../raw/code/graphify/tests/test_watch.py#L345) — Destination-only rename reconciliation also covers AST-backed docs.
- `test_rebuild_code_prunes_renamed_source_not_listed_by_hook(tmp_path)` — [`L281`](../../../../../raw/code/graphify/tests/test_watch.py#L281) — A hook-style rename list may contain only the destination path.
- `test_rebuild_code_queues_on_lock_contention(tmp_path, monkeypatch, capsys)` — [`L1156`](../../../../../raw/code/graphify/tests/test_watch.py#L1156) — #1059: when the rebuild lock is held, an incremental hook must queue
- `test_rebuild_code_skips_cluster_when_topology_unchanged(tmp_path, monkeypatch)` — [`L548`](../../../../../raw/code/graphify/tests/test_watch.py#L548)
- `test_rebuild_code_subdir_preserves_outside_ast_nodes(tmp_path, changed_paths)` — [`L890`](../../../../../raw/code/graphify/tests/test_watch.py#L890) — A full rebuild of a subdirectory must not prune graph data outside it.
- `test_rebuild_code_subdir_survives_absolute_to_relative_invocation(tmp_path)` — [`L953`](../../../../../raw/code/graphify/tests/test_watch.py#L953) — Persisted source paths keep their meaning when invocation style changes.
- `test_rebuild_lock_does_not_accumulate_pids_across_runs(tmp_path)` — [`L131`](../../../../../raw/code/graphify/tests/test_watch.py#L131) — GH-858: each acquisition truncates and rewrites the PID line rather
- `test_rebuild_lock_non_blocking_does_not_clobber_holder(tmp_path)` — [`L501`](../../../../../raw/code/graphify/tests/test_watch.py#L501) — GH-858: a non-blocking caller that fails to acquire the lock must not
- `test_rebuild_lock_removed_after_release(tmp_path)` — [`L120`](../../../../../raw/code/graphify/tests/test_watch.py#L120) — GH-858: lock file must be unlinked once the rebuild completes so
- `test_rebuild_lock_writes_pid_with_newline(tmp_path)` — [`L109`](../../../../../raw/code/graphify/tests/test_watch.py#L109)
- `test_watch_handler_honors_graphifyignore(tmp_path, monkeypatch)` — [`L583`](../../../../../raw/code/graphify/tests/test_watch.py#L583) — gh-928: the watch Handler must short-circuit paths matching
- `test_watch_loads_graphifyignore_once(tmp_path, monkeypatch)` — [`L629`](../../../../../raw/code/graphify/tests/test_watch.py#L629) — gh-928: .graphifyignore must be parsed exactly once at watch() startup,
- `test_watch_raises_without_watchdog(tmp_path, monkeypatch)` — [`L89`](../../../../../raw/code/graphify/tests/test_watch.py#L89)
- `test_watched_extensions_excludes_noise()` — [`L51`](../../../../../raw/code/graphify/tests/test_watch.py#L51)
- `test_watched_extensions_includes_code()` — [`L36`](../../../../../raw/code/graphify/tests/test_watch.py#L36)
- `test_watched_extensions_includes_docs()` — [`L42`](../../../../../raw/code/graphify/tests/test_watch.py#L42)
- `test_watched_extensions_includes_images()` — [`L47`](../../../../../raw/code/graphify/tests/test_watch.py#L47)

