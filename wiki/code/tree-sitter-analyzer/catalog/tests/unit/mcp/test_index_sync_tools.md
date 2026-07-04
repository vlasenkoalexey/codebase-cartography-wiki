---
title: 'Module: tests/unit/mcp/test_index_sync_tools.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_index_sync_tools.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_index_sync_tools`/
symbols:
  TestCodeGraphFullIndexTool.test_tool_definition: TestCodeGraphFullIndexTool#test_tool_definition().
  TestCodeGraphFullIndexTool.test_schema_defaults: TestCodeGraphFullIndexTool#test_schema_defaults().
  TestCodeGraphFullIndexTool.test_validate_arguments_valid: TestCodeGraphFullIndexTool#test_validate_arguments_valid().
  TestCodeGraphFullIndexTool.test_validate_arguments_invalid: TestCodeGraphFullIndexTool#test_validate_arguments_invalid().
  TestCodeGraphFullIndexTool.test_execute_no_project_root: TestCodeGraphFullIndexTool#test_execute_no_project_root().
  TestCodeGraphFullIndexTool.test_execute_incremental: TestCodeGraphFullIndexTool#test_execute_incremental().
  TestCodeGraphFullIndexTool.test_execute_full: TestCodeGraphFullIndexTool#test_execute_full().
  TestCodeGraphAutoIndexTool.test_tool_definition: TestCodeGraphAutoIndexTool#test_tool_definition().
  TestCodeGraphAutoIndexTool.test_schema_defaults: TestCodeGraphAutoIndexTool#test_schema_defaults().
  TestCodeGraphAutoIndexTool.test_validate_arguments_valid: TestCodeGraphAutoIndexTool#test_validate_arguments_valid().
  TestCodeGraphAutoIndexTool.test_validate_arguments_invalid: TestCodeGraphAutoIndexTool#test_validate_arguments_invalid().
  TestCodeGraphAutoIndexTool.test_execute_status_no_root: TestCodeGraphAutoIndexTool#test_execute_status_no_root().
  TestCodeGraphAutoIndexTool.test_execute_status: TestCodeGraphAutoIndexTool#test_execute_status().
  TestCodeGraphAutoIndexTool.test_execute_warm: TestCodeGraphAutoIndexTool#test_execute_warm().
  TestCodeGraphAutoIndexTool.test_execute_reset: TestCodeGraphAutoIndexTool#test_execute_reset().
  TestCodeGraphIncrementalSyncTool.test_tool_definition: TestCodeGraphIncrementalSyncTool#test_tool_definition().
  TestCodeGraphIncrementalSyncTool.test_validate_arguments_valid: TestCodeGraphIncrementalSyncTool#test_validate_arguments_valid().
  TestCodeGraphIncrementalSyncTool.test_validate_arguments_invalid: TestCodeGraphIncrementalSyncTool#test_validate_arguments_invalid().
  TestCodeGraphIncrementalSyncTool.test_execute_no_project_root: TestCodeGraphIncrementalSyncTool#test_execute_no_project_root().
  TestCodeGraphIncrementalSyncTool.test_execute_sync: TestCodeGraphIncrementalSyncTool#test_execute_sync().
  TestCodeGraphIncrementalSyncTool.test_execute_changes: TestCodeGraphIncrementalSyncTool#test_execute_changes().
  TestCodeGraphIncrementalSyncTool.test_execute_status: TestCodeGraphIncrementalSyncTool#test_execute_status().
  TestIndexToolsRegistered.test_full_index_registered: TestIndexToolsRegistered#test_full_index_registered().
  TestIndexToolsRegistered.test_autoindex_registered: TestIndexToolsRegistered#test_autoindex_registered().
  TestIndexToolsRegistered.test_incremental_sync_registered: TestIndexToolsRegistered#test_incremental_sync_registered().
  TestIndexToolsRegistered.test_registered_tool_count: TestIndexToolsRegistered#test_registered_tool_count().
  project_root: project_root().
  TestCodeGraphFullIndexTool: TestCodeGraphFullIndexTool#
  TestCodeGraphAutoIndexTool: TestCodeGraphAutoIndexTool#
  TestCodeGraphIncrementalSyncTool: TestCodeGraphIncrementalSyncTool#
  TestIndexToolsRegistered: TestIndexToolsRegistered#
---
# Module: [`tests/unit/mcp/test_index_sync_tools.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py)

## Classes
### `TestCodeGraphAutoIndexTool`
- def: [`tests/unit/mcp/test_index_sync_tools.py:101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L101)
- signature: `class TestCodeGraphAutoIndexTool:`
- members:
  - `test_execute_reset(self, project_root)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L177)
  - `test_execute_status(self, project_root)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L153)
  - `test_execute_status_no_root(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L142)
  - `test_execute_warm(self, project_root)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L164)
  - `test_schema_defaults(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L113)
  - `test_tool_definition(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L102)
  - `test_validate_arguments_invalid(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L132)
  - `test_validate_arguments_valid(self)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L122)
- uses (calls/refs, reference-scoped): [`CodeGraphAutoIndexTool`](../../../tree_sitter_analyzer/mcp/tools/auto_index_tool.md#CodeGraphAutoIndexTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/auto_index_tool.md#CodeGraphAutoIndexTool.execute), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/auto_index_tool.md#CodeGraphAutoIndexTool.validate_arguments), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/auto_index_tool.md#CodeGraphAutoIndexTool.get_tool_definition), [`get_tool_schema`](../../../tree_sitter_analyzer/mcp/tools/auto_index_tool.md#CodeGraphAutoIndexTool.get_tool_schema)

### `TestCodeGraphFullIndexTool`
- def: [`tests/unit/mcp/test_index_sync_tools.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L17)
- signature: `class TestCodeGraphFullIndexTool:`
- members:
  - `test_execute_full(self, project_root)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L87)
  - `test_execute_incremental(self, project_root)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L73)
  - `test_execute_no_project_root(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L62)
  - `test_schema_defaults(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L32)
  - `test_tool_definition(self)` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L18)
  - `test_validate_arguments_invalid(self)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L52)
  - `test_validate_arguments_valid(self)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L43)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/mcp/tools/full_index_tool.md#CodeGraphFullIndexTool.execute), [`CodeGraphFullIndexTool`](../../../tree_sitter_analyzer/mcp/tools/full_index_tool.md#CodeGraphFullIndexTool), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/full_index_tool.md#CodeGraphFullIndexTool.validate_arguments), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/full_index_tool.md#CodeGraphFullIndexTool.get_tool_definition), [`get_tool_schema`](../../../tree_sitter_analyzer/mcp/tools/full_index_tool.md#CodeGraphFullIndexTool.get_tool_schema)

### `TestCodeGraphIncrementalSyncTool`
- def: [`tests/unit/mcp/test_index_sync_tools.py:188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L188)
- signature: `class TestCodeGraphIncrementalSyncTool:`
- members:
  - `test_execute_changes(self, project_root)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L244)
  - `test_execute_no_project_root(self)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L221)
  - `test_execute_status(self, project_root)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L254)
  - `test_execute_sync(self, project_root)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L231)
  - `test_tool_definition(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L189)
  - `test_validate_arguments_invalid(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L211)
  - `test_validate_arguments_valid(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L201)
- uses (calls/refs, reference-scoped): [`CodeGraphIncrementalSyncTool`](../../../tree_sitter_analyzer/mcp/tools/incremental_sync_tool.md#CodeGraphIncrementalSyncTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/incremental_sync_tool.md#CodeGraphIncrementalSyncTool.execute), [`validate_arguments`](../../../tree_sitter_analyzer/mcp/tools/incremental_sync_tool.md#CodeGraphIncrementalSyncTool.validate_arguments), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/incremental_sync_tool.md#CodeGraphIncrementalSyncTool.get_tool_definition)

### `TestIndexToolsRegistered`
- def: [`tests/unit/mcp/test_index_sync_tools.py:264`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L264)
- doc: Wave C2: the three index lifecycle tools are no longer top-level
- signature: `class TestIndexToolsRegistered:`
- members:
  - `test_autoindex_registered(self)` — [`L282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L282)
  - `test_full_index_registered(self)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L271)
  - `test_incremental_sync_registered(self)` — [`L292`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L292)
  - `test_registered_tool_count(self)` — [`L302`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L302)
- uses (calls/refs, reference-scoped): [`create_tool_registry`](../../../tree_sitter_analyzer/mcp/_tool_registry.md#create_tool_registry)

## Functions
- `project_root(tmp_path)` — [`L8`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_index_sync_tools.py#L8)

