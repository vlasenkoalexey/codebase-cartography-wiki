---
title: 'Module: tree_sitter_analyzer/mcp/subscription_registry.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/subscription_registry.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.subscription_registry`/
symbols:
  SubscriptionRegistry.subscribe: SubscriptionRegistry#subscribe().
  SubscriptionRegistry.compute_delta: SubscriptionRegistry#compute_delta().
  SubscriptionRegistry: SubscriptionRegistry#
  SubscriptionRegistry._subs: SubscriptionRegistry#_subs.
  _hashable: _hashable().
  SubscriptionRegistry.remove_session: SubscriptionRegistry#remove_session().
  SubscriptionRegistry.subscriptions_for: SubscriptionRegistry#subscriptions_for().
  SubscriptionRegistry._lock: SubscriptionRegistry#_lock.
  SubscriptionRegistry.unsubscribe: SubscriptionRegistry#unsubscribe().
  SubscriptionRegistry.notify_all: SubscriptionRegistry#notify_all().
  SubscriptionRegistry.notify_change: SubscriptionRegistry#notify_change().
  SubscriptionRegistry.subscription_count: SubscriptionRegistry#subscription_count().
  SubscriptionRegistry.all_sessions: SubscriptionRegistry#all_sessions().
  SubscriptionRegistry.gc_empty_sessions: SubscriptionRegistry#gc_empty_sessions().
  _Subscription.last_snapshot: _Subscription#last_snapshot.
  SubscriptionRegistry.register_weakref_cleanup: SubscriptionRegistry#register_weakref_cleanup().
  _Subscription: _Subscription#
  _Subscription.last_sent_at: _Subscription#last_sent_at.
  SubscriptionRegistry._on_delta: SubscriptionRegistry#_on_delta.
  _Subscription.session_id: _Subscription#session_id.
  _Subscription.selector: _Subscription#selector.
  SubscriptionRegistry._min_interval_s: SubscriptionRegistry#_min_interval_s.
  SubscriptionRegistry.__init__: SubscriptionRegistry#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/subscription_registry.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py)

## Classes
### `SubscriptionRegistry`
- def: [`tree_sitter_analyzer/mcp/subscription_registry.py:34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L34)
- doc: Thread-safe registry mapping sessions to Hyphae selector subscriptions.
- signature: `class SubscriptionRegistry:`
- members:
  - `__init__(self, *, min_interval_s: float = 2, on_delta: Callable[[str, str, list[Any], list[Any]], None] | None = None)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L49) — Parameters
  - `all_sessions(self)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L99) — Return all sessions that have at least one active subscription.
  - `compute_delta(self, session_id: str, selector: str, new_snapshot: list[Any])` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L113) — Compare *new_snapshot* with the stored last snapshot.
  - `gc_empty_sessions(self)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L187) — Remove sessions with no remaining subscriptions.  Returns count removed.
  - `notify_all(self, evaluate: Callable[[str, str], list[Any]])` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L162) — Re-evaluate every active (session, selector) pair.
  - `notify_change(self, session_id: str, selector: str, new_snapshot: list[Any])` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L151) — Compute delta and, if non-empty, fire ``on_delta`` callback.
  - `register_weakref_cleanup(self, session_obj: Any, session_id: str)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L195) — Remove *session_id* automatically when *session_obj* is garbage-collected.
  - `remove_session(self, session_id: str)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L89) — Remove all subscriptions for a dead/disconnected session.
  - `subscribe(self, session_id: str, selector: str)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L73) — Register *session_id* as watching *selector*.  Idempotent.
  - `subscription_count(self)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L104) — Total number of (session, selector) pairs currently tracked.
  - `subscriptions_for(self, session_id: str)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L94) — Return the list of active selectors for *session_id*.
  - `unsubscribe(self, session_id: str, selector: str)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L84) — Remove *selector* from *session_id*.  No-op if absent.
- protocol/private: `_lock`[`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L64), `_min_interval_s`[`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L66), `_on_delta`[`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L67), `_subs`[`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L65)
- uses (calls/refs, reference-scoped): [`_hashable`](subscription_registry.md#_hashable), [`last_snapshot`](subscription_registry.md#_Subscription.last_snapshot), [`_Subscription`](subscription_registry.md#_Subscription), [`last_sent_at`](subscription_registry.md#_Subscription.last_sent_at), [`selector`](subscription_registry.md#_Subscription.selector), [`session_id`](subscription_registry.md#_Subscription.session_id)
- used by: [`execute`](tools/hyphae_subscribe_tool.md#HyphaeSubscribeTool.execute), [`execute`](tools/hyphae_subscribe_tool.md#HyphaeUnsubscribeTool.execute), [`_push`](watch_push_bridge.md#_drive_subscriptions._push), [`get_subscription_registry`](../_singleton_registry.md#get_subscription_registry), [`_registry`](../_singleton_registry.md#_registry._registry)  (18 test-only)

### `_Subscription`
- def: [`tree_sitter_analyzer/mcp/subscription_registry.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L25)
- doc: One active subscription: session → selector → last snapshot.
- signature: `class _Subscription:`
- members:
  - `last_sent_at` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L31)
  - `last_snapshot` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L30)
  - `selector` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L29)
  - `session_id` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L28)
- used by: [`subscribe`](subscription_registry.md#SubscriptionRegistry.subscribe), [`compute_delta`](subscription_registry.md#SubscriptionRegistry.compute_delta), [`_subs`](subscription_registry.md#SubscriptionRegistry._subs)

## Functions
- `_hashable(item: Any)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/subscription_registry.py#L205) — Convert a snapshot item to a hashable representation for set operations.

