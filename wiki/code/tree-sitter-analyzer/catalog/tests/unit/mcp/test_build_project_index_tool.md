---
title: 'Module: tests/unit/mcp/test_build_project_index_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_build_project_index_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_build_project_index_tool`/
symbols:
  TestBuildProjectIndexToolExecution.test_add_notes_stored: TestBuildProjectIndexToolExecution#test_add_notes_stored().
  TestBuildProjectIndexToolExecution.test_existing_notes_preserved_when_add_notes_empty: TestBuildProjectIndexToolExecution#test_existing_notes_preserved_when_add_notes_empty().
  TestBuildProjectIndexToolDefinition.test_description_contains_when_to_use: TestBuildProjectIndexToolDefinition#test_description_contains_when_to_use().
  TestBuildProjectIndexToolDefinition.test_description_contains_when_not_to_use: TestBuildProjectIndexToolDefinition#test_description_contains_when_not_to_use().
  TestBuildProjectIndexToolDefinition.test_add_notes_property_exists: TestBuildProjectIndexToolDefinition#test_add_notes_property_exists().
  TestBuildProjectIndexToolDefinition.test_roots_property_exists: TestBuildProjectIndexToolDefinition#test_roots_property_exists().
  TestBuildProjectIndexToolExecution.test_returns_build_status: TestBuildProjectIndexToolExecution#test_returns_build_status().
  TestBuildProjectIndexToolExecution.test_returns_build_duration: TestBuildProjectIndexToolExecution#test_returns_build_duration().
  TestBuildProjectIndexToolExecution.test_saves_index_to_disk: TestBuildProjectIndexToolExecution#test_saves_index_to_disk().
  TestBuildProjectIndexToolExecution.test_index_saved_to_path_reported: TestBuildProjectIndexToolExecution#test_index_saved_to_path_reported().
  TestBuildProjectIndexToolExecution.test_files_scanned_positive: TestBuildProjectIndexToolExecution#test_files_scanned_positive().
  TestBuildProjectIndexToolExecution.test_languages_found_dict: TestBuildProjectIndexToolExecution#test_languages_found_dict().
  TestBuildProjectIndexToolExecution.test_next_step_field_present: TestBuildProjectIndexToolExecution#test_next_step_field_present().
  TestBuildProjectIndexToolExecution.test_index_content_valid_json: TestBuildProjectIndexToolExecution#test_index_content_valid_json().
  tool: tool().
  TestBuildProjectIndexToolInitialization.test_init_creates_tool: TestBuildProjectIndexToolInitialization#test_init_creates_tool().
  project_dir: project_dir().
  TestBuildProjectIndexToolInitialization: TestBuildProjectIndexToolInitialization#
  TestBuildProjectIndexToolDefinition: TestBuildProjectIndexToolDefinition#
  TestBuildProjectIndexToolExecution: TestBuildProjectIndexToolExecution#
---
# Module: [`tests/unit/mcp/test_build_project_index_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py)

## Classes
### `TestBuildProjectIndexToolDefinition`
- def: [`tests/unit/mcp/test_build_project_index_tool.py:49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L49)
- doc: Tests for get_tool_definition().
- signature: `class TestBuildProjectIndexToolDefinition:`
- members:
  - `test_add_notes_property_exists(self, tool: BuildProjectIndexTool)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L66) — Test that add_notes property is in the schema.
  - `test_description_contains_when_not_to_use(self, tool: BuildProjectIndexTool)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L59) — Test that the description contains WHEN NOT TO USE section.
  - `test_description_contains_when_to_use(self, tool: BuildProjectIndexTool)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L52) — Test that the description contains WHEN TO USE section.
  - `test_roots_property_exists(self, tool: BuildProjectIndexTool)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L72) — Test that roots property is in the schema.
- uses (calls/refs, reference-scoped): [`BuildProjectIndexTool`](../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool.get_tool_definition)

### `TestBuildProjectIndexToolExecution`
- def: [`tests/unit/mcp/test_build_project_index_tool.py:80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L80)
- doc: Tests for execute() — core test class.
- signature: `class TestBuildProjectIndexToolExecution:`
- members:
  - `test_add_notes_stored(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L116) — Test that add_notes is stored in custom_notes field of the index.
  - `test_existing_notes_preserved_when_add_notes_empty(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L165) — Test that existing custom_notes are preserved when add_notes is empty.
  - `test_files_scanned_positive(self, tool: BuildProjectIndexTool)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L129) — Test that files_scanned is a positive integer.
  - `test_index_content_valid_json(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L152) — Test that the saved index file is valid JSON with expected keys.
  - `test_index_saved_to_path_reported(self, tool: BuildProjectIndexTool)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L107) — Test that the result reports the index_saved_to path.
  - `test_languages_found_dict(self, tool: BuildProjectIndexTool)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L137) — Test that languages_found is a dict with at least python.
  - `test_next_step_field_present(self, tool: BuildProjectIndexTool)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L146) — Test that the result contains a next_step field.
  - `test_returns_build_duration(self, tool: BuildProjectIndexTool)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L90) — Test that the result contains a build_duration_ms field.
  - `test_returns_build_status(self, tool: BuildProjectIndexTool)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L84) — Test that the result contains status='built'.
  - `test_saves_index_to_disk(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L98) — Test that the tool saves the index to .tree-sitter-cache/project-index.json.
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`load`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.load), [`BuildProjectIndexTool`](../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool.execute), [`custom_notes`](../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.custom_notes)

### `TestBuildProjectIndexToolInitialization`
- def: [`tests/unit/mcp/test_build_project_index_tool.py:41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L41)
- doc: Tests for tool initialization.
- signature: `class TestBuildProjectIndexToolInitialization:`
- members:
  - `test_init_creates_tool(self, tool: BuildProjectIndexTool)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L44) — Test that initialization creates a tool instance.
- uses (calls/refs, reference-scoped): [`BuildProjectIndexTool`](../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool)

## Functions
- `project_dir(tmp_path: Path)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L23) — Create a minimal project directory for testing.
- `tool(project_dir: Path)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_build_project_index_tool.py#L36) — Create a BuildProjectIndexTool pointing at the temp project directory.

