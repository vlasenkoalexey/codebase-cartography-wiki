---
title: 'Module: src/extraction/wasm-runtime-flags.ts'
type: catalog
provenance: extracted
module: src/extraction/wasm-runtime-flags.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`wasm-runtime-flags.ts`/
symbols:
  relaunchWithWasmRuntimeFlagsIfNeeded: relaunchWithWasmRuntimeFlagsIfNeeded().
  HOST_PPID_ENV: HOST_PPID_ENV.
  processHasWasmRuntimeFlags: processHasWasmRuntimeFlags().
  buildRelaunchArgv: buildRelaunchArgv().
  WASM_RUNTIME_FLAGS: WASM_RUNTIME_FLAGS.
  RELAUNCH_GUARD_ENV: RELAUNCH_GUARD_ENV.
---
# Module: [`src/extraction/wasm-runtime-flags.ts`](../../../../../../raw/code/codegraph/src/extraction/wasm-runtime-flags.ts)

## Functions
- `buildRelaunchArgv(scriptPath: string, scriptArgs: readonly string[], execArgv?: readonly string[])` — [`L74`](../../../../../../raw/code/codegraph/src/extraction/wasm-runtime-flags.ts#L74) — Build the argv for re-execing node with the WASM runtime flags: our flags
- `processHasWasmRuntimeFlags(execArgv?: readonly string[])` — [`L63`](../../../../../../raw/code/codegraph/src/extraction/wasm-runtime-flags.ts#L63) — True when every required WASM runtime flag is already present in `execArgv`.
- `relaunchWithWasmRuntimeFlagsIfNeeded(scriptPath: string)` — [`L92`](../../../../../../raw/code/codegraph/src/extraction/wasm-runtime-flags.ts#L92) — If the current process is missing the WASM runtime flags, re-exec it once

## Module values
- `HOST_PPID_ENV` — [`L60`](../../../../../../raw/code/codegraph/src/extraction/wasm-runtime-flags.ts#L60) — Env var carrying the *host* PID (the relauncher's own parent) across the
- `RELAUNCH_GUARD_ENV` — [`L47`](../../../../../../raw/code/codegraph/src/extraction/wasm-runtime-flags.ts#L47) — Env var set on the relaunched child so a detection slip can never cause an
- `WASM_RUNTIME_FLAGS` — [`L41`](../../../../../../raw/code/codegraph/src/extraction/wasm-runtime-flags.ts#L41) — The V8 flag(s) that keep tree-sitter grammar compilation off the turboshaft

