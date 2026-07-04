---
title: Global config & env-var resolution
type: doc-concept
provenance: doc
source: docs/getting-started/environment-variables.md
updated: 2026-07-04
status: fresh
---
# Global config & env-var resolution

## Definition
Claude Context is configured almost entirely through environment variables. To avoid
re-declaring them in every MCP client, it also reads a **global config file** at
`~/.context/.env`. Every knob resolves through a fixed three-tier priority:
**process environment variables** (highest) → **`~/.context/.env`** → **built-in defaults**
(lowest). "Configure once, use everywhere."

## In claude-context (grounded)
The MCP server's config resolver is [`createMcpConfig`](../catalog/packages/mcp/src/config.ts.md#createMcpConfig),
which builds a [`ContextMcpConfig`](../catalog/packages/mcp/src/config.ts.md#ContextMcpConfig) by
reading each variable through `envManager.get(...)`. Every read goes through the shared
[`envManager`](../catalog/packages/core/src/utils/env-manager.ts.md#envManager) singleton, whose
[`get`](../catalog/packages/core/src/utils/env-manager.ts.md#EnvManager.get) method implements the
priority exactly: it returns `process.env[name]` first, and only if that is unset does it parse
`~/.context/.env`; otherwise the caller's `|| <default>` supplies the default. So the doc's priority
table is not a convention — it is a single method every knob funnels through.

`createMcpConfig` resolves the **connection/provider** subset of knobs into the typed config object
(embedding provider + model, provider API keys and base URLs, Ollama host/model/dimension, Milvus
address/token, collection-name override). Other knobs documented here — `HYBRID_MODE`,
`EMBEDDING_BATCH_SIZE`, `SPLITTER_TYPE`, `CUSTOM_EXTENSIONS`, `CUSTOM_IGNORE_PATTERNS`,
`MILVUS_COLLECTION_LIMIT_CHECK_TIMEOUT_MS` — are **not** part of `ContextMcpConfig`; they are read at
their point of use in the core `Context` / vector-DB layer (see the related pages below). Both kinds
still resolve through the same `envManager` priority.

After building the config, [`logConfigurationSummary`](../catalog/packages/mcp/src/config.ts.md#logConfigurationSummary)
prints a redacted summary (provider, model, Milvus address or "auto-resolve from token", whether keys
are configured) so a misconfiguration is visible at startup without leaking secrets.

## Why it matters / when it applies
This is the entry point for every "how do I configure X" question: one file (`~/.context/.env`), one
priority order, one resolver. It also explains a common surprise — a value set in the global file is
silently overridden by a `-e VAR=...` passed on the MCP client's command line, because process env
wins. The redacted startup summary is the fastest way to confirm what actually took effect.

## Connections
- Code concepts: [MCP env-var config resolution](../concepts/packages-mcp-src-config.ts.md) — the resolver in depth.
- Module catalogs: [config.ts](../catalog/packages/mcp/src/config.ts.md) · [env-manager.ts](../catalog/packages/core/src/utils/env-manager.ts.md)
- Related doc-concepts: [Embedding provider & model selection](env-embedding-provider.md) · [Vector DB connection](env-vector-db-connection.md) · [Splitter selection & file filters](env-splitter.md) · [Search & indexing tuning knobs](env-tuning-knobs.md)

## Source
Extracted from `docs/getting-started/environment-variables.md` (kept in place).
