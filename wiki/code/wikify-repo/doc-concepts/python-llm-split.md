---
title: The Python/LLM split — grounding is mechanical, only synthesis is a model
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# The Python/LLM split — grounding is mechanical, only synthesis is a model

## Definition
The hard architectural rule behind everything else: **the deterministic stages are
pure Python — zero model calls** (SCIP parse, reconcile diff, packet build,
coverage, citation lint), and the LLM is invoked at exactly **one** step — concept
*synthesis* (plus concept-link judgment for connect). Synthesis never leaks into
Python and linting never leaks into a prompt: the model proposes prose, Python
decides what's true. That boundary is what keeps the wiki both grounded *and* cheap —
the expensive, hallucination-prone work is fenced to a single file-handoff stage,
while everything that must be exact stays mechanical and testable.

## In wikify-repo (grounded)
The split is a **file handoff on disk** (implementation.md §2): the deterministic
half never calls a model; the agent half never parses protobuf. The CLI exposes the
two halves the skill orchestrates around agent synthesis —
[`prepare`](../catalog/wikify/cli.md#prepare) (Stages 0–4: acquire, index, graph,
diff, evidence → emits synthesis packets) and
[`finalize`](../catalog/wikify/cli.md#finalize) (Stage 6/6b: lint, coverage
catalogs, assemble). Between them, the agent writes one page per packet:

```
wikify prepare <repo>  (Python) → packets
   ↓  [agent writes one page per packet]  (LLM, driven by SKILL.md)
wikify finalize <repo> (Python) → lint, assemble, state
   ↓  (lint fails?) → agent fixes flagged pages → finalize again
```

The deterministic side owns [`build_packet`](../catalog/wikify/packet.md#build_packet)
/ [`write_packet`](../catalog/wikify/packet.md#write_packet) (the LLM's input),
[`lint_silo`](../catalog/wikify/lint.md#lint_silo) (the gate on the LLM's output),
and [`emit_catalogs`](../catalog/wikify/coverage.md#emit_catalogs) (representation
without a model). The [`app`](../catalog/wikify/cli.md#app) surface is the whole
control plane. Coverage being a deterministic *set-difference* (not a model pass) is
a direct consequence: enumeration can't miss a module, so the LLM is spent only where
truth is genuinely cross-symbol.

## Why it matters / when it applies
Two failure modes this prevents: putting synthesis logic in Python yields rigid
templated junk; pushing linting into a prompt yields nondeterministic validation. The
boundary is the most important implementation rule — it is what lets the tool claim
"grounded" as a *build property* rather than a hope, and it makes the risky part
(prose) cheap to re-run without re-running the exact part (grounding).

## Connections
- Code concepts: [wikify CLI](../concepts/wikify-cli.md) — the prepare/finalize control surface; [The citation linter](../concepts/wikify-lint.md) — the gate on synthesized prose; [Coverage](../concepts/wikify-coverage.md) — deterministic representation.
- Module catalogs: [cli](../catalog/wikify/cli.md), [lint](../catalog/wikify/lint.md), [packet](../catalog/wikify/packet.md), [coverage](../catalog/wikify/coverage.md).
- Related doc-concepts: [packet-based-synthesis](packet-based-synthesis.md), [citation-linter-grounding-gate](citation-linter-grounding-gate.md), [concept-driven-synthesis-and-coverage](concept-driven-synthesis-and-coverage.md).

## Source
Extracted from `README.md` ("Architecture — the Python ↔ LLM split is hard"), with
the file-handoff contract from `docs/implementation.md` (§2 "The Python ↔ LLM
division"). Kept in place.
