---
title: 'Module: tests/integration/mcp/test_tools/test_file_output_manager.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_tools/test_file_output_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_tools.test_file_output_manager`/TestFileOutputManager#
symbols:
  TestFileOutputManager.manager: manager.
  TestFileOutputManager.temp_dir: temp_dir.
  TestFileOutputManager.test_init_with_project_root: test_init_with_project_root().
  TestFileOutputManager.test_save_to_file_with_filename: test_save_to_file_with_filename().
  TestFileOutputManager.test_save_to_file_with_base_name: test_save_to_file_with_base_name().
  TestFileOutputManager.test_save_to_file_creates_directory: test_save_to_file_creates_directory().
  TestFileOutputManager.test_set_output_path_valid: test_set_output_path_valid().
  TestFileOutputManager.test_set_project_root_updates_output_path: test_set_project_root_updates_output_path().
  TestFileOutputManager.test_set_project_root_preserves_env_path: test_set_project_root_preserves_env_path().
  TestFileOutputManager.test_init_with_env_variable: test_init_with_env_variable().
  TestFileOutputManager.test_validate_output_path_valid: test_validate_output_path_valid().
  TestFileOutputManager.test_validate_output_path_no_write_permission: test_validate_output_path_no_write_permission().
  TestFileOutputManager.test_set_output_path_invalid: test_set_output_path_invalid().
  TestFileOutputManager.test_set_output_path_not_directory: test_set_output_path_not_directory().
  TestFileOutputManager.test_detect_content_type_json: test_detect_content_type_json().
  TestFileOutputManager.test_detect_content_type_csv: test_detect_content_type_csv().
  TestFileOutputManager.test_detect_content_type_markdown: test_detect_content_type_markdown().
  TestFileOutputManager.test_detect_content_type_text: test_detect_content_type_text().
  TestFileOutputManager.test_get_file_extension: test_get_file_extension().
  TestFileOutputManager.test_generate_output_filename: test_generate_output_filename().
  TestFileOutputManager.test_save_to_file_missing_parameters: test_save_to_file_missing_parameters().
  TestFileOutputManager.test_content_type_edge_cases: test_content_type_edge_cases().
  TestFileOutputManager.test_filename_generation_edge_cases: test_filename_generation_edge_cases().
  TestFileOutputManager.teardown_method: teardown_method().
  TestFileOutputManager: ''
  TestFileOutputManager.setup_method: setup_method().
---
# Module: [`tests/integration/mcp/test_tools/test_file_output_manager.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py)

## Classes
### `TestFileOutputManager`
- def: [`tests/integration/mcp/test_tools/test_file_output_manager.py:19`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L19)
- doc: Test cases for FileOutputManager class.
- signature: `class TestFileOutputManager:`
- members:
  - `setup_method(self)` — [`L22`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L22) — Set up test fixtures before each test method.
  - `teardown_method(self)` — [`L27`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L27) — Clean up test fixtures after each test method.
  - `test_content_type_edge_cases(self)` — [`L244`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L244) — Test content type detection edge cases.
  - `test_detect_content_type_csv(self)` — [`L57`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L57) — Test content type detection for CSV content.
  - `test_detect_content_type_json(self)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L46) — Test content type detection for JSON content.
  - `test_detect_content_type_markdown(self)` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L63) — Test content type detection for Markdown content.
  - `test_detect_content_type_text(self)` — [`L82`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L82) — Test content type detection for plain text content.
  - `test_filename_generation_edge_cases(self)` — [`L260`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L260) — Test filename generation edge cases.
  - `test_generate_output_filename(self)` — [`L96`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L96) — Test output filename generation.
  - `test_get_file_extension(self)` — [`L88`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L88) — Test file extension mapping.
  - `test_init_with_env_variable(self, monkeypatch)` — [`L40`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L40) — Test FileOutputManager initialization with environment variable.
  - `test_init_with_project_root(self)` — [`L34`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L34) — Test FileOutputManager initialization with project root.
  - `test_save_to_file_creates_directory(self)` — [`L158`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L158) — Test that save_to_file creates parent directories if needed.
  - `test_save_to_file_missing_parameters(self)` — [`L149`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L149) — Test saving content to file with missing parameters.
  - `test_save_to_file_with_base_name(self)` — [`L133`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L133) — Test saving content to file with base name (auto extension).
  - `test_save_to_file_with_filename(self)` — [`L117`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L117) — Test saving content to file with specific filename.
  - `test_set_output_path_invalid(self)` — [`L198`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L198) — Test setting invalid output path.
  - `test_set_output_path_not_directory(self)` — [`L206`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L206) — Test setting output path to a file instead of directory.
  - `test_set_output_path_valid(self)` — [`L193`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L193) — Test setting valid output path.
  - `test_set_project_root_preserves_env_path(self, monkeypatch)` — [`L224`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L224) — Test that setting project root preserves env var path.
  - `test_set_project_root_updates_output_path(self)` — [`L214`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L214) — Test that setting project root updates output path when no env var is set.
  - `test_validate_output_path_no_write_permission(self, monkeypatch)` — [`L180`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L180) — Test output path validation with no write permission.
  - `test_validate_output_path_valid(self)` — [`L172`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L172) — Test output path validation with valid path.
  - `manager` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L25)
  - `temp_dir` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_tools/test_file_output_manager.py#L24)
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root), [`detect_content_type`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.detect_content_type), [`save_to_file`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.save_to_file), [`get_output_path`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_output_path), [`generate_output_filename`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.generate_output_filename), [`get_file_extension`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_file_extension), [`set_output_path`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.set_output_path), [`set_project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.set_project_root), [`validate_output_path`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.validate_output_path)

