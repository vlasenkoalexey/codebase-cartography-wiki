---
title: 'Module: tests/unit/mcp/test_fd_rg_native_flags.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_fd_rg_native_flags.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_fd_rg_native_flags`/
symbols:
  _BASE_RG_KW._BASE_RG_KW: _BASE_RG_KW._BASE_RG_KW.
  _BASE_FD_KW._BASE_FD_KW: _BASE_FD_KW._BASE_FD_KW.
  TestRgHiddenBug.test_hidden_true_uses_long_form: TestRgHiddenBug#test_hidden_true_uses_long_form().
  TestRgHiddenBug.test_hidden_false_emits_neither: TestRgHiddenBug#test_hidden_false_emits_neither().
  TestRgNewFlags.test_file_types: TestRgNewFlags#test_file_types().
  TestRgNewFlags.test_exclude_types: TestRgNewFlags#test_exclude_types().
  TestRgNewFlags.test_files_with_matches_drops_json: TestRgNewFlags#test_files_with_matches_drops_json().
  TestRgNewFlags.test_only_matching: TestRgNewFlags#test_only_matching().
  TestRgNewFlags.test_context_combined: TestRgNewFlags#test_context_combined().
  TestRgNewFlags.test_context_combined_yields_to_explicit_before_after: TestRgNewFlags#test_context_combined_yields_to_explicit_before_after().
  TestRgNewFlags.test_pcre2: TestRgNewFlags#test_pcre2().
  TestRgNewFlags.test_max_depth: TestRgNewFlags#test_max_depth().
  TestRgNewFlags.test_sort: TestRgNewFlags#test_sort().
  TestRgNewFlags.test_invert_match: TestRgNewFlags#test_invert_match().
  TestRgNewFlags.test_include_stats: TestRgNewFlags#test_include_stats().
  TestRgNewFlags.test_no_config_always_on: TestRgNewFlags#test_no_config_always_on().
  TestFdNewFlags.test_min_depth: TestFdNewFlags#test_min_depth().
  TestFdNewFlags.test_prune: TestFdNewFlags#test_prune().
  TestFdNewFlags.test_threads: TestFdNewFlags#test_threads().
  TestFdNewFlags.test_threads_zero_omitted: TestFdNewFlags#test_threads_zero_omitted().
  TestFdNewFlags.test_strip_cwd_prefix: TestFdNewFlags#test_strip_cwd_prefix().
  TestFdNewFlags.test_one_file_system: TestFdNewFlags#test_one_file_system().
  TestFdNewFlags.test_show_errors: TestFdNewFlags#test_show_errors().
  TestBackwardCompat.test_rg_minimal_call_unchanged: TestBackwardCompat#test_rg_minimal_call_unchanged().
  TestBackwardCompat.test_fd_minimal_call_unchanged: TestBackwardCompat#test_fd_minimal_call_unchanged().
  TestRgHiddenBug: TestRgHiddenBug#
  TestRgNewFlags: TestRgNewFlags#
  TestFdNewFlags: TestFdNewFlags#
  TestBackwardCompat: TestBackwardCompat#
---
# Module: [`tests/unit/mcp/test_fd_rg_native_flags.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py)

## Classes
### `TestBackwardCompat`
- def: [`tests/unit/mcp/test_fd_rg_native_flags.py:193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L193)
- doc: The new kwargs must default to off — existing call sites unaffected.
- signature: `class TestBackwardCompat:`
- members:
  - `test_fd_minimal_call_unchanged(self)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L216)
  - `test_rg_minimal_call_unchanged(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L196)
- uses (calls/refs, reference-scoped): [`build_rg_command`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#build_rg_command), [`build_fd_command`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#build_fd_command)  (2 test-only)

### `TestFdNewFlags`
- def: [`tests/unit/mcp/test_fd_rg_native_flags.py:159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L159)
- doc: Each new fd keyword propagates to the right fd CLI token.
- signature: `class TestFdNewFlags:`
- members:
  - `test_min_depth(self)` — [`L162`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L162)
  - `test_one_file_system(self)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L184)
  - `test_prune(self)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L167)
  - `test_show_errors(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L188)
  - `test_strip_cwd_prefix(self)` — [`L180`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L180)
  - `test_threads(self)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L171)
  - `test_threads_zero_omitted(self)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L176)
- uses (calls/refs, reference-scoped): [`build_fd_command`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#build_fd_command)  (1 test-only)

### `TestRgHiddenBug`
- def: [`tests/unit/mcp/test_fd_rg_native_flags.py:68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L68)
- doc: Pain #27: hidden=True must emit --hidden, NOT -H.
- signature: `class TestRgHiddenBug:`
- members:
  - `test_hidden_false_emits_neither(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L79)
  - `test_hidden_true_uses_long_form(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L71)
- uses (calls/refs, reference-scoped): [`build_rg_command`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#build_rg_command)  (1 test-only)

### `TestRgNewFlags`
- def: [`tests/unit/mcp/test_fd_rg_native_flags.py:85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L85)
- doc: Each new keyword propagates to the right ripgrep CLI token.
- signature: `class TestRgNewFlags:`
- members:
  - `test_context_combined(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L110)
  - `test_context_combined_yields_to_explicit_before_after(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L118)
  - `test_exclude_types(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L95)
  - `test_file_types(self)` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L88)
  - `test_files_with_matches_drops_json(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L100)
  - `test_include_stats(self)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L149)
  - `test_invert_match(self)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L145)
  - `test_max_depth(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L132)
  - `test_no_config_always_on(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L153)
  - `test_only_matching(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L106)
  - `test_pcre2(self)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L128)
  - `test_sort(self, sort_val)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L140)
- uses (calls/refs, reference-scoped): [`build_rg_command`](../../../tree_sitter_analyzer/mcp/tools/fd_rg_utils.md#build_rg_command)  (1 test-only)

## Module values
- `_BASE_FD_KW` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L48)
- `_BASE_RG_KW` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_fd_rg_native_flags.py#L27)

