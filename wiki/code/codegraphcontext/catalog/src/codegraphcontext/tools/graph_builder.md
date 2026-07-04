---
title: 'Module: src/codegraphcontext/tools/graph_builder.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/graph_builder.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.graph_builder`/GraphBuilder#
symbols:
  GraphBuilder.link_inheritance: link_inheritance().
  GraphBuilder.build_graph_from_path_async: build_graph_from_path_async().
  GraphBuilder: ''
  GraphBuilder._writer: _writer.
  GraphBuilder.parse_file: parse_file().
  GraphBuilder.link_function_calls: link_function_calls().
  GraphBuilder.update_file_in_graph: update_file_in_graph().
  GraphBuilder.get_parser: get_parser().
  GraphBuilder._build_graph_from_scip: _build_graph_from_scip().
  GraphBuilder.driver: driver.
  GraphBuilder.add_file_to_graph: add_file_to_graph().
  GraphBuilder.pre_scan_imports: pre_scan_imports().
  GraphBuilder._create_all_function_calls: _create_all_function_calls().
  GraphBuilder.create_schema: create_schema().
  GraphBuilder.parsers: parsers.
  GraphBuilder._parsed_cache: _parsed_cache.
  GraphBuilder.estimate_processing_time: estimate_processing_time().
  GraphBuilder.delete_file_from_graph: delete_file_from_graph().
  GraphBuilder.delete_outgoing_calls_from_files: delete_outgoing_calls_from_files().
  GraphBuilder.delete_inherits_for_files: delete_inherits_for_files().
  GraphBuilder.add_minimal_file_node: add_minimal_file_node().
  GraphBuilder.job_manager: job_manager.
  GraphBuilder.delete_repository_from_graph: delete_repository_from_graph().
  GraphBuilder.get_caller_file_paths: get_caller_file_paths().
  GraphBuilder.get_repo_file_paths: get_repo_file_paths().
  GraphBuilder.get_inheritance_neighbor_paths: get_inheritance_neighbor_paths().
  GraphBuilder.get_repo_class_lookup: get_repo_class_lookup().
  GraphBuilder.__init__: __init__().
  GraphBuilder.delete_relationship_links: delete_relationship_links().
  GraphBuilder._resolve_function_call: _resolve_function_call().
  GraphBuilder.add_repository_to_graph: add_repository_to_graph().
  GraphBuilder._sanitize_props: _sanitize_props().
  GraphBuilder._create_all_inheritance_links: _create_all_inheritance_links().
  GraphBuilder.db_manager: db_manager.
  GraphBuilder.last_call_resolution_diagnostics: last_call_resolution_diagnostics.
  GraphBuilder._MAX_STR_LEN: _MAX_STR_LEN.
  GraphBuilder._name_from_symbol: _name_from_symbol().
  GraphBuilder.generic_extensions: generic_extensions.
  GraphBuilder.generic_filenames: generic_filenames.
  GraphBuilder.loop: loop.
  GraphBuilder._resolve_inheritance_link: _resolve_inheritance_link().
  GraphBuilder._create_csharp_inheritance_and_interfaces: _create_csharp_inheritance_and_interfaces().
---
# Module: [`src/codegraphcontext/tools/graph_builder.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py)

## Classes
### `GraphBuilder`
- def: [`src/codegraphcontext/tools/graph_builder.py:34`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L34) — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- doc: Build and manage the code graph.
- signature: `class GraphBuilder:`
- members:
  - `__init__(self, db_manager: DatabaseManager, job_manager: JobManager, loop: asyncio.AbstractEventLoop)` — [`L42`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L42) — Initialize GraphBuilder.
  - `_create_all_function_calls(self, all_file_data: list[Dict], imports_map: dict, file_class_lookup: Optional[Dict] = None)` — [`L496`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L496) — Create CALLS relationships using fully label-specific UNWIND queries (V3). — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `_create_all_inheritance_links(self, all_file_data: list[Dict], imports_map: dict)` — [`L738`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L738) — Create INHERITS relationships for all classes using batched UNWIND queries.
  - `_create_csharp_inheritance_and_interfaces(self, session, file_data: Dict, imports_map: dict)` — [`L680`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L680) — Create INHERITS and IMPLEMENTS relationships for C# types.
  - `_name_from_symbol(self, symbol: str)` — [`L1102`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L1102) — Extract a human-readable name from a SCIP symbol string.
  - `_resolve_inheritance_link(self, class_item: Dict, base_class_str: str, caller_file_path: str, local_class_names: set, local_imports: dict, imports_map: dict)` — [`L638`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L638) — Resolve a single inheritance link. Returns a dict with params or None.
  - `add_file_to_graph(self, file_data: Dict, repo_name: str, imports_map: dict, repo_path_str: str = None)` — [`L187`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L187) — Adds a file and its contents using batched UNWIND queries (one round-trip per node type). — documented in [codegraphcontext-tools-graph_builder](../../../../concepts/codegraphcontext-tools-graph_builder.md)
  - `add_minimal_file_node(self, file_path: Path, repo_path: Path, is_dependency: bool = False)` — [`L1197`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L1197) — Create a minimal File node without parsing (for unsupported file types).
  - `add_repository_to_graph(self, repo_path: Path, is_dependency: bool = False)` — [`L171`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L171) — Adds a repository node using its absolute path as the unique key.
  - `build_graph_from_path_async(self, path: Path, is_dependency: bool = False, job_id: str = None, cgcignore_path: str = None)` — [`L1117`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L1117) — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
  - `create_schema(self)` — [`L129`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L129)
  - `delete_file_from_graph(self, path: str)` — [`L860`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L860) — Remove a file node and all its relationships from the graph.
  - `delete_inherits_for_files(self, file_paths: list)` — [`L940`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L940) — Remove INHERITS relationships for the specified files.
  - `delete_outgoing_calls_from_files(self, file_paths: list)` — [`L930`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L930) — Remove outgoing CALLS relationships from the specified files.
  - `delete_relationship_links(self, repo_path: Path)` — [`L965`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L965) — Remove all relationship links for a repository.
  - `delete_repository_from_graph(self, repo_path: str)` — [`L870`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L870) — Remove a repository node and all its contents from the graph. — documented in [codegraphcontext-tools-indexing-persistence-writer](../../../../concepts/codegraphcontext-tools-indexing-persistence-writer.md)
  - `estimate_processing_time(self, path: Path)` — [`L1057`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L1057) — Estimate the time required to index a repository.
  - `get_caller_file_paths(self, file_path_str: str)` — [`L885`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L885) — Get all files that have CALLS relationships to the given file.
  - `get_inheritance_neighbor_paths(self, file_path_str: str)` — [`L915`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L915) — Get files with INHERITS relationships to/from the given file.
  - `get_parser(self, extension: str)` — [`L112`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L112) — Gets or creates a TreeSitterParser for the given extension (thread-local). — documented in [codegraphcontext-tools-graph_builder](../../../../concepts/codegraphcontext-tools-graph_builder.md)
  - `get_repo_class_lookup(self, repo_path: Path)` — [`L950`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L950) — Get a mapping of file paths to their defined class names.
  - `get_repo_file_paths(self, repo_path: Path)` — [`L900`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L900) — Get all file paths indexed for a repository.
  - `link_function_calls(self, all_file_data: list[Dict], imports_map: dict, file_class_lookup: Optional[Dict[str, set]] = None)` — [`L776`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L776) — Resolve and persist CALLS relationships. — documented in [codegraphcontext-server](../../../../concepts/codegraphcontext-server.md)
  - `link_inheritance(self, all_file_data: list[Dict], imports_map: dict)` — [`L821`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L821) — Resolve and persist INHERITS / C# IMPLEMENTS / Go IMPLEMENTS relationships. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
  - `parse_file(self, repo_path: Path, path: Path, is_dependency: bool = False)` — [`L1006`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L1006) — Parse a source file and extract code structure. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
  - `pre_scan_imports(self, files: list[Path])` — [`L151`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L151) — Build global imports map from language pre-scans.
  - `update_file_in_graph(self, path: Path, repo_path: Path, imports_map: dict)` — [`L975`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L975) — Update a file node in the graph (delete and re-index).
  - `db_manager` — [`L54`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L54)
  - `driver` — [`L57`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L57) — documented in [codegraphcontext-tools-graph_builder](../../../../concepts/codegraphcontext-tools-graph_builder.md)
  - `generic_extensions` — [`L100`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L100)
  - `generic_filenames` — [`L104`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L104)
  - `job_manager` — [`L55`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L55)
  - `last_call_resolution_diagnostics` — [`L59`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L59)
  - `loop` — [`L56`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L56)
  - `parsers` — [`L60`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L60)
- protocol/private: `_MAX_STR_LEN`[`L132`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L132), `_build_graph_from_scip`[`L1084`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L1084), `_parsed_cache`[`L109`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L109), `_resolve_function_call`[`L138`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L138), `_sanitize_props`[`L135`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L135), `_writer`[`L58`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/graph_builder.py#L58)
- uses (calls/refs, reference-scoped): [`info_logger`](../utils/debug_log.md#info_logger), [`warning_logger`](../utils/debug_log.md#warning_logger), [`run_tree_sitter_index_async`](indexing/pipeline.md#run_tree_sitter_index_async), [`debug_log`](../utils/debug_log.md#debug_log), [`error_logger`](../utils/debug_log.md#error_logger), [`build_function_call_groups`](indexing/resolution/calls.md#build_function_call_groups), [`run_scip_index_async`](indexing/scip_pipeline.md#run_scip_index_async), [`get_driver`](../core/database.md#DatabaseManager.get_driver), [`DatabaseManager`](../core/database.md#DatabaseManager), [`get_config_value`](../cli/config_manager.md#get_config_value), [`resolve_function_call`](indexing/resolution/calls.md#resolve_function_call), [`delete_repository_from_graph`](indexing/persistence/writer.md#GraphWriter.delete_repository_from_graph), [`discover_files_to_index`](indexing/discovery.md#discover_files_to_index), [`update_job`](../core/jobs.md#JobManager.update_job), [`JobStatus`](../core/jobs.md#JobStatus), [`language_name`](tree_sitter_parser.md#TreeSitterParser.language_name), [`add_repository_to_graph`](indexing/persistence/writer.md#GraphWriter.add_repository_to_graph), [`add_file_to_graph`](indexing/persistence/writer.md#GraphWriter.add_file_to_graph), [`delete_relationship_links`](indexing/persistence/writer.md#GraphWriter.delete_relationship_links), [`write_inheritance_links`](indexing/persistence/writer.md#GraphWriter.write_inheritance_links), [`JobManager`](../core/jobs.md#JobManager), [`write_companion_of_links`](indexing/persistence/writer.md#GraphWriter.write_companion_of_links), [`write_decorated_by_links`](indexing/persistence/writer.md#GraphWriter.write_decorated_by_links), [`write_embeds_links`](indexing/persistence/writer.md#GraphWriter.write_embeds_links), [`write_implements_links`](indexing/persistence/writer.md#GraphWriter.write_implements_links), [`write_metaclass_links`](indexing/persistence/writer.md#GraphWriter.write_metaclass_links), [`write_part_of_links`](indexing/persistence/writer.md#GraphWriter.write_part_of_links), [`write_partial_of_links`](indexing/persistence/writer.md#GraphWriter.write_partial_of_links), [`add_minimal_file_node`](indexing/persistence/writer.md#GraphWriter.add_minimal_file_node), [`delete_file_from_graph`](indexing/persistence/writer.md#GraphWriter.delete_file_from_graph), [`delete_inherits_for_files`](indexing/persistence/writer.md#GraphWriter.delete_inherits_for_files), [`delete_outgoing_calls_from_files`](indexing/persistence/writer.md#GraphWriter.delete_outgoing_calls_from_files), [`get_repo_class_lookup`](indexing/persistence/writer.md#GraphWriter.get_repo_class_lookup), [`get_repo_file_paths`](indexing/persistence/writer.md#GraphWriter.get_repo_file_paths), [`write_function_call_groups`](indexing/persistence/writer.md#GraphWriter.write_function_call_groups), [`get_caller_file_paths`](indexing/persistence/writer.md#GraphWriter.get_caller_file_paths), [`get_inheritance_neighbor_paths`](indexing/persistence/writer.md#GraphWriter.get_inheritance_neighbor_paths), [`build_inheritance_and_csharp_files`](indexing/resolution/inheritance.md#build_inheritance_and_csharp_files), [`parse`](tree_sitter_parser.md#TreeSitterParser.parse), [`pre_scan_for_imports`](indexing/pre_scan.md#pre_scan_for_imports)  (+22 more)
- used by: [`_initialize_services`](../cli/cli_helpers.md#_initialize_services), [`switch_context_tool`](../server.md#MCPServer.switch_context_tool), [`_handle_modification`](../core/watcher.md#RepositoryEventHandler._handle_modification), [`_run_index_with_progress`](../cli/cli_helpers.md#_run_index_with_progress), [`synchronize_with_disk`](../core/watcher.md#RepositoryEventHandler.synchronize_with_disk), [`_initial_scan`](../core/watcher.md#RepositoryEventHandler._initial_scan), [`graph_builder`](../server.md#MCPServer.graph_builder), [`_iter_supported_files`](../core/watcher.md#RepositoryEventHandler._iter_supported_files), [`delete_repository`](handlers/management_handlers.md#delete_repository), [`_is_supported_code_file`](../core/watcher.md#RepositoryEventHandler._is_supported_code_file), [`_update_imports_map_for_file`](../core/watcher.md#RepositoryEventHandler._update_imports_map_for_file), [`_print_call_resolution_diagnostics`](../cli/cli_helpers.md#_print_call_resolution_diagnostics), [`__init__`](../core/watcher.md#CodeWatcher.__init__), [`__init__`](../core/watcher.md#RepositoryEventHandler.__init__)

