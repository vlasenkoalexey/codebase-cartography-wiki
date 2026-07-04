---
title: 'Module: tests/unit/mcp/test_utils/test_file_output_manager.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_utils/test_file_output_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_utils.test_file_output_manager`/
symbols:
  TestFileOutputManagerInit.test_init_with_project_root: TestFileOutputManagerInit#test_init_with_project_root().
  TestFileOutputManagerInit.test_init_without_project_root: TestFileOutputManagerInit#test_init_without_project_root().
  TestFileOutputManagerGetManagedInstance.test_get_managed_instance_returns_file_output_manager: TestFileOutputManagerGetManagedInstance#test_get_managed_instance_returns_file_output_manager().
  TestFileOutputManagerCreateInstance.test_create_instance_direct: TestFileOutputManagerCreateInstance#test_create_instance_direct().
  TestFileOutputManagerSetProjectRoot.test_set_project_root_preserves_env_path: TestFileOutputManagerSetProjectRoot#test_set_project_root_preserves_env_path().
  TestFileOutputManagerInit.test_init_with_env_variable: TestFileOutputManagerInit#test_init_with_env_variable().
  TestFileOutputManagerGetManagedInstance.setup_method: TestFileOutputManagerGetManagedInstance#setup_method().
  TestFileOutputManagerGetManagedInstance.test_get_managed_instance_same_root_returns_same_object: TestFileOutputManagerGetManagedInstance#test_get_managed_instance_same_root_returns_same_object().
  TestFileOutputManagerGetManagedInstance.test_get_managed_instance_different_roots_return_different_objects: TestFileOutputManagerGetManagedInstance#test_get_managed_instance_different_roots_return_different_objects().
  manager: manager().
  TestFileOutputManagerSetOutputPath.test_set_output_path_valid: TestFileOutputManagerSetOutputPath#test_set_output_path_valid().
  _normalize_path: _normalize_path().
  temp_dir: temp_dir().
  TestFileOutputManagerInit: TestFileOutputManagerInit#
  TestFileOutputManagerGetManagedInstance: TestFileOutputManagerGetManagedInstance#
  TestFileOutputManagerCreateInstance: TestFileOutputManagerCreateInstance#
  TestFileOutputManagerGetOutputPath: TestFileOutputManagerGetOutputPath#
  TestFileOutputManagerGetOutputPath.test_get_output_path: TestFileOutputManagerGetOutputPath#test_get_output_path().
  TestFileOutputManagerSetOutputPath: TestFileOutputManagerSetOutputPath#
  TestFileOutputManagerSetOutputPath.test_set_output_path_not_exists: TestFileOutputManagerSetOutputPath#test_set_output_path_not_exists().
  TestFileOutputManagerSetOutputPath.test_set_output_path_not_directory: TestFileOutputManagerSetOutputPath#test_set_output_path_not_directory().
  TestFileOutputManagerDetectContentType: TestFileOutputManagerDetectContentType#
  TestFileOutputManagerDetectContentType.test_detect_json_content: TestFileOutputManagerDetectContentType#test_detect_json_content().
  TestFileOutputManagerDetectContentType.test_detect_json_array_content: TestFileOutputManagerDetectContentType#test_detect_json_array_content().
  TestFileOutputManagerDetectContentType.test_detect_toon_content: TestFileOutputManagerDetectContentType#test_detect_toon_content().
  TestFileOutputManagerDetectContentType.test_detect_csv_content: TestFileOutputManagerDetectContentType#test_detect_csv_content().
  TestFileOutputManagerDetectContentType.test_detect_markdown_content: TestFileOutputManagerDetectContentType#test_detect_markdown_content().
  TestFileOutputManagerDetectContentType.test_detect_markdown_table_content: TestFileOutputManagerDetectContentType#test_detect_markdown_table_content().
  TestFileOutputManagerDetectContentType.test_detect_text_content: TestFileOutputManagerDetectContentType#test_detect_text_content().
  TestFileOutputManagerGetFileExtension: TestFileOutputManagerGetFileExtension#
  TestFileOutputManagerGetFileExtension.test_get_extension_json: TestFileOutputManagerGetFileExtension#test_get_extension_json().
  TestFileOutputManagerGetFileExtension.test_get_extension_csv: TestFileOutputManagerGetFileExtension#test_get_extension_csv().
  TestFileOutputManagerGetFileExtension.test_get_extension_markdown: TestFileOutputManagerGetFileExtension#test_get_extension_markdown().
  TestFileOutputManagerGetFileExtension.test_get_extension_toon: TestFileOutputManagerGetFileExtension#test_get_extension_toon().
  TestFileOutputManagerGetFileExtension.test_get_extension_text: TestFileOutputManagerGetFileExtension#test_get_extension_text().
  TestFileOutputManagerGetFileExtension.test_get_extension_unknown: TestFileOutputManagerGetFileExtension#test_get_extension_unknown().
  TestFileOutputManagerGenerateOutputFilename: TestFileOutputManagerGenerateOutputFilename#
  TestFileOutputManagerGenerateOutputFilename.test_generate_filename_json: TestFileOutputManagerGenerateOutputFilename#test_generate_filename_json().
  TestFileOutputManagerGenerateOutputFilename.test_generate_filename_with_existing_extension: TestFileOutputManagerGenerateOutputFilename#test_generate_filename_with_existing_extension().
  TestFileOutputManagerGenerateOutputFilename.test_generate_filename_toon: TestFileOutputManagerGenerateOutputFilename#test_generate_filename_toon().
  TestFileOutputManagerGenerateOutputFilename.test_generate_filename_csv: TestFileOutputManagerGenerateOutputFilename#test_generate_filename_csv().
  TestFileOutputManagerGenerateOutputFilename.test_generate_filename_markdown: TestFileOutputManagerGenerateOutputFilename#test_generate_filename_markdown().
  TestFileOutputManagerGenerateOutputFilename.test_generate_filename_text: TestFileOutputManagerGenerateOutputFilename#test_generate_filename_text().
  TestFileOutputManagerSaveToFile: TestFileOutputManagerSaveToFile#
  TestFileOutputManagerSaveToFile.test_save_to_file_with_filename: TestFileOutputManagerSaveToFile#test_save_to_file_with_filename().
  TestFileOutputManagerSaveToFile.test_save_to_file_with_base_name: TestFileOutputManagerSaveToFile#test_save_to_file_with_base_name().
  TestFileOutputManagerSaveToFile.test_save_to_file_without_filename_or_base_name: TestFileOutputManagerSaveToFile#test_save_to_file_without_filename_or_base_name().
  TestFileOutputManagerSaveToFile.test_save_to_file_creates_directory: TestFileOutputManagerSaveToFile#test_save_to_file_creates_directory().
  TestFileOutputManagerSaveToFile.test_save_to_file_base_name_none: TestFileOutputManagerSaveToFile#test_save_to_file_base_name_none().
  TestFileOutputManagerValidateOutputPath: TestFileOutputManagerValidateOutputPath#
  TestFileOutputManagerValidateOutputPath.test_validate_valid_path: TestFileOutputManagerValidateOutputPath#test_validate_valid_path().
  TestFileOutputManagerValidateOutputPath.test_validate_nonexistent_parent: TestFileOutputManagerValidateOutputPath#test_validate_nonexistent_parent().
  TestFileOutputManagerValidateOutputPath.test_validate_no_write_permission: TestFileOutputManagerValidateOutputPath#test_validate_no_write_permission().
  TestFileOutputManagerSetProjectRoot: TestFileOutputManagerSetProjectRoot#
  TestFileOutputManagerSetProjectRoot.test_set_project_root: TestFileOutputManagerSetProjectRoot#test_set_project_root().
  TestFileOutputManagerSetProjectRoot.test_set_project_root_reinitializes_output_path: TestFileOutputManagerSetProjectRoot#test_set_project_root_reinitializes_output_path().
  TestFileOutputManagerIsToonFormat: TestFileOutputManagerIsToonFormat#
  TestFileOutputManagerIsToonFormat.test_is_toon_format_array_header: TestFileOutputManagerIsToonFormat#test_is_toon_format_array_header().
  TestFileOutputManagerIsToonFormat.test_is_toon_format_key_value_lines: TestFileOutputManagerIsToonFormat#test_is_toon_format_key_value_lines().
  TestFileOutputManagerIsToonFormat.test_is_toon_format_mixed: TestFileOutputManagerIsToonFormat#test_is_toon_format_mixed().
  TestFileOutputManagerIsToonFormat.test_is_toon_format_json: TestFileOutputManagerIsToonFormat#test_is_toon_format_json().
  TestFileOutputManagerIsToonFormat.test_is_toon_format_plain_text: TestFileOutputManagerIsToonFormat#test_is_toon_format_plain_text().
  TestFileOutputManagerIsToonFormat.test_is_toon_format_empty: TestFileOutputManagerIsToonFormat#test_is_toon_format_empty().
---
# Module: [`tests/unit/mcp/test_utils/test_file_output_manager.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py)

## Classes
### `TestFileOutputManagerCreateInstance`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:95`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L95)
- doc: Tests for create_instance method.
- signature: `class TestFileOutputManagerCreateInstance:`
- members:
  - `test_create_instance_direct(self, temp_dir)` — [`L98`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L98) — Test create_instance creates new instance directly.
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root), [`create_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.create_instance)

### `TestFileOutputManagerDetectContentType`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:139`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L139)
- doc: Tests for detect_content_type method.
- signature: `class TestFileOutputManagerDetectContentType:`
- members:
  - `test_detect_csv_content(self, manager)` — [`L157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L157) — Test detecting CSV content.
  - `test_detect_json_array_content(self, manager)` — [`L147`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L147) — Test detecting JSON array content.
  - `test_detect_json_content(self, manager)` — [`L142`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L142) — Test detecting JSON content.
  - `test_detect_markdown_content(self, manager)` — [`L162`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L162) — Test detecting Markdown content.
  - `test_detect_markdown_table_content(self, manager)` — [`L167`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L167) — Test detecting Markdown table content.
  - `test_detect_text_content(self, manager)` — [`L172`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L172) — Test detecting plain text content.
  - `test_detect_toon_content(self, manager)` — [`L152`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L152) — Test detecting TOON content.

### `TestFileOutputManagerGenerateOutputFilename`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:206`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L206)
- doc: Tests for generate_output_filename method.
- signature: `class TestFileOutputManagerGenerateOutputFilename:`
- members:
  - `test_generate_filename_csv(self, manager)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L227) — Test generating filename for CSV content.
  - `test_generate_filename_json(self, manager)` — [`L209`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L209) — Test generating filename for JSON content.
  - `test_generate_filename_markdown(self, manager)` — [`L233`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L233) — Test generating filename for Markdown content.
  - `test_generate_filename_text(self, manager)` — [`L239`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L239) — Test generating filename for text content.
  - `test_generate_filename_toon(self, manager)` — [`L221`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L221) — Test generating filename for TOON content.
  - `test_generate_filename_with_existing_extension(self, manager)` — [`L215`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L215) — Test generating filename removes existing extension.

### `TestFileOutputManagerGetFileExtension`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L178)
- doc: Tests for get_file_extension method.
- signature: `class TestFileOutputManagerGetFileExtension:`
- members:
  - `test_get_extension_csv(self, manager)` — [`L185`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L185) — Test getting extension for CSV.
  - `test_get_extension_json(self, manager)` — [`L181`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L181) — Test getting extension for JSON.
  - `test_get_extension_markdown(self, manager)` — [`L189`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L189) — Test getting extension for Markdown.
  - `test_get_extension_text(self, manager)` — [`L197`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L197) — Test getting extension for text.
  - `test_get_extension_toon(self, manager)` — [`L193`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L193) — Test getting extension for TOON.
  - `test_get_extension_unknown(self, manager)` — [`L201`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L201) — Test getting extension for unknown type.

### `TestFileOutputManagerGetManagedInstance`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:66`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L66)
- doc: Tests for get_managed_instance singleton caching.
- signature: `class TestFileOutputManagerGetManagedInstance:`
- members:
  - `setup_method(self)` — [`L69`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L69)
  - `test_get_managed_instance_different_roots_return_different_objects(self, tmp_path)` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L84) — Test different project_roots return distinct instances.
  - `test_get_managed_instance_returns_file_output_manager(self, tmp_path)` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L72) — Test get_managed_instance returns a FileOutputManager.
  - `test_get_managed_instance_same_root_returns_same_object(self, tmp_path)` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L78) — Test same project_root returns cached instance.
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root), [`get_managed_instance`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_managed_instance), [`_instances`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager._instances)

### `TestFileOutputManagerGetOutputPath`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:105`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L105)
- doc: Tests for get_output_path method.
- signature: `class TestFileOutputManagerGetOutputPath:`
- members:
  - `test_get_output_path(self, manager, temp_dir)` — [`L108`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L108) — Test getting output path.

### `TestFileOutputManagerInit`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:44`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L44)
- doc: Tests for FileOutputManager initialization.
- signature: `class TestFileOutputManagerInit:`
- members:
  - `test_init_with_env_variable(self, temp_dir, monkeypatch)` — [`L59`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L59) — Test initialization with TREE_SITTER_OUTPUT_PATH env variable.
  - `test_init_with_project_root(self, temp_dir)` — [`L47`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L47) — Test initialization with project root.
  - `test_init_without_project_root(self)` — [`L53`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L53) — Test initialization without project root uses cwd.
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.project_root), [`get_output_path`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_output_path)

### `TestFileOutputManagerIsToonFormat`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:366`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L366)
- doc: Tests for _is_toon_format method.
- signature: `class TestFileOutputManagerIsToonFormat:`
- members:
  - `test_is_toon_format_array_header(self, manager)` — [`L369`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L369) — Test detecting TOON array header format.
  - `test_is_toon_format_empty(self, manager)` — [`L394`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L394) — Test empty content is not TOON.
  - `test_is_toon_format_json(self, manager)` — [`L384`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L384) — Test JSON is not detected as TOON.
  - `test_is_toon_format_key_value_lines(self, manager)` — [`L374`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L374) — Test detecting TOON key-value format.
  - `test_is_toon_format_mixed(self, manager)` — [`L379`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L379) — Test detecting TOON format with mixed content.
  - `test_is_toon_format_plain_text(self, manager)` — [`L389`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L389) — Test plain text is not detected as TOON.

### `TestFileOutputManagerSaveToFile`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:246`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L246)
- doc: Tests for save_to_file method.
- signature: `class TestFileOutputManagerSaveToFile:`
- members:
  - `test_save_to_file_base_name_none(self, manager)` — [`L288`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L288) — Test save_to_file fails when base_name is None.
  - `test_save_to_file_creates_directory(self, manager, temp_dir)` — [`L277`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L277) — Test save_to_file creates output directory if needed.
  - `test_save_to_file_with_base_name(self, manager, temp_dir)` — [`L260`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L260) — Test saving content with base name (auto extension).
  - `test_save_to_file_with_filename(self, manager, temp_dir)` — [`L249`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L249) — Test saving content with explicit filename.
  - `test_save_to_file_without_filename_or_base_name(self, manager)` — [`L272`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L272) — Test save_to_file fails without filename or base_name.

### `TestFileOutputManagerSetOutputPath`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:113`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L113)
- doc: Tests for set_output_path method.
- signature: `class TestFileOutputManagerSetOutputPath:`
- members:
  - `test_set_output_path_not_directory(self, manager, temp_dir)` — [`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L130) — Test set_output_path fails when path is not a directory.
  - `test_set_output_path_not_exists(self, manager)` — [`L125`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L125) — Test set_output_path fails when path doesn't exist.
  - `test_set_output_path_valid(self, manager, temp_dir)` — [`L116`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L116) — Test setting valid output path.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestFileOutputManagerSetProjectRoot`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:323`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L323)
- doc: Tests for set_project_root method.
- signature: `class TestFileOutputManagerSetProjectRoot:`
- members:
  - `test_set_project_root(self, manager, temp_dir)` — [`L326`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L326) — Test setting project root.
  - `test_set_project_root_preserves_env_path(self, temp_dir, monkeypatch)` — [`L347`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L347) — Test setting project root doesn't change output path if env is set.
  - `test_set_project_root_reinitializes_output_path(self, manager, temp_dir, monkeypatch)` — [`L334`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L334) — Test setting project root reinitializes output path when not set by env.
- uses (calls/refs, reference-scoped): [`FileOutputManager`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager), [`get_output_path`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.get_output_path), [`set_project_root`](../../../../tree_sitter_analyzer/mcp/utils/file_output_manager.md#FileOutputManager.set_project_root)

### `TestFileOutputManagerValidateOutputPath`
- def: [`tests/unit/mcp/test_utils/test_file_output_manager.py:294`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L294)
- doc: Tests for validate_output_path method.
- signature: `class TestFileOutputManagerValidateOutputPath:`
- members:
  - `test_validate_no_write_permission(self, manager, temp_dir)` — [`L313`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L313) — Test validation fails for no write permission.
  - `test_validate_nonexistent_parent(self, manager, temp_dir)` — [`L303`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L303) — Test validation creates parent directory if it doesn't exist.
  - `test_validate_valid_path(self, manager, temp_dir)` — [`L297`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L297) — Test validating a valid path.

## Functions
- `_normalize_path(path: str)` — [`L18`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L18) — Normalize path to handle Windows short path names (8.3 format).
- `manager(temp_dir)` — [`L39`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L39) — Create a FileOutputManager instance with temp directory.
- `temp_dir()` — [`L32`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_utils/test_file_output_manager.py#L32) — Create a temporary directory for testing.

