---
title: 'Module: tests/unit/security/test_boundary_manager_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_boundary_manager_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_boundary_manager_coverage`/Test
symbols:
  TestProjectBoundaryManagerInit.test_init_with_valid_path: ProjectBoundaryManagerInit#test_init_with_valid_path().
  TestAddAllowedDirectory.test_add_valid_directory: AddAllowedDirectory#test_add_valid_directory().
  TestAddAllowedDirectory.test_add_empty_directory_raises_error: AddAllowedDirectory#test_add_empty_directory_raises_error().
  TestAddAllowedDirectory.test_add_nonexistent_directory_raises_error: AddAllowedDirectory#test_add_nonexistent_directory_raises_error().
  TestAddAllowedDirectory.test_add_file_as_directory_raises_error: AddAllowedDirectory#test_add_file_as_directory_raises_error().
  TestIsWithinProject.test_file_in_allowed_directory: IsWithinProject#test_file_in_allowed_directory().
  TestListAllowedDirectories.test_list_allowed_directories: ListAllowedDirectories#test_list_allowed_directories().
  TestProjectBoundaryManagerInit.test_init_with_empty_path_raises_error: ProjectBoundaryManagerInit#test_init_with_empty_path_raises_error().
  TestProjectBoundaryManagerInit.test_init_with_none_path_raises_error: ProjectBoundaryManagerInit#test_init_with_none_path_raises_error().
  TestProjectBoundaryManagerInit.test_init_with_nonexistent_path_raises_error: ProjectBoundaryManagerInit#test_init_with_nonexistent_path_raises_error().
  TestProjectBoundaryManagerInit.test_init_with_file_path_raises_error: ProjectBoundaryManagerInit#test_init_with_file_path_raises_error().
  TestProjectBoundaryManagerInit.test_init_with_invalid_type_raises_error: ProjectBoundaryManagerInit#test_init_with_invalid_type_raises_error().
  TestIsWithinProject.test_file_within_project: IsWithinProject#test_file_within_project().
  TestIsWithinProject.test_file_outside_project: IsWithinProject#test_file_outside_project().
  TestIsWithinProject.test_empty_path_returns_false: IsWithinProject#test_empty_path_returns_false().
  TestGetRelativePath.test_relative_path_within_project: GetRelativePath#test_relative_path_within_project().
  TestGetRelativePath.test_relative_path_outside_project: GetRelativePath#test_relative_path_outside_project().
  TestValidateAndResolvePath.test_validate_absolute_path_within_project: ValidateAndResolvePath#test_validate_absolute_path_within_project().
  TestValidateAndResolvePath.test_validate_relative_path_within_project: ValidateAndResolvePath#test_validate_relative_path_within_project().
  TestValidateAndResolvePath.test_validate_path_outside_project: ValidateAndResolvePath#test_validate_path_outside_project().
  TestIsSymlinkSafe.test_nonexistent_file_is_safe: IsSymlinkSafe#test_nonexistent_file_is_safe().
  TestIsSymlinkSafe.test_regular_file_is_safe: IsSymlinkSafe#test_regular_file_is_safe().
  TestIsSymlinkSafe.test_safe_symlink_within_project: IsSymlinkSafe#test_safe_symlink_within_project().
  TestAuditAccess.test_audit_allowed_access: AuditAccess#test_audit_allowed_access().
  TestAuditAccess.test_audit_denied_access: AuditAccess#test_audit_denied_access().
  TestStringRepresentations.test_str_representation: StringRepresentations#test_str_representation().
  TestStringRepresentations.test_repr_representation: StringRepresentations#test_repr_representation().
  TestProjectBoundaryManagerInit: ProjectBoundaryManagerInit#
  TestAddAllowedDirectory: AddAllowedDirectory#
  TestIsWithinProject: IsWithinProject#
  TestGetRelativePath: GetRelativePath#
  TestValidateAndResolvePath: ValidateAndResolvePath#
  TestListAllowedDirectories: ListAllowedDirectories#
  TestIsSymlinkSafe: IsSymlinkSafe#
  TestAuditAccess: AuditAccess#
  TestStringRepresentations: StringRepresentations#
---
# Module: [`tests/unit/security/test_boundary_manager_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py)

## Classes
### `TestAddAllowedDirectory`
- def: [`tests/unit/security/test_boundary_manager_coverage.py:56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L56)
- doc: Tests for add_allowed_directory method
- signature: `class TestAddAllowedDirectory:`
- members:
  - `test_add_empty_directory_raises_error(self, tmp_path)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L69) — Test adding empty string raises SecurityError
  - `test_add_file_as_directory_raises_error(self, tmp_path)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L83) — Test adding file as directory raises SecurityError
  - `test_add_nonexistent_directory_raises_error(self, tmp_path)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L76) — Test adding nonexistent directory raises SecurityError
  - `test_add_valid_directory(self, tmp_path)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L59) — Test adding a valid directory
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`add_allowed_directory`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.add_allowed_directory), [`allowed_directories`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.allowed_directories)

### `TestAuditAccess`
- def: [`tests/unit/security/test_boundary_manager_coverage.py:227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L227)
- doc: Tests for audit_access method
- signature: `class TestAuditAccess:`
- members:
  - `test_audit_allowed_access(self, tmp_path)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L230) — Test auditing allowed file access
  - `test_audit_denied_access(self, tmp_path)` — [`L239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L239) — Test auditing denied file access
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`audit_access`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.audit_access)

### `TestGetRelativePath`
- def: [`tests/unit/security/test_boundary_manager_coverage.py:128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L128)
- doc: Tests for get_relative_path method
- signature: `class TestGetRelativePath:`
- members:
  - `test_relative_path_outside_project(self, tmp_path)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L144) — Test relative path for file outside project returns None
  - `test_relative_path_within_project(self, tmp_path)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L131) — Test relative path for file within project
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`get_relative_path`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.get_relative_path)

### `TestIsSymlinkSafe`
- def: [`tests/unit/security/test_boundary_manager_coverage.py:197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L197)
- doc: Tests for is_symlink_safe method
- signature: `class TestIsSymlinkSafe:`
- members:
  - `test_nonexistent_file_is_safe(self, tmp_path)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L200) — Test nonexistent file is considered safe
  - `test_regular_file_is_safe(self, tmp_path)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L205) — Test regular file is considered safe
  - `test_safe_symlink_within_project(self, tmp_path)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L216) — Test symlink within project is safe
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`is_symlink_safe`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_symlink_safe)

### `TestIsWithinProject`
- def: [`tests/unit/security/test_boundary_manager_coverage.py:94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L94)
- doc: Tests for is_within_project method
- signature: `class TestIsWithinProject:`
- members:
  - `test_empty_path_returns_false(self, tmp_path)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L110) — Test empty path returns False
  - `test_file_in_allowed_directory(self, tmp_path)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L115) — Test file in allowed directory returns True
  - `test_file_outside_project(self, tmp_path)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L105) — Test file outside project returns False
  - `test_file_within_project(self, tmp_path)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L97) — Test file within project returns True
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`is_within_project`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_within_project), [`add_allowed_directory`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.add_allowed_directory)

### `TestListAllowedDirectories`
- def: [`tests/unit/security/test_boundary_manager_coverage.py:180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L180)
- doc: Tests for list_allowed_directories method
- signature: `class TestListAllowedDirectories:`
- members:
  - `test_list_allowed_directories(self, tmp_path)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L183) — Test listing allowed directories
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`add_allowed_directory`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.add_allowed_directory), [`list_allowed_directories`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.list_allowed_directories)

### `TestProjectBoundaryManagerInit`
- def: [`tests/unit/security/test_boundary_manager_coverage.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L17)
- doc: Tests for ProjectBoundaryManager initialization
- signature: `class TestProjectBoundaryManagerInit:`
- members:
  - `test_init_with_empty_path_raises_error(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L26) — Test initialization with empty path raises SecurityError
  - `test_init_with_file_path_raises_error(self, tmp_path)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L41) — Test initialization with file path raises SecurityError
  - `test_init_with_invalid_type_raises_error(self, tmp_path)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L49) — Test initialization with invalid type raises SecurityError
  - `test_init_with_none_path_raises_error(self)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L31) — Test initialization with None raises SecurityError
  - `test_init_with_nonexistent_path_raises_error(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L36) — Test initialization with nonexistent path raises SecurityError
  - `test_init_with_valid_path(self, tmp_path)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L20) — Test initialization with valid path
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`allowed_directories`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.allowed_directories), [`project_root`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.project_root)

### `TestStringRepresentations`
- def: [`tests/unit/security/test_boundary_manager_coverage.py:246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L246)
- doc: Tests for __str__ and __repr__ methods
- signature: `class TestStringRepresentations:`
- members:
  - `test_repr_representation(self, tmp_path)` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L258) — Test repr representation
  - `test_str_representation(self, tmp_path)` — [`L249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L249) — Test string representation
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager)

### `TestValidateAndResolvePath`
- def: [`tests/unit/security/test_boundary_manager_coverage.py:150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L150)
- doc: Tests for validate_and_resolve_path method
- signature: `class TestValidateAndResolvePath:`
- members:
  - `test_validate_absolute_path_within_project(self, tmp_path)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L153) — Test validating absolute path within project
  - `test_validate_path_outside_project(self, tmp_path)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L174) — Test validating path outside project returns None
  - `test_validate_relative_path_within_project(self, tmp_path)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager_coverage.py#L164) — Test validating relative path within project
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`validate_and_resolve_path`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.validate_and_resolve_path)

