---
title: Docs mode — prose as a first-class source, grounded on document sections
type: doc-concept
provenance: doc
source: docs/design.md
updated: 2026-07-04
status: fresh
---
# Docs mode — prose as a first-class source, grounded on document sections

## Definition
wikify's identity is *Karpathy synthesis wrapped in a deterministic shell*: a
**grounding gate** + a **coverage floor**, with the LLM doing only synthesis. Code
mode anchors that shell to SCIP symbols. A repo that is *documentation, not code* has
no symbols — so rather than degrade, **docs mode (`source_type: docs`) swaps the
anchor** while keeping the shell identical: the grounding anchor becomes a **source
document + `#section`**, and the coverage domain becomes a set-difference over **doc
files** instead of modules. The Python↔LLM split is unchanged.

## In wikify-repo (grounded)
Realized in `wikify/docs.py`. [`cli.py`](../catalog/wikify/cli.md) branches on
`source_type`: [`_prepare_docs`](../catalog/wikify/cli.md#_prepare_docs) and
[`_finalize_docs`](../catalog/wikify/cli.md#_finalize_docs) replace the SCIP path.
- **Enumerate + anchor.** [`enumerate_docs`](../catalog/wikify/docs.md#enumerate_docs)
  (vendor-skipped globs) → [`build_doc_map`](../catalog/wikify/docs.md#build_doc_map)
  runs per-format **anchor adapters** — [`_markdown_anchors`](../catalog/wikify/docs.md#_markdown_anchors)
  (ATX/setext heading slugs), `_html_anchors` (headings + `id`), else whole-file —
  producing [`DocInfo`](../catalog/wikify/docs.md#DocInfo) with its
  [`DocInfo.anchors`](../catalog/wikify/docs.md#DocInfo.anchors).
- **Packet + synthesis.** [`write_doc_packets`](../catalog/wikify/docs.md#write_doc_packets)
  hands the agent the exact `src:<doc>#<anchor>` tokens to cite verbatim (mirroring
  how a code packet hands over `cite:` catalog anchors); synthesis writes `topics/`
  (cross-source, reconciled) + `sources/` (per-doc).
- **The gate + floor.** [`lint_docs`](../catalog/wikify/docs.md#lint_docs) fails the
  build if any `src:` citation points at a doc/section that doesn't exist;
  [`docs_coverage`](../catalog/wikify/docs.md#docs_coverage) is the set-difference so
  no doc is silently dropped; [`assemble_docs_index`](../catalog/wikify/docs.md#assemble_docs_index)
  writes the index. Config keys [`RepoConfig.source_type`](../catalog/wikify/config.md#RepoConfig.source_type)
  and [`RepoConfig.doc_globs`](../catalog/wikify/config.md#RepoConfig.doc_globs)
  select the mode.

## Why it matters / when it applies
Docs mode is what makes the framework **one polymorphic grounding target + one
coverage domain**, instantiated for code (symbol/module) or docs (section/file) —
*not a forked pipeline*. It adds to a manual knowledge-base the two things it lacks: a
citation that **fails the build** on a dead section, and a coverage floor. **Honest
limit:** grounding *strength* degrades with format fidelity — markdown/HTML get
fine-grained section anchors; PDF/images fall back to page-/file-level. (Distinct
from the *doc-concept extraction* step that produced this very page, which grounds a
code repo's own docs onto its SCIP catalog; docs mode grounds a docs-only repo onto
its own sections.)

## Connections
- Code concepts: [Docs mode](../concepts/wikify-docs.md) — the prose-ingestion pipeline; [wikify config](../concepts/wikify-config.md) — the `source_type` switch; [wikify CLI](../concepts/wikify-cli.md) — the prepare/finalize branch.
- Module catalogs: [docs](../catalog/wikify/docs.md), [config](../catalog/wikify/config.md), [cli](../catalog/wikify/cli.md).
- Related doc-concepts: [citation-linter-grounding-gate](citation-linter-grounding-gate.md), [concept-driven-synthesis-and-coverage](concept-driven-synthesis-and-coverage.md), [python-llm-split](python-llm-split.md).

## Source
Extracted from `docs/design.md` ("Docs mode — prose as a first-class source type"),
with the realized module map from `docs/implementation.md` (§10.7 `wikify/docs.py`).
Kept in place.
