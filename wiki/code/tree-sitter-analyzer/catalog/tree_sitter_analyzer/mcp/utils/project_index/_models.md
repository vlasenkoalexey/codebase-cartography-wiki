---
title: 'Module: tree_sitter_analyzer/mcp/utils/project_index/_models.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/project_index/_models.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.project_index._models`/
symbols:
  ProjectIndex: ProjectIndex#
  ProjectIndex.language_distribution: ProjectIndex#language_distribution.
  ProjectIndex.custom_notes: ProjectIndex#custom_notes.
  ProjectIndex.updated_at: ProjectIndex#updated_at.
  ProjectIndex.file_count: ProjectIndex#file_count.
  ProjectIndex.entry_points: ProjectIndex#entry_points.
  ProjectIndex.module_descriptions: ProjectIndex#module_descriptions.
  ProjectIndex.readme_excerpt: ProjectIndex#readme_excerpt.
  ProjectIndex.top_level_structure: ProjectIndex#top_level_structure.
  ProjectIndex.key_files: ProjectIndex#key_files.
  ProjectIndex.critical_nodes: ProjectIndex#critical_nodes.
  ProjectIndex.project_root: ProjectIndex#project_root.
  ProjectIndex.schema_version: ProjectIndex#schema_version.
  ProjectIndex.created_at: ProjectIndex#created_at.
  _ENTRY_POINT_NAMES._ENTRY_POINT_NAMES: _ENTRY_POINT_NAMES._ENTRY_POINT_NAMES.
  _LANGUAGE_COUNT_EXCLUDED_SEGMENTS._LANGUAGE_COUNT_EXCLUDED_SEGMENTS: _LANGUAGE_COUNT_EXCLUDED_SEGMENTS._LANGUAGE_COUNT_EXCLUDED_SEGMENTS.
  _PAGERANK_STDLIB_BLOCKLIST._PAGERANK_STDLIB_BLOCKLIST: _PAGERANK_STDLIB_BLOCKLIST._PAGERANK_STDLIB_BLOCKLIST.
  _EXT_TO_LANGUAGE._EXT_TO_LANGUAGE: _EXT_TO_LANGUAGE._EXT_TO_LANGUAGE.
  _KEY_FILE_NAMES._KEY_FILE_NAMES: _KEY_FILE_NAMES._KEY_FILE_NAMES.
  _DIR_CONVENTIONS._DIR_CONVENTIONS: _DIR_CONVENTIONS._DIR_CONVENTIONS.
  ProjectIndex.module_dependency_order: ProjectIndex#module_dependency_order.
---
# Module: [`tree_sitter_analyzer/mcp/utils/project_index/_models.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py)

## Classes
### `ProjectIndex`
- def: [`tree_sitter_analyzer/mcp/utils/project_index/_models.py:240`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L240)
- doc: Persistent snapshot of a project's architecture.
- signature: `class ProjectIndex:`
- members:
  - `created_at` — [`L244`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L244)
  - `critical_nodes` — [`L255`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L255)
  - `custom_notes` — [`L251`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L251)
  - `entry_points` — [`L250`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L250)
  - `file_count` — [`L246`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L246)
  - `key_files` — [`L249`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L249)
  - `language_distribution` — [`L247`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L247)
  - `module_dependency_order` — [`L256`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L256)
  - `module_descriptions` — [`L254`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L254)
  - `project_root` — [`L243`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L243)
  - `readme_excerpt` — [`L253`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L253)
  - `schema_version` — [`L252`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L252)
  - `top_level_structure` — [`L248`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L248)
  - `updated_at` — [`L245`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L245)
- used by: [`build`](_manager.md#ProjectIndexManager.build), [`load`](_manager.md#ProjectIndexManager.load), [`_assemble_project_index`](_manager.md#ProjectIndexManager._assemble_project_index), [`_execute_json`](../../tools/get_project_summary_tool.md#GetProjectSummaryTool._execute_json), [`_do_execute`](../../tools/build_project_index_tool.md#BuildProjectIndexTool._do_execute), [`render_toon`](_toon.md#render_toon), [`_execute_toon`](../../tools/get_project_summary_tool.md#GetProjectSummaryTool._execute_toon), [`save`](_manager.md#ProjectIndexManager.save), [`_build_project_summary_line`](../../tools/get_project_summary_tool.md#_build_project_summary_line), [`render_toon`](_manager.md#ProjectIndexManager.render_toon), [`_persist_project_index`](_manager.md#ProjectIndexManager._persist_project_index), [`_emit_header_block`](../../tools/get_project_summary_tool.md#_emit_header_block), [`_make_quick_start`](../../tools/get_project_summary_tool.md#_make_quick_start), [`_emit_structure_block`](../../tools/get_project_summary_tool.md#_emit_structure_block), [`_read_or_render_toon`](../../tools/get_project_summary_tool.md#GetProjectSummaryTool._read_or_render_toon), [`_render_core`](_toon.md#_render_core), [`_render_scale`](_toon.md#_render_scale), [`_top_code_languages`](../../tools/get_project_summary_tool.md#_top_code_languages), [`_try_load_fresh_cache`](_manager.md#ProjectIndexManager._try_load_fresh_cache), [`is_stale`](_manager.md#ProjectIndexManager.is_stale), [`_append_custom_notes_if_needed`](../../tools/get_project_summary_tool.md#GetProjectSummaryTool._append_custom_notes_if_needed), [`_render_tooling`](_toon.md#_render_tooling), [`_format_toon`](../../tools/get_project_summary_tool.md#_format_toon), [`_render_critical`](_toon.md#_render_critical), [`_render_entry`](_toon.md#_render_entry), [`_render_header`](_toon.md#_render_header)  (26 test-only)

## Module values
- `_DIR_CONVENTIONS` — [`L209`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L209)
- `_ENTRY_POINT_NAMES` — [`L183`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L183)
- `_EXT_TO_LANGUAGE` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L87)
- `_KEY_FILE_NAMES` — [`L155`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L155)
- `_LANGUAGE_COUNT_EXCLUDED_SEGMENTS` — [`L15`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L15)
- `_PAGERANK_STDLIB_BLOCKLIST` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_models.py#L46)

