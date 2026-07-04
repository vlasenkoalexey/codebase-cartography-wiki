---
title: Multi-repo connect — cross-linking the same concept across silos, inline
type: doc-concept
provenance: doc
source: docs/design.md
updated: 2026-07-04
status: fresh
---
# Multi-repo connect — cross-linking the same concept across silos, inline

## Definition
A single ingest produces a self-contained **silo** (`wiki/code/<slug>/`). With
several silos in one wiki, `wikify-connect-repo` (Stage 7) cross-links the same
concept across them so cross-framework questions ("**who implements** splash
attention?") resolve — without turning the wiki into an O(N²) hairball. Crucially,
the links are **inline, as a normal wiki**: the host's shared concept page is a hub
that links *down* to each repo's implementation, and each implementation links *up*.
There is **no `_connect/` side-table and no new page type** — connection state *is*
the wiki itself.

## In wikify-repo (grounded)
Realized in `wikify/connect.py`, whole-wiki (no slug).
[`load_vocabulary`](../catalog/wikify/connect.md#load_vocabulary) reads the host's
concept keys (the `wiki/concepts/` filenames — the host owns the vocabulary, not
wikify) × [`discover_silos`](../catalog/wikify/connect.md#discover_silos) (any dir
with `overview.md` + `concepts/`) → [`build_index`](../catalog/wikify/connect.md#build_index)
proposes `concept → [`[`Match`](../catalog/wikify/connect.md#Match)`]` candidates. A
[`SiloPage`](../catalog/wikify/connect.md#SiloPage) matches a key by an explicit
`concepts:` frontmatter tag (authoritative) or a name/token heuristic — the LLM only
confirms or rejects a grounded candidate, never conjures one.

Connect is **two operations**: (a) *dependency links* — deterministic re-resolution
of an external citation against another silo's SCIP index (touches citations, not
prose; not yet automated); (b) *concept correspondences* — the realized, selective,
inline linking. [`compute_report`](../catalog/wikify/connect.md#compute_report)
proposes; the human picks *which* keys (connecting everything drowns the pages);
`--apply` runs [`apply_connections`](../catalog/wikify/connect.md#apply_connections),
writing a `## In this wiki's repos` down-block on each concept page and a one-line
up-link block on each silo page — both inside regenerable `connect:auto` blocks so
hand-written prose is untouched. [`connected_keys`](../catalog/wikify/connect.md#connected_keys)
= the pages that carry a block (the state), and `--refresh` regenerates them after a
new ingest. Idempotent — re-apply yields no churn.

## Why it matters / when it applies
This is the multi-repo comprehension axis for the survey: one silo answers "how does
*this repo* do X"; connect adds "**who implements X** across the ecosystem". It is
selective by design and re-runnable as a cheap deterministic post-pass, so adding the
Nth repo costs one ingest + one connect — not a rebuild of the whole wiki. It never
re-synthesizes linted silo prose (the sole exception being optional human-authored hub
prose *above* the auto block).

## Connections
- Code concepts: [wikify connect](../concepts/wikify-connect.md) — the connection engine.
- Module catalogs: [connect](../catalog/wikify/connect.md).
- Related doc-concepts: [idempotent-reconcile](idempotent-reconcile.md), [devirtualization-dispatch-seam](devirtualization-dispatch-seam.md), [concept-driven-synthesis-and-coverage](concept-driven-synthesis-and-coverage.md), [tool-positioning-comparison](tool-positioning-comparison.md).

## Source
Extracted from `docs/design.md` (Stage 7 "Multi-repo connection"; "Connect is two
operations"; "Links are inline through the concept page"), with the realized module
from `docs/implementation.md` (§10.10 `wikify/connect.py`). Kept in place.
