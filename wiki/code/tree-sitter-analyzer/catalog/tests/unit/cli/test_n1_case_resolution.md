---
title: 'Module: tests/unit/cli/test_n1_case_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_n1_case_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_n1_case_resolution`/
symbols:
  TestN1SearchContentCaseEcho.test_search_content_default_case_is_bool_false: TestN1SearchContentCaseEcho#test_search_content_default_case_is_bool_false().
  TestN1SearchContentCaseEcho.test_search_content_case_sensitive_is_bool_true: TestN1SearchContentCaseEcho#test_search_content_case_sensitive_is_bool_true().
  PROJECT_ROOT: PROJECT_ROOT.
  TestN1CaseResolutionHelpers.test_collect_case_args_space_form: TestN1CaseResolutionHelpers#test_collect_case_args_space_form().
  TestN1CaseResolutionHelpers.test_collect_case_args_equals_form: TestN1CaseResolutionHelpers#test_collect_case_args_equals_form().
  TestN1CaseResolutionHelpers.test_collect_case_args_duplicates: TestN1CaseResolutionHelpers#test_collect_case_args_duplicates().
  TestN1CaseResolutionHelpers.test_case_to_sensitive_bool_returns_bool: TestN1CaseResolutionHelpers#test_case_to_sensitive_bool_returns_bool().
  TestN1CaseResolutionHelpers.test_warn_on_duplicate_case_no_duplicate: TestN1CaseResolutionHelpers#test_warn_on_duplicate_case_no_duplicate().
  TestN1CaseResolutionHelpers.test_warn_on_duplicate_case_emits_warning: TestN1CaseResolutionHelpers#test_warn_on_duplicate_case_emits_warning().
  TestN1FindAndGrepCaseEcho.test_case_sensitive_echoed_in_response: TestN1FindAndGrepCaseEcho#test_case_sensitive_echoed_in_response().
  TestN1FindAndGrepCaseEcho.test_case_insensitive_echoed: TestN1FindAndGrepCaseEcho#test_case_insensitive_echoed().
  TestN1FindAndGrepCaseEcho.test_default_case_echoed_as_bool: TestN1FindAndGrepCaseEcho#test_default_case_echoed_as_bool().
  TestN1DuplicateCaseFlagsEmitWarning.test_duplicate_case_flags_emit_warning: TestN1DuplicateCaseFlagsEmitWarning#test_duplicate_case_flags_emit_warning().
  TestN1CaseResolutionHelpers: TestN1CaseResolutionHelpers#
  TestN1FindAndGrepCaseEcho: TestN1FindAndGrepCaseEcho#
  TestN1DuplicateCaseFlagsEmitWarning: TestN1DuplicateCaseFlagsEmitWarning#
  TestN1SearchContentCaseEcho: TestN1SearchContentCaseEcho#
---
# Module: [`tests/unit/cli/test_n1_case_resolution.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py)

## Classes
### `TestN1CaseResolutionHelpers`
- def: [`tests/unit/cli/test_n1_case_resolution.py:39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L39)
- doc: Unit tests for the `--case` resolution helper.
- signature: `class TestN1CaseResolutionHelpers:`
- members:
  - `test_case_to_sensitive_bool_returns_bool(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L62)
  - `test_collect_case_args_duplicates(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L50)
  - `test_collect_case_args_equals_form(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L46)
  - `test_collect_case_args_space_form(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L42)
  - `test_warn_on_duplicate_case_emits_warning(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L81)
  - `test_warn_on_duplicate_case_no_duplicate(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L71)
- uses (calls/refs, reference-scoped): [`warn_on_duplicate_case`](../../../tree_sitter_analyzer/cli/commands/_case_resolution.md#warn_on_duplicate_case), [`collect_case_args`](../../../tree_sitter_analyzer/cli/commands/_case_resolution.md#collect_case_args), [`case_to_sensitive_bool`](../../../tree_sitter_analyzer/cli/commands/_case_resolution.md#case_to_sensitive_bool)

### `TestN1DuplicateCaseFlagsEmitWarning`
- def: [`tests/unit/cli/test_n1_case_resolution.py:153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L153)
- doc: End-to-end check via subprocess for the CLI warning.
- signature: `class TestN1DuplicateCaseFlagsEmitWarning:`
- members:
  - `test_duplicate_case_flags_emit_warning(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L157) — ``--case sensitive --case insensitive`` warns on stderr.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestN1FindAndGrepCaseEcho`
- def: [`tests/unit/cli/test_n1_case_resolution.py:105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L105)
- doc: find_and_grep emits a strict bool `case_sensitive` in `meta`.
- signature: `class TestN1FindAndGrepCaseEcho:`
- members:
  - `test_case_insensitive_echoed(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L119)
  - `test_case_sensitive_echoed_in_response(self)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L108)
  - `test_default_case_echoed_as_bool(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L130) — Default ``--case`` (smart / missing) must echo as ``False`` — never None.
- uses (calls/refs, reference-scoped): [`build_search_meta`](../../../tree_sitter_analyzer/mcp/tools/find_and_grep_helpers.md#build_search_meta)

### `TestN1SearchContentCaseEcho`
- def: [`tests/unit/cli/test_n1_case_resolution.py:212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L212)
- doc: search_content also emits a strict bool `case_sensitive`.
- signature: `class TestN1SearchContentCaseEcho:`
- members:
  - `test_search_content_case_sensitive_is_bool_true(self, tmp_path: Path)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L243)
  - `test_search_content_default_case_is_bool_false(self, tmp_path: Path)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L216) — Default ``case`` (no flag) → top-level ``case_sensitive=False bool``.
- uses (calls/refs, reference-scoped): [`SearchContentTool`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool), [`execute`](../../../tree_sitter_analyzer/mcp/tools/search_content_tool.md#SearchContentTool.execute)

## Module values
- `PROJECT_ROOT` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_n1_case_resolution.py#L36)

