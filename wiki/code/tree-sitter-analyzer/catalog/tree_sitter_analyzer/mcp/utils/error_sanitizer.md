---
title: 'Module: tree_sitter_analyzer/mcp/utils/error_sanitizer.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/error_sanitizer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.error_sanitizer`/
symbols:
  safe_error_message: safe_error_message().
  sanitize_message: sanitize_message().
  sanitize_exception: sanitize_exception().
  sanitize_message._replace: sanitize_message()._replace().
  project_root_from_env: project_root_from_env().
  _ABSOLUTE_PATH_RE: _ABSOLUTE_PATH_RE.
  _sanitize_path_token: _sanitize_path_token().
---
# Module: [`tree_sitter_analyzer/mcp/utils/error_sanitizer.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_sanitizer.py)

## Functions
- `_replace(match: re.Match[str])` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_sanitizer.py#L81)
- `_sanitize_path_token(token: str, project_root: str | None)` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_sanitizer.py#L53) — Convert one absolute-path token to a relative or redacted form.
- `project_root_from_env()` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_sanitizer.py#L123) — Best-effort fallback when a caller doesn't pass project_root.
- `safe_error_message(exc: BaseException, project_root: str | None = None, *, include_class: bool = True)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_sanitizer.py#L107) — Convenience wrapper used inside MCP tool error returns.
- `sanitize_exception(exc: BaseException, project_root: str | None = None)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_sanitizer.py#L87) — Build a sanitised error string from an exception.
- `sanitize_message(text: str, project_root: str | None = None)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_sanitizer.py#L72) — Replace absolute-path tokens in ``text`` with relative/redacted forms.

## Module values
- `_ABSOLUTE_PATH_RE` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/error_sanitizer.py#L36)

