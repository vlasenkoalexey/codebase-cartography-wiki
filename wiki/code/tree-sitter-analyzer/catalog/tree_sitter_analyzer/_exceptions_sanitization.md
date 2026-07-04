---
title: 'Module: tree_sitter_analyzer/_exceptions_sanitization.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_exceptions_sanitization.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._exceptions_sanitization`/_
symbols:
  _sanitize_error_context: sanitize_error_context().
  _sanitize_context_value: sanitize_context_value().
  _sanitize_params: sanitize_params().
  _is_sensitive_key: is_sensitive_key().
  _sanitize_param_value: sanitize_param_value().
  _sanitize_parameter_value: sanitize_parameter_value().
  _SENSITIVE_KEYS: SENSITIVE_KEYS.
---
# Module: [`tree_sitter_analyzer/_exceptions_sanitization.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_sanitization.py)

## Functions
- `_is_sensitive_key(key: str)` — [`L62`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_sanitization.py#L62)
- `_sanitize_context_value(key: str, value: Any)` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_sanitization.py#L48) — Sanitize a single key-value pair for logging.
- `_sanitize_error_context(context: dict[str, Any])` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_sanitization.py#L35) — Sanitize sensitive information from error context.
- `_sanitize_param_value(key: str, value: Any)` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_sanitization.py#L40)
- `_sanitize_parameter_value(parameter_value: Any)` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_sanitization.py#L29)
- `_sanitize_params(params: dict[str, Any])` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_sanitization.py#L21) — Sanitize sensitive information from parameters.

## Module values
- `_SENSITIVE_KEYS` — [`L5`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_sanitization.py#L5)

