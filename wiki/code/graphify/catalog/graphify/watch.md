---
title: 'Module: graphify/watch.py'
type: catalog
provenance: extracted
module: graphify/watch.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.watch`/
symbols:
  _rebuild_code: _rebuild_code().
  _reconcile_existing_graph: _reconcile_existing_graph().
  _WATCHED_EXTENSIONS: _WATCHED_EXTENSIONS.
  watch: watch().
  _check_shrink: _check_shrink().
  _StoredSourcePaths.identity: _StoredSourcePaths#identity().
  _queue_pending: _queue_pending().
  _StoredSourcePaths.rebase_preserved: _StoredSourcePaths#rebase_preserved().
  _PENDING_FILENAME: _PENDING_FILENAME.
  _drain_pending: _drain_pending().
  check_update: check_update().
  _StoredSourcePaths.in_watch_root: _StoredSourcePaths#in_watch_root().
  args: args.
  _rebuild_lock: _rebuild_lock().
  _notify_only: _notify_only().
  watch.Handler.on_any_event: watch().Handler#on_any_event().
  _StoredSourcePaths.normalize: _StoredSourcePaths#normalize().
  _StoredSourcePaths.absolute_identity: _StoredSourcePaths#absolute_identity().
  _StoredSourcePaths.existing_source_root: _StoredSourcePaths#existing_source_root.
  _StoredSourcePaths.is_evicted: _StoredSourcePaths#is_evicted().
  parser: parser.
  _is_relative_to: _is_relative_to().
  _CODE_EXTENSIONS: _CODE_EXTENSIONS.
  _StoredSourcePaths.legacy_watch_relative: _StoredSourcePaths#legacy_watch_relative.
  _rebuild_code._add_deleted_source: _rebuild_code()._add_deleted_source().
  _canonical_graph_for_compare: _canonical_graph_for_compare().
  _relativize_source_files: _relativize_source_files().
  _check_shrink._accounted: _check_shrink()._accounted().
  _has_non_code: _has_non_code().
  _merge_changed_paths: _merge_changed_paths().
  _StoredSourcePaths.watch_root: _StoredSourcePaths#watch_root.
  _StoredSourcePaths._normalize_source: _StoredSourcePaths#_normalize_source.
  _StoredSourcePaths.project_root: _StoredSourcePaths#project_root.
  _canonical_topology_for_compare: _canonical_topology_for_compare().
  _report_for_compare: _report_for_compare().
  _PENDING_DRAIN_MAX_PASSES: _PENDING_DRAIN_MAX_PASSES.
  _git_head: _git_head().
  _report_root_label: _report_root_label().
  _changed_path_candidates: _changed_path_candidates().
  _rebase_relative_source_files: _rebase_relative_source_files().
  _StoredSourcePaths: _StoredSourcePaths#
  _node_community_map: _node_community_map().
  _topology_from_graph: _topology_from_graph().
  _json_text: _json_text().
  watch.Handler: watch().Handler#
  _apply_resource_limits: _apply_resource_limits().
  _StoredSourcePaths.__init__: _StoredSourcePaths#__init__().
---
# Module: [`graphify/watch.py`](../../../../../raw/code/graphify/graphify/watch.py)

## Classes
### `Handler`
- def: [`graphify/watch.py:1138`](../../../../../raw/code/graphify/graphify/watch.py#L1138)
- signature: `class Handler(FileSystemEventHandler):`
- members:
  - `on_any_event(self, event)` — [`L1139`](../../../../../raw/code/graphify/graphify/watch.py#L1139)
- uses (calls/refs, reference-scoped): [`GRAPHIFY_OUT`](paths.md#GRAPHIFY_OUT), [`_is_ignored`](detect.md#_is_ignored), [`_WATCHED_EXTENSIONS`](watch.md#_WATCHED_EXTENSIONS)
- used by: [`watch`](watch.md#watch)

### `_StoredSourcePaths`
- def: [`graphify/watch.py:276`](../../../../../raw/code/graphify/graphify/watch.py#L276)
- doc: Resolve source_file values across current and legacy graph roots.
- signature: `class _StoredSourcePaths:`
- members:
  - `absolute_identity(self, source_file: str | None, root: Path)` — [`L331`](../../../../../raw/code/graphify/graphify/watch.py#L331)
  - `identity(self, source_file: str | None)` — [`L340`](../../../../../raw/code/graphify/graphify/watch.py#L340)
  - `in_watch_root(self, source_file: str | None)` — [`L346`](../../../../../raw/code/graphify/graphify/watch.py#L346)
  - `is_evicted(self, item: dict, identities: set[str])` — [`L350`](../../../../../raw/code/graphify/graphify/watch.py#L350)
  - `normalize(self, source_file: str | None)` — [`L327`](../../../../../raw/code/graphify/graphify/watch.py#L327)
  - `rebase_preserved(self, item: dict)` — [`L353`](../../../../../raw/code/graphify/graphify/watch.py#L353)
  - `existing_source_root` — [`L291`](../../../../../raw/code/graphify/graphify/watch.py#L291)
  - `legacy_watch_relative` — [`L308`](../../../../../raw/code/graphify/graphify/watch.py#L308)
  - `project_root` — [`L288`](../../../../../raw/code/graphify/graphify/watch.py#L288)
  - `watch_root` — [`L289`](../../../../../raw/code/graphify/graphify/watch.py#L289)
- protocol/private: `__init__`[`L279`](../../../../../raw/code/graphify/graphify/watch.py#L279), `_normalize_source`[`L290`](../../../../../raw/code/graphify/graphify/watch.py#L290)
- uses (calls/refs, reference-scoped): [`_is_relative_to`](watch.md#_is_relative_to)
- used by: [`_reconcile_existing_graph`](watch.md#_reconcile_existing_graph)

## Functions
- `_accounted(n: dict)` — [`L633`](../../../../../raw/code/graphify/graphify/watch.py#L633)
- `_add_deleted_source(path: Path)` — [`L777`](../../../../../raw/code/graphify/graphify/watch.py#L777)
- `_apply_resource_limits()` — [`L153`](../../../../../raw/code/graphify/graphify/watch.py#L153) — Best-effort nice + memory cap. Called from inline hook scripts.
- `_canonical_graph_for_compare(graph_data: dict)` — [`L516`](../../../../../raw/code/graphify/graphify/watch.py#L516)
- `_canonical_topology_for_compare(graph_data: dict)` — [`L528`](../../../../../raw/code/graphify/graphify/watch.py#L528)
- `_changed_path_candidates(raw: Path, *, change_root: Path, watch_root: Path)` — [`L218`](../../../../../raw/code/graphify/graphify/watch.py#L218) — Return plausible absolute locations for a hook-provided changed path.
- `_check_shrink(force: bool, existing_data: dict, new_data: dict, tmp: Path | None = None, *, had_explicit_deletions: bool = False, rebuilt_sources: set[str] | None = None)` — [`L594`](../../../../../raw/code/graphify/graphify/watch.py#L594) — Return True (ok to proceed) or False (shrink refused).
- `_drain_pending(out_dir: Path)` — [`L40`](../../../../../raw/code/graphify/graphify/watch.py#L40) — Read + unlink ``out_dir/.pending_changes`` and return deduplicated paths.
- `_git_head()` — [`L181`](../../../../../raw/code/graphify/graphify/watch.py#L181) — Return current git HEAD commit hash, or None outside a repo.
- `_has_non_code(changed_paths: list[Path])` — [`L1103`](../../../../../raw/code/graphify/graphify/watch.py#L1103)
- `_is_relative_to(path: Path, root: Path)` — [`L210`](../../../../../raw/code/graphify/graphify/watch.py#L210)
- `_json_text(data: dict)` — [`L656`](../../../../../raw/code/graphify/graphify/watch.py#L656)
- `_merge_changed_paths(*sources: list[Path] | None)` — [`L72`](../../../../../raw/code/graphify/graphify/watch.py#L72) — Concatenate path lists, preserving order and dropping duplicates.
- `_node_community_map(graph_data: dict)` — [`L497`](../../../../../raw/code/graphify/graphify/watch.py#L497)
- `_notify_only(watch_path: Path)` — [`L1092`](../../../../../raw/code/graphify/graphify/watch.py#L1092) — Write a flag file and print a notification (fallback for non-code-only corpora).
- `_queue_pending(out_dir: Path, changed_paths: list[Path])` — [`L18`](../../../../../raw/code/graphify/graphify/watch.py#L18) — Append ``changed_paths`` to ``out_dir/.pending_changes`` (one per line).
- `_rebase_relative_source_files(payload: dict, source_root: Path, target_root: Path)` — [`L261`](../../../../../raw/code/graphify/graphify/watch.py#L261) — Rebase cache-root-relative source paths onto the project root.
- `_rebuild_code(watch_path: Path, *, changed_paths: list[Path] | None = None, follow_symlinks: bool = False, force: bool = False, no_cluster: bool = False, acquire_lock: bool = True, block_on_lock: bool = False)` — [`L660`](../../../../../raw/code/graphify/graphify/watch.py#L660) — Re-run AST extraction + build + optional cluster + report for code files. No LLM needed. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `_rebuild_lock(out_dir: Path, *, blocking: bool = False)` — [`L94`](../../../../../raw/code/graphify/graphify/watch.py#L94) — Per-repo advisory lock around a rebuild.
- `_reconcile_existing_graph(existing_graph: Path, result: dict, *, out: Path, project_root: Path, watch_root: Path, code_files: list[Path], extract_targets: list[Path], full_rebuild: bool, deleted_paths: set[str], deleted_source_identities: set[str])` — [`L369`](../../../../../raw/code/graphify/graphify/watch.py#L369) — Merge fresh extraction with preserved graph entries and evict stale sources. — documented in [graphify-security](../../concepts/graphify-security.md)
- `_relativize_source_files(payload: dict, root: Path, *, scope: Path | None = None)` — [`L243`](../../../../../raw/code/graphify/graphify/watch.py#L243)
- `_report_for_compare(report_text: str)` — [`L652`](../../../../../raw/code/graphify/graphify/watch.py#L652)
- `_report_root_label(watch_path: Path)` — [`L204`](../../../../../raw/code/graphify/graphify/watch.py#L204)
- `_topology_from_graph(G)` — [`L584`](../../../../../raw/code/graphify/graphify/watch.py#L584)
- `check_update(watch_path: Path)` — [`L1077`](../../../../../raw/code/graphify/graphify/watch.py#L1077) — Check for pending semantic update flag and notify the user if set.
- `watch(watch_path: Path, debounce: float = 3)` — [`L1107`](../../../../../raw/code/graphify/graphify/watch.py#L1107) — Watch watch_path for new or modified files and auto-update the graph. — documented in [graphify-watch](../../concepts/graphify-watch.md)

## Module values
- `_CODE_EXTENSIONS` — [`L201`](../../../../../raw/code/graphify/graphify/watch.py#L201)
- `_PENDING_DRAIN_MAX_PASSES` — [`L15`](../../../../../raw/code/graphify/graphify/watch.py#L15)
- `_PENDING_FILENAME` — [`L14`](../../../../../raw/code/graphify/graphify/watch.py#L14)
- `_WATCHED_EXTENSIONS` — [`L200`](../../../../../raw/code/graphify/graphify/watch.py#L200) — documented in [graphify-watch](../../concepts/graphify-watch.md)
- `args` — [`L1203`](../../../../../raw/code/graphify/graphify/watch.py#L1203)
- `parser` — [`L1199`](../../../../../raw/code/graphify/graphify/watch.py#L1199)

