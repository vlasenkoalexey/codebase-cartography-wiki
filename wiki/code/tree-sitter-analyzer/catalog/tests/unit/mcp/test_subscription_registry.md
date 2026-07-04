---
title: 'Module: tests/unit/mcp/test_subscription_registry.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_subscription_registry.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_subscription_registry`/Test
symbols:
  TestSubscribeUnsubscribe.test_remove_session_clears_all: SubscribeUnsubscribe#test_remove_session_clears_all().
  TestGC.test_gc_removes_empty_sessions: GC#test_gc_removes_empty_sessions().
  TestSubscribeUnsubscribe.test_unsubscribe_removes_selector: SubscribeUnsubscribe#test_unsubscribe_removes_selector().
  TestSubscribeUnsubscribe.test_multiple_sessions_independent: SubscribeUnsubscribe#test_multiple_sessions_independent().
  TestNotifyAll.test_on_delta_callback_fires: NotifyAll#test_on_delta_callback_fires().
  TestNotifyAll.test_notify_all_evaluates_all_subscriptions: NotifyAll#test_notify_all_evaluates_all_subscriptions().
  TestSubscribeUnsubscribe.test_subscribe_adds_selector: SubscribeUnsubscribe#test_subscribe_adds_selector().
  TestSubscribeUnsubscribe.test_subscribe_is_idempotent: SubscribeUnsubscribe#test_subscribe_is_idempotent().
  TestDeltaComputation.test_empty_to_items_produces_added: DeltaComputation#test_empty_to_items_produces_added().
  TestDeltaComputation.test_items_to_empty_produces_removed: DeltaComputation#test_items_to_empty_produces_removed().
  TestDeltaComputation.test_unchanged_snapshot_produces_no_delta: DeltaComputation#test_unchanged_snapshot_produces_no_delta().
  TestDeltaComputation.test_throttle_suppresses_rapid_calls: DeltaComputation#test_throttle_suppresses_rapid_calls().
  TestSubscribeUnsubscribe.test_unsubscribe_noop_if_absent: SubscribeUnsubscribe#test_unsubscribe_noop_if_absent().
  TestDeltaComputation.test_unknown_session_returns_empty: DeltaComputation#test_unknown_session_returns_empty().
  TestHashable.test_dict_is_hashable: Hashable#test_dict_is_hashable().
  TestHashable.test_nested_dict_is_hashable: Hashable#test_nested_dict_is_hashable().
  TestNotifyAll.cb: NotifyAll#cb().
  TestNotifyAll.evaluate: NotifyAll#evaluate().
  TestSubscribeUnsubscribe: SubscribeUnsubscribe#
  TestDeltaComputation: DeltaComputation#
  TestNotifyAll: NotifyAll#
  TestGC: GC#
  TestHashable: Hashable#
---
# Module: [`tests/unit/mcp/test_subscription_registry.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py)

## Classes
### `TestDeltaComputation`
- def: [`tests/unit/mcp/test_subscription_registry.py:50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L50)
- signature: `class TestDeltaComputation:`
- members:
  - `test_empty_to_items_produces_added(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L51)
  - `test_items_to_empty_produces_removed(self)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L58)
  - `test_throttle_suppresses_rapid_calls(self)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L79)
  - `test_unchanged_snapshot_produces_no_delta(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L66)
  - `test_unknown_session_returns_empty(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L74)
- uses (calls/refs, reference-scoped): [`subscribe`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.subscribe), [`compute_delta`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.compute_delta), [`SubscriptionRegistry`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry)

### `TestGC`
- def: [`tests/unit/mcp/test_subscription_registry.py:119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L119)
- signature: `class TestGC:`
- members:
  - `test_gc_removes_empty_sessions(self)` — [`L120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L120)
- uses (calls/refs, reference-scoped): [`subscribe`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.subscribe), [`SubscriptionRegistry`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry), [`unsubscribe`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.unsubscribe), [`all_sessions`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.all_sessions), [`gc_empty_sessions`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.gc_empty_sessions)

### `TestHashable`
- def: [`tests/unit/mcp/test_subscription_registry.py:129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L129)
- signature: `class TestHashable:`
- members:
  - `test_dict_is_hashable(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L130)
  - `test_nested_dict_is_hashable(self)` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L134)
- uses (calls/refs, reference-scoped): [`_hashable`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#_hashable)

### `TestNotifyAll`
- def: [`tests/unit/mcp/test_subscription_registry.py:88`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L88)
- signature: `class TestNotifyAll:`
- members:
  - `cb(session_id: str, selector: str, added: list, removed: list)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L92)
  - `evaluate(session_id: str, selector: str)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L107)
  - `test_notify_all_evaluates_all_subscriptions(self)` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L104)
  - `test_on_delta_callback_fires(self)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L89)
- uses (calls/refs, reference-scoped): [`subscribe`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.subscribe), [`SubscriptionRegistry`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry), [`notify_all`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.notify_all), [`notify_change`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.notify_change)

### `TestSubscribeUnsubscribe`
- def: [`tests/unit/mcp/test_subscription_registry.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L11)
- signature: `class TestSubscribeUnsubscribe:`
- members:
  - `test_multiple_sessions_independent(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L41)
  - `test_remove_session_clears_all(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L33)
  - `test_subscribe_adds_selector(self)` — [`L12`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L12)
  - `test_subscribe_is_idempotent(self)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L17)
  - `test_unsubscribe_noop_if_absent(self)` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L29)
  - `test_unsubscribe_removes_selector(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_subscription_registry.py#L23)
- uses (calls/refs, reference-scoped): [`subscribe`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.subscribe), [`SubscriptionRegistry`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry), [`remove_session`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.remove_session), [`subscriptions_for`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.subscriptions_for), [`unsubscribe`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.unsubscribe), [`subscription_count`](../../../tree_sitter_analyzer/mcp/subscription_registry.md#SubscriptionRegistry.subscription_count)

