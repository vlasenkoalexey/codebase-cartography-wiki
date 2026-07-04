---
title: 'Module: src/bin/command-supervision.ts'
type: catalog
provenance: extracted
module: src/bin/command-supervision.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/bin/`command-supervision.ts`/
symbols:
  installCommandSupervision: installCommandSupervision().
  CommandSupervision.stop: CommandSupervision#stop().
  CommandSupervision: CommandSupervision#
---
# Module: [`src/bin/command-supervision.ts`](../../../../../../raw/code/codegraph/src/bin/command-supervision.ts)

## Classes
### `CommandSupervision`
- def: [`src/bin/command-supervision.ts:36`](../../../../../../raw/code/codegraph/src/bin/command-supervision.ts#L36)
- signature: `interface CommandSupervision`
- members:
  - `stop(method)` — [`L38`](../../../../../../raw/code/codegraph/src/bin/command-supervision.ts#L38) — Tear down both watchdogs. Idempotent; call when the command finishes.
- used by: [`main`](codegraph.ts.md#main), [`installCommandSupervision`](command-supervision.ts.md#installCommandSupervision)

## Functions
- `installCommandSupervision(label: string)` — [`L47`](../../../../../../raw/code/codegraph/src/bin/command-supervision.ts#L47) — Install the liveness + PPID watchdogs for the duration of a CLI command.

