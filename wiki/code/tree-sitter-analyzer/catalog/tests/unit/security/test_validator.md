---
title: 'Module: tests/unit/security/test_validator.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_validator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_validator`/Test
symbols:
  TestSecurityValidatorInitialization.test_default_initialization: SecurityValidatorInitialization#test_default_initialization().
  TestSecurityValidatorInitialization.test_initialization_with_project_root: SecurityValidatorInitialization#test_initialization_with_project_root().
  TestSanitizeInput.test_sanitize_input_too_long: SanitizeInput#test_sanitize_input_too_long().
  TestSanitizeInput.test_sanitize_input_non_string: SanitizeInput#test_sanitize_input_non_string().
  TestIntegration.test_complete_file_validation_workflow: Integration#test_complete_file_validation_workflow().
  TestSecurityValidatorInitialization.test_initialization_with_invalid_project_root: SecurityValidatorInitialization#test_initialization_with_invalid_project_root().
  TestValidateFilePath.test_validate_file_path_valid_relative: ValidateFilePath#test_validate_file_path_valid_relative().
  TestValidateFilePath.test_validate_file_path_empty: ValidateFilePath#test_validate_file_path_empty().
  TestValidateFilePath.test_validate_file_path_none: ValidateFilePath#test_validate_file_path_none().
  TestValidateFilePath.test_validate_file_path_non_string: ValidateFilePath#test_validate_file_path_non_string().
  TestValidateFilePath.test_validate_file_path_null_byte: ValidateFilePath#test_validate_file_path_null_byte().
  TestValidateFilePath.test_validate_file_path_with_base_path: ValidateFilePath#test_validate_file_path_with_base_path().
  TestValidateFilePath.test_validate_file_path_traversal: ValidateFilePath#test_validate_file_path_traversal().
  TestValidateFilePath.test_validate_file_path_traversal_backslash: ValidateFilePath#test_validate_file_path_traversal_backslash().
  TestValidateFilePath.test_validate_file_path_absolute_with_boundary: ValidateFilePath#test_validate_file_path_absolute_with_boundary().
  TestValidateFilePath.test_validate_file_path_absolute_outside_boundary: ValidateFilePath#test_validate_file_path_absolute_outside_boundary().
  TestValidateFilePath.test_validate_file_path_symlink: ValidateFilePath#test_validate_file_path_symlink().
  TestValidateFilePath.test_validate_file_path_exception_handling: ValidateFilePath#test_validate_file_path_exception_handling().
  TestValidateDirectoryPath.test_validate_directory_path_valid: ValidateDirectoryPath#test_validate_directory_path_valid().
  TestValidateDirectoryPath.test_validate_directory_path_nonexistent: ValidateDirectoryPath#test_validate_directory_path_nonexistent().
  TestValidateDirectoryPath.test_validate_directory_path_file_instead: ValidateDirectoryPath#test_validate_directory_path_file_instead().
  TestValidateDirectoryPath.test_validate_directory_path_must_exist_false: ValidateDirectoryPath#test_validate_directory_path_must_exist_false().
  TestValidateDirectoryPath.test_validate_directory_path_with_base_path: ValidateDirectoryPath#test_validate_directory_path_with_base_path().
  TestValidateRegexPattern.test_validate_regex_pattern_safe: ValidateRegexPattern#test_validate_regex_pattern_safe().
  TestValidateRegexPattern.test_validate_regex_pattern_dangerous: ValidateRegexPattern#test_validate_regex_pattern_dangerous().
  TestValidateRegexPattern.test_validate_regex_pattern_invalid: ValidateRegexPattern#test_validate_regex_pattern_invalid().
  TestSanitizeInput.test_sanitize_input_normal: SanitizeInput#test_sanitize_input_normal().
  TestSanitizeInput.test_sanitize_input_null_bytes: SanitizeInput#test_sanitize_input_null_bytes().
  TestSanitizeInput.test_sanitize_input_html_tags: SanitizeInput#test_sanitize_input_html_tags().
  TestSanitizeInput.test_sanitize_input_control_chars: SanitizeInput#test_sanitize_input_control_chars().
  TestSanitizeInput.test_sanitize_input_dangerous_chars: SanitizeInput#test_sanitize_input_dangerous_chars().
  TestValidateGlobPattern.test_validate_glob_pattern_valid: ValidateGlobPattern#test_validate_glob_pattern_valid().
  TestValidateGlobPattern.test_validate_glob_pattern_empty: ValidateGlobPattern#test_validate_glob_pattern_empty().
  TestValidateGlobPattern.test_validate_glob_pattern_traversal: ValidateGlobPattern#test_validate_glob_pattern_traversal().
  TestValidateGlobPattern.test_validate_glob_pattern_double_slash: ValidateGlobPattern#test_validate_glob_pattern_double_slash().
  TestValidateGlobPattern.test_validate_glob_pattern_double_backslash: ValidateGlobPattern#test_validate_glob_pattern_double_backslash().
  TestValidateGlobPattern.test_validate_glob_pattern_too_long: ValidateGlobPattern#test_validate_glob_pattern_too_long().
  TestValidatePathAlias.test_validate_path_alias: ValidatePathAlias#test_validate_path_alias().
  TestIsSafePath.test_is_safe_path_valid: IsSafePath#test_is_safe_path_valid().
  TestIsSafePath.test_is_safe_path_invalid: IsSafePath#test_is_safe_path_invalid().
  TestValidateWindowsDriveLetter.test_validate_windows_drive_letter_on_windows: ValidateWindowsDriveLetter#test_validate_windows_drive_letter_on_windows().
  TestValidateWindowsDriveLetter.test_validate_windows_drive_letter_on_non_windows: ValidateWindowsDriveLetter#test_validate_windows_drive_letter_on_non_windows().
  TestValidateWindowsDriveLetter.test_validate_windows_drive_letter_normal_path: ValidateWindowsDriveLetter#test_validate_windows_drive_letter_normal_path().
  TestValidateAbsolutePath.test_validate_absolute_path_with_boundary: ValidateAbsolutePath#test_validate_absolute_path_with_boundary().
  TestValidateAbsolutePath.test_validate_absolute_path_outside_boundary: ValidateAbsolutePath#test_validate_absolute_path_outside_boundary().
  TestValidateAbsolutePath.test_validate_absolute_path_no_boundary: ValidateAbsolutePath#test_validate_absolute_path_no_boundary().
  TestValidatePathTraversal.test_validate_path_traversal_normal: ValidatePathTraversal#test_validate_path_traversal_normal().
  TestValidatePathTraversal.test_validate_path_traversal_double_dot: ValidatePathTraversal#test_validate_path_traversal_double_dot().
  TestValidatePathTraversal.test_validate_path_traversal_double_dot_slash: ValidatePathTraversal#test_validate_path_traversal_double_dot_slash().
  TestValidatePathTraversal.test_validate_path_traversal_triple_dot: ValidatePathTraversal#test_validate_path_traversal_triple_dot().
  TestValidateProjectBoundary.test_validate_project_boundary_no_manager: ValidateProjectBoundary#test_validate_project_boundary_no_manager().
  TestValidateProjectBoundary.test_validate_project_boundary_within: ValidateProjectBoundary#test_validate_project_boundary_within().
  TestValidateProjectBoundary.test_validate_project_boundary_outside: ValidateProjectBoundary#test_validate_project_boundary_outside().
  TestIsJunctionOrReparsePoint.test_is_junction_or_reparse_point_non_windows: IsJunctionOrReparsePoint#test_is_junction_or_reparse_point_non_windows().
  TestIsJunctionOrReparsePoint.test_is_junction_or_reparse_point_nonexistent: IsJunctionOrReparsePoint#test_is_junction_or_reparse_point_nonexistent().
  TestIsJunctionOrReparsePoint.test_is_junction_or_reparse_point_exception: IsJunctionOrReparsePoint#test_is_junction_or_reparse_point_exception().
  TestHasJunctionInPath.test_has_junction_in_path_non_windows: HasJunctionInPath#test_has_junction_in_path_non_windows().
  TestHasJunctionInPath.test_has_junction_in_path_exception: HasJunctionInPath#test_has_junction_in_path_exception().
  TestCheckTestEnvironmentAccess.test_check_test_environment_access_temp_dir: CheckTestEnvironmentAccess#test_check_test_environment_access_temp_dir().
  TestCheckTestEnvironmentAccess.test_check_test_environment_access_non_test: CheckTestEnvironmentAccess#test_check_test_environment_access_non_test().
  TestCheckTestEnvironmentAccess.test_check_test_environment_access_test_file: CheckTestEnvironmentAccess#test_check_test_environment_access_test_file().
  TestIntegration.test_complete_directory_validation_workflow: Integration#test_complete_directory_validation_workflow().
  TestIntegration.test_security_layered_validation: Integration#test_security_layered_validation().
  TestSecurityValidatorInitialization: SecurityValidatorInitialization#
  TestValidateFilePath: ValidateFilePath#
  TestValidateDirectoryPath: ValidateDirectoryPath#
  TestValidateRegexPattern: ValidateRegexPattern#
  TestSanitizeInput: SanitizeInput#
  TestValidateGlobPattern: ValidateGlobPattern#
  TestValidatePathAlias: ValidatePathAlias#
  TestIsSafePath: IsSafePath#
  TestValidateWindowsDriveLetter: ValidateWindowsDriveLetter#
  TestValidateAbsolutePath: ValidateAbsolutePath#
  TestValidatePathTraversal: ValidatePathTraversal#
  TestValidateProjectBoundary: ValidateProjectBoundary#
  TestIsJunctionOrReparsePoint: IsJunctionOrReparsePoint#
  TestHasJunctionInPath: HasJunctionInPath#
  TestCheckTestEnvironmentAccess: CheckTestEnvironmentAccess#
  TestIntegration: Integration#
---
# Module: [`tests/unit/security/test_validator.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py)

## Classes
### `TestCheckTestEnvironmentAccess`
- def: [`tests/unit/security/test_validator.py:540`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L540)
- doc: 测试 _check_test_environment_access 方法
- signature: `class TestCheckTestEnvironmentAccess:`
- members:
  - `test_check_test_environment_access_non_test(self)` — [`L555`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L555) — 测试非测试环境
  - `test_check_test_environment_access_temp_dir(self)` — [`L543`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L543) — 测试临时目录访问
  - `test_check_test_environment_access_test_file(self)` — [`L568`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L568) — 测试测试文件
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`_check_test_environment_access`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._check_test_environment_access)

### `TestHasJunctionInPath`
- def: [`tests/unit/security/test_validator.py:516`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L516)
- doc: 测试 _has_junction_in_path 方法
- signature: `class TestHasJunctionInPath:`
- members:
  - `test_has_junction_in_path_exception(self)` — [`L527`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L527) — 测试异常处理
  - `test_has_junction_in_path_non_windows(self)` — [`L519`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L519) — 测试非Windows系统
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`_has_junction_in_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._has_junction_in_path)

### `TestIntegration`
- def: [`tests/unit/security/test_validator.py:581`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L581)
- doc: 测试集成场景
- signature: `class TestIntegration:`
- members:
  - `test_complete_directory_validation_workflow(self)` — [`L601`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L601) — 测试完整目录验证工作流
  - `test_complete_file_validation_workflow(self)` — [`L584`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L584) — 测试完整文件验证工作流
  - `test_security_layered_validation(self)` — [`L615`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L615) — 测试分层安全验证
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path), [`validate_directory_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_directory_path), [`is_safe_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.is_safe_path)

### `TestIsJunctionOrReparsePoint`
- def: [`tests/unit/security/test_validator.py:489`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L489)
- doc: 测试 _is_junction_or_reparse_point 方法
- signature: `class TestIsJunctionOrReparsePoint:`
- members:
  - `test_is_junction_or_reparse_point_exception(self)` — [`L506`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L506) — 测试异常处理
  - `test_is_junction_or_reparse_point_non_windows(self)` — [`L492`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L492) — 测试非Windows系统
  - `test_is_junction_or_reparse_point_nonexistent(self)` — [`L500`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L500) — 测试不存在的路径
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`_is_junction_or_reparse_point`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._is_junction_or_reparse_point)

### `TestIsSafePath`
- def: [`tests/unit/security/test_validator.py:345`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L345)
- doc: 测试 is_safe_path 方法
- signature: `class TestIsSafePath:`
- members:
  - `test_is_safe_path_invalid(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L354) — 测试不安全路径
  - `test_is_safe_path_valid(self)` — [`L348`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L348) — 测试安全路径
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`is_safe_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.is_safe_path)

### `TestSanitizeInput`
- def: [`tests/unit/security/test_validator.py:239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L239)
- doc: 测试 sanitize_input 方法
- signature: `class TestSanitizeInput:`
- members:
  - `test_sanitize_input_control_chars(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L261) — 测试控制字符清理
  - `test_sanitize_input_dangerous_chars(self)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L268) — 测试危险字符清理
  - `test_sanitize_input_html_tags(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L254) — 测试HTML标签清理
  - `test_sanitize_input_non_string(self)` — [`L281`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L281) — 测试非字符串输入
  - `test_sanitize_input_normal(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L242) — 测试正常输入
  - `test_sanitize_input_null_bytes(self)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L248) — 测试空字节清理
  - `test_sanitize_input_too_long(self)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L275) — 测试过长输入
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`sanitize_input`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.sanitize_input)

### `TestSecurityValidatorInitialization`
- def: [`tests/unit/security/test_validator.py:20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L20)
- doc: 测试 SecurityValidator 初始化
- signature: `class TestSecurityValidatorInitialization:`
- members:
  - `test_default_initialization(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L23) — 测试默认初始化
  - `test_initialization_with_invalid_project_root(self)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L37) — 测试无效项目根目录的初始化
  - `test_initialization_with_project_root(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L30) — 测试带项目根目录的初始化
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`boundary_manager`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.boundary_manager), [`regex_checker`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.regex_checker)

### `TestValidateAbsolutePath`
- def: [`tests/unit/security/test_validator.py:390`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L390)
- doc: 测试 _validate_absolute_path 方法
- signature: `class TestValidateAbsolutePath:`
- members:
  - `test_validate_absolute_path_no_boundary(self)` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L412) — 测试无边界的绝对路径
  - `test_validate_absolute_path_outside_boundary(self)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L404) — 测试边界外的绝对路径
  - `test_validate_absolute_path_with_boundary(self)` — [`L393`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L393) — 测试带边界的绝对路径
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`_validate_absolute_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_absolute_path)

### `TestValidateDirectoryPath`
- def: [`tests/unit/security/test_validator.py:156`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L156)
- doc: 测试 validate_directory_path 方法
- signature: `class TestValidateDirectoryPath:`
- members:
  - `test_validate_directory_path_file_instead(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L177) — 测试文件而非目录
  - `test_validate_directory_path_must_exist_false(self)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L192) — 测试不检查存在性
  - `test_validate_directory_path_nonexistent(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L167) — 测试不存在的目录
  - `test_validate_directory_path_valid(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L159) — 测试有效目录路径
  - `test_validate_directory_path_with_base_path(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L202) — 测试带基础路径的目录验证
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`validate_directory_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_directory_path)

### `TestValidateFilePath`
- def: [`tests/unit/security/test_validator.py:45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L45)
- doc: 测试 validate_file_path 方法
- signature: `class TestValidateFilePath:`
- members:
  - `test_validate_file_path_absolute_outside_boundary(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L117) — 测试边界外的绝对路径
  - `test_validate_file_path_absolute_with_boundary(self)` — [`L105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L105) — 测试带边界管理的绝对路径
  - `test_validate_file_path_empty(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L55) — 测试空路径
  - `test_validate_file_path_exception_handling(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L142) — 测试异常处理
  - `test_validate_file_path_non_string(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L69) — 测试非字符串路径
  - `test_validate_file_path_none(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L62) — 测试 None 路径
  - `test_validate_file_path_null_byte(self)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L76) — 测试空字节注入
  - `test_validate_file_path_symlink(self)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L125) — 测试符号链接路径
  - `test_validate_file_path_traversal(self)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L91) — 测试路径遍历攻击
  - `test_validate_file_path_traversal_backslash(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L98) — 测试反斜杠路径遍历
  - `test_validate_file_path_valid_relative(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L48) — 测试有效的相对路径
  - `test_validate_file_path_with_base_path(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L83) — 测试带基础路径的验证
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`validate_file_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_file_path)

### `TestValidateGlobPattern`
- def: [`tests/unit/security/test_validator.py:288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L288)
- doc: 测试 validate_glob_pattern 方法
- signature: `class TestValidateGlobPattern:`
- members:
  - `test_validate_glob_pattern_double_backslash(self)` — [`L319`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L319) — 测试双反斜杠glob模式
  - `test_validate_glob_pattern_double_slash(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L312) — 测试双斜杠glob模式
  - `test_validate_glob_pattern_empty(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L298) — 测试空glob模式
  - `test_validate_glob_pattern_too_long(self)` — [`L326`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L326) — 测试过长glob模式
  - `test_validate_glob_pattern_traversal(self)` — [`L305`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L305) — 测试路径遍历glob模式
  - `test_validate_glob_pattern_valid(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L291) — 测试有效的glob模式
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`validate_glob_pattern`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_glob_pattern)

### `TestValidatePathAlias`
- def: [`tests/unit/security/test_validator.py:334`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L334)
- doc: 测试 validate_path 别名方法
- signature: `class TestValidatePathAlias:`
- members:
  - `test_validate_path_alias(self)` — [`L337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L337) — 测试validate_path别名方法
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`validate_path`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_path)

### `TestValidatePathTraversal`
- def: [`tests/unit/security/test_validator.py:425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L425)
- doc: 测试 _validate_path_traversal 方法
- signature: `class TestValidatePathTraversal:`
- members:
  - `test_validate_path_traversal_double_dot(self)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L435) — 测试双点路径遍历
  - `test_validate_path_traversal_double_dot_slash(self)` — [`L442`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L442) — 测试双点斜杠路径遍历
  - `test_validate_path_traversal_normal(self)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L428) — 测试正常路径
  - `test_validate_path_traversal_triple_dot(self)` — [`L449`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L449) — 测试三点路径遍历
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`_validate_path_traversal`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_path_traversal)

### `TestValidateProjectBoundary`
- def: [`tests/unit/security/test_validator.py:458`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L458)
- doc: 测试 _validate_project_boundary 方法
- signature: `class TestValidateProjectBoundary:`
- members:
  - `test_validate_project_boundary_no_manager(self)` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L461) — 测试无边界管理器
  - `test_validate_project_boundary_outside(self)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L478) — 测试边界外路径
  - `test_validate_project_boundary_within(self)` — [`L468`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L468) — 测试边界内路径
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`_validate_project_boundary`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_project_boundary)

### `TestValidateRegexPattern`
- def: [`tests/unit/security/test_validator.py:214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L214)
- doc: 测试 validate_regex_pattern 方法
- signature: `class TestValidateRegexPattern:`
- members:
  - `test_validate_regex_pattern_dangerous(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L224) — 测试危险的正则表达式
  - `test_validate_regex_pattern_invalid(self)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L231) — 测试无效的正则表达式
  - `test_validate_regex_pattern_safe(self)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L217) — 测试安全的正则表达式
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`validate_regex_pattern`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator.validate_regex_pattern)

### `TestValidateWindowsDriveLetter`
- def: [`tests/unit/security/test_validator.py:361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L361)
- doc: 测试 _validate_windows_drive_letter 方法
- signature: `class TestValidateWindowsDriveLetter:`
- members:
  - `test_validate_windows_drive_letter_normal_path(self)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L382) — 测试正常路径
  - `test_validate_windows_drive_letter_on_non_windows(self)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L373) — 测试非Windows系统上的驱动器字母
  - `test_validate_windows_drive_letter_on_windows(self)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_validator.py#L364) — 测试Windows系统上的驱动器字母
- uses (calls/refs, reference-scoped): [`SecurityValidator`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator), [`_validate_windows_drive_letter`](../../../tree_sitter_analyzer/security/validator.md#SecurityValidator._validate_windows_drive_letter)

