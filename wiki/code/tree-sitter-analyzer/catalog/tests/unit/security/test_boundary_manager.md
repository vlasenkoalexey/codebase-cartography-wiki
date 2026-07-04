---
title: 'Module: tests/unit/security/test_boundary_manager.py'
type: catalog
provenance: extracted
module: tests/unit/security/test_boundary_manager.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.security.test_boundary_manager`/
symbols:
  TestIntegration.test_complete_workflow: TestIntegration#test_complete_workflow().
  _normalize_path: _normalize_path().
  TestBoundaryManagerInitialization.test_default_initialization: TestBoundaryManagerInitialization#test_default_initialization().
  TestAddAllowedDirectory.test_add_allowed_directory: TestAddAllowedDirectory#test_add_allowed_directory().
  TestListAllowedDirectories.test_list_allowed_directories: TestListAllowedDirectories#test_list_allowed_directories().
  TestIntegration.test_boundary_enforcement: TestIntegration#test_boundary_enforcement().
  TestBoundaryManagerInitialization.test_custom_project_root: TestBoundaryManagerInitialization#test_custom_project_root().
  TestBoundaryManagerInitialization.test_project_root_as_string: TestBoundaryManagerInitialization#test_project_root_as_string().
  TestAddAllowedDirectory.test_add_nonexistent_directory: TestAddAllowedDirectory#test_add_nonexistent_directory().
  TestAddAllowedDirectory.test_add_file_as_directory: TestAddAllowedDirectory#test_add_file_as_directory().
  TestAddAllowedDirectory.test_add_empty_directory: TestAddAllowedDirectory#test_add_empty_directory().
  TestEdgeCases.test_multiple_allowed_directories: TestEdgeCases#test_multiple_allowed_directories().
  TestBoundaryManagerInitialization.test_empty_project_root: TestBoundaryManagerInitialization#test_empty_project_root().
  TestBoundaryManagerInitialization.test_nonexistent_project_root: TestBoundaryManagerInitialization#test_nonexistent_project_root().
  TestBoundaryManagerInitialization.test_project_root_as_file: TestBoundaryManagerInitialization#test_project_root_as_file().
  TestIsWithinProject.test_is_within_project_valid: TestIsWithinProject#test_is_within_project_valid().
  TestIsWithinProject.test_is_within_project_outside: TestIsWithinProject#test_is_within_project_outside().
  TestIsWithinProject.test_is_within_project_empty_path: TestIsWithinProject#test_is_within_project_empty_path().
  TestIsWithinProject.test_is_within_project_nonexistent: TestIsWithinProject#test_is_within_project_nonexistent().
  TestGetRelativePath.test_get_relative_path_valid: TestGetRelativePath#test_get_relative_path_valid().
  TestGetRelativePath.test_get_relative_path_outside: TestGetRelativePath#test_get_relative_path_outside().
  TestGetRelativePath.test_get_relative_path_with_dots: TestGetRelativePath#test_get_relative_path_with_dots().
  TestValidateAndResolvePath.test_validate_and_resolve_path_valid: TestValidateAndResolvePath#test_validate_and_resolve_path_valid().
  TestValidateAndResolvePath.test_validate_and_resolve_path_relative: TestValidateAndResolvePath#test_validate_and_resolve_path_relative().
  TestValidateAndResolvePath.test_validate_and_resolve_path_outside: TestValidateAndResolvePath#test_validate_and_resolve_path_outside().
  TestValidateAndResolvePath.test_validate_and_resolve_path_nonexistent: TestValidateAndResolvePath#test_validate_and_resolve_path_nonexistent().
  TestIsSymlinkSafe.test_is_symlink_safe_regular_file: TestIsSymlinkSafe#test_is_symlink_safe_regular_file().
  TestIsSymlinkSafe.test_is_symlink_safe_within_boundary: TestIsSymlinkSafe#test_is_symlink_safe_within_boundary().
  TestIsSymlinkSafe.test_is_symlink_safe_outside_boundary: TestIsSymlinkSafe#test_is_symlink_safe_outside_boundary().
  TestIsSymlinkSafe.test_is_symlink_safe_nonexistent: TestIsSymlinkSafe#test_is_symlink_safe_nonexistent().
  TestAuditAccess.test_audit_access_within_boundary: TestAuditAccess#test_audit_access_within_boundary().
  TestAuditAccess.test_audit_access_outside_boundary: TestAuditAccess#test_audit_access_outside_boundary().
  TestEdgeCases.test_deeply_nested_directory: TestEdgeCases#test_deeply_nested_directory().
  TestEdgeCases.test_unicode_filename: TestEdgeCases#test_unicode_filename().
  TestEdgeCases.test_path_with_spaces: TestEdgeCases#test_path_with_spaces().
  TestStringRepresentation.test_str_representation: TestStringRepresentation#test_str_representation().
  TestStringRepresentation.test_repr_representation: TestStringRepresentation#test_repr_representation().
  TestBoundaryManagerInitialization: TestBoundaryManagerInitialization#
  TestAddAllowedDirectory: TestAddAllowedDirectory#
  TestIsWithinProject: TestIsWithinProject#
  TestGetRelativePath: TestGetRelativePath#
  TestValidateAndResolvePath: TestValidateAndResolvePath#
  TestListAllowedDirectories: TestListAllowedDirectories#
  TestIsSymlinkSafe: TestIsSymlinkSafe#
  TestAuditAccess: TestAuditAccess#
  TestStringRepresentation: TestStringRepresentation#
  TestEdgeCases: TestEdgeCases#
  TestIntegration: TestIntegration#
---
# Module: [`tests/unit/security/test_boundary_manager.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py)

## Classes
### `TestAddAllowedDirectory`
- def: [`tests/unit/security/test_boundary_manager.py:93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L93)
- doc: 测试添加允许的目录
- signature: `class TestAddAllowedDirectory:`
- members:
  - `test_add_allowed_directory(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L96) — 测试添加允许的目录
  - `test_add_empty_directory(self)` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L135) — 测试添加空目录路径
  - `test_add_file_as_directory(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L124) — 测试添加文件作为目录
  - `test_add_nonexistent_directory(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L110) — 测试添加不存在的目录
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`add_allowed_directory`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.add_allowed_directory), [`allowed_directories`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.allowed_directories)  (1 test-only)

### `TestAuditAccess`
- def: [`tests/unit/security/test_boundary_manager.py:358`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L358)
- doc: 测试访问审计
- signature: `class TestAuditAccess:`
- members:
  - `test_audit_access_outside_boundary(self)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L373) — 测试审计边界外访问
  - `test_audit_access_within_boundary(self)` — [`L361`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L361) — 测试审计边界内访问
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`audit_access`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.audit_access)

### `TestBoundaryManagerInitialization`
- def: [`tests/unit/security/test_boundary_manager.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L37)
- doc: 测试 ProjectBoundaryManager 初始化
- signature: `class TestBoundaryManagerInitialization:`
- members:
  - `test_custom_project_root(self)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L53) — 测试自定义项目根路径
  - `test_default_initialization(self)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L40) — 测试默认初始化
  - `test_empty_project_root(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L67) — 测试空项目根路径
  - `test_nonexistent_project_root(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L73) — 测试不存在的项目根路径
  - `test_project_root_as_file(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L84) — 测试项目根路径是文件而非目录
  - `test_project_root_as_string(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L60) — 测试项目根路径作为字符串
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`SecurityError`](../../../tree_sitter_analyzer/_exceptions_security.md#SecurityError), [`allowed_directories`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.allowed_directories), [`project_root`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.project_root)  (1 test-only)

### `TestEdgeCases`
- def: [`tests/unit/security/test_boundary_manager.py:411`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L411)
- doc: 测试边缘情况
- signature: `class TestEdgeCases:`
- members:
  - `test_deeply_nested_directory(self)` — [`L414`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L414) — 测试深层嵌套目录
  - `test_multiple_allowed_directories(self)` — [`L447`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L447) — 测试多个允许的目录
  - `test_path_with_spaces(self)` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L436) — 测试包含空格的路径
  - `test_unicode_filename(self)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L425) — 测试 Unicode 文件名
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`is_within_project`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_within_project), [`add_allowed_directory`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.add_allowed_directory), [`allowed_directories`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.allowed_directories)

### `TestGetRelativePath`
- def: [`tests/unit/security/test_boundary_manager.py:190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L190)
- doc: 测试获取相对路径
- signature: `class TestGetRelativePath:`
- members:
  - `test_get_relative_path_outside(self)` — [`L205`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L205) — 测试获取项目外路径的相对路径
  - `test_get_relative_path_valid(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L193) — 测试获取有效的相对路径
  - `test_get_relative_path_with_dots(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L215) — 测试包含点的路径
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`get_relative_path`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.get_relative_path)

### `TestIntegration`
- def: [`tests/unit/security/test_boundary_manager.py:461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L461)
- doc: 集成测试
- signature: `class TestIntegration:`
- members:
  - `test_boundary_enforcement(self)` — [`L490`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L490) — 测试边界强制执行
  - `test_complete_workflow(self)` — [`L464`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L464) — 测试完整工作流程
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`is_within_project`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_within_project), [`validate_and_resolve_path`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.validate_and_resolve_path), [`get_relative_path`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.get_relative_path), [`is_symlink_safe`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_symlink_safe), [`audit_access`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.audit_access)

### `TestIsSymlinkSafe`
- def: [`tests/unit/security/test_boundary_manager.py:295`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L295)
- doc: 测试符号链接安全性检查
- signature: `class TestIsSymlinkSafe:`
- members:
  - `test_is_symlink_safe_nonexistent(self)` — [`L346`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L346) — 测试不存在的文件
  - `test_is_symlink_safe_outside_boundary(self)` — [`L330`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L330) — 测试边界外符号链接的安全性
  - `test_is_symlink_safe_regular_file(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L298) — 测试常规文件的安全性
  - `test_is_symlink_safe_within_boundary(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L312) — 测试边界内符号链接的安全性
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`is_symlink_safe`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_symlink_safe)

### `TestIsWithinProject`
- def: [`tests/unit/security/test_boundary_manager.py:145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L145)
- doc: 测试项目边界检查
- signature: `class TestIsWithinProject:`
- members:
  - `test_is_within_project_empty_path(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L169) — 测试空路径
  - `test_is_within_project_nonexistent(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L177) — 测试不存在的文件
  - `test_is_within_project_outside(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L159) — 测试项目外路径
  - `test_is_within_project_valid(self)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L148) — 测试有效的项目内路径
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`is_within_project`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.is_within_project)

### `TestListAllowedDirectories`
- def: [`tests/unit/security/test_boundary_manager.py:274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L274)
- doc: 测试列出允许的目录
- signature: `class TestListAllowedDirectories:`
- members:
  - `test_list_allowed_directories(self)` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L277) — 测试列出允许的目录
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`add_allowed_directory`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.add_allowed_directory), [`list_allowed_directories`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.list_allowed_directories)  (1 test-only)

### `TestStringRepresentation`
- def: [`tests/unit/security/test_boundary_manager.py:385`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L385)
- doc: 测试字符串表示
- signature: `class TestStringRepresentation:`
- members:
  - `test_repr_representation(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L399) — 测试 __repr__ 方法
  - `test_str_representation(self)` — [`L388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L388) — 测试 __str__ 方法
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager)

### `TestValidateAndResolvePath`
- def: [`tests/unit/security/test_boundary_manager.py:227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L227)
- doc: 测试路径验证和解析
- signature: `class TestValidateAndResolvePath:`
- members:
  - `test_validate_and_resolve_path_nonexistent(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L263) — 测试验证和解析不存在的路径
  - `test_validate_and_resolve_path_outside(self)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L253) — 测试验证和解析项目外路径
  - `test_validate_and_resolve_path_relative(self)` — [`L241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L241) — 测试验证和解析相对路径
  - `test_validate_and_resolve_path_valid(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L230) — 测试验证和解析有效路径
- uses (calls/refs, reference-scoped): [`ProjectBoundaryManager`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager), [`validate_and_resolve_path`](../../../tree_sitter_analyzer/security/boundary_manager.md#ProjectBoundaryManager.validate_and_resolve_path)

## Functions
- `_normalize_path(path: str)` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/security/test_boundary_manager.py#L24) — Normalize path to handle Windows short path names (8.3 format).

