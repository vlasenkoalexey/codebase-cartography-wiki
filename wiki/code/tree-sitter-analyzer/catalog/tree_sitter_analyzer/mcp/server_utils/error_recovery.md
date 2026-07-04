---
title: 'Module: tree_sitter_analyzer/mcp/server_utils/error_recovery.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/server_utils/error_recovery.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.server_utils.error_recovery`/
symbols:
  build_agent_friendly_error: build_agent_friendly_error().
  ensure_canonical_success_envelope: ensure_canonical_success_envelope().
  ensure_canonical_error_envelope: ensure_canonical_error_envelope().
  _populate_summary_line: _populate_summary_line().
  _classify: _classify().
  _normalize_echoed_file_path: _normalize_echoed_file_path().
  _pick_identifier: _pick_identifier().
  _build_envelope: _build_envelope().
  _ensure_language_echo: _ensure_language_echo().
  _verdict_suffix: _verdict_suffix().
  _IDENTIFIER_FIELDS._IDENTIFIER_FIELDS: _IDENTIFIER_FIELDS._IDENTIFIER_FIELDS.
  _summary_line: _summary_line().
  _real_verdict: _real_verdict().
  _ERROR_RECOVERY_HINTS._ERROR_RECOVERY_HINTS: _ERROR_RECOVERY_HINTS._ERROR_RECOVERY_HINTS.
  _normalize_path_string: _normalize_path_string().
  _populate_agent_summary_block: _populate_agent_summary_block().
  _mirror_verdict: _mirror_verdict().
  _EXC_CLASS_TO_TYPE._EXC_CLASS_TO_TYPE: _EXC_CLASS_TO_TYPE._EXC_CLASS_TO_TYPE.
  _FILE_PATH_ECHO_KEYS._FILE_PATH_ECHO_KEYS: _FILE_PATH_ECHO_KEYS._FILE_PATH_ECHO_KEYS.
  _SUCCESS_LIKE_VERDICTS._SUCCESS_LIKE_VERDICTS: _SUCCESS_LIKE_VERDICTS._SUCCESS_LIKE_VERDICTS.
  _CANONICAL_KEYS._CANONICAL_KEYS: _CANONICAL_KEYS._CANONICAL_KEYS.
---
# Module: [`tree_sitter_analyzer/mcp/server_utils/error_recovery.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py)

## Functions
- `_build_envelope(*, tool_name: str, error_msg: str, error_type: str, recovery_hint: str, suggested_tool: str, identifier_key: str | None, identifier_value: str | None, extras: dict[str, Any] | None = None)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L200) — Compose the canonical envelope from already-resolved fields.
- `_classify(error_msg: str, error_type_hint: str | None = None)` — [`L156`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L156) — Pick (error_type, recovery_hint, suggested_tool) for a given message.
- `_ensure_language_echo(response: dict[str, Any], arguments: dict[str, Any] | None)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L318) — Ensure single-file responses echo ``language: <detected>`` (M14).
- `_mirror_verdict(response: dict[str, Any], agent_summary: dict[str, Any])` — [`L513`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L513) — Mirror ``verdict`` between top-level and ``agent_summary`` (M10).
- `_normalize_echoed_file_path(response: dict[str, Any])` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L308) — Normalize echoed ``file_path`` / ``source_file`` in place (K12).
- `_normalize_path_string(raw: str)` — [`L294`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L294) — Strip leading ``./`` and convert separators for K12 echo parity.
- `_pick_identifier(arguments: dict[str, Any] | None)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L182) — Pull the most informative (key, value) identifier from arguments.
- `_populate_agent_summary_block(response: dict[str, Any], summary_line_value: str)` — [`L475`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L475) — Ensure ``agent_summary`` is a dict with mirrored summary_line + next_step.
- `_populate_summary_line(response: dict[str, Any], tool_name: str, arguments: dict[str, Any] | None)` — [`L429`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L429) — Mirror agent_summary.summary_line → top-level, or synthesize when both missing.
- `_real_verdict(value: Any)` — [`L502`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L502) — Return ``value`` only if it is a *real* verdict.
- `_summary_line(tool_name: str, error_type: str, identifier: str | None)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L176)
- `_verdict_suffix(response: dict[str, Any])` — [`L412`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L412) — Pick the no-identifier summary-line suffix from the response verdict.
- `build_agent_friendly_error(tool_name: str, error: Exception, *, arguments: dict[str, Any] | None = None)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L245) — Build the canonical error envelope for an exception raised by a tool.
- `ensure_canonical_error_envelope(tool_name: str, response: dict[str, Any], *, arguments: dict[str, Any] | None = None)` — [`L543`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L543) — Augment a tool's existing ``{success: False, ...}`` dict in place.
- `ensure_canonical_success_envelope(tool_name: str, response: dict[str, Any], *, arguments: dict[str, Any] | None = None)` — [`L367`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L367) — Augment a tool's success-path response with the canonical envelope keys.

## Module values
- `_CANONICAL_KEYS` — [`L277`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L277)
- `_ERROR_RECOVERY_HINTS` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L45)
- `_EXC_CLASS_TO_TYPE` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L138)
- `_FILE_PATH_ECHO_KEYS` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L291)
- `_IDENTIFIER_FIELDS` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L134)
- `_SUCCESS_LIKE_VERDICTS` — [`L409`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/server_utils/error_recovery.py#L409)

