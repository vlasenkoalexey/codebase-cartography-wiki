---
title: 'Module: tests/unit/mcp/test_hyphae_push_wiring.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_hyphae_push_wiring.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_hyphae_push_wiring`/test_
symbols:
  test_send_update_calls_session_when_present: send_update_calls_session_when_present().
  test_session_obj_store_roundtrip: session_obj_store_roundtrip().
  test_session_loop_store_roundtrip: session_loop_store_roundtrip().
  test_send_update_no_session_is_noop: send_update_no_session_is_noop().
  test_capture_session_obj_returns_none_outside_request_context: capture_session_obj_returns_none_outside_request_context().
  test_send_update_calls_session_when_present.FakeSession: send_update_calls_session_when_present().FakeSession#
  test_send_update_calls_session_when_present.FakeSession.send_resource_updated: send_update_calls_session_when_present().FakeSession#send_resource_updated().
---
# Module: [`tests/unit/mcp/test_hyphae_push_wiring.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_push_wiring.py)

## Classes
### `FakeSession`
- def: [`tests/unit/mcp/test_hyphae_push_wiring.py:63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_push_wiring.py#L63)
- signature: `class FakeSession:`
- members:
  - `send_resource_updated(self, uri: object)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_push_wiring.py#L64)
- used by: (1 test-only callers)

## Functions
- `test_capture_session_obj_returns_none_outside_request_context()` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_push_wiring.py#L18) — Outside an MCP request, request_ctx is unset → capture returns None,
- `test_send_update_calls_session_when_present()` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_push_wiring.py#L58) — When a session is captured, _send_update awaits send_resource_updated
- `test_send_update_no_session_is_noop()` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_push_wiring.py#L48) — _send_update returns quietly when no session was captured for the id —
- `test_session_loop_store_roundtrip()` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_push_wiring.py#L35) — get_session_loop mirrors the captured loop; None when absent.
- `test_session_obj_store_roundtrip()` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_push_wiring.py#L24) — get_session_obj returns what was captured, and None for unknown ids.

