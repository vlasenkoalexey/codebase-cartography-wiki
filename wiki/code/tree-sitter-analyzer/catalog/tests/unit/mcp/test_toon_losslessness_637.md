---
title: 'Module: tests/unit/mcp/test_toon_losslessness_637.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_toon_losslessness_637.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_toon_losslessness_637`/
symbols:
  TestToonLosslessnessInvariant.test_heterogeneous_rows_lossless_through_boundary: TestToonLosslessnessInvariant#test_heterogeneous_rows_lossless_through_boundary().
  _capture_call_tool_handler: _capture_call_tool_handler().
  _call: _call().
  _iter_row_dicts: _iter_row_dicts().
  _capture_call_tool_handler.capture_decorator: _capture_call_tool_handler().capture_decorator().
  _fake_inline_neighbor_bodies: _fake_inline_neighbor_bodies().
  _capture_call_tool_handler.capture_decorator.decorator: _capture_call_tool_handler().capture_decorator().decorator().
  _CALLERS: _CALLERS.
  _BODIES: _BODIES.
  TestToonLosslessnessInvariant: TestToonLosslessnessInvariant#
---
# Module: [`tests/unit/mcp/test_toon_losslessness_637.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py)

## Classes
### `TestToonLosslessnessInvariant`
- def: [`tests/unit/mcp/test_toon_losslessness_637.py:122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py#L122)
- doc: Structural ⊇ invariant: TOON output covers the JSON payload.
- signature: `class TestToonLosslessnessInvariant:`
- members:
  - `test_heterogeneous_rows_lossless_through_boundary(self, tmp_path)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py#L126)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)  (3 test-only)

## Functions
- `_call(handler, output_format: str)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py#L92)
- `_capture_call_tool_handler(server: TreeSitterAnalyzerMCPServer)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py#L27) — Capture the ``handle_call_tool`` closure registered by ``create_server``.
- `_fake_inline_neighbor_bodies(project_root: str, cache: Any, neighbors: list[dict[str, Any]])` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py#L65) — Deterministic stand-in for symbol_body_inline.inline_neighbor_bodies:
- `_iter_row_dicts(node: Any)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py#L80) — Yield every dict that appears inside any list, at any depth.
- `capture_decorator(name)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py#L37)
- `decorator(func)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py#L38)

## Module values
- `_BODIES` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py#L57)
- `_CALLERS` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_toon_losslessness_637.py#L50)

