---
title: 'Module: tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_r37as_docstring_comment_suppression`/
symbols:
  _ids: _ids().
  TestSecurityScannerDocstringSuppression.test_eval_inside_triple_quoted_docstring_is_ignored: TestSecurityScannerDocstringSuppression#test_eval_inside_triple_quoted_docstring_is_ignored().
  TestSecurityScannerDocstringSuppression.test_real_eval_call_still_detected: TestSecurityScannerDocstringSuppression#test_real_eval_call_still_detected().
  TestSecurityScannerDocstringSuppression.test_bare_except_inside_docstring_is_ignored: TestSecurityScannerDocstringSuppression#test_bare_except_inside_docstring_is_ignored().
  TestAntiPatternCommentSuppression.test_mutable_default_in_comment_is_ignored: TestAntiPatternCommentSuppression#test_mutable_default_in_comment_is_ignored().
  TestAntiPatternCommentSuppression.test_real_mutable_default_still_detected: TestAntiPatternCommentSuppression#test_real_mutable_default_still_detected().
  TestAntiPatternCommentSuppression.test_bare_except_in_comment_is_ignored: TestAntiPatternCommentSuppression#test_bare_except_in_comment_is_ignored().
  TestSecurityScannerDocstringSuppression: TestSecurityScannerDocstringSuppression#
  TestAntiPatternCommentSuppression: TestAntiPatternCommentSuppression#
  test_refactoring_suggestions_tool_self_scan: test_refactoring_suggestions_tool_self_scan().
---
# Module: [`tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py)

## Classes
### `TestAntiPatternCommentSuppression`
- def: [`tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py:99`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py#L99)
- doc: AP001 (mutable default) etc. must NOT fire on `#`-comment lines.
- signature: `class TestAntiPatternCommentSuppression:`
- members:
  - `test_bare_except_in_comment_is_ignored(self, tmp_path: Path)` — [`L125`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py#L125) — AP002 ``bare_except`` must skip ``#``-comment lines too.
  - `test_mutable_default_in_comment_is_ignored(self, tmp_path: Path)` — [`L102`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py#L102) — A comment that mentions ``def f(x=[])`` is documentation, not code.
  - `test_real_mutable_default_still_detected(self, tmp_path: Path)` — [`L116`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py#L116) — Sanity — the comment skip must not blind the detector to real bugs.
- uses (calls/refs, reference-scoped): [`detect_anti_patterns`](../../../../tree_sitter_analyzer/mcp/tools/utils/anti_patterns.md#detect_anti_patterns)  (1 test-only)

### `TestSecurityScannerDocstringSuppression`
- def: [`tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py:46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py#L46)
- doc: `eval_usage` etc. must NOT fire inside multi-line docstrings.
- signature: `class TestSecurityScannerDocstringSuppression:`
- members:
  - `test_bare_except_inside_docstring_is_ignored(self)` — [`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py#L81) — ``bare_except`` is also in the safe-issues set.
  - `test_eval_inside_triple_quoted_docstring_is_ignored(self)` — [`L49`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py#L49)
  - `test_real_eval_call_still_detected(self)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py#L68) — Sanity — the suppression must not blind the scanner to real evals.
- uses (calls/refs, reference-scoped): [`detect_security_issues`](../../../../tree_sitter_analyzer/mcp/tools/security_scanner.md#detect_security_issues)  (1 test-only)

## Functions
- `_ids(findings: list[dict[str, object]])` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py#L35) — Extract finding identifiers (``issue`` for security, ``id`` for AP).
- `test_refactoring_suggestions_tool_self_scan(smell_id_in_target_file: str)` — [`L151`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_r37as_docstring_comment_suppression.py#L151) — End-to-end: scan refactoring_suggestions_tool.py — both false

