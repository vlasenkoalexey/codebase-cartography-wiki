---
title: 'Module: tests/unit/mcp/test_hyphae_resource_read.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_hyphae_resource_read.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_hyphae_resource_read`/
symbols:
  TestHyphaeResourceReadBoundary.test_unsubscribe_cleanup_does_not_affect_resource_read: TestHyphaeResourceReadBoundary#test_unsubscribe_cleanup_does_not_affect_resource_read().
  _capture_decorator: _capture_decorator().
  TestHyphaeResourceReadBoundary.test_returns_list_of_read_resource_contents: TestHyphaeResourceReadBoundary#test_returns_list_of_read_resource_contents().
  TestHyphaeResourceReadBoundary.test_read_resource_contents_survive_sdk_iteration: TestHyphaeResourceReadBoundary#test_read_resource_contents_survive_sdk_iteration().
  TestDegenerateHyphaeURI.test_empty_selector_uri_returns_wrapped_contents: TestDegenerateHyphaeURI#test_empty_selector_uri_returns_wrapped_contents().
  _make_instance: _make_instance().
  _capture_decorator.decorator: _capture_decorator().decorator().
  _capture_decorator.decorator.wrapper: _capture_decorator().decorator().wrapper().
  TestHyphaeResourceReadBoundary: TestHyphaeResourceReadBoundary#
  TestDegenerateHyphaeURI: TestDegenerateHyphaeURI#
---
# Module: [`tests/unit/mcp/test_hyphae_resource_read.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py)

## Classes
### `TestDegenerateHyphaeURI`
- def: [`tests/unit/mcp/test_hyphae_resource_read.py:198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py#L198)
- doc: P3 (review): tsa://hyphae/ with an empty selector must not crash.
- signature: `class TestDegenerateHyphaeURI:`
- members:
  - `test_empty_selector_uri_returns_wrapped_contents(self, tmp_path)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py#L202)
- uses (calls/refs, reference-scoped): [`register_resources`](../../../tree_sitter_analyzer/mcp/server_utils/resource_registration.md#register_resources)  (2 test-only)

### `TestHyphaeResourceReadBoundary`
- def: [`tests/unit/mcp/test_hyphae_resource_read.py:67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py#L67)
- doc: handle_read_resource must return ReadResourceContents, not a raw dict.
- signature: `class TestHyphaeResourceReadBoundary:`
- members:
  - `test_read_resource_contents_survive_sdk_iteration(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py#L127) — Each item in the result must have .content and .mime_type attributes.
  - `test_returns_list_of_read_resource_contents(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py#L71) — Issue #454: tsa://hyphae/ URIs must not return a raw dict.
  - `test_unsubscribe_cleanup_does_not_affect_resource_read(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py#L161) — Unsubscribe path: removing session state must not break resource reads.
- uses (calls/refs, reference-scoped): [`register_resources`](../../../tree_sitter_analyzer/mcp/server_utils/resource_registration.md#register_resources), [`_SESSION_SESSIONS`](../../../tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.md#_SESSION_SESSIONS._SESSION_SESSIONS), [`_SESSION_LOOPS`](../../../tree_sitter_analyzer/mcp/tools/hyphae_subscribe_tool.md#_SESSION_LOOPS._SESSION_LOOPS)  (2 test-only)

## Functions
- `_capture_decorator(handlers, attr_name)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py#L32)
- `_make_instance(project_root: str = "/tmp/proj")` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py#L43)
- `decorator()` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py#L33)
- `wrapper(func)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_hyphae_resource_read.py#L34)

