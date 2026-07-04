---
title: 'Module: tests/unit/core/test_intermediate_files_management.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_intermediate_files_management.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_intermediate_files_management`/
symbols:
  IntermediateFilesManager.is_intermediate_file: IntermediateFilesManager#is_intermediate_file().
  IntermediateFilesManager.track_file: IntermediateFilesManager#track_file().
  IntermediateFilesManager.cleanup_file: IntermediateFilesManager#cleanup_file().
  TestIntermediateFilesManager.test_disabled_manager: TestIntermediateFilesManager#test_disabled_manager().
  IntermediateFilesManager: IntermediateFilesManager#
  TestIntermediateFilesIntegration.test_full_lifecycle: TestIntermediateFilesIntegration#test_full_lifecycle().
  TestIntermediateFilesManager.test_manager_initialization: TestIntermediateFilesManager#test_manager_initialization().
  TestIntermediateFilesIntegration.test_logging_integration: TestIntermediateFilesIntegration#test_logging_integration().
  IntermediateFilesManager.tracked_files: IntermediateFilesManager#tracked_files.
  IntermediateFilesManager.validate_cleanup: IntermediateFilesManager#validate_cleanup().
  IntermediateFilesManager.enabled: IntermediateFilesManager#enabled.
  IntermediateFilesManager.create_temp_directory: IntermediateFilesManager#create_temp_directory().
  IntermediateFilesManager.check_temp_file_limit: IntermediateFilesManager#check_temp_file_limit().
  IntermediateFilesManager.cleanup_expired_files: IntermediateFilesManager#cleanup_expired_files().
  IntermediateFilesManager.get_status: IntermediateFilesManager#get_status().
  TestIntermediateFilesManager.test_get_status: TestIntermediateFilesManager#test_get_status().
  IntermediateFilesManager.cleanup_all: IntermediateFilesManager#cleanup_all().
  TestIntermediateFilesManager.test_track_file: TestIntermediateFilesManager#test_track_file().
  TestIntermediateFilesManager.test_cleanup_file: TestIntermediateFilesManager#test_cleanup_file().
  TestIntermediateFilesManager.test_cleanup_expired_files: TestIntermediateFilesManager#test_cleanup_expired_files().
  TestIntermediateFilesManager.test_cleanup_all: TestIntermediateFilesManager#test_cleanup_all().
  TestIntermediateFilesManager.test_validate_cleanup: TestIntermediateFilesManager#test_validate_cleanup().
  TestIntermediateFilesErrorHandling.test_cleanup_with_permission_error: TestIntermediateFilesErrorHandling#test_cleanup_with_permission_error().
  TestIntermediateFilesErrorHandling.test_invalid_configuration: TestIntermediateFilesErrorHandling#test_invalid_configuration().
  IntermediateFilesManager.temp_directory: IntermediateFilesManager#temp_directory.
  IntermediateFilesManager.config: IntermediateFilesManager#config.
  IntermediateFilesManager.monitoring: IntermediateFilesManager#monitoring.
  TestIntermediateFilesManager.test_create_temp_directory: TestIntermediateFilesManager#test_create_temp_directory().
  TestIntermediateFilesManager.test_check_temp_file_limit: TestIntermediateFilesManager#test_check_temp_file_limit().
  IntermediateFilesManager.creation_times: IntermediateFilesManager#creation_times.
  IntermediateFilesManager.auto_cleanup: IntermediateFilesManager#auto_cleanup.
  IntermediateFilesManager.cleanup_rules: IntermediateFilesManager#cleanup_rules.
  TestIntermediateFilesManager.test_is_intermediate_file_matching: TestIntermediateFilesManager#test_is_intermediate_file_matching().
  TestIntermediateFilesManager.test_cleanup_nonexistent_file: TestIntermediateFilesManager#test_cleanup_nonexistent_file().
  TestIntermediateFilesErrorHandling.test_pattern_matching_edge_cases: TestIntermediateFilesErrorHandling#test_pattern_matching_edge_cases().
  IntermediateFilesManager.intermediate_file_patterns: IntermediateFilesManager#intermediate_file_patterns.
  IntermediateFilesManager.excluded_patterns: IntermediateFilesManager#excluded_patterns.
  IntermediateFilesManager.strict_isolation: IntermediateFilesManager#strict_isolation.
  IntermediateFilesManager.project_pollution_prevention: IntermediateFilesManager#project_pollution_prevention.
  TestIntermediateFilesManager.manager: TestIntermediateFilesManager#manager().
  TestIntermediateFilesErrorHandling.manager: TestIntermediateFilesErrorHandling#manager().
  IntermediateFilesManager._matches_pattern: IntermediateFilesManager#_matches_pattern().
  IntermediateFilesManager.__init__: IntermediateFilesManager#__init__().
  TestIntermediateFilesManager: TestIntermediateFilesManager#
  TestIntermediateFilesManager.config: TestIntermediateFilesManager#config().
  TestIntermediateFilesIntegration: TestIntermediateFilesIntegration#
  TestIntermediateFilesErrorHandling: TestIntermediateFilesErrorHandling#
  TestIntermediateFilesErrorHandling.config: TestIntermediateFilesErrorHandling#config().
---
# Module: [`tests/unit/core/test_intermediate_files_management.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py)

## Classes
### `IntermediateFilesManager`
- def: [`tests/unit/core/test_intermediate_files_management.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L19)
- doc: Intermediate files manager implementation based on .roo-config.json requirements
- signature: `class IntermediateFilesManager:`
- members:
  - `__init__(self, config: dict[str, Any])` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L27) — Initialize the intermediate files manager with configuration
  - `_matches_pattern(self, file_path: str, pattern: str)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L67) — Check if file path matches a glob-like pattern
  - `check_temp_file_limit(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L177) — Check if the number of temp files exceeds the warning limit
  - `cleanup_all(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L145) — Clean up all tracked intermediate files
  - `cleanup_expired_files(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L123) — Clean up files that have exceeded the auto-delete time limit
  - `cleanup_file(self, file_path: str)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L97) — Clean up a specific intermediate file
  - `create_temp_directory(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L73) — Create and return the temporary directory path
  - `get_status(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L192) — Get current status of intermediate files management
  - `is_intermediate_file(self, file_path: str)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L48) — Check if a file matches intermediate file patterns
  - `track_file(self, file_path: str)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L86) — Track an intermediate file for cleanup
  - `validate_cleanup(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L159) — Validate that cleanup was successful
  - `auto_cleanup` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L32)
  - `cleanup_rules` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L38)
  - `config` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L29)
  - `creation_times` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L46)
  - `enabled` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L30)
  - `excluded_patterns` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L37)
  - `intermediate_file_patterns` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L34)
  - `monitoring` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L42)
  - `project_pollution_prevention` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L39)
  - `strict_isolation` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L31)
  - `temp_directory` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L33)
  - `tracked_files` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L45)
- uses (calls/refs, reference-scoped): [`log_error`](../../../tree_sitter_analyzer/utils/logging.md#log_error), [`log_warning`](../../../tree_sitter_analyzer/utils/logging.md#log_warning), [`log_info`](../../../tree_sitter_analyzer/utils/logging.md#log_info)
- used by: (19 test-only callers)

### `TestIntermediateFilesErrorHandling`
- def: [`tests/unit/core/test_intermediate_files_management.py:582`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L582)
- doc: Test error handling in intermediate files management
- signature: `class TestIntermediateFilesErrorHandling:`
- members:
  - `config(self)` — [`L586`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L586) — Provide test configuration
  - `manager(self, config: dict[str, Any])` — [`L602`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L602) — Provide intermediate files manager instance
  - `test_cleanup_with_permission_error(self, manager: IntermediateFilesManager, tmp_path: Path)` — [`L606`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L606) — Test cleanup behavior when file deletion fails
  - `test_invalid_configuration(self)` — [`L647`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L647) — Test manager with invalid or missing configuration
  - `test_pattern_matching_edge_cases(self, manager: IntermediateFilesManager)` — [`L624`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L624) — Test edge cases in pattern matching
- uses (calls/refs, reference-scoped): (8 test-only callers)

### `TestIntermediateFilesIntegration`
- def: [`tests/unit/core/test_intermediate_files_management.py:461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L461)
- doc: Integration tests for intermediate files management
- signature: `class TestIntermediateFilesIntegration:`
- members:
  - `test_full_lifecycle(self, tmp_path: Path)` — [`L464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L464) — Test complete lifecycle of intermediate files management
  - `test_logging_integration(self, mock_log_info: Mock, mock_log_warning: Mock, tmp_path: Path)` — [`L521`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L521) — Test integration with logging system
- uses (calls/refs, reference-scoped): [`log_info`](../../../tree_sitter_analyzer/utils/logging.md#log_info)  (10 test-only)

### `TestIntermediateFilesManager`
- def: [`tests/unit/core/test_intermediate_files_management.py:205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L205)
- doc: Test intermediate files manager functionality
- signature: `class TestIntermediateFilesManager:`
- members:
  - `config(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L209) — Provide test configuration based on .roo-config.json
  - `manager(self, config: dict[str, Any])` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L263) — Provide intermediate files manager instance
  - `test_check_temp_file_limit(self, manager: IntermediateFilesManager)` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L409) — Test temporary file limit checking
  - `test_cleanup_all(self, manager: IntermediateFilesManager, tmp_path: Path)` — [`L370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L370) — Test cleanup of all tracked files
  - `test_cleanup_expired_files(self, manager: IntermediateFilesManager, tmp_path: Path)` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L345) — Test cleanup of expired files
  - `test_cleanup_file(self, manager: IntermediateFilesManager, tmp_path: Path)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L324) — Test individual file cleanup
  - `test_cleanup_nonexistent_file(self, manager: IntermediateFilesManager)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L340) — Test cleanup of non-existent file
  - `test_create_temp_directory(self, manager: IntermediateFilesManager, tmp_path: Path)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L297) — Test temporary directory creation
  - `test_disabled_manager(self)` — [`L442`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L442) — Test manager behavior when disabled
  - `test_get_status(self, manager: IntermediateFilesManager, tmp_path: Path)` — [`L421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L421) — Test status reporting
  - `test_is_intermediate_file_matching(self, manager: IntermediateFilesManager)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L276) — Test intermediate file pattern matching
  - `test_manager_initialization(self, manager: IntermediateFilesManager)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L267) — Test manager initialization with configuration
  - `test_track_file(self, manager: IntermediateFilesManager)` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L310) — Test file tracking functionality
  - `test_validate_cleanup(self, manager: IntermediateFilesManager, tmp_path: Path)` — [`L390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_intermediate_files_management.py#L390) — Test cleanup validation
- uses (calls/refs, reference-scoped): (18 test-only callers)

