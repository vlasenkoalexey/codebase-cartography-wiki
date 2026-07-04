---
title: 'Module: tests/unit/test_change_impact_git.py'
type: catalog
provenance: extracted
module: tests/unit/test_change_impact_git.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_change_impact_git`/Test
symbols:
  TestRunGit.test_success: RunGit#test_success().
  TestRunGit.test_failure: RunGit#test_failure().
  TestRunGit.test_timeout: RunGit#test_timeout().
  TestSplitGitLines.test_splits_lines: SplitGitLines#test_splits_lines().
  TestSplitGitLines.test_empty: SplitGitLines#test_empty().
  TestSplitGitLines.test_whitespace_only: SplitGitLines#test_whitespace_only().
  TestUniquePreserveOrder.test_deduplicates: UniquePreserveOrder#test_deduplicates().
  TestUniquePreserveOrder.test_empty: UniquePreserveOrder#test_empty().
  TestNormalizeScopePaths.test_none_returns_empty: NormalizeScopePaths#test_none_returns_empty().
  TestNormalizeScopePaths.test_empty_list: NormalizeScopePaths#test_empty_list().
  TestNormalizeScopePaths.test_deduplicates: NormalizeScopePaths#test_deduplicates().
  TestWithPathspec.test_no_scope: WithPathspec#test_no_scope().
  TestWithPathspec.test_with_scope: WithPathspec#test_with_scope().
  TestGetUntrackedFiles.test_returns_files: GetUntrackedFiles#test_returns_files().
  TestGetUntrackedFiles.test_git_failure: GetUntrackedFiles#test_git_failure().
  TestGetChangedFiles.test_default_mode: GetChangedFiles#test_default_mode().
  TestGetChangedFiles.test_staged_mode: GetChangedFiles#test_staged_mode().
  TestGetChangedFiles.test_branch_mode: GetChangedFiles#test_branch_mode().
  TestGetDiffStat.test_returns_stat: GetDiffStat#test_returns_stat().
  TestGetDiffStat.test_git_failure: GetDiffStat#test_git_failure().
  TestRunGit: RunGit#
  TestSplitGitLines: SplitGitLines#
  TestUniquePreserveOrder: UniquePreserveOrder#
  TestNormalizeScopePaths: NormalizeScopePaths#
  TestWithPathspec: WithPathspec#
  TestGetUntrackedFiles: GetUntrackedFiles#
  TestGetChangedFiles: GetChangedFiles#
  TestGetDiffStat: GetDiffStat#
---
# Module: [`tests/unit/test_change_impact_git.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py)

## Classes
### `TestGetChangedFiles`
- def: [`tests/unit/test_change_impact_git.py:98`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L98)
- signature: `class TestGetChangedFiles:`
- members:
  - `test_branch_mode(self, mock_git)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L113)
  - `test_default_mode(self, mock_git)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L100)
  - `test_staged_mode(self, mock_git)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L107)
- uses (calls/refs, reference-scoped): [`_get_changed_files`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_git.md#_get_changed_files)

### `TestGetDiffStat`
- def: [`tests/unit/test_change_impact_git.py:119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L119)
- signature: `class TestGetDiffStat:`
- members:
  - `test_git_failure(self, mock_git)` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L130)
  - `test_returns_stat(self, mock_git)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L121)
- uses (calls/refs, reference-scoped): [`_get_diff_stat`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_git.md#_get_diff_stat)

### `TestGetUntrackedFiles`
- def: [`tests/unit/test_change_impact_git.py:85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L85)
- signature: `class TestGetUntrackedFiles:`
- members:
  - `test_git_failure(self, mock_git)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L93)
  - `test_returns_files(self, mock_git)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L87)
- uses (calls/refs, reference-scoped): [`_get_untracked_files`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_git.md#_get_untracked_files)

### `TestNormalizeScopePaths`
- def: [`tests/unit/test_change_impact_git.py:61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L61)
- signature: `class TestNormalizeScopePaths:`
- members:
  - `test_deduplicates(self)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L68)
  - `test_empty_list(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L65)
  - `test_none_returns_empty(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L62)
- uses (calls/refs, reference-scoped): [`_normalize_scope_paths`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_git.md#_normalize_scope_paths)

### `TestRunGit`
- def: [`tests/unit/test_change_impact_git.py:19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L19)
- signature: `class TestRunGit:`
- members:
  - `test_failure(self, mock_run)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L28)
  - `test_success(self, mock_run)` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L21)
  - `test_timeout(self, mock_run)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L34)
- uses (calls/refs, reference-scoped): [`_run_git`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_git.md#_run_git)

### `TestSplitGitLines`
- def: [`tests/unit/test_change_impact_git.py:42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L42)
- signature: `class TestSplitGitLines:`
- members:
  - `test_empty(self)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L46)
  - `test_splits_lines(self)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L43)
  - `test_whitespace_only(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L49)
- uses (calls/refs, reference-scoped): [`_split_git_lines`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_git.md#_split_git_lines)

### `TestUniquePreserveOrder`
- def: [`tests/unit/test_change_impact_git.py:53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L53)
- signature: `class TestUniquePreserveOrder:`
- members:
  - `test_deduplicates(self)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L54)
  - `test_empty(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L57)
- uses (calls/refs, reference-scoped): [`_unique_preserve_order`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_git.md#_unique_preserve_order)

### `TestWithPathspec`
- def: [`tests/unit/test_change_impact_git.py:72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L72)
- signature: `class TestWithPathspec:`
- members:
  - `test_no_scope(self)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L73)
  - `test_with_scope(self)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_change_impact_git.py#L78)
- uses (calls/refs, reference-scoped): [`_with_pathspec`](../../tree_sitter_analyzer/mcp/tools/utils/change_impact_git.md#_with_pathspec)

