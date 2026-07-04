---
title: 'Module: src/sync/watch-policy.ts'
type: catalog
provenance: extracted
module: src/sync/watch-policy.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/sync/`watch-policy.ts`/
symbols:
  watchDisabledReason: watchDisabledReason().
  wslValue: wslValue.
  detectWsl: detectWsl().
  __resetWslCacheForTests: __resetWslCacheForTests().
  isWindowsDriveMount: isWindowsDriveMount().
  wslChecked: wslChecked.
  WatchProbe: WatchProbe#
  WatchProbe.env: WatchProbe#env.
  WatchProbe.isWsl: WatchProbe#isWsl.
---
# Module: [`src/sync/watch-policy.ts`](../../../../../../raw/code/codegraph/src/sync/watch-policy.ts)

## Classes
### `WatchProbe`
- def: [`src/sync/watch-policy.ts:64`](../../../../../../raw/code/codegraph/src/sync/watch-policy.ts#L64)
- doc: Inputs that can be overridden in tests so the decision is deterministic
- signature: `interface WatchProbe`
- members:
  - `env` — [`L66`](../../../../../../raw/code/codegraph/src/sync/watch-policy.ts#L66) — Defaults to `process.env`.
  - `isWsl` — [`L68`](../../../../../../raw/code/codegraph/src/sync/watch-policy.ts#L68) — Defaults to `detectWsl()`.
- used by: [`watchDisabledReason`](watch-policy.ts.md#watchDisabledReason)

## Functions
- `__resetWslCacheForTests()` — [`L101`](../../../../../../raw/code/codegraph/src/sync/watch-policy.ts#L101) — Test-only: reset the cached WSL detection.
- `detectWsl()` — [`L30`](../../../../../../raw/code/codegraph/src/sync/watch-policy.ts#L30) — Detect whether the current process is running under WSL (Windows — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)
- `isWindowsDriveMount(projectRoot: string)` — [`L56`](../../../../../../raw/code/codegraph/src/sync/watch-policy.ts#L56) — True for WSL Windows-drive mounts like `/mnt/c` or `/mnt/d/project`. — documented in [utils.ts](../../../concepts/utils.ts.md)
- `watchDisabledReason(projectRoot: string, probe?: WatchProbe)` — [`L82`](../../../../../../raw/code/codegraph/src/sync/watch-policy.ts#L82) — Decide whether the file watcher should be disabled for a project, and why. — documented in [sync-watcher.ts](../../../concepts/sync-watcher.ts.md)

## Module values
- `wslChecked` — [`L20`](../../../../../../raw/code/codegraph/src/sync/watch-policy.ts#L20)
- `wslValue` — [`L21`](../../../../../../raw/code/codegraph/src/sync/watch-policy.ts#L21)

