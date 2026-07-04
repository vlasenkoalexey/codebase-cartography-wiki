---
title: 'Module: tests/unit/mcp/test_get_project_summary_tool.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_get_project_summary_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_get_project_summary_tool`/
symbols:
  TestGetProjectSummaryToolExecution.test_stale_index_reports_age_correctly: TestGetProjectSummaryToolExecution#test_stale_index_reports_age_correctly().
  TestGetProjectSummaryToolExecution.test_force_refresh_on_stale_rebuilds: TestGetProjectSummaryToolExecution#test_force_refresh_on_stale_rebuilds().
  TestGetProjectSummaryToolExecution.test_custom_notes_included_in_toon_format: TestGetProjectSummaryToolExecution#test_custom_notes_included_in_toon_format().
  TestGetProjectSummaryToolExecution.test_fresh_index_loaded_from_disk: TestGetProjectSummaryToolExecution#test_fresh_index_loaded_from_disk().
  TestGetProjectSummaryToolDefinition.test_description_contains_when_to_use: TestGetProjectSummaryToolDefinition#test_description_contains_when_to_use().
  TestGetProjectSummaryToolDefinition.test_description_contains_when_not_to_use: TestGetProjectSummaryToolDefinition#test_description_contains_when_not_to_use().
  TestGetProjectSummaryToolDefinition.test_format_property_enum: TestGetProjectSummaryToolDefinition#test_format_property_enum().
  TestGetProjectSummaryToolExecution.test_returns_toon_format_by_default: TestGetProjectSummaryToolExecution#test_returns_toon_format_by_default().
  TestGetProjectSummaryToolExecution.test_toon_format_contains_project_name: TestGetProjectSummaryToolExecution#test_toon_format_contains_project_name().
  TestGetProjectSummaryToolExecution.test_toon_format_contains_purpose: TestGetProjectSummaryToolExecution#test_toon_format_contains_purpose().
  TestGetProjectSummaryToolExecution.test_json_format_option: TestGetProjectSummaryToolExecution#test_json_format_option().
  TestGetProjectSummaryToolExecution.test_force_refresh_rebuilds_index: TestGetProjectSummaryToolExecution#test_force_refresh_rebuilds_index().
  TestGetProjectSummaryToolExecution.test_python_language_detected: TestGetProjectSummaryToolExecution#test_python_language_detected().
  tool: tool().
  TestGetProjectSummaryToolInitialization.test_init_creates_tool: TestGetProjectSummaryToolInitialization#test_init_creates_tool().
  project_dir: project_dir().
  TestGetProjectSummaryToolInitialization: TestGetProjectSummaryToolInitialization#
  TestGetProjectSummaryToolDefinition: TestGetProjectSummaryToolDefinition#
  TestGetProjectSummaryToolExecution: TestGetProjectSummaryToolExecution#
---
# Module: [`tests/unit/mcp/test_get_project_summary_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py)

## Classes
### `TestGetProjectSummaryToolDefinition`
- def: [`tests/unit/mcp/test_get_project_summary_tool.py:55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L55)
- doc: Tests for get_tool_definition().
- signature: `class TestGetProjectSummaryToolDefinition:`
- members:
  - `test_description_contains_when_not_to_use(self, tool: GetProjectSummaryTool)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L65) — Test that the description contains WHEN NOT TO USE.
  - `test_description_contains_when_to_use(self, tool: GetProjectSummaryTool)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L58) — Test that the description contains WHEN TO USE.
  - `test_format_property_enum(self, tool: GetProjectSummaryTool)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L72) — Test that the format property has toon and json options.
- uses (calls/refs, reference-scoped): [`GetProjectSummaryTool`](../../../tree_sitter_analyzer/mcp/tools/get_project_summary_tool.md#GetProjectSummaryTool), [`get_tool_definition`](../../../tree_sitter_analyzer/mcp/tools/get_project_summary_tool.md#GetProjectSummaryTool.get_tool_definition)

### `TestGetProjectSummaryToolExecution`
- def: [`tests/unit/mcp/test_get_project_summary_tool.py:80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L80)
- doc: Tests for execute() — core test class.
- signature: `class TestGetProjectSummaryToolExecution:`
- members:
  - `test_custom_notes_included_in_toon_format(self, tool: GetProjectSummaryTool, project_dir: Path)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L197) — Test that custom_notes appear in the toon output when include_notes=True.
  - `test_force_refresh_on_stale_rebuilds(self, tool: GetProjectSummaryTool, project_dir: Path)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L160) — Test that force_refresh=True on a stale index triggers a rebuild.
  - `test_force_refresh_rebuilds_index(self, tool: GetProjectSummaryTool, project_dir: Path)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L122) — Test that force_refresh=True triggers a rebuild and saves a fresh index.
  - `test_fresh_index_loaded_from_disk(self, tool: GetProjectSummaryTool, project_dir: Path)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L177) — Test that a fresh on-disk index is loaded without rebuilding.
  - `test_json_format_option(self, tool: GetProjectSummaryTool)` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L112) — Test that format='json' returns a structured dictionary.
  - `test_python_language_detected(self, tool: GetProjectSummaryTool)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L211) — Test that Python files are counted in language_distribution.
  - `test_returns_toon_format_by_default(self, tool: GetProjectSummaryTool)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L84) — Test that default call returns format='toon' and a summary string.
  - `test_stale_index_reports_age_correctly(self, tool: GetProjectSummaryTool, project_dir: Path)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L139) — Test that a stale index (>24h) is loaded and its age reported correctly.
  - `test_toon_format_contains_project_name(self, tool: GetProjectSummaryTool, project_dir: Path)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L94) — Test that the toon summary contains the project name.
  - `test_toon_format_contains_purpose(self, tool: GetProjectSummaryTool)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L103) — Test that the toon summary includes a purpose line when README is present.
- uses (calls/refs, reference-scoped): [`ProjectIndexManager`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager), [`build`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.build), [`execute`](../../../tree_sitter_analyzer/mcp/tools/get_project_summary_tool.md#GetProjectSummaryTool.execute), [`GetProjectSummaryTool`](../../../tree_sitter_analyzer/mcp/tools/get_project_summary_tool.md#GetProjectSummaryTool), [`save`](../../../tree_sitter_analyzer/mcp/utils/project_index/_manager.md#ProjectIndexManager.save), [`custom_notes`](../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.custom_notes), [`updated_at`](../../../tree_sitter_analyzer/mcp/utils/project_index/_models.md#ProjectIndex.updated_at)

### `TestGetProjectSummaryToolInitialization`
- def: [`tests/unit/mcp/test_get_project_summary_tool.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L47)
- doc: Tests for tool initialization.
- signature: `class TestGetProjectSummaryToolInitialization:`
- members:
  - `test_init_creates_tool(self, tool: GetProjectSummaryTool)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L50) — Test that initialization creates a tool instance.
- uses (calls/refs, reference-scoped): [`GetProjectSummaryTool`](../../../tree_sitter_analyzer/mcp/tools/get_project_summary_tool.md#GetProjectSummaryTool)

## Functions
- `project_dir(tmp_path: Path)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L24) — Create a minimal project structure for testing.
- `tool(project_dir: Path)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_get_project_summary_tool.py#L42) — Create a GetProjectSummaryTool pointing at the temp project directory.

