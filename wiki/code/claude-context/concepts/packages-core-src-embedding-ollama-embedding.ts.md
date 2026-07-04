---
title: Ollama embedding provider — local, keyless, self-measuring dimensions
type: concept
provenance: mixed
concept: packages-core-src-embedding-ollama-embedding.ts
updated: 2026-07-04
status: fresh
---
# Ollama embedding provider — local, keyless, self-measuring dimensions

## Overview
`OllamaEmbedding` is the **local, self-hosted** grounding substrate for claude-context's semantic
search: instead of calling a cloud API, it talks to an Ollama daemon on `localhost` and asks it to
turn code chunks into vectors. It is one of several interchangeable implementations of the abstract
[`Embedding`](packages-core-src-embedding-base-embedding.ts.md) contract — it inherits the shared
text-preprocessing/truncation machinery and only supplies the two provider-specific verbs,
[`embed`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embed) and
[`embedBatch`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embedBatch).
What makes the Ollama provider distinctive is that it carries **no API key and no fixed vector width**:
the host defaults to a loopback URL in the
[`<constructor>`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.-constructor),
and the embedding
[`dimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimension)
is *discovered at runtime* by sending one probe request rather than being hard-coded per model.

## Diagram
```mermaid
flowchart TD
    CTOR["&lt;constructor&gt;(OllamaEmbeddingConfig)"] -->|host || 127.0.0.1:11434| CLIENT[client: Ollama]
    CTOR -->|config.dimension?| DDET[dimensionDetected]
    CTOR -->|no maxTokens| SDMT[setDefaultMaxTokensForModel]
    EMBED[embed] --> PRE[preprocessText]
    EMBED -->|first use| DETECT[detectDimension]
    EMBEDB[embedBatch] --> PRES[preprocessTexts]
    EMBEDB -->|first use| DETECT
    DETECT --> CLIENT
    EMBED --> CLIENT
    EMBEDB --> CLIENT
    CLIENT --> EV[EmbeddingVector]
    SETMODEL[setModel] --> DETECT
    SETHOST[setHost] --> CLIENT
```

## Design rationale (why it's built this way)
The central non-obvious decision is **lazy, measured dimensionality**. Cloud providers know their
vector width ahead of time; a local Ollama server can be running any embedding model the user pulled,
so the width is unknown until the model actually answers. The class encodes this with a
`768`-valued default on
[`dimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimension)
(commented in source as *"Default dimension for many embedding models"*) plus a
[`dimensionDetected`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimensionDetected)
flag *"Track if dimension has been detected"*. If the caller supplied a
[`dimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.dimension)
in config, the
[`<constructor>`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.-constructor)
trusts it and marks detection done; otherwise the true width is filled in on the first embed call. This
matters downstream because the vector store's collection is created with a fixed dimension — a wrong
guess would poison the index, so the provider prefers to *ask the server* over assuming.

The second decision is **keyless, loopback-first connectivity**. The
[`<constructor>`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.-constructor)
builds the `ollama` [`client`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.client)
with `host: config.host || 'http://127.0.0.1:11434'` — the default Ollama port on localhost — and takes
an optional
[`fetch`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.fetch)
override, but there is **no `apiKey` field** on
[`OllamaEmbeddingConfig`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig)
at all — the defining contrast with the OpenAI/Voyage/Gemini providers, which are keyed cloud clients.

The third is a **per-model token budget baked in as a lookup**.
[`setDefaultMaxTokensForModel`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setDefaultMaxTokensForModel)
special-cases `nomic-embed-text` and `snowflake-arctic-embed` to `8192` and falls back to `2048`
otherwise (the source comment on
[`maxTokens`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.maxTokens)
calls `2048` the *"Default context window for Ollama"*). That number feeds the inherited
[`preprocessText`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.preprocessText)
character-truncation, so the provider must know a sane budget before the first chunk is truncated.

> [!inferred]
> The `keep_alive`/`options` pass-through and the loopback default read as an intent to make Ollama a
> zero-config, privacy-preserving alternative to cloud embedding — code never leaves the machine — but
> the source does not state this motivation explicitly.

## Entry points
- [`<constructor>`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.-constructor)
  — reached when the indexing pipeline instantiates the provider from an
  [`OllamaEmbeddingConfig`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig).
  It wires the [`client`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.client),
  seeds [`dimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimension)/[`dimensionDetected`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimensionDetected),
  and sets the token budget.
- [`embed`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embed) —
  *"Generate text embedding vector"*; the single-text path, hit once per query or per chunk when the
  caller embeds one string. Returns one
  [`EmbeddingVector`](../catalog/packages/core/src/embedding/base-embedding.ts.md#EmbeddingVector).
- [`embedBatch`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embedBatch)
  — *"Generate text embedding vectors in batch"*; the bulk-indexing path, hit for arrays of chunks. It
  concretely overrides the abstract
  [`embedBatch`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.embedBatch).
- [`setModel`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setModel),
  [`setHost`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setHost),
  [`setKeepAlive`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setKeepAlive),
  [`setOptions`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setOptions),
  [`setMaxTokens`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setMaxTokens)
  — post-construction mutators reached when a UI/config layer reconfigures the live provider.

## Mechanism (step-by-step)
1. **Construct and connect.** The
   [`<constructor>`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.-constructor)
   stores the [`config`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.config)
   and builds an `Ollama` [`client`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.client)
   pointed at [`host`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.host)
   or the `127.0.0.1:11434` loopback default, passing the optional
   [`fetch`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.fetch)
   implementation through. If the config carried an explicit
   [`dimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.dimension),
   it is copied to the instance
   [`dimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimension)
   and [`dimensionDetected`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimensionDetected)
   is set true so no probe is needed later.

2. **Establish the token budget.** Still in the
   [`<constructor>`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.-constructor),
   an explicit config
   [`maxTokens`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.maxTokens)
   wins; otherwise
   [`setDefaultMaxTokensForModel`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setDefaultMaxTokensForModel)
   inspects the [`model`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.model)
   name and picks `8192` for `nomic-embed-text`/`snowflake-arctic-embed`, else `2048`, writing the
   instance [`maxTokens`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.maxTokens)
   the base class reads during truncation.

3. **Preprocess before embedding.** On each call,
   [`embed`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embed) runs
   the input through the inherited
   [`preprocessText`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.preprocessText)
   (empty string → single space, then character-truncate at `maxTokens * 4`), and
   [`embedBatch`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embedBatch)
   maps the whole array through
   [`preprocessTexts`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.preprocessTexts).
   This is shared contract, not provider-specific.

4. **Detect dimension on first real use.** Both
   [`embed`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embed) and
   [`embedBatch`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embedBatch)
   check `!dimensionDetected && !config.dimension`; if so they `await`
   [`detectDimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.detectDimension),
   which embeds the literal probe text `"test"`, reads `response.embeddings[0].length`, and returns it —
   the width the running model actually produces. The result is stored on
   [`dimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimension)
   and [`dimensionDetected`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimensionDetected)
   is flipped so the probe runs at most once.

5. **Call the Ollama embed API and shape the result.** Both methods build an `embedOptions` object with
   [`model`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.model),
   the preprocessed `input`, and provider-tuning
   [`options`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.options),
   conditionally attaching `keep_alive` from
   [`keepAlive`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.keepAlive)
   only when it is a non-empty value. `embedBatch` passes the array straight to Ollama's *native batch
   API* (one round trip, not a loop) and maps each returned row into an
   [`EmbeddingVector`](../catalog/packages/core/src/embedding/base-embedding.ts.md#EmbeddingVector)
   `{ vector, dimension }`; `embed` returns the single
   [`EmbeddingVector`](../catalog/packages/core/src/embedding/base-embedding.ts.md#EmbeddingVector)
   from `response.embeddings[0]`. Each throws if the response has no `embeddings`.

6. **Reconfigure a live provider.**
   [`setModel`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setModel)
   *"Set model type and detect its dimension"*: it swaps
   [`config.model`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.model),
   **resets** [`dimensionDetected`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimensionDetected)
   to false, re-derives the budget via
   [`setDefaultMaxTokensForModel`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setDefaultMaxTokensForModel),
   and (unless a config dimension is pinned) immediately re-runs
   [`detectDimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.detectDimension).
   [`setHost`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setHost)
   rebuilds the [`client`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.client)
   against a new [`host`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.host),
   while [`setKeepAlive`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setKeepAlive)
   and [`setOptions`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setOptions)
   just mutate the stored [`config`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.config).
   [`setMaxTokens`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setMaxTokens)
   writes **both** `config.maxTokens` *and* the live `this.maxTokens` field, so it takes effect on the
   next `embed`/`embedBatch` without a rebuild (the shared truncation budget is read from the instance).

## Key data structures
- [`OllamaEmbeddingConfig`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig)
  — the provider's whole surface: a required
  [`model`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.model)
  plus optional
  [`host`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.host),
  [`fetch`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.fetch),
  [`keepAlive`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.keepAlive),
  [`options`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.options),
  [`dimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.dimension),
  and [`maxTokens`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.maxTokens).
  Notably **no API key** — the local-provider tell.
- The instance state that a cloud provider wouldn't need:
  [`client`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.client) (the
  `Ollama` SDK handle),
  [`dimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimension)
  (mutable, starts at `768`), and
  [`dimensionDetected`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimensionDetected)
  (the one-shot latch guarding the probe).
- [`EmbeddingVector`](../catalog/packages/core/src/embedding/base-embedding.ts.md#EmbeddingVector) —
  the `{ vector: number[]; dimension: number }` shape defined in the base module and shared by every
  provider; this is the common currency the vector store consumes.
- [`maxTokens`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.maxTokens)
  — the concrete override of the base class's abstract
  [`maxTokens`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.maxTokens); its
  Ollama default (`2048`) differs from the OpenAI (`8192`), Gemini (`2048`), and Voyage (`32000`)
  siblings, so the truncation budget is genuinely provider-specific.

## Dynamics (design intent)
The abstract-method contract is what lets the pipeline treat any provider uniformly: the class's
[`embed`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embed)/[`embedBatch`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embedBatch)
concretely implement the abstract
[`embed`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.embed)/[`embedBatch`](../catalog/packages/core/src/embedding/base-embedding.ts.md#Embedding.embedBatch)
declared on the base. The cross-provider test doubles corroborate this substitutability: every
`TestEmbedding`/`FailingEmbedding` in the suite pins its own
[`maxTokens`](../catalog/packages/core/src/context.abort.test.ts.md#TestEmbedding.maxTokens) and the
tests exercise both verbs against the shared
[`EmbeddingVector`](../catalog/packages/core/src/embedding/base-embedding.ts.md#EmbeddingVector) shape
(`context.abort.test.ts`, `context.embedding-error.test.ts`, `context.splitter.test.ts`,
`context.ignore-patterns.test.ts`) — evidence that the indexing/search code depends only on the base
contract, never on Ollama specifics.

> [!inferred]
> The dimension probe is guarded so it runs at most once per model, so the `embed`/`embedBatch` calls
> for a warm provider make a single round trip. I read this from the
> `!dimensionDetected && !config.dimension` guard and the flag flip in source, not from a concurrency
> test — there is no test in the packet exercising the Ollama provider directly.

## Edge cases
- **Explicit config dimension short-circuits detection.** Passing
  [`dimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.dimension)
  makes the [`<constructor>`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.-constructor)
  set [`dimensionDetected`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.dimensionDetected)
  true, so [`detectDimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.detectDimension)
  never runs even on the first call — the server's true width is trusted to match.
- **Empty / non-empty `keepAlive`.** `keep_alive` is attached only when
  [`keepAlive`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbeddingConfig.keepAlive)
  is truthy and not `''`; an empty string is treated as "unset" so the daemon uses its own default.
- **Malformed responses throw.**
  [`embed`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embed) throws
  `'Ollama API returned invalid response'` when `embeddings[0]` is missing;
  [`embedBatch`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.embedBatch)
  throws `'Ollama API returned invalid batch response'` when `embeddings` is not an array; and
  [`detectDimension`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.detectDimension)
  wraps failures as `'Failed to detect Ollama embedding dimension: …'` — a connection-refused localhost
  daemon surfaces here.
- **Model change mid-session.**
  [`setModel`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setModel)
  resets detection, so a switch from e.g. a 768-wide to a 1024-wide model re-probes; but a collection
  already created at the old width is not migrated by this class.
- **Unknown model name → default budget.**
  [`setDefaultMaxTokensForModel`](../catalog/packages/core/src/embedding/ollama-embedding.ts.md#OllamaEmbedding.setDefaultMaxTokensForModel)
  falls back to `2048` for any model outside its two hard-coded families, which may under- or
  over-estimate the real context window.

## Open questions
- `getDimension()` and `getProvider()` (which returns the literal `'Ollama'`) exist in the source but
  are **not in this packet's Subgraph**, so how downstream code reads the settled dimension or
  branches on provider name is described from source only, not a citable symbol.
- The `Ollama` SDK's `client.embed(...)` and the `response.embeddings` shape are external to the
  Subgraph; the exact batch semantics (partial failures, ordering guarantees) live in the `ollama`
  package, not here.
- Who constructs `OllamaEmbedding` and how the vector store's collection dimension is reconciled with a
  *detected* (vs. configured) width is outside this packet — see the context/vectordb concept pages.

## See also
- [`Embedding` base contract](packages-core-src-embedding-base-embedding.ts.md) — the shared abstract
  class, `preprocessText`/`preprocessTexts` truncation, and the `EmbeddingVector` shape all providers
  return.
- [`OpenAI embedding provider`](packages-core-src-embedding-openai-embedding.ts.md),
  [`Gemini embedding provider`](packages-core-src-embedding-gemini-embedding.ts.md),
  [`VoyageAI embedding provider`](packages-core-src-embedding-voyageai-embedding.ts.md) — the keyed
  cloud siblings this local provider contrasts with (fixed dimensions, API keys, different token budgets).
- [`context` orchestration](packages-core-src-context.ts.md) — where an embedding provider is wired
  into the index/search pipeline alongside the splitter and vector store.
