---
title: 'Module: src/codegraphcontext/core/watcher.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/watcher.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.watcher`/
symbols:
  RepositoryEventHandler._handle_modification: RepositoryEventHandler#_handle_modification().
  RepositoryEventHandler.synchronize_with_disk: RepositoryEventHandler#synchronize_with_disk().
  RepositoryEventHandler._initial_scan: RepositoryEventHandler#_initial_scan().
  RepositoryEventHandler.graph_builder: RepositoryEventHandler#graph_builder.
  RepositoryEventHandler.imports_map: RepositoryEventHandler#imports_map.
  CodeWatcher.watch_directory: CodeWatcher#watch_directory().
  RepositoryEventHandler.repo_path: RepositoryEventHandler#repo_path.
  RepositoryEventHandler._load_ignore_spec: RepositoryEventHandler#_load_ignore_spec().
  RepositoryEventHandler._iter_supported_files: RepositoryEventHandler#_iter_supported_files().
  RepositoryEventHandler._should_ignore: RepositoryEventHandler#_should_ignore().
  CodeWatcher.unwatch_directory: CodeWatcher#unwatch_directory().
  RepositoryEventHandler._is_supported_code_file: RepositoryEventHandler#_is_supported_code_file().
  RepositoryEventHandler._debounce: RepositoryEventHandler#_debounce().
  RepositoryEventHandler._update_imports_map_for_file: RepositoryEventHandler#_update_imports_map_for_file().
  RepositoryEventHandler.on_created: RepositoryEventHandler#on_created().
  RepositoryEventHandler.on_modified: RepositoryEventHandler#on_modified().
  CodeWatcher.observer: CodeWatcher#observer.
  CodeWatcher.stop: CodeWatcher#stop().
  should_use_polling_observer: should_use_polling_observer().
  CodeWatcher: CodeWatcher#
  RepositoryEventHandler.ignore_spec: RepositoryEventHandler#ignore_spec.
  CodeWatcher.start: CodeWatcher#start().
  RepositoryEventHandler.timers: RepositoryEventHandler#timers.
  RepositoryEventHandler.all_file_data: RepositoryEventHandler#all_file_data.
  RepositoryEventHandler.on_deleted: RepositoryEventHandler#on_deleted().
  RepositoryEventHandler.on_moved: RepositoryEventHandler#on_moved().
  CodeWatcher.watched_paths: CodeWatcher#watched_paths.
  CodeWatcher.handlers: CodeWatcher#handlers.
  RepositoryEventHandler.ignore_root: RepositoryEventHandler#ignore_root.
  CodeWatcher.graph_builder: CodeWatcher#graph_builder.
  RepositoryEventHandler.__init__: RepositoryEventHandler#__init__().
  RepositoryEventHandler.cancel_timers: RepositoryEventHandler#cancel_timers().
  CodeWatcher.__init__: CodeWatcher#__init__().
  CodeWatcher.list_watched_paths: CodeWatcher#list_watched_paths().
  CodeWatcher.watches: CodeWatcher#watches.
  POLLING_ENV_VAR: POLLING_ENV_VAR.
  TRUE_ENV_VALUES: TRUE_ENV_VALUES.
  RepositoryEventHandler: RepositoryEventHandler#
  RepositoryEventHandler.debounce_interval: RepositoryEventHandler#debounce_interval.
---
# Module: [`src/codegraphcontext/core/watcher.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py)

## Classes
### `CodeWatcher`
- def: [`src/codegraphcontext/core/watcher.py:321`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L321)
- signature: `class CodeWatcher:`
- members:
  - `list_watched_paths(self)` — [`L380`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L380)
  - `start(self)` — [`L383`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L383)
  - `stop(self)` — [`L387`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L387)
  - `unwatch_directory(self, path: str)` — [`L365`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L365)
  - `watch_directory(self, path: str, perform_initial_scan: bool = True, cgcignore_path: str = None, sync_on_start: bool = False)` — [`L336`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L336) — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
  - `graph_builder` — [`L328`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L328)
  - `handlers` — [`L334`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L334)
  - `observer` — [`L330`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L330)
  - `watched_paths` — [`L332`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L332)
  - `watches` — [`L333`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L333)
- protocol/private: `__init__`[`L322`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L322)
- uses (calls/refs, reference-scoped): [`GraphBuilder`](../tools/graph_builder.md#GraphBuilder), [`should_use_polling_observer`](watcher.md#should_use_polling_observer), [`RepositoryEventHandler`](watcher.md#RepositoryEventHandler)
- used by: [`switch_context_tool`](../server.md#MCPServer.switch_context_tool), [`watch_helper`](../cli/cli_helpers.md#watch_helper), [`code_watcher`](../server.md#MCPServer.code_watcher), [`shutdown`](../server.md#MCPServer.shutdown), [`run`](../server.md#MCPServer.run), [`_start_watcher_if`](../server.md#MCPServer._start_watcher_if)

### `RepositoryEventHandler`
- def: [`src/codegraphcontext/core/watcher.py:36`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L36)
- signature: `class RepositoryEventHandler(FileSystemEventHandler):`
- members:
  - `_handle_modification(self, event_path_str: str)` — [`L212`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L212) — Incremental update: re-parse and re-link only the changed file and its neighbours. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `_update_imports_map_for_file(self, changed_path: Path)` — [`L194`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L194) — Re-scan a single file and merge its contributions into self.imports_map.
  - `cancel_timers(self)` — [`L189`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L189)
  - `on_created(self, event)` — [`L304`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L304)
  - `on_deleted(self, event)` — [`L312`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L312)
  - `on_modified(self, event)` — [`L308`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L308)
  - `on_moved(self, event)` — [`L316`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L316)
  - `synchronize_with_disk(self)` — [`L150`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L150) — documented in [codegraphcontext-tools-graph_builder](../../../../concepts/codegraphcontext-tools-graph_builder.md)
  - `all_file_data` — [`L57`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L57)
  - `debounce_interval` — [`L50`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L50)
  - `graph_builder` — [`L48`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L48)
  - `ignore_root` — [`L53`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L53)
  - `ignore_spec` — [`L54`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L54)
  - `imports_map` — [`L58`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L58)
  - `repo_path` — [`L49`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L49)
  - `timers` — [`L51`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L51)
- protocol/private: `__init__`[`L37`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L37), `_debounce`[`L182`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L182), `_initial_scan`[`L123`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L123), `_is_supported_code_file`[`L105`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L105), `_iter_supported_files`[`L113`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L113), `_load_ignore_spec`[`L65`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L65), `_should_ignore`[`L80`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L80)
- uses (calls/refs, reference-scoped): [`info_logger`](../utils/debug_log.md#info_logger), [`warning_logger`](../utils/debug_log.md#warning_logger), [`debug_log`](../utils/debug_log.md#debug_log), [`link_inheritance`](../tools/graph_builder.md#GraphBuilder.link_inheritance), [`GraphBuilder`](../tools/graph_builder.md#GraphBuilder), [`get_config_value`](../cli/config_manager.md#get_config_value), [`run_inheritance_reresolve`](../tools/indexing/resolution/post_resolution.md#run_inheritance_reresolve), [`discover_files_to_index`](../tools/indexing/discovery.md#discover_files_to_index), [`run`](../tools/indexing/embeddings.md#EmbeddingPipeline.run), [`parse_file`](../tools/graph_builder.md#GraphBuilder.parse_file), [`link_function_calls`](../tools/graph_builder.md#GraphBuilder.link_function_calls), [`build_ignore_spec`](cgcignore.md#build_ignore_spec), [`update_file_in_graph`](../tools/graph_builder.md#GraphBuilder.update_file_in_graph), [`add_file_to_graph`](../tools/graph_builder.md#GraphBuilder.add_file_to_graph), [`driver`](../tools/graph_builder.md#GraphBuilder.driver), [`pre_scan_imports`](../tools/graph_builder.md#GraphBuilder.pre_scan_imports), [`parsers`](../tools/graph_builder.md#GraphBuilder.parsers), [`DEFAULT_IGNORE_PATTERNS`](../tools/indexing/constants.md#DEFAULT_IGNORE_PATTERNS), [`delete_file_from_graph`](../tools/graph_builder.md#GraphBuilder.delete_file_from_graph), [`delete_inherits_for_files`](../tools/graph_builder.md#GraphBuilder.delete_inherits_for_files), [`delete_outgoing_calls_from_files`](../tools/graph_builder.md#GraphBuilder.delete_outgoing_calls_from_files), [`get_caller_file_paths`](../tools/graph_builder.md#GraphBuilder.get_caller_file_paths), [`get_inheritance_neighbor_paths`](../tools/graph_builder.md#GraphBuilder.get_inheritance_neighbor_paths), [`get_repo_class_lookup`](../tools/graph_builder.md#GraphBuilder.get_repo_class_lookup), [`get_repo_file_paths`](../tools/graph_builder.md#GraphBuilder.get_repo_file_paths), [`invalidate_for_file`](../tools/indexing/embeddings.md#EmbeddingPipeline.invalidate_for_file), [`add_repository_to_graph`](../tools/graph_builder.md#GraphBuilder.add_repository_to_graph), [`EmbeddingPipeline`](../tools/indexing/embeddings.md#EmbeddingPipeline), [`VectorResolver`](../tools/indexing/vector_resolver.md#VectorResolver)
- used by: [`watch_directory`](watcher.md#CodeWatcher.watch_directory)

## Functions
- `should_use_polling_observer(use_polling: typing.Optional[bool] = None)` — [`L30`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L30)

## Module values
- `POLLING_ENV_VAR` — [`L26`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L26)
- `TRUE_ENV_VALUES` — [`L27`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/watcher.py#L27)

