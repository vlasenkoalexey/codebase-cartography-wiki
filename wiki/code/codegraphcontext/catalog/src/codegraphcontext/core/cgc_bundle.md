---
title: 'Module: src/codegraphcontext/core/cgc_bundle.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/cgc_bundle.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.cgc_bundle`/
symbols:
  CGCBundle.export_to_bundle: CGCBundle#export_to_bundle().
  CGCBundle.import_from_bundle: CGCBundle#import_from_bundle().
  CGCBundle._extract_nodes: CGCBundle#_extract_nodes().
  CGCBundle._import_node_batch: CGCBundle#_import_node_batch().
  CGCBundle._extract_edges: CGCBundle#_extract_edges().
  CGCBundle.db_manager: CGCBundle#db_manager.
  CGCBundle._extract_metadata: CGCBundle#_extract_metadata().
  CGCBundle._import_edge_batch: CGCBundle#_import_edge_batch().
  CGCBundle: CGCBundle#
  CGCBundle._delete_repository: CGCBundle#_delete_repository().
  CGCBundle._extract_schema: CGCBundle#_extract_schema().
  CGCBundle._import_nodes: CGCBundle#_import_nodes().
  CGCBundle._import_edges: CGCBundle#_import_edges().
  _BundleEncoder: _BundleEncoder#
  CGCBundle._get_id_function: CGCBundle#_get_id_function().
  CGCBundle._uses_pk_edge_matching: CGCBundle#_uses_pk_edge_matching().
  CGCBundle._node_lookup_key: CGCBundle#_node_lookup_key().
  CGCBundle._generate_stats: CGCBundle#_generate_stats().
  CGCBundle._check_existing_repository: CGCBundle#_check_existing_repository().
  CGCBundle._clear_graph: CGCBundle#_clear_graph().
  CGCBundle._import_schema: CGCBundle#_import_schema().
  CGCBundle._repo_scope_params: CGCBundle#_repo_scope_params().
  CGCBundle._run_session_query: CGCBundle#_run_session_query().
  CGCBundle._PK_MAP: CGCBundle#_PK_MAP.
  CGCBundle.VERSION: CGCBundle#VERSION.
  CGCBundle._normalize_labels: CGCBundle#_normalize_labels().
  CGCBundle._node_to_dict: CGCBundle#_node_to_dict().
  CGCBundle._node_identity: CGCBundle#_node_identity().
  CGCBundle._repo_node_queries: CGCBundle#_repo_node_queries().
  CGCBundle._repo_edge_queries: CGCBundle#_repo_edge_queries().
  CGCBundle._create_readme: CGCBundle#_create_readme().
  CGCBundle._create_zip: CGCBundle#_create_zip().
  CGCBundle._validate_bundle: CGCBundle#_validate_bundle().
  CGCBundle._UID_PARTS: CGCBundle#_UID_PARTS.
  _BundleEncoder.default: _BundleEncoder#default().
  CGCBundle.__init__: CGCBundle#__init__().
  CGCBundle._id_mapping: CGCBundle#_id_mapping.
---
# Module: [`src/codegraphcontext/core/cgc_bundle.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py)

## Classes
### `CGCBundle`
- def: [`src/codegraphcontext/core/cgc_bundle.py:53`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L53)
- doc: Handles creation and loading of .cgc bundle files.
- signature: `class CGCBundle:`
- members:
  - `__init__(self, db_manager)` — [`L58`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L58) — Initialize the CGC Bundle handler.
  - `_check_existing_repository(self, repo_name: str, repo_path: Optional[str])` — [`L813`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L813) — Check if a repository already exists in the database.
  - `_clear_graph(self)` — [`L880`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L880) — Clear all nodes and relationships from the graph in batches.
  - `_create_readme(self, output_file: Path, metadata: Dict, stats: Optional[Dict])` — [`L733`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L733) — Create a human-readable README for the bundle.
  - `_create_zip(self, source_dir: Path, output_file: Path)` — [`L782`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L782) — Create a ZIP archive from the bundle directory.
  - `_delete_repository(self, repo_identifier: str)` — [`L835`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L835) — Delete a specific repository and all its related nodes from the graph.
  - `_extract_edges(self, output_file: Path, repo_path: Optional[Path])` — [`L577`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L577) — Extract all relationships to JSONL format.
  - `_extract_metadata(self, repo_path: Optional[Path])` — [`L301`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L301) — Extract metadata about the repository and indexing process.
  - `_extract_nodes(self, output_file: Path, repo_path: Optional[Path])` — [`L526`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L526) — Extract all nodes to JSONL format.
  - `_extract_schema(self)` — [`L379`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L379) — Extract the graph schema (node labels, relationship types, constraints).
  - `_generate_stats(self, repo_path: Optional[Path], node_count: int, edge_count: int)` — [`L675`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L675) — Generate statistics about the graph.
  - `_get_id_function(self)` — [`L67`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L67) — Get the appropriate ID function based on the database backend.
  - `_import_edge_batch(self, session, batch: List[Dict])` — [`L1030`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L1030) — Import a batch of edges.
  - `_import_edges(self, edges_file: Path)` — [`L1008`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L1008) — Import edges from JSONL file.
  - `_import_node_batch(self, session, batch: List[Tuple], id_mapping: Dict)` — [`L967`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L967) — Import a batch of nodes.
  - `_import_nodes(self, nodes_file: Path)` — [`L901`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L901) — Import nodes from JSONL file.
  - `_import_schema(self, schema_file: Path)` — [`L891`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L891) — Import schema (constraints and indexes).
  - `_uses_pk_edge_matching(self)` — [`L79`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L79) — Kùzu/Ladybug internal IDs are not comparable via id() in MATCH.
  - `_validate_bundle(self, bundle_dir: Path)` — [`L794`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L794) — Validate that the bundle contains all required files.
  - `export_to_bundle(self, output_path: Path, repo_path: Optional[Path] = None, include_stats: bool = True)` — [`L95`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L95) — Export the current graph (or a specific repository) to a .cgc bundle.
  - `import_from_bundle(self, bundle_path: Path, clear_existing: bool = False, readonly: bool = False)` — [`L209`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L209) — Import a .cgc bundle into the current database.
  - `VERSION` — [`L56`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L56)
  - `db_manager` — [`L65`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L65)
- protocol/private: `_PK_MAP`[`L942`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L942), `_UID_PARTS`[`L951`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L951), `_id_mapping`[`L938`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L938), `_node_identity`[`L477`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L477), `_node_lookup_key`[`L83`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L83), `_node_to_dict`[`L462`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L462), `_normalize_labels`[`L453`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L453), `_repo_edge_queries`[`L506`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L506), `_repo_node_queries`[`L487`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L487), `_repo_scope_params`[`L443`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L443), `_run_session_query`[`L447`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L447)
- uses (calls/refs, reference-scoped): [`info_logger`](../utils/debug_log.md#info_logger), [`warning_logger`](../utils/debug_log.md#warning_logger), [`debug_log`](../utils/debug_log.md#debug_log), [`error_logger`](../utils/debug_log.md#error_logger), [`_BundleEncoder`](cgc_bundle.md#_BundleEncoder), [`get_repo_commit_hash`](../utils/git_utils.md#get_repo_commit_hash), [`RELATIONSHIP_TYPES`](../tools/indexing/schema_contract.md#RELATIONSHIP_TYPES), [`get_repo_branch_name`](../utils/git_utils.md#get_repo_branch_name)
- used by: [`load_bundle`](../tools/handlers/management_handlers.md#load_bundle), [`bundle_import`](../cli/main.md#bundle_import), [`bundle_export`](../cli/main.md#bundle_export), [`load_bundle_command`](../cli/registry_commands.md#load_bundle_command)

### `_BundleEncoder`  ·  implements/extends JSONEncoder
- def: [`src/codegraphcontext/core/cgc_bundle.py:35`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L35)
- doc: Handles Neo4j DateTime and other non-standard types for bundle serialization.
- signature: `class _BundleEncoder(json.JSONEncoder):`
- members:
  - `default(self, obj)` — [`L37`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgc_bundle.py#L37)
- used by: [`export_to_bundle`](cgc_bundle.md#CGCBundle.export_to_bundle), [`_extract_nodes`](cgc_bundle.md#CGCBundle._extract_nodes), [`_extract_edges`](cgc_bundle.md#CGCBundle._extract_edges)

