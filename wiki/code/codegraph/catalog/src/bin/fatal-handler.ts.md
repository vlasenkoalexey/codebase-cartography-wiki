---
title: 'Module: src/bin/fatal-handler.ts'
type: catalog
provenance: extracted
module: src/bin/fatal-handler.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/bin/`fatal-handler.ts`/
symbols:
  installFatalHandlers: installFatalHandlers().
  describeFatal: describeFatal().
  writeStderr: writeStderr().
  FatalHandlerDeps: FatalHandlerDeps#
  FatalHandlerDeps.target: FatalHandlerDeps#target.
  FatalHandlerDeps.exit: FatalHandlerDeps#exit.
  FatalHandlerDeps.write: FatalHandlerDeps#write.
---
# Module: [`src/bin/fatal-handler.ts`](../../../../../../raw/code/codegraph/src/bin/fatal-handler.ts)

## Classes
### `FatalHandlerDeps`
- def: [`src/bin/fatal-handler.ts:66`](../../../../../../raw/code/codegraph/src/bin/fatal-handler.ts#L66)
- doc: Injectable seams so the wiring is testable without registering real handlers.
- signature: `interface FatalHandlerDeps`
- members:
  - `exit` — [`L70`](../../../../../../raw/code/codegraph/src/bin/fatal-handler.ts#L70) — How to terminate. Defaults to `process.exit`.
  - `target` — [`L68`](../../../../../../raw/code/codegraph/src/bin/fatal-handler.ts#L68) — Event target to attach to. Defaults to `process`.
  - `write` — [`L72`](../../../../../../raw/code/codegraph/src/bin/fatal-handler.ts#L72) — How to emit the bounded line. Defaults to a synchronous fd-2 write.
- used by: [`installFatalHandlers`](fatal-handler.ts.md#installFatalHandlers)

## Functions
- `describeFatal(value: unknown)` — [`L40`](../../../../../../raw/code/codegraph/src/bin/fatal-handler.ts#L40) — Render an uncaught value for the last-resort log WITHOUT triggering stack
- `installFatalHandlers(deps?: FatalHandlerDeps)` — [`L79`](../../../../../../raw/code/codegraph/src/bin/fatal-handler.ts#L79) — Install the uncaught-exception / unhandled-rejection handlers. Both log a
- `writeStderr(line: string)` — [`L57`](../../../../../../raw/code/codegraph/src/bin/fatal-handler.ts#L57) — Best-effort synchronous stderr write that can never keep a doomed process alive.

