---
title: 'Module: src/mcp/daemon-manager.ts'
type: catalog
provenance: extracted
module: src/mcp/daemon-manager.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/mcp/`daemon-manager.ts`/
symbols:
  runDaemonPicker: runDaemonPicker().
  buildPickItems: buildPickItems().
  PickerDeps.list: PickerDeps#list.
  PickerDeps.stop: PickerDeps#stop.
  PickerDeps.stopAll: PickerDeps#stopAll.
  PickerDeps.select: PickerDeps#select.
  PickerDeps.done: PickerDeps#done.
  CANCEL: CANCEL.
  PickItem: PickItem#
  PickItem.value: PickItem#value.
  PickerDeps.note: PickerDeps#note.
  STOP_ALL: STOP_ALL.
  PickItem.label: PickItem#label.
  PickItem.hint: PickItem#hint.
  PickerDeps.cwdRoot: PickerDeps#cwdRoot.
  PickerDeps.now: PickerDeps#now.
  PickerDeps.isCancel: PickerDeps#isCancel.
  formatUptime: formatUptime().
  PickerDeps: PickerDeps#
---
# Module: [`src/mcp/daemon-manager.ts`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts)

## Classes
### `PickItem`
- def: [`src/mcp/daemon-manager.ts:16`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L16)
- signature: `interface PickItem`
- members:
  - `hint` — [`L19`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L19)
  - `label` — [`L18`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L18)
  - `value` — [`L17`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L17)
- used by: [`runDaemonPicker`](daemon-manager.ts.md#runDaemonPicker), [`buildPickItems`](daemon-manager.ts.md#buildPickItems), [`select`](daemon-manager.ts.md#PickerDeps.select)

### `PickerDeps`
- def: [`src/mcp/daemon-manager.ts:63`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L63)
- signature: `interface PickerDeps`
- members:
  - `cwdRoot` — [`L68`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L68) — Realpath'd root of the current project's daemon, or null.
  - `done` — [`L76`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L76) — Final line + teardown (clack outro).
  - `isCancel` — [`L72`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L72)
  - `list` — [`L64`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L64)
  - `note` — [`L74`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L74) — Per-action note (e.g. "Stopped daemon …").
  - `now` — [`L69`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L69)
  - `select` — [`L71`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L71) — Render the picker; returns the chosen value or a cancel sentinel.
  - `stop` — [`L65`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L65)
  - `stopAll` — [`L66`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L66)
- uses (calls/refs, reference-scoped): [`DaemonRecord`](daemon-registry.ts.md#DaemonRecord), [`StopResult`](daemon-registry.ts.md#StopResult), [`PickItem`](daemon-manager.ts.md#PickItem)
- used by: [`main`](../bin/codegraph.ts.md#main), [`runDaemonPicker`](daemon-manager.ts.md#runDaemonPicker)

## Functions
- `buildPickItems(daemons: DaemonRecord[], cwdRoot: string | null, now: number)` — [`L37`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L37) — Build the ordered, UI-ready option list: the current project's daemon first
- `formatUptime(ms: number)` — [`L23`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L23) — Compact uptime: `45s`, `12m`, `3h 5m`.
- `runDaemonPicker(deps: PickerDeps)` — [`L83`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L83) — Pick a daemon → stop it → re-prompt with what's left, until the user cancels

## Module values
- `CANCEL` — [`L14`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L14)
- `STOP_ALL` — [`L13`](../../../../../../raw/code/codegraph/src/mcp/daemon-manager.ts#L13) — Sentinel option values (not real roots, so they can't collide with a project path).

