---
title: 'Module: tree_sitter_analyzer/mcp/utils/file_output_factory.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/file_output_factory.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.file_output_factory`/
symbols:
  FileOutputManagerFactory: FileOutputManagerFactory#
  FileOutputManagerFactory.get_instance: FileOutputManagerFactory#get_instance().
  FileOutputManagerFactory.clear_all_instances: FileOutputManagerFactory#clear_all_instances().
  FileOutputManagerFactory.get_instance_count: FileOutputManagerFactory#get_instance_count().
  FileOutputManagerFactory.update_project_root: FileOutputManagerFactory#update_project_root().
  get_file_output_manager: get_file_output_manager().
  FileOutputManagerFactory.clear_instance: FileOutputManagerFactory#clear_instance().
  FileOutputManagerFactory._instances: FileOutputManagerFactory#_instances.
  logger: logger.
  FileOutputManagerFactory._normalize_project_root: FileOutputManagerFactory#_normalize_project_root().
  FileOutputManagerFactory.get_managed_project_roots: FileOutputManagerFactory#get_managed_project_roots().
  FileOutputManagerFactory._create_or_get_instance: FileOutputManagerFactory#_create_or_get_instance().
  FileOutputManagerFactory._lock: FileOutputManagerFactory#_lock.
---
# Module: [`tree_sitter_analyzer/mcp/utils/file_output_factory.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py)

## Classes
### `FileOutputManagerFactory`
- def: [`tree_sitter_analyzer/mcp/utils/file_output_factory.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L20)
- doc: Factory class that manages FileOutputManager instances using a Managed Singleton
- signature: `class FileOutputManagerFactory:`
- members:
  - `_create_or_get_instance(cls, normalized_root: str)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L60) — Slow-path: acquire the lock, double-check, and create if needed.
  - `_normalize_project_root(cls, project_root: str | None)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L83) — Normalize project root path for consistent key generation.
  - `clear_all_instances(cls)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L132) — Clear all FileOutputManager instances from the factory.
  - `clear_instance(cls, project_root: str | None = None)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L103) — Clear a specific FileOutputManager instance from the factory.
  - `get_instance(cls, project_root: str | None = None)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L34) — Get or create a FileOutputManager instance for the specified project root.
  - `get_instance_count(cls)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L151) — Get the current number of managed instances.
  - `get_managed_project_roots(cls)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L162) — Get list of all currently managed project roots.
  - `update_project_root(cls, old_root: str | None, new_root: str)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L173) — Update the project root for an existing instance.
- protocol/private: `_instances`[`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L31), `_lock`[`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L28)
- uses (calls/refs, reference-scoped): [`FileOutputManager`](file_output_manager.md#FileOutputManager), [`logger`](file_output_factory.md#logger), [`set_project_root`](file_output_manager.md#FileOutputManager.set_project_root)
- used by: [`get_file_output_manager`](file_output_factory.md#get_file_output_manager)  (56 test-only)

## Functions
- `get_file_output_manager(project_root: str | None = None)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L217) — Convenience function to get a FileOutputManager instance.

## Module values
- `logger` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/file_output_factory.py#L17)

