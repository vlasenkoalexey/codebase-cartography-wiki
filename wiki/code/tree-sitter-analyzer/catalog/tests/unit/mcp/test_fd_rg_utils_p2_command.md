---
title: 'Module: tests/unit/mcp/test_fd_rg_utils_p2_command.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_fd_rg_utils_p2_command.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_fd_rg_utils_p2_command`/TestBuildRgCommand#
symbols:
  TestBuildRgCommand.test_build_basic_command: test_build_basic_command().
  TestBuildRgCommand.test_build_with_case_smart: test_build_with_case_smart().
  TestBuildRgCommand.test_build_with_case_insensitive: test_build_with_case_insensitive().
  TestBuildRgCommand.test_build_with_case_sensitive: test_build_with_case_sensitive().
  TestBuildRgCommand.test_build_with_fixed_strings: test_build_with_fixed_strings().
  TestBuildRgCommand.test_build_with_word: test_build_with_word().
  TestBuildRgCommand.test_build_with_multiline: test_build_with_multiline().
  TestBuildRgCommand.test_build_with_include_globs: test_build_with_include_globs().
  TestBuildRgCommand.test_build_with_exclude_globs: test_build_with_exclude_globs().
  TestBuildRgCommand.test_build_with_context_before: test_build_with_context_before().
  TestBuildRgCommand.test_build_with_context_after: test_build_with_context_after().
  TestBuildRgCommand.test_build_with_encoding: test_build_with_encoding().
  TestBuildRgCommand.test_build_with_max_count: test_build_with_max_count().
  TestBuildRgCommand.test_build_with_max_filesize: test_build_with_max_filesize().
  TestBuildRgCommand.test_build_with_follow_symlinks: test_build_with_follow_symlinks().
  TestBuildRgCommand.test_build_with_hidden: test_build_with_hidden().
  TestBuildRgCommand.test_build_with_no_ignore: test_build_with_no_ignore().
  TestBuildRgCommand.test_build_count_only_matches: test_build_count_only_matches().
  TestBuildRgCommand: ''
---
# Module: [`tests/unit/mcp/test_fd_rg_utils_p2_command.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py)

## Classes
### `TestBuildRgCommand`
- def: [`tests/unit/mcp/test_fd_rg_utils_p2_command.py:12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L12)
- doc: Tests for build_rg_command function.
- signature: `class TestBuildRgCommand:`
- members:
  - `test_build_basic_command(self)` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L15) — Test building basic ripgrep command.
  - `test_build_count_only_matches(self)` — [`L443`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L443) — Test building with count only matches.
  - `test_build_with_case_insensitive(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L69) — Test building with insensitive case.
  - `test_build_with_case_sensitive(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L93) — Test building with sensitive case.
  - `test_build_with_case_smart(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L45) — Test building with smart case sensitivity.
  - `test_build_with_context_after(self)` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L265) — Test building with context after.
  - `test_build_with_context_before(self)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L240) — Test building with context before.
  - `test_build_with_encoding(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L290) — Test building with encoding.
  - `test_build_with_exclude_globs(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L215) — Test building with exclude globs.
  - `test_build_with_fixed_strings(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L117) — Test building with fixed strings.
  - `test_build_with_follow_symlinks(self)` — [`L365`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L365) — Test building with follow symlinks.
  - `test_build_with_hidden(self)` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L389) — Test building with hidden files.
  - `test_build_with_include_globs(self)` — [`L189`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L189) — Test building with include globs.
  - `test_build_with_max_count(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L315) — Test building with max count.
  - `test_build_with_max_filesize(self)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L340) — Test building with max filesize.
  - `test_build_with_multiline(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L165) — Test building with multiline support.
  - `test_build_with_no_ignore(self)` — [`L419`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L419) — Test building with no ignore.
  - `test_build_with_word(self)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_utils_p2_command.py#L141) — Test building with word matching.
- uses (calls/refs, reference-scoped): [`build_rg_command`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#build_rg_command)

