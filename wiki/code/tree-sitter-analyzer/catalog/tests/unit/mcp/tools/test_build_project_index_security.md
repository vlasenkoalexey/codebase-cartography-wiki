---
title: 'Module: tests/unit/mcp/tools/test_build_project_index_security.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_build_project_index_security.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_build_project_index_security`/
symbols:
  TestAbsolutePathOutsideProject.test_etc_raises: TestAbsolutePathOutsideProject#test_etc_raises().
  TestAbsolutePathOutsideProject.test_tmp_raises_when_not_project: TestAbsolutePathOutsideProject#test_tmp_raises_when_not_project().
  TestAbsolutePathOutsideProject.test_home_dot_ssh_raises: TestAbsolutePathOutsideProject#test_home_dot_ssh_raises().
  TestRelativeTraversalOutsideProject.test_dotdot_slash_raises: TestRelativeTraversalOutsideProject#test_dotdot_slash_raises().
  TestRelativeTraversalOutsideProject.test_dotdot_raises: TestRelativeTraversalOutsideProject#test_dotdot_raises().
  TestRelativeTraversalOutsideProject.test_deep_traversal_raises: TestRelativeTraversalOutsideProject#test_deep_traversal_raises().
  TestValidRootsWithinProject.test_dot_succeeds: TestValidRootsWithinProject#test_dot_succeeds().
  TestValidRootsWithinProject.test_absolute_project_root_succeeds: TestValidRootsWithinProject#test_absolute_project_root_succeeds().
  TestValidRootsWithinProject.test_subdirectory_succeeds: TestValidRootsWithinProject#test_subdirectory_succeeds().
  TestEmptyOrMissingRoots.test_missing_roots_key_uses_project_root: TestEmptyOrMissingRoots#test_missing_roots_key_uses_project_root().
  TestEmptyOrMissingRoots.test_empty_list_uses_project_root: TestEmptyOrMissingRoots#test_empty_list_uses_project_root().
  TestEmptyOrMissingRoots.test_none_uses_project_root: TestEmptyOrMissingRoots#test_none_uses_project_root().
  TestNonExistentPath.test_nonexistent_relative_raises: TestNonExistentPath#test_nonexistent_relative_raises().
  TestNonExistentPath.test_nonexistent_absolute_within_project_raises: TestNonExistentPath#test_nonexistent_absolute_within_project_raises().
  TestExecuteSecurityEnvelope.test_etc_returns_error_envelope: TestExecuteSecurityEnvelope#test_etc_returns_error_envelope().
  TestExecuteSecurityEnvelope.test_dotdot_returns_error_envelope: TestExecuteSecurityEnvelope#test_dotdot_returns_error_envelope().
  tool: tool().
  project_dir: project_dir().
  TestAbsolutePathOutsideProject: TestAbsolutePathOutsideProject#
  TestRelativeTraversalOutsideProject: TestRelativeTraversalOutsideProject#
  TestValidRootsWithinProject: TestValidRootsWithinProject#
  TestEmptyOrMissingRoots: TestEmptyOrMissingRoots#
  TestNonExistentPath: TestNonExistentPath#
  TestExecuteSecurityEnvelope: TestExecuteSecurityEnvelope#
---
# Module: [`tests/unit/mcp/tools/test_build_project_index_security.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py)

## Classes
### `TestAbsolutePathOutsideProject`
- def: [`tests/unit/mcp/tools/test_build_project_index_security.py:43`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L43)
- doc: roots=\['/etc'\] must raise ValueError (path traversal attack).
- signature: `class TestAbsolutePathOutsideProject:`
- members:
  - `test_etc_raises(self, tool: BuildProjectIndexTool)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L46)
  - `test_home_dot_ssh_raises(self, tool: BuildProjectIndexTool)` — [`L55`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L55) — Sensitive absolute paths must be refused.
  - `test_tmp_raises_when_not_project(self, tool: BuildProjectIndexTool)` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L50) — Any absolute path not under project_root must be refused.
- uses (calls/refs, reference-scoped): [`BuildProjectIndexTool`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool.validate_arguments)

### `TestEmptyOrMissingRoots`
- def: [`tests/unit/mcp/tools/test_build_project_index_security.py:116`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L116)
- doc: Omitted or empty roots fall back to project_root without error.
- signature: `class TestEmptyOrMissingRoots:`
- members:
  - `test_empty_list_uses_project_root(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L128`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L128)
  - `test_missing_roots_key_uses_project_root(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L119`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L119)
  - `test_none_uses_project_root(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L136`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L136)
- uses (calls/refs, reference-scoped): [`BuildProjectIndexTool`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool.validate_arguments)

### `TestExecuteSecurityEnvelope`
- def: [`tests/unit/mcp/tools/test_build_project_index_security.py:171`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L171)
- doc: execute() must NOT propagate ValueError — it must return a safe envelope.
- signature: `class TestExecuteSecurityEnvelope:`
- members:
  - `test_dotdot_returns_error_envelope(self, tool: BuildProjectIndexTool)` — [`L185`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L185)
  - `test_etc_returns_error_envelope(self, tool: BuildProjectIndexTool)` — [`L175`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L175)
- uses (calls/refs, reference-scoped): [`BuildProjectIndexTool`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool.execute)

### `TestNonExistentPath`
- def: [`tests/unit/mcp/tools/test_build_project_index_security.py:150`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L150)
- doc: roots=\['nonexistent_path'\] must raise ValueError (directory does not exist).
- signature: `class TestNonExistentPath:`
- members:
  - `test_nonexistent_absolute_within_project_raises(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L157`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L157) — Even within project_root, nonexistent directories are rejected.
  - `test_nonexistent_relative_raises(self, tool: BuildProjectIndexTool)` — [`L153`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L153)
- uses (calls/refs, reference-scoped): [`BuildProjectIndexTool`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool.validate_arguments)

### `TestRelativeTraversalOutsideProject`
- def: [`tests/unit/mcp/tools/test_build_project_index_security.py:69`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L69)
- doc: roots=\['../'\] resolves outside project_root and must be refused.
- signature: `class TestRelativeTraversalOutsideProject:`
- members:
  - `test_deep_traversal_raises(self, tool: BuildProjectIndexTool)` — [`L80`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L80)
  - `test_dotdot_raises(self, tool: BuildProjectIndexTool)` — [`L76`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L76)
  - `test_dotdot_slash_raises(self, tool: BuildProjectIndexTool)` — [`L72`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L72)
- uses (calls/refs, reference-scoped): [`BuildProjectIndexTool`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool.validate_arguments)

### `TestValidRootsWithinProject`
- def: [`tests/unit/mcp/tools/test_build_project_index_security.py:90`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L90)
- doc: roots=\['.'\] and roots=\[project_root\] must pass validation.
- signature: `class TestValidRootsWithinProject:`
- members:
  - `test_absolute_project_root_succeeds(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L98`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L98)
  - `test_dot_succeeds(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L93`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L93)
  - `test_subdirectory_succeeds(self, tool: BuildProjectIndexTool, project_dir: Path)` — [`L104`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L104)
- uses (calls/refs, reference-scoped): [`BuildProjectIndexTool`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool), [`validate_arguments`](../../../../tree_sitter_analyzer/mcp/tools/build_project_index_tool.md#BuildProjectIndexTool.validate_arguments)

## Functions
- `project_dir(tmp_path: Path)` — [`L25`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L25) — Minimal project directory used as project_root for all security tests.
- `tool(project_dir: Path)` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_build_project_index_security.py#L33) — Tool bound to the temp project directory.

