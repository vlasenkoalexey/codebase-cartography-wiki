---
title: 'Module: tests/unit/mcp/test_watch_push_bridge.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_watch_push_bridge.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_watch_push_bridge`/
symbols:
  _seed: _seed().
  test_only_the_moved_selector_among_many_is_pushed: test_only_the_moved_selector_among_many_is_pushed().
  test_unchanged_selector_is_not_pushed: test_unchanged_selector_is_not_pushed().
  test_changed_selector_is_pushed: test_changed_selector_is_pushed().
  test_only_the_moved_selector_among_many_is_pushed.evaluate: test_only_the_moved_selector_among_many_is_pushed().evaluate().
---
# Module: [`tests/unit/mcp/test_watch_push_bridge.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_watch_push_bridge.py)

## Functions
- `_seed(registry: SubscriptionRegistry, session: str, selector: str, snap: list)` — [`L9`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_watch_push_bridge.py#L9) — Subscribe and prime the stored snapshot so later diffs are meaningful.
- `evaluate(_sid: str, selector: str)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_watch_push_bridge.py#L48)
- `test_changed_selector_is_pushed()` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_watch_push_bridge.py#L27) — When the selector result moves, exactly that pair is returned.
- `test_only_the_moved_selector_among_many_is_pushed()` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_watch_push_bridge.py#L40) — An unrelated subscription is not woken when another selector changes.
- `test_unchanged_selector_is_not_pushed()` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_watch_push_bridge.py#L16) — A sync event that does not move the result pushes nothing.

