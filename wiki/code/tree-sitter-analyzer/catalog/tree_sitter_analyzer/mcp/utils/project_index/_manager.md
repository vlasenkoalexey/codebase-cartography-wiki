---
title: 'Module: tree_sitter_analyzer/mcp/utils/project_index/_manager.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/project_index/_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.project_index._manager`/
symbols:
  ProjectIndexManager: ProjectIndexManager#
  ProjectIndexManager.build: ProjectIndexManager#build().
  ProjectIndexManager.load: ProjectIndexManager#load().
  ProjectIndexManager._assemble_project_index: ProjectIndexManager#_assemble_project_index().
  ProjectIndexManager._extract_edges_from_file: ProjectIndexManager#_extract_edges_from_file().
  ProjectIndexManager.save: ProjectIndexManager#save().
  ProjectIndexManager.render_toon: ProjectIndexManager#render_toon().
  ProjectIndexManager._persist_project_index: ProjectIndexManager#_persist_project_index().
  ProjectIndexManager.project_root: ProjectIndexManager#project_root.
  ProjectIndexManager._classify_dir: ProjectIndexManager#_classify_dir().
  ProjectIndexManager._compute_pagerank: ProjectIndexManager#_compute_pagerank().
  ProjectIndexManager._try_load_fresh_cache: ProjectIndexManager#_try_load_fresh_cache().
  ProjectIndexManager._save_file_hashes: ProjectIndexManager#_save_file_hashes().
  ProjectIndexManager._save_toon: ProjectIndexManager#_save_toon().
  ProjectIndexManager._save_critical_nodes: ProjectIndexManager#_save_critical_nodes().
  ProjectIndexManager.is_stale: ProjectIndexManager#is_stale().
  logger: logger.
  ProjectIndexManager._describe_dir: ProjectIndexManager#_describe_dir().
  ProjectIndexManager.SCHEMA_VERSION: ProjectIndexManager#SCHEMA_VERSION.
  ProjectIndexManager._cache_path: ProjectIndexManager#_cache_path.
  ProjectIndexManager._load_file_hashes: ProjectIndexManager#_load_file_hashes().
  ProjectIndexManager._compute_file_hashes: ProjectIndexManager#_compute_file_hashes().
  ProjectIndexManager._normalize_scan_roots: ProjectIndexManager#_normalize_scan_roots().
  ProjectIndexManager._list_files: ProjectIndexManager#_list_files().
  ProjectIndexManager._extract_readme_excerpt: ProjectIndexManager#_extract_readme_excerpt().
  ProjectIndexManager.CACHE_FILE: ProjectIndexManager#CACHE_FILE.
  ProjectIndexManager.TOON_FILE: ProjectIndexManager#TOON_FILE.
  ProjectIndexManager.__init__: ProjectIndexManager#__init__().
  ProjectIndexManager.HASHES_FILE: ProjectIndexManager#HASHES_FILE.
  ProjectIndexManager.CRITICAL_FILE: ProjectIndexManager#CRITICAL_FILE.
  ProjectIndexManager._BUILD_FILE_NAMES: ProjectIndexManager#_BUILD_FILE_NAMES.
  ProjectIndexManager._BUILD_DIR_NAMES: ProjectIndexManager#_BUILD_DIR_NAMES.
---
# Module: [`tree_sitter_analyzer/mcp/utils/project_index/_manager.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py)

## Classes
### `ProjectIndexManager`
- def: [`tree_sitter_analyzer/mcp/utils/project_index/_manager.py:30`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L30) — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)
- doc: Manage the persistent project index stored on disk.
- signature: `class ProjectIndexManager:`
- members:
  - `_assemble_project_index(self, *, now: float, all_files: list[str], lang_dist: dict[str, int], top_level: list[dict[str, Any]], key_files: list[str], entry_points: list[str], readme_excerpt: str, module_descriptions: dict[str, str], critical_nodes: list[dict[str, Any]])` — [`L217`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L217) — Construct a ``ProjectIndex`` dataclass, preserving ``created_at``.
  - `_classify_dir(self, path: Path)` — [`L267`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L267) — Classify a top-level directory as core / context / tooling.
  - `_compute_file_hashes(self, roots: list[str])` — [`L342`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L342) — Return {filepath: [mtime, size]} for all files under roots.
  - `_compute_pagerank(self, edges: list[tuple[str, str]], top_n: int = 10, alpha: float = 0.85, max_iter: int = 100)` — [`L306`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L306) — Proxy for ``compute_pagerank`` — preserved for test compatibility.
  - `_describe_dir(cls, dir_path: Path, dir_name: str)` — [`L300`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L300) — Proxy for ``describe_dir`` — preserved for test compatibility.
  - `_extract_edges_from_file(self, path: Path)` — [`L322`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L322) — Extract edges via language-specific extractor (plugin registry).
  - `_extract_readme_excerpt(self, root_path: Path)` — [`L295`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L295) — Proxy for ``extract_readme_excerpt`` — preserved for test compatibility.
  - `_list_files(self, roots: list[str])` — [`L291`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L291) — Proxy for ``list_files`` — preserved for test compatibility.
  - `_normalize_scan_roots(self, roots: Path | list[str] | None)` — [`L198`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L198) — Return ``roots`` as a list[str], defaulting to ``[project_root]``.
  - `_persist_project_index(self, index: ProjectIndex, scan_roots: list[str], critical_nodes: list[dict[str, Any]])` — [`L249`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L249) — Persist index + derived artifacts (hashes, TOON snapshot, nodes).
  - `_try_load_fresh_cache(self, scan_roots: list[str])` — [`L206`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L206) — Return the cached index if file hashes are unchanged, else None.
  - `build(self, roots: Path | list[str] | None = None, force_refresh: bool = False)` — [`L138`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L138) — Build or load a cached project index.
  - `is_stale(self, index: ProjectIndex, max_age_hours: int = 24)` — [`L133`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L133) — Return True if the index is older than *max_age_hours*.
  - `load(self)` — [`L77`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L77) — Load index from disk. Returns None if missing or schema mismatch.
  - `render_toon(self, index: ProjectIndex)` — [`L190`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L190) — Render the project index as TOON-format text.
  - `save(self, index: ProjectIndex)` — [`L117`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L117) — Persist index to disk, creating the cache directory if needed.
  - `CACHE_FILE` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L33)
  - `CRITICAL_FILE` — [`L36`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L36)
  - `HASHES_FILE` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L35)
  - `SCHEMA_VERSION` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L37)
  - `TOON_FILE` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L34)
  - `project_root` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L70)
- protocol/private: `_BUILD_DIR_NAMES`[`L56`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L56), `_BUILD_FILE_NAMES`[`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L40), `__init__`[`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L69), `_cache_path`[`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L71), `_load_file_hashes`[`L353`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L353), `_save_critical_nodes`[`L387`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L387), `_save_file_hashes`[`L364`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L364), `_save_toon`[`L376`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L376)
- uses (calls/refs, reference-scoped): [`ProjectIndex`](_models.md#ProjectIndex), [`render_toon`](_toon.md#render_toon), [`assert_cache_path`](../cache_paths.md#assert_cache_path), [`custom_notes`](_models.md#ProjectIndex.custom_notes), [`language_distribution`](_models.md#ProjectIndex.language_distribution), [`updated_at`](_models.md#ProjectIndex.updated_at), [`file_count`](_models.md#ProjectIndex.file_count), [`compute_pagerank`](_pagerank.md#compute_pagerank), [`entry_points`](_models.md#ProjectIndex.entry_points), [`describe_dir`](_filesystem.md#describe_dir), [`module_descriptions`](_models.md#ProjectIndex.module_descriptions), [`readme_excerpt`](_models.md#ProjectIndex.readme_excerpt), [`extract`](../edge_extractors/base.md#EdgeExtractor.extract), [`extract_readme_excerpt`](_filesystem.md#extract_readme_excerpt), [`key_files`](_models.md#ProjectIndex.key_files), [`logger`](_manager.md#logger), [`top_level_structure`](_models.md#ProjectIndex.top_level_structure), [`build_top_level_structure`](_filesystem.md#build_top_level_structure), [`compute_language_distribution`](_filesystem.md#compute_language_distribution), [`critical_nodes`](_models.md#ProjectIndex.critical_nodes), [`extract_module_descriptions`](_filesystem.md#extract_module_descriptions), [`find_entry_points`](_filesystem.md#find_entry_points), [`get_extractor`](../edge_extractors/__init__.md#get_extractor), [`project_root`](_models.md#ProjectIndex.project_root), [`schema_version`](_models.md#ProjectIndex.schema_version), [`collect_critical_nodes`](_pagerank.md#collect_critical_nodes), [`collect_root_key_files`](_filesystem.md#collect_root_key_files), [`created_at`](_models.md#ProjectIndex.created_at), [`list_files`](_filesystem.md#list_files), [`module_dependency_order`](_models.md#ProjectIndex.module_dependency_order)
- used by: [`_execute_json`](../../tools/get_project_summary_tool.md#GetProjectSummaryTool._execute_json), [`_do_execute`](../../tools/build_project_index_tool.md#BuildProjectIndexTool._do_execute), [`execute`](../../tools/get_project_summary_tool.md#GetProjectSummaryTool.execute), [`_execute_toon`](../../tools/get_project_summary_tool.md#GetProjectSummaryTool._execute_toon), [`_read_or_render_toon`](../../tools/get_project_summary_tool.md#GetProjectSummaryTool._read_or_render_toon), [`_append_custom_notes_if_needed`](../../tools/get_project_summary_tool.md#GetProjectSummaryTool._append_custom_notes_if_needed)  (72 test-only)

## Module values
- `logger` — [`L27`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_manager.py#L27)

