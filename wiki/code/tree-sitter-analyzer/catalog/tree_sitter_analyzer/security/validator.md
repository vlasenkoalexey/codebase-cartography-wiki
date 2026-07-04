---
title: 'Module: tree_sitter_analyzer/security/validator.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/security/validator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.security.validator`/
symbols:
  SecurityValidator: SecurityValidator#
  SecurityValidator.validate_file_path: SecurityValidator#validate_file_path().
  SecurityValidator.sanitize_input: SecurityValidator#sanitize_input().
  SecurityValidator.boundary_manager: SecurityValidator#boundary_manager.
  SecurityValidator._validate_absolute_path: SecurityValidator#_validate_absolute_path().
  HAS_CTYPES: HAS_CTYPES.
  SecurityValidator.validate_regex_pattern: SecurityValidator#validate_regex_pattern().
  SecurityValidator.validate_directory_path: SecurityValidator#validate_directory_path().
  SecurityValidator._is_junction_or_reparse_point: SecurityValidator#_is_junction_or_reparse_point().
  SecurityValidator._check_test_environment_access: SecurityValidator#_check_test_environment_access().
  SecurityValidator.validate_glob_pattern: SecurityValidator#validate_glob_pattern().
  SecurityValidator._validate_project_boundary: SecurityValidator#_validate_project_boundary().
  SecurityValidator._validate_path_traversal: SecurityValidator#_validate_path_traversal().
  SecurityValidator.regex_checker: SecurityValidator#regex_checker.
  SecurityValidator._scan_path_for_symlinks_and_junctions: SecurityValidator#_scan_path_for_symlinks_and_junctions().
  SecurityValidator.is_safe_path: SecurityValidator#is_safe_path().
  _ctypes_reparse_check: _ctypes_reparse_check().
  SecurityValidator._validate_symlinks_and_junctions: SecurityValidator#_validate_symlinks_and_junctions().
  SecurityValidator._reject_if_parent_has_junction: SecurityValidator#_reject_if_parent_has_junction().
  SecurityValidator._validate_windows_drive_letter: SecurityValidator#_validate_windows_drive_letter().
  SecurityValidator._has_junction_in_path: SecurityValidator#_has_junction_in_path().
  SecurityValidator.validate_path: SecurityValidator#validate_path().
  SecurityValidator._path_under_test_temp_dirs: SecurityValidator#_path_under_test_temp_dirs().
  IS_WINDOWS: IS_WINDOWS.
  FILE_ATTRIBUTE_REPARSE_POINT: FILE_ATTRIBUTE_REPARSE_POINT.
  INVALID_FILE_ATTRIBUTES: INVALID_FILE_ATTRIBUTES.
  _matches_temp_file_pattern: _matches_temp_file_pattern().
  SecurityValidator._is_test_environment_active: SecurityValidator#_is_test_environment_active().
  SecurityValidator.__init__: SecurityValidator#__init__().
---
# Module: [`tree_sitter_analyzer/security/validator.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py)

## Classes
### `SecurityValidator`
- def: [`tree_sitter_analyzer/security/validator.py:70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L70) — documented in [tree_sitter_analyzer-mcp-server](../../../concepts/tree_sitter_analyzer-mcp-server.md)
- doc: Unified security validation framework.
- signature: `class SecurityValidator:`
- members:
  - `__init__(self, project_root: str | None = None)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L84) — Initialize security validator.
  - `_check_test_environment_access(self, file_path: str)` — [`L516`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L516) — Check if absolute path access is allowed in test/development environment.
  - `_has_junction_in_path(self, path: Path)` — [`L441`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L441) — Check if any parent directory in the path is a junction.
  - `_is_junction_or_reparse_point(self, path: Path)` — [`L413`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L413) — Check if a path is a Windows junction or reparse point.
  - `_is_test_environment_active()` — [`L556`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L556) — Return True if pytest/CI/GitHub-Actions/test-arg env markers are present.
  - `_path_under_test_temp_dirs(self, file_path: str)` — [`L573`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L573) — Return True if ``file_path`` resolves under any common temp directory.
  - `_reject_if_parent_has_junction(self, full_path: Path)` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L254) — Walk parent dirs for junctions/reparse points. OS errors → accept.
  - `_scan_path_for_symlinks_and_junctions(self, path_obj: Path, *, label: str)` — [`L213`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L213) — Reject ``path_obj`` if it's a symlink, junction, or reparse point.
  - `_validate_absolute_path(self, file_path: str)` — [`L489`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L489) — Validate absolute path with project boundary and test environment checks. — documented in [tree_sitter_analyzer-security-validator](../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `_validate_path_traversal(self, file_path: str)` — [`L598`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L598) — Validate file path for directory traversal attempts. — documented in [tree_sitter_analyzer-security-validator](../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `_validate_project_boundary(self, file_path: str, base_path: str | None)` — [`L621`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L621) — Validate file path against project boundaries when base_path is provided. — documented in [tree_sitter_analyzer-security-validator](../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `_validate_symlinks_and_junctions(self, file_path: str, base_path: str | None)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L174) — Layer 7: reject symbolic links, Windows junctions, and reparse points.
  - `_validate_windows_drive_letter(self, file_path: str)` — [`L465`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L465) — Validate Windows drive letter on non-Windows systems.
  - `is_safe_path(self, path: str, base_path: str | None = None)` — [`L399`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L399) — Check if a path is safe (backward compatibility method).
  - `sanitize_input(self, user_input: str, max_length: int = 1000)` — [`L312`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L312) — Sanitize user input by removing dangerous characters. — documented in [tree_sitter_analyzer-security-validator](../../../concepts/tree_sitter_analyzer-security-validator.md)
  - `validate_directory_path(self, dir_path: str, must_exist: bool = True)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L265) — Validate directory path for security and existence.
  - `validate_file_path(self, file_path: str, base_path: str | None = None)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L113) — Validate file path with comprehensive security checks. — documented in [tree_sitter_analyzer-mcp-tools-read_partial_tool](../../../concepts/tree_sitter_analyzer-mcp-tools-read_partial_tool.md)
  - `validate_glob_pattern(self, pattern: str)` — [`L347`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L347) — Validate glob pattern for safe file matching.
  - `validate_path(self, path: str, base_path: str | None = None)` — [`L384`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L384) — Alias for validate_file_path for backward compatibility.
  - `validate_regex_pattern(self, pattern: str)` — [`L300`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L300) — Validate regex pattern for ReDoS attack prevention.
  - `boundary_manager` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L91)
  - `regex_checker` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L109)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`log_warning`](../utils/logging.md#log_warning), [`ProjectBoundaryManager`](boundary_manager.md#ProjectBoundaryManager), [`SecurityError`](../_exceptions_security.md#SecurityError), [`RegexSafetyChecker`](regex_checker.md#RegexSafetyChecker), [`validate_pattern`](regex_checker.md#RegexSafetyChecker.validate_pattern), [`is_within_project`](boundary_manager.md#ProjectBoundaryManager.is_within_project), [`HAS_CTYPES`](validator.md#HAS_CTYPES), [`project_root`](boundary_manager.md#ProjectBoundaryManager.project_root), [`_ctypes_reparse_check`](validator.md#_ctypes_reparse_check), [`IS_WINDOWS`](validator.md#IS_WINDOWS), [`_matches_temp_file_pattern`](validator.md#_matches_temp_file_pattern)
- used by: [`resolve_and_validate_file_path`](../mcp/tools/base_tool.md#BaseMCPTool.resolve_and_validate_file_path), [`set_project_path`](../mcp/server.md#TreeSitterAnalyzerMCPServer.set_project_path), [`execute`](../mcp/tools/universal_analyze_tool.md#UniversalAnalyzeTool.execute), [`_ensure_initialized`](../core/analysis_engine.md#UnifiedAnalysisEngine._ensure_initialized), [`security_validator`](../mcp/tools/base_tool.md#BaseMCPTool.security_validator), [`_resolve_query`](../cli/commands/query_command.md#QueryCommand._resolve_query), [`detect_language`](../cli/commands/base_command.md#BaseCommand.detect_language), [`resolve_and_validate_directory_path`](../mcp/tools/base_tool.md#BaseMCPTool.resolve_and_validate_directory_path), [`_execute_single_file`](../mcp/tools/analyze_scale_tool.md#AnalyzeScaleTool._execute_single_file), [`validate_file`](../cli/commands/base_command.md#BaseCommand.validate_file), [`security_validator`](../mcp/server.md#TreeSitterAnalyzerMCPServer.security_validator), [`_validate_file_path_security`](../mcp/server.md#TreeSitterAnalyzerMCPServer._validate_file_path_security), [`security_validator`](../cli/commands/base_command.md#BaseCommand.security_validator), [`_validate_skills_root`](../mcp/tools/agent_skills_tool.md#AgentSkillsTool._validate_skills_root), [`_validate_target_path`](../mcp/tools/agent_workflow_tool.md#AgentWorkflowTool._validate_target_path), [`_sanitize_optional_arg`](../mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool._sanitize_optional_arg)  (142 test-only)

## Functions
- `_ctypes_reparse_check(path: Path)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L33) — Return reparse-point status via the Windows ctypes call, or ``None`` if unsupported.
- `_matches_temp_file_pattern(file_name: str)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L55) — Return True for filenames that look like test/temp artifacts.

## Module values
- `FILE_ATTRIBUTE_REPARSE_POINT` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L29)
- `HAS_CTYPES` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L18)
- `INVALID_FILE_ATTRIBUTES` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L30)
- `IS_WINDOWS` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/validator.py#L28)

