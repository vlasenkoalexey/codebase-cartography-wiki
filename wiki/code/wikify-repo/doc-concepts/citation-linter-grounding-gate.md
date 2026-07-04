---
title: The citation linter — the hallucination floor as a hard build gate
type: doc-concept
provenance: doc
source: docs/implementation.md
updated: 2026-07-04
status: fresh
---
# The citation linter — the hallucination floor as a hard build gate

## Definition
The faithfulness mechanism that distinguishes wikify-repo from tools whose LLM
summaries are unverified: **every claim traces to a real, compiler-resolved symbol,
behind a citation linter that fails the build if one doesn't check out.** A
hallucinated API name cannot survive `finalize`. Provenance is layered on top —
uncited interpretation must live in `> [!inferred]` blocks, and pages are tagged
`extracted` vs `inferred` so a consumer never mistakes a model guess for ground
truth. The README's comparison table frames this as the single axis where
wikify-repo is "hard gate" while graphify is "honest labels, not gated" and
understand-anything / Google Code Wiki are "unverified / not a source of truth".

## In wikify-repo (grounded)
The linter is deterministic and checkable **without NLP** because its rules are
scoped to named sections and list items (implementation.md §5.3). A citation is a
markdown link to a **catalog anchor** `../catalog/<module>.md#<QualifiedName>`;
[`page_citations`](../catalog/wikify/lint.md#page_citations) extracts them and
[`_resolve_citation`](../catalog/wikify/lint.md#_resolve_citation) checks each
against the catalog's frontmatter `symbols:` map — reconstructing a moniker that must
exist in the silo's SCIP graph. [`lint_page`](../catalog/wikify/lint.md#lint_page) /
[`lint_silo`](../catalog/wikify/lint.md#lint_silo) enforce three hard rules,
producing [`LintError`](../catalog/wikify/lint.md#LintError) records on failure:

1. every catalog citation must resolve;
2. in `## Entry points` and `## Mechanism` sections, every list item carries ≥1
   citation or L2 evidence link;
3. no symbol cited that is absent from the concept's packet subgraph (catches
   invented symbols).

The anchor↔moniker contract is owned by
[`catalog_ref`](../catalog/wikify/coverage.md#catalog_ref) /
[`qualified_name`](../catalog/wikify/coverage.md#qualified_name) (the single source
of the citation-target format, shared by the packet and the catalog) and resolved
through [`parse_symbol`](../catalog/wikify/monikers.md#parse_symbol). Doc-concept
pages like this one get **rule 1 only**, via
[`lint_doc_concepts`](../catalog/wikify/lint.md#lint_doc_concepts) — they come from a
project doc, not a packet, so there is no subgraph/uncited gate.

## Why it matters / when it applies
This is *the hallucination floor*. Grounding is enforced as a build property, not a
prompt instruction — "the citation linter is a build gate, not a prompt". It is the
lower of two correctness altitudes: the linter proves a claim *cites a real symbol*;
the adversarial [verify](adversarial-verify.md) pass proves the claim is *true*.

## Connections
- Code concepts: [The citation linter](../concepts/wikify-lint.md) — the gate itself; [Monikers](../concepts/wikify-monikers.md) — the anchor↔moniker resolution; [Coverage](../concepts/wikify-coverage.md) — owns the citation-target format.
- Module catalogs: [lint](../catalog/wikify/lint.md), [monikers](../catalog/wikify/monikers.md), [coverage](../catalog/wikify/coverage.md).
- Related doc-concepts: [scip-vs-ast-grounding](scip-vs-ast-grounding.md), [adversarial-verify](adversarial-verify.md), [python-llm-split](python-llm-split.md), [packet-based-synthesis](packet-based-synthesis.md).

## Source
Extracted from `docs/implementation.md` (§5.3 citation grammar & lint rules; §10.4
`finalize --fix`), with the framing from `README.md` (faithfulness column;
"hallucination floor") and `docs/design.md` ("How this minimizes hallucination";
Stage 6). Kept in place.
