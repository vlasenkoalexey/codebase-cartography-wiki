---
title: Idempotent reconcile — ingest as declarative apply, --ref as update
type: doc-concept
provenance: doc
source: docs/design.md
updated: 2026-07-04
status: fresh
---
# Idempotent reconcile — ingest as declarative apply, --ref as update

## Definition
Ingest is a **declarative reconcile** (like `make` / `terraform apply`), not an
imperative build. Its desired state is `{pinned commit's symbols} × {requested
concept set}`, and re-running *converges* the wiki to it: same inputs → no-op; a new
concept in the config → build only that page; a moved `--ref` → diff symbols, rebuild
only stale pages; a wiped cache → regenerate SCIP. There is therefore **no separate
`update` skill** — "update" is just `ingest --ref <newcommit>`. Before expensive
work, reconcile **previews its delta** (`will build / rebuild (stale) / leave`) — the
plan-then-apply split, so an overloaded ingest never surprises you.

## In wikify-repo (grounded)
The reconcile mechanism is the Stage 2 structural diff.
[`current_hashes`](../catalog/wikify/diff.md#current_hashes) hashes each symbol's
`(signature + body-span)` — bodies read via
[`body_span`](../catalog/wikify/source.md#body_span) /
[`body_hash`](../catalog/wikify/source.md#body_hash);
[`compute_plan`](../catalog/wikify/diff.md#compute_plan) diffs new vs stored hashes
into a [`Plan`](../catalog/wikify/diff.md#Plan) of `{build, rebuild, leave}`, with
[`Plan.is_noop`](../catalog/wikify/diff.md#Plan.is_noop) the idempotency check and
[`Plan.changed_symbols`](../catalog/wikify/diff.md#Plan.changed_symbols) driving
**citation-aware invalidation**: any page whose cited symbols intersect the changed
set is flagged `stale` (the citation graph gives this for free). The ledger is
`.cache/state/<slug>.json` — [`load_state`](../catalog/wikify/state.md#load_state) /
[`save_state`](../catalog/wikify/state.md#save_state), with
[`record_page`](../catalog/wikify/state.md#record_page) /
[`page_cited`](../catalog/wikify/state.md#page_cited) tracking each page's cited
monikers and built ref. Stage 0's pin —
[`acquire`](../catalog/wikify/acquire.md#acquire) →
[`Acquired`](../catalog/wikify/acquire.md#Acquired),
[`checkout`](../catalog/wikify/acquire.md#checkout),
[`commit_of`](../catalog/wikify/acquire.md#commit_of) — records the single commit SHA
the whole silo is valid against (stored once, per-repo, not per-page).

Adding a concept later is a *same-commit* reconcile: it builds only the new page from
the existing SCIP index — no re-extraction, no commit bump, nothing marked stale.

## Why it matters / when it applies
This is the "cheap to upgrade" half of the goal. A version bump costs only the
`changed` symbols and `stale` pages, not a full re-synthesis; a batch ingest is
safe to re-run because a no-op is genuinely a no-op. Behavioral changes that are *not*
AST-visible (a lowering tweak with an identical signature) are flagged
`behavioral_recheck` rather than silently missed — AST-diff alone drives core
re-ingestion.

## Connections
- Code concepts: [wikify-diff](../concepts/wikify-diff.md) — the reconcile engine; [Reconcile state](../concepts/wikify-state.md) — the idempotency ledger; [wikify-acquire](../concepts/wikify-acquire.md) — the commit pin.
- Module catalogs: [diff](../catalog/wikify/diff.md), [state](../catalog/wikify/state.md), [source](../catalog/wikify/source.md), [acquire](../catalog/wikify/acquire.md).
- Related doc-concepts: [python-llm-split](python-llm-split.md), [concept-driven-synthesis-and-coverage](concept-driven-synthesis-and-coverage.md), [multi-repo-connect](multi-repo-connect.md).

## Source
Extracted from `docs/design.md` ("Product surface — two skills"; "ingest is a
declarative reconcile"; Stage 2), with the state/diff contracts from
`docs/implementation.md` (§5.5, §5.1). Kept in place.
