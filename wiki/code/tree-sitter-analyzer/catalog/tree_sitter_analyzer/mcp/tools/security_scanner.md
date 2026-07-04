---
title: 'Module: tree_sitter_analyzer/mcp/tools/security_scanner.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/security_scanner.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.security_scanner`/
symbols:
  detect_security_issues: detect_security_issues().
  _PATTERNS_BY_LANG._PATTERNS_BY_LANG: _PATTERNS_BY_LANG._PATTERNS_BY_LANG.
  _SECRET_PATTERNS: _SECRET_PATTERNS.
  _should_ignore_match: _should_ignore_match().
  _line_has_security_match: _line_has_security_match().
  _SQL_INJECTION: _SQL_INJECTION.
  _EVAL_USAGE: _EVAL_USAGE.
  _XSS_PATTERNS: _XSS_PATTERNS.
  _PYTHON_STRING_OR_COMMENT_SAFE_ISSUES: _PYTHON_STRING_OR_COMMENT_SAFE_ISSUES.
  _SHELL_INJECTION: _SHELL_INJECTION.
  _PICKLE_USAGE: _PICKLE_USAGE.
  _ASSERT_IN_PROD: _ASSERT_IN_PROD.
  _EXCEPT_BARE: _EXCEPT_BARE.
  _INSECURE_HASH: _INSECURE_HASH.
  _TLS_DISABLE: _TLS_DISABLE.
  _is_test_path: _is_test_path().
  _python_lines_inside_multiline_strings: _python_lines_inside_multiline_strings().
  _is_python_string_or_comment_position: _is_python_string_or_comment_position().
---
# Module: [`tree_sitter_analyzer/mcp/tools/security_scanner.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py)

## Functions
- `_is_python_string_or_comment_position(line: str, column: int)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L364) — Return True when a column falls inside a Python string/comment token.
- `_is_test_path(file_path: str | None)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L229) — Return True for conventional test file paths.
- `_line_has_security_match(line: str, pattern: re.Pattern[str], issue_name: str, language: str)` — [`L338`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L338) — Return True when a security pattern matches executable source text.
- `_python_lines_inside_multiline_strings(source: str)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L304) — Return the 1-indexed line numbers covered by any multi-line STRING token.
- `_should_ignore_match(line: str, column: int, issue_name: str, language: str)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L352) — Suppress Python false positives inside strings and comments.
- `detect_security_issues(source: str, language: str, file_path: str | None = None)` — [`L243`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L243)

## Module values
- `_ASSERT_IN_PROD` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L67)
- `_EVAL_USAGE` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L54)
- `_EXCEPT_BARE` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L69)
- `_INSECURE_HASH` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L71)
- `_PATTERNS_BY_LANG` — [`L88`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L88)
- `_PICKLE_USAGE` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L65)
- `_PYTHON_STRING_OR_COMMENT_SAFE_ISSUES` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L79)
- `_SECRET_PATTERNS` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L16)
- `_SHELL_INJECTION` — [`L56`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L56)
- `_SQL_INJECTION` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L31)
- `_TLS_DISABLE` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L75)
- `_XSS_PATTERNS` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/security_scanner.py#L61)

