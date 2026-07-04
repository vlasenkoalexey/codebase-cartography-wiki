---
title: 'Module: tree_sitter_analyzer/mcp/utils/file_output_manager.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/file_output_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.file_output_manager`/
symbols:
  FileOutputManager: FileOutputManager#
  FileOutputManager.project_root: FileOutputManager#project_root.
  FileOutputManager.get_managed_instance: FileOutputManager#get_managed_instance().
  FileOutputManager.detect_content_type: FileOutputManager#detect_content_type().
  FileOutputManager.save_to_file: FileOutputManager#save_to_file().
  FileOutputManager.get_output_path: FileOutputManager#get_output_path().
  FileOutputManager.generate_output_filename: FileOutputManager#generate_output_filename().
  FileOutputManager.set_output_path: FileOutputManager#set_output_path().
  FileOutputManager.get_file_extension: FileOutputManager#get_file_extension().
  FileOutputManager.set_project_root: FileOutputManager#set_project_root().
  FileOutputManager._initialize_output_path: FileOutputManager#_initialize_output_path().
  FileOutputManager._output_path: FileOutputManager#_output_path.
  logger: logger.
  FileOutputManager._instances: FileOutputManager#_instances.
  FileOutputManager.create_instance: FileOutputManager#create_instance().
  FileOutputManager.__init__: FileOutputManager#__init__().
  FileOutputManager.validate_output_path: FileOutputManager#validate_output_path().
  _similar_comma_count: _similar_comma_count().
  FileOutputManager._is_toon_format: FileOutputManager#_is_toon_format().
---
# Module: [`tree_sitter_analyzer/mcp/utils/file_output_manager.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py)

## Classes
### `FileOutputManager`
- def: [`tree_sitter_analyzer/mcp/utils/file_output_manager.py:32`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L32) — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
- doc: Manages file output for analysis results with automatic extension detection
- signature: `class FileOutputManager:`
- members:
  - `_initialize_output_path(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L72) — Initialize the output path from environment variables or project root.
  - `_is_toon_format(self, content: str)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L184) — Detect if content is in TOON format.
  - `create_instance(cls, project_root: str | None = None)` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L56) — Create a new FileOutputManager instance directly (bypass factory).
  - `detect_content_type(self, content: str)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L124) — Detect content type based on content structure.
  - `generate_output_filename(self, base_name: str, content: str)` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L247) — Generate output filename with appropriate extension.
  - `get_file_extension(self, content_type: str)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L228) — Get file extension for content type.
  - `get_managed_instance(cls, project_root: str | None = None)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L46) — Return a cached instance per project_root (one per root).
  - `get_output_path(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L96) — Get the current output path.
  - `save_to_file(self, content: str, filename: str | None = None, base_name: str | None = None)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L266) — Save content to file with automatic extension detection.
  - `set_output_path(self, output_path: str)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L105) — Set a custom output path.
  - `set_project_root(self, project_root: str)` — [`L368`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L368) — Update the project root and reinitialize output path if needed.
  - `validate_output_path(self, path: str)` — [`L334`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L334) — Validate if a path is safe for output.
  - `project_root` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L41)
- protocol/private: `__init__`[`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L40), `_instances`[`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L38), `_output_path`[`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L42)
- uses (calls/refs, reference-scoped): [`write_file_safe`](../../encoding_utils.md#write_file_safe), [`logger`](file_output_manager.md#logger), [`_similar_comma_count`](file_output_manager.md#_similar_comma_count)
- used by: [`get_instance`](file_output_factory.md#FileOutputManagerFactory.get_instance), [`update_project_root`](file_output_factory.md#FileOutputManagerFactory.update_project_root), [`get_file_output_manager`](file_output_factory.md#get_file_output_manager), [`_instances`](file_output_factory.md#FileOutputManagerFactory._instances), [`file_output_manager`](../tools/read_partial_tool.md#ReadPartialTool.file_output_manager), [`_on_project_root_changed`](../tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool._on_project_root_changed), [`_on_project_root_changed`](../tools/query_tool.md#QueryTool._on_project_root_changed), [`_save_to_file`](../tools/list_files_helpers.md#_save_to_file), [`_create_or_get_instance`](file_output_factory.md#FileOutputManagerFactory._create_or_get_instance), [`file_output_manager`](../tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.file_output_manager), [`_on_project_root_changed`](../tools/find_and_grep_tool.md#FindAndGrepTool._on_project_root_changed), [`_on_project_root_changed`](../tools/search_content_tool.md#SearchContentTool._on_project_root_changed), [`file_output_manager`](../tools/query_tool.md#QueryTool.file_output_manager), [`file_output_manager`](../tools/search_content_tool.md#SearchContentTool.file_output_manager), [`file_output_manager`](../tools/find_and_grep_tool.md#FindAndGrepTool.file_output_manager)  (67 test-only)

## Functions
- `_similar_comma_count(line: str, ref_count: int)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L22) — Return True if *line*'s comma count is within 1 of *ref_count*.

## Module values
- `logger` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_manager.py#L19)

