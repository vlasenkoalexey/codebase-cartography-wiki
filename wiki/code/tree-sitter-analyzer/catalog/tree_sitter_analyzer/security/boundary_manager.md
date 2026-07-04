---
title: 'Module: tree_sitter_analyzer/security/boundary_manager.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/security/boundary_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.security.boundary_manager`/ProjectBoundaryManager#
symbols:
  ProjectBoundaryManager: ''
  ProjectBoundaryManager.is_within_project: is_within_project().
  ProjectBoundaryManager.add_allowed_directory: add_allowed_directory().
  ProjectBoundaryManager.allowed_directories: allowed_directories.
  ProjectBoundaryManager.validate_and_resolve_path: validate_and_resolve_path().
  ProjectBoundaryManager.get_relative_path: get_relative_path().
  ProjectBoundaryManager.is_symlink_safe: is_symlink_safe().
  ProjectBoundaryManager.audit_access: audit_access().
  ProjectBoundaryManager.project_root: project_root.
  ProjectBoundaryManager._no_unsafe_symlink_hop: _no_unsafe_symlink_hop().
  ProjectBoundaryManager.__str__: __str__().
  ProjectBoundaryManager.__repr__: __repr__().
  ProjectBoundaryManager.list_allowed_directories: list_allowed_directories().
  ProjectBoundaryManager.__init__: __init__().
---
# Module: [`tree_sitter_analyzer/security/boundary_manager.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py)

## Classes
### `ProjectBoundaryManager`
- def: [`tree_sitter_analyzer/security/boundary_manager.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L15) — documented in [tree_sitter_analyzer-security-validator](../../../concepts/tree_sitter_analyzer-security-validator.md)
- doc: Project boundary manager for access control.
- signature: `class ProjectBoundaryManager:`
- members:
  - `__init__(self, project_root: str)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L29) — Initialize project boundary manager.
  - `__repr__(self)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L264) — Detailed representation of boundary manager.
  - `__str__(self)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L260) — String representation of boundary manager.
  - `_no_unsafe_symlink_hop(self, file_path_obj: Path)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L226) — Walk each path component; reject when any symlink leaves the project.
  - `add_allowed_directory(self, directory: str)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L73) — Add an additional allowed directory.
  - `audit_access(self, file_path: str, operation: str)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L244) — Log file access for security auditing.
  - `get_relative_path(self, file_path: str)` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L134) — Get relative path from project root if within boundaries.
  - `is_symlink_safe(self, file_path: str)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L205) — Check if file path is safe from symlink attacks.
  - `is_within_project(self, file_path: str)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L98) — Check if file path is within project boundaries. — documented in [tree_sitter_analyzer-security-validator](../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `list_allowed_directories(self)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L196) — Get list of all allowed directories.
  - `validate_and_resolve_path(self, file_path: str)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L167) — Validate path and return resolved absolute path if within boundaries.
  - `allowed_directories` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L60) — documented in [tree_sitter_analyzer-security-validator](../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `project_root` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/boundary_manager.py#L59)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`log_warning`](../utils/logging.md#log_warning), [`SecurityError`](../_exceptions_security.md#SecurityError), [`log_info`](../utils/logging.md#log_info)
- used by: [`boundary_manager`](validator.md#SecurityValidator.boundary_manager), [`_validate_absolute_path`](validator.md#SecurityValidator._validate_absolute_path), [`HAS_CTYPES`](validator.md#HAS_CTYPES), [`_validate_project_boundary`](validator.md#SecurityValidator._validate_project_boundary)  (84 test-only)

