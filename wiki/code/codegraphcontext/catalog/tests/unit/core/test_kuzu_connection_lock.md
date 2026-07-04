---
title: 'Module: tests/unit/core/test_kuzu_connection_lock.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_kuzu_connection_lock.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.core.test_kuzu_connection_lock`/
symbols:
  _make_session: _make_session().
  TestConcurrentAccessSerialization.test_concurrent_write_calls_are_serialised: TestConcurrentAccessSerialization#test_concurrent_write_calls_are_serialised().
  TestLockHeldDuringExecute.test_lock_acquired_before_write_execute: TestLockHeldDuringExecute#test_lock_acquired_before_write_execute().
  TestLockHeldDuringExecute.test_lock_acquired_during_read_execute: TestLockHeldDuringExecute#test_lock_acquired_during_read_execute().
  TestRLockReentrance.test_recursive_run_does_not_deadlock: TestRLockReentrance#test_recursive_run_does_not_deadlock().
  TestLockHeldDuringExecute.test_lock_released_after_write_execute: TestLockHeldDuringExecute#test_lock_released_after_write_execute().
  TestLockHeldDuringExecute.test_lock_released_after_write_exception: TestLockHeldDuringExecute#test_lock_released_after_write_exception().
  TestAlreadyExistsLogging.test_already_exists_returns_empty_result: TestAlreadyExistsLogging#test_already_exists_returns_empty_result().
  TestAlreadyExistsLogging.test_already_exists_calls_debug_log: TestAlreadyExistsLogging#test_already_exists_calls_debug_log().
  TestAlreadyExistsLogging.test_other_errors_still_propagate: TestAlreadyExistsLogging#test_other_errors_still_propagate().
  TestLockHeldDuringExecute.fake_execute: TestLockHeldDuringExecute#fake_execute().
  TestConcurrentAccessSerialization.worker: TestConcurrentAccessSerialization#worker().
  TestConcurrentAccessSerialization.fake_execute: TestConcurrentAccessSerialization#fake_execute().
  TestRLockReentrance.fake_execute: TestRLockReentrance#fake_execute().
  TestLockPlumbing: TestLockPlumbing#
  TestLockPlumbing.test_driver_wrapper_accepts_write_lock_compat: TestLockPlumbing#test_driver_wrapper_accepts_write_lock_compat().
  TestLockPlumbing.test_driver_wrapper_accepts_pool_and_lock: TestLockPlumbing#test_driver_wrapper_accepts_pool_and_lock().
  TestLockHeldDuringExecute: TestLockHeldDuringExecute#
  TestPoolReturnOnExit: TestPoolReturnOnExit#
  TestPoolReturnOnExit.test_session_wrapper_returns_connection_to_pool: TestPoolReturnOnExit#test_session_wrapper_returns_connection_to_pool().
  TestConcurrentAccessSerialization: TestConcurrentAccessSerialization#
  TestRLockReentrance: TestRLockReentrance#
  TestAlreadyExistsLogging: TestAlreadyExistsLogging#
---
# Module: [`tests/unit/core/test_kuzu_connection_lock.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py)

## Classes
### `TestAlreadyExistsLogging`
- def: [`tests/unit/core/test_kuzu_connection_lock.py:251`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L251)
- signature: `class TestAlreadyExistsLogging:`
- members:
  - `test_already_exists_calls_debug_log(self)` — [`L261`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L261) — 'already exists' errors must emit a debug_log message, not be silently dropped.
  - `test_already_exists_returns_empty_result(self)` — [`L252`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L252) — 'already exists' errors must still return an empty KuzuResultWrapper.
  - `test_other_errors_still_propagate(self)` — [`L273`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L273) — Errors that are not 'already exists' must still raise.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestConcurrentAccessSerialization`
- def: [`tests/unit/core/test_kuzu_connection_lock.py:162`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L162)
- signature: `class TestConcurrentAccessSerialization:`
- members:
  - `fake_execute(query, params)` — [`L174`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L174)
  - `test_concurrent_write_calls_are_serialised(self)` — [`L163`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L163) — Two threads calling session.run() with a write query must never execute
  - `worker()` — [`L189`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L189)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestLockHeldDuringExecute`
- def: [`tests/unit/core/test_kuzu_connection_lock.py:76`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L76)
- signature: `class TestLockHeldDuringExecute:`
- members:
  - `fake_execute(query, params)` — [`L83`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L83)
  - `test_lock_acquired_before_write_execute(self)` — [`L77`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L77) — conn.execute() must only be called while the _write_lock is held for writes.
  - `test_lock_acquired_during_read_execute(self)` — [`L95`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L95) — conn.execute() must hold _write_lock for reads too — kuzu.Connection is not thread-safe.
  - `test_lock_released_after_write_exception(self)` — [`L124`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L124) — The _write_lock must be released even when write execution raises an exception.
  - `test_lock_released_after_write_execute(self)` — [`L113`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L113) — The _write_lock must be released after run() on a write query returns normally.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestLockPlumbing`
- def: [`tests/unit/core/test_kuzu_connection_lock.py:44`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L44)
- signature: `class TestLockPlumbing:`
- members:
  - `test_driver_wrapper_accepts_pool_and_lock(self)` — [`L54`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L54) — KuzuDriverWrapper must store pool and write_lock and forward them to sessions.
  - `test_driver_wrapper_accepts_write_lock_compat(self)` — [`L45`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L45) — KuzuDriverWrapper must accept a single lock for backward compatibility.

### `TestPoolReturnOnExit`
- def: [`tests/unit/core/test_kuzu_connection_lock.py:141`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L141)
- signature: `class TestPoolReturnOnExit:`
- members:
  - `test_session_wrapper_returns_connection_to_pool(self)` — [`L142`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L142) — KuzuSessionWrapper must return the connection to the pool on __exit__.

### `TestRLockReentrance`
- def: [`tests/unit/core/test_kuzu_connection_lock.py:218`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L218)
- signature: `class TestRLockReentrance:`
- members:
  - `fake_execute(query, params)` — [`L229`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L229)
  - `test_recursive_run_does_not_deadlock(self)` — [`L219`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L219) — The UNWIND fallback calls self.run() recursively from the same thread.
- uses (calls/refs, reference-scoped): (1 test-only callers)

## Functions
- `_make_session(conn=None, lock=None)` — [`L30`](../../../../../../../raw/code/codegraphcontext/tests/unit/core/test_kuzu_connection_lock.py#L30) — Return a KuzuSessionWrapper with a fresh Lock/RLock and optional mock conn.

