---
title: 'Module: tests/unit/mcp/test_toon_compact_only.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_toon_compact_only.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_toon_compact_only`/
symbols:
  _capture_call_tool_handler: _capture_call_tool_handler().
  test_execute_compact_only_on_syntax_error_path_file_health: test_execute_compact_only_on_syntax_error_path_file_health().
  test_execute_compact_only_on_syntax_error_path_safe_to_edit: test_execute_compact_only_on_syntax_error_path_safe_to_edit().
  TestReduceToControlSurface.test_keeps_only_control_surface_on_toon: TestReduceToControlSurface#test_keeps_only_control_surface_on_toon().
  TestApplyToonCompactOnly.test_compact_only_drops_duplicated_metadata: TestApplyToonCompactOnly#test_compact_only_drops_duplicated_metadata().
  test_boundary_compact_only_survives_canonical_envelope: test_boundary_compact_only_survives_canonical_envelope().
  test_boundary_compact_only_second_tool: test_boundary_compact_only_second_tool().
  test_boundary_compact_only_error_envelope_keeps_hint: test_boundary_compact_only_error_envelope_keeps_hint().
  test_boundary_compact_only_legacy_keeps_deprecation: test_boundary_compact_only_legacy_keeps_deprecation().
  test_boundary_reduction_is_idempotent: test_boundary_reduction_is_idempotent().
  _METADATA_HEAVY: _METADATA_HEAVY.
  TestReduceToControlSurface.test_idempotent: TestReduceToControlSurface#test_idempotent().
  TestApplyToonCompactOnly.test_default_is_unchanged_byte_parity: TestApplyToonCompactOnly#test_default_is_unchanged_byte_parity().
  TestApplyToonCompactOnly.test_compact_only_is_noop_for_json: TestApplyToonCompactOnly#test_compact_only_is_noop_for_json().
  test_boundary_default_unaffected: test_boundary_default_unaffected().
  _capture_call_tool_handler.capture_decorator: _capture_call_tool_handler().capture_decorator().
  TestReduceToControlSurface.test_noop_on_non_toon: TestReduceToControlSurface#test_noop_on_non_toon().
  _BROKEN_PY: _BROKEN_PY.
  _capture_call_tool_handler.capture_decorator.decorator: _capture_call_tool_handler().capture_decorator().decorator().
  TestReduceToControlSurface: TestReduceToControlSurface#
  TestApplyToonCompactOnly: TestApplyToonCompactOnly#
---
# Module: [`tests/unit/mcp/test_toon_compact_only.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py)

## Classes
### `TestApplyToonCompactOnly`
- def: [`tests/unit/mcp/test_toon_compact_only.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L67)
- signature: `class TestApplyToonCompactOnly:`
- members:
  - `test_compact_only_drops_duplicated_metadata(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L83)
  - `test_compact_only_is_noop_for_json(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L93)
  - `test_default_is_unchanged_byte_parity(self)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L68)
- uses (calls/refs, reference-scoped): [`apply_toon_format_to_response`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#apply_toon_format_to_response), [`TOON_CONTROL_SURFACE`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#TOON_CONTROL_SURFACE.TOON_CONTROL_SURFACE)  (1 test-only)

### `TestReduceToControlSurface`
- def: [`tests/unit/mcp/test_toon_compact_only.py:44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L44)
- signature: `class TestReduceToControlSurface:`
- members:
  - `test_idempotent(self)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L61)
  - `test_keeps_only_control_surface_on_toon(self)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L45)
  - `test_noop_on_non_toon(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L57)
- uses (calls/refs, reference-scoped): [`TOON_CONTROL_SURFACE`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#TOON_CONTROL_SURFACE.TOON_CONTROL_SURFACE), [`reduce_to_control_surface`](../../../tree_sitter_analyzer/mcp/utils/format_helper.md#reduce_to_control_surface)  (1 test-only)

## Functions
- `_capture_call_tool_handler(server: TreeSitterAnalyzerMCPServer)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L107)
- `capture_decorator(name)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L113)
- `decorator(func)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L114)
- `test_boundary_compact_only_error_envelope_keeps_hint(tmp_path)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L204) — An ERROR response under compact_only must still carry the recovery
- `test_boundary_compact_only_legacy_keeps_deprecation(tmp_path)` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L227) — Codex P2 #393: a LEGACY tool name (e.g. check_file_health) routed through
- `test_boundary_compact_only_second_tool(tmp_path)` — [`L184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L184) — The boundary reduction is generic — exercise a second decision tool
- `test_boundary_compact_only_survives_canonical_envelope(tmp_path)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L131) — Through the FULL handle_call_tool boundary: a file_health call with
- `test_boundary_default_unaffected(tmp_path)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L166) — Without compact_only the boundary leaves the response shape as-is.
- `test_boundary_reduction_is_idempotent(tmp_path)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L254) — Reducing an already-compact response at the boundary is a no-op — guards
- `test_execute_compact_only_on_syntax_error_path_file_health(tmp_path)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L279) — file_health's syntax-error early return must honor compact_only too.
- `test_execute_compact_only_on_syntax_error_path_safe_to_edit(tmp_path)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L293) — safe_to_edit's syntax-error early return must honor compact_only too.

## Module values
- `_BROKEN_PY` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L276)
- `_METADATA_HEAVY` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_compact_only.py#L32)

