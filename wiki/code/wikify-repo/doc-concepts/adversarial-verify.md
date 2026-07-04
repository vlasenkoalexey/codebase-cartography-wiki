---
title: Adversarial verify — the correctness floor above the grounding floor
type: doc-concept
provenance: doc
source: docs/implementation.md
updated: 2026-07-04
status: fresh
---
# Adversarial verify — the correctness floor above the grounding floor

## Definition
Two gates at different altitudes. The citation linter is the **grounding floor**: it
proves every claim *cites a real symbol*. But a claim can cite real symbols and still
be *false* (wrong mechanism, wrong order). **Adversarial verify** is the
**correctness floor** on top: skeptic agents try to *refute* each load-bearing claim
against the real source, and verdicts fold to pass/fail. On jax it caught 3 real
errors in 323 claims.

## In wikify-repo (grounded)
The deterministic half (`wikify verify`, `wikify/verify.py`) prepares the worklist
and aggregates verdicts; the refutation itself is the LLM half
(`prompts/verify.md`). [`load_bearing_claims`](../catalog/wikify/verify.md#load_bearing_claims)
extracts each [`Claim`](../catalog/wikify/verify.md#Claim) from a page's cited
sections, carrying its [`Claim.citations`](../catalog/wikify/verify.md#Claim.citations)
and [`Claim.section`](../catalog/wikify/verify.md#Claim.section). A skeptic agent
returns a [`Verdict`](../catalog/wikify/verify.md#Verdict) per claim
([`Verdict.refuted`](../catalog/wikify/verify.md#Verdict.refuted) +
[`Verdict.note`](../catalog/wikify/verify.md#Verdict.note)), and
[`aggregate`](../catalog/wikify/verify.md#aggregate) folds them into a
[`PageReport`](../catalog/wikify/verify.md#PageReport)
([`PageReport.refuted`](../catalog/wikify/verify.md#PageReport.refuted) /
[`PageReport.ok`](../catalog/wikify/verify.md#PageReport.ok)). This keeps the
Python/LLM split intact — the worklist and verdict math are deterministic; only the
refutation judgment is a model.

## Why it matters / when it applies
Grounding is necessary but not sufficient: a wiki whose every claim cites a real
symbol can still mislead if the *reasoning* is wrong. Verify is the adversarial check
that a reader can trust the prose, not just the anchors — the pairing of a
build-gating linter (grounding) with a skeptic pass (correctness) is what makes the
wiki trustworthy end to end, and it is a distinguishing rigor step relative to tools
whose LLM summaries are simply unverified.

## Connections
- Code concepts: [wikify verify](../concepts/wikify-verify.md) — adversarial claim verification; [The citation linter](../concepts/wikify-lint.md) — the grounding floor below it.
- Module catalogs: [verify](../catalog/wikify/verify.md), [lint](../catalog/wikify/lint.md).
- Related doc-concepts: [citation-linter-grounding-gate](citation-linter-grounding-gate.md), [python-llm-split](python-llm-split.md), [tool-positioning-comparison](tool-positioning-comparison.md).

## Source
Extracted from `docs/implementation.md` (§10.4 "Adversarial verify"), with the
"correctness floor above the grounding floor" decision from `docs/design.md`
(Decisions log). Kept in place.
