---
title: Inference provider configuration
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Inference provider configuration

## Definition
The README's "Customizing" section states OpenWiki "supports OpenRouter, Fireworks, Baseten, OpenAI and
Anthropic out of the box," ships a few pre-defined models (GLM 5.2, Kimi K2.6, Sonnet 5, …), and lets each
provider take a custom model id. On the first interactive run it walks the user through configuring provider,
API key, and model, saving them to `~/.openwiki/.env` (optionally with a LangSmith tracing key).

## In openwiki (grounded)
The provider/model catalog is [`PROVIDER_CONFIGS`](../catalog/src/constants.ts.md#PROVIDER_CONFIGS) — a table
keyed by [`OpenWikiProvider`](../catalog/src/constants.ts.md#OpenWikiProvider) with each provider's API-key env
var, optional OpenAI-compatible `baseURL`, label, and curated model list. The active provider is chosen by
[`resolveConfiguredProvider`](../catalog/src/constants.ts.md#resolveConfiguredProvider) (explicit
`OPENWIKI_PROVIDER`, else an inferred OpenRouter if its key is present, else the default). The README's "first
interactive run" setup is the credential wizard, which accumulates the chosen provider/key/model and commits
them in one [`saveOpenWikiEnv`](../catalog/src/env.ts.md#saveOpenWikiEnv) call to `~/.openwiki/.env` at `0600`. The "custom
model id" affordance is the wizard's custom option plus the `--modelId` flag, both validated by
[`isValidModelId`](../catalog/src/constants.ts.md#isValidModelId).

## Why it matters / when it applies
Making the *inference backend* the configurable axis (five providers, BYO model) is the mirror image of the
other survey tools, whose configurable axis is the *code-analysis backend* (indexers, languages, extraction).
OpenWiki has no analysis backend to configure — only which model reads the repo. The LangSmith option exists
so runs can be traced to an "openwiki" tracing project.

## Connections
- Code concepts: [Provider & model catalog](../concepts/openwiki-constants.ts.md);
  [Credential store](../concepts/openwiki-env.ts.md);
  [Interactive credential setup wizard](../concepts/openwiki-credentials.tsx.md).
- Module catalogs: [src/constants.ts](../catalog/src/constants.ts.md), [src/env.ts](../catalog/src/env.ts.md),
  [src/credentials.tsx](../catalog/src/credentials.tsx.md).
- Related doc-concepts: [Agent-native documentation](agent-native-documentation.md).

## Source
Extracted from `README.md` (kept in place).
