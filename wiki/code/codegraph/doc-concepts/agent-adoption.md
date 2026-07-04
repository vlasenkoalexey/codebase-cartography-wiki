---
title: Agent adoption of codegraph (Read-parity + startup readiness)
type: doc-concept
provenance: doc
source: docs/design/agent-codegraph-adoption.md
updated: 2026-07-04
status: fresh
---
# Agent adoption of codegraph (Read-parity + startup readiness)

## Definition
Two problems keep an agent from *actually using* codegraph instead of `Read`/`grep`:
**(P1)** even with codegraph attached, the agent reflexively Reads/greps
mid-implementation; **(P2)** on startup the codegraph MCP server can be `pending`
when the agent's first turn fires, so the session runs with **no codegraph at
all**. This doc-concept captures the doctrine and the shipped fixes for both.

## Mental model
**Adapt the tool to the agent — don't try to change the agent.** codegraph's only
channels to the agent (the MCP `initialize` instructions and tool descriptions)
are **low-salience**: wording changes do not reliably move tool-*choice* and have
*regressed* wall-clock before; new tools fare worse than extending an existing one
(the agent under-picks even `trace`). The mechanism behind everything: **an agent
falls back to Read/Grep the instant a codegraph answer is insufficient.** So the
real levers are **coverage** (more flows connect statically → explore surfaces
them) and **sufficiency** (output complete enough that the agent *stops* reading).
The P1 fix follows directly: don't *force* the agent off Read with a hook — make
`codegraph_node` **read a file exactly like the Read tool, only faster**, so the
agent reaches for it naturally. The optimization target is **wall-clock +
tool-call count + Read=0**, not token cost.

## In codegraph (grounded)
**P1 — Read-parity file-view** (in `src/mcp/tools.ts`):
- [`ToolHandler.handleFileView`](../catalog/src/mcp/tools.ts.md#ToolHandler.handleFileView)
  — a `file` with no `symbol` returns the file's source numbered **byte-for-byte
  the way Read does** (`<n>\t<line>`, no padding, trailing empty line kept), plus a
  one-line blast-radius header. `offset`/`limit` mean exactly what they do on Read
  (1-based, default whole file capped at 2000 lines). Content is the **default**;
  `symbolsOnly: true` returns the cheap structural map. Security preserved (yaml/
  properties summarized, reads via `validatePathWithinRoot`).
- Reached through
  [`ToolHandler.handleNode`](../catalog/src/mcp/tools.ts.md#ToolHandler.handleNode)
  (the `codegraph_node` handler) alongside
  [`ToolHandler.handleSearch`](../catalog/src/mcp/tools.ts.md#ToolHandler.handleSearch).
  The **PreToolUse Read-redirect hook** (idea 1) was A/B'd and **REJECTED** — a
  blanket Read-deny roughly doubled tool calls and the agent routed around it
  (`Bash python3` to read the file). Forcing is the wrong lever.

**P2 — expose the static tool list instantly, decoupled from the daemon:**
- The suspected cause is that `serve --mcp` forwards `tools/list` to the
  still-connecting daemon instead of answering it locally. The fix is to advertise
  the static tools the moment the client asks — the tool surface is built by
  [`getStaticTools`](../catalog/src/mcp/tools.ts.md#getStaticTools) (also imported
  into the proxy), served through the fast local handshake
  [`runLocalHandshakeProxy`](../catalog/src/mcp/proxy.ts.md#runLocalHandshakeProxy)
  (which answers `initialize` in ~107ms) driven by
  [`MCPServer.runProxyWithLocalHandshake`](../catalog/src/mcp/index.ts.md#MCPServer.runProxyWithLocalHandshake).
- The startup cost is the `--liftoff-only` **re-exec** (for a V8 memory flag) plus
  binding a **detached daemon** via
  [`spawnDetachedDaemon`](../catalog/src/mcp/index.ts.md#spawnDetachedDaemon) →
  [`Daemon.start`](../catalog/src/mcp/daemon.ts.md#Daemon.start). The re-exec is
  guarded by
  [`RELAUNCH_GUARD_ENV`](../catalog/src/extraction/wasm-runtime-flags.ts.md#RELAUNCH_GUARD_ENV)
  (`CODEGRAPH_WASM_RELAUNCHED=1` skips it) built by
  [`relaunchWithWasmRuntimeFlagsIfNeeded`](../catalog/src/extraction/wasm-runtime-flags.ts.md#relaunchWithWasmRuntimeFlagsIfNeeded);
  the host PPID env is
  [`HOST_PPID_ENV`](../catalog/src/extraction/wasm-runtime-flags.ts.md#HOST_PPID_ENV).
  Actual tool *calls* still run on the daemon-backed query pool
  ([`QueryPool.run`](../catalog/src/mcp/query-pool.ts.md#QueryPool.run)) — only
  tool *exposure* is decoupled to remove `pending`-at-startup.
- Mitigation ideas: a SessionStart hook that pre-warms the daemon; a host-side
  "wait/retry on pending" (a Claude Code MCP-client behavior, not codegraph's to
  fix — `MCP_TIMEOUT` did **not** help, because the problem is tool-exposure
  *timing*, not a connection timeout).

## Why it matters / when it applies
- A clean A/B showed the reframed steering *did* move tool-choice (baseline: 0
  codegraph calls / 8 Reads → new: 2 `explore` calls / 5 Reads), but the agent
  never used the file-view and still Read 5× — confirming wording alone can't fix
  P1; sufficiency (Read-parity) can.
- **Validate any behavioral claim with an A/B** — `scripts/agent-eval/ab-new-vs-baseline.sh`
  (new-build vs baseline, both codegraph-on) for Read displacement; time
  `tools/list` from `serve --mcp` for startup. n≥2 runs/arm (n=1 is noisy); the
  host's `init` snapshot can lie (`pending` even when it connects) — judge by
  actual codegraph usage. Both arms always run `--model sonnet` (the deliberate
  floor model).

## Connections
- Code concepts: [MCP tools — explore/node/file-view](../concepts/mcp-tools.ts.md);
  [MCP daemon — detached server + startup](../concepts/mcp-daemon.ts.md);
  [MCP query pool — worker-backed tool calls](../concepts/mcp-query-pool.ts.md).
- Module catalogs: [src/mcp/tools.ts](../catalog/src/mcp/tools.ts.md),
  [src/mcp/proxy.ts](../catalog/src/mcp/proxy.ts.md),
  [src/mcp/index.ts](../catalog/src/mcp/index.ts.md),
  [src/mcp/daemon.ts](../catalog/src/mcp/daemon.ts.md),
  [src/mcp/query-pool.ts](../catalog/src/mcp/query-pool.ts.md),
  [src/extraction/wasm-runtime-flags.ts](../catalog/src/extraction/wasm-runtime-flags.ts.md).
- Related doc-concepts: [Adaptive explore sizing](adaptive-explore-sizing.md) —
  the "sufficiency" lever (a smaller, complete explore answer) applied to output.

## Source
Extracted from `docs/design/agent-codegraph-adoption.md` (kept in place).
