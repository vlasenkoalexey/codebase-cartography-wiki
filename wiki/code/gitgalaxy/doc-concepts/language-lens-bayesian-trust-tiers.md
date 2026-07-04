---
title: The Bayesian Trust Matrix — language identity as a graded, auditable claim
type: doc-concept
provenance: doc
source: docs/wiki/02-05-language-lens.md
updated: 2026-07-04
status: fresh
---
# The Bayesian Trust Matrix — language identity as a graded, auditable claim

## Definition
The doc frames `LanguageDetector` not as a classifier that outputs a single label, but as an
engine performing an "Entity Census": every file's language is a *claim* that must be proven
through a strict hierarchy of evidence before it is trusted, not assumed from its extension
alone. It names six discrete confidence rungs — Tier 0 Convergent Lock (0.95-0.99, two
independent signals agree), Tier 1 Roadmap Lock (0.95, a build manifest says so), Tier 1.5
Ecosystem Gravity (0.95, neighborhood-dominance collision resolution — see
[ecosystem-gravity-and-confidence-override](ecosystem-gravity-and-confidence-override.md)),
Tier 1.7 Exo-Species (0.95, an unrecognized-but-plausible extension), Tier 2 Single Signature
(0.91, one unverified signal, triggers mandatory spectral verification), Tier 3 Contextual
Proof (0.90, a GuideStar bias), Tier 4 Discovery (0.10, zero context, must earn its way up
via density scanning), and Tier 5 Absolute Distrust (0.00, contradictory signals — see
[identity-deception-and-extension-mismatch](identity-deception-and-extension-mismatch.md)).
"True confidence requires convergence": a single metadata signature is a suggestion, never a
verdict.

## In gitgalaxy (grounded)
The tier ladder is a direct, faithful description of the code, not marketing gloss on top of
it. Every result [`LanguageDetector.inspect`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.inspect)
produces is packed into a [`DetectorResult`](../catalog/gitgalaxy/standards/language_lens.md#DetectorResult)
that carries its own `lock_tier` and `source_proof` fields — the tier is not an internal
implementation detail discarded after the decision, it is the decision's audit trail, present
on every classified file. The doc's "Single Signature ... Triggers mandatory spectral
verification" is exactly the `needs_spectral` gate inside `inspect` that routes low-confidence
or collision-extension files into
[`_tier_3_lexical_scan`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector._tier_3_lexical_scan)
or [`_tier_4_heuristic_discovery`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector._tier_4_heuristic_discovery)
rather than accepting the claim at face value.

The doc's own "Determinism and Inventory Integrity" section connects this tier machinery to a
concrete downstream consumer: [`main`](../catalog/gitgalaxy/tools/compliance/sbom_generator.md#main),
the standalone SBOM generator, constructs a `LanguageDetector` directly to produce a Software
Bill of Materials. This is the load-bearing reason the tiers exist as a *visible* field rather
than a collapsed confidence float — an SBOM consumer (a security or compliance team) needs to
distinguish "Tier 1: Roadmap Lock via package.json" (authoritative) from "Tier 4: Spectral
Discovery" (heuristic best guess) when deciding how much to trust an entry in the inventory.

## Why it matters / when it applies
This is the doc's explicit contrast with "black-box LLMs that might return varying results
based on floating-point drift or prompt phrasing": the same file, scanned under the same
context, always yields the same `lock_tier`/confidence pair, because every tier is a
deterministic function of the file's bytes and a fixed configuration table
([language standards](../concepts/gitgalaxy-standards-language_standards.md)), never a model
sample. That repeatability is precisely what an SBOM or compliance audit needs and what a
probabilistic classifier cannot promise — the tier system trades a single confidence number
for a traceable, always-reproducible chain of evidence.

## Connections
- Code concepts: [Language lens](../concepts/gitgalaxy-standards-language_lens.md) — the full
  tier-cascade mechanism this page's tier table summarizes; [Language standards](../concepts/gitgalaxy-standards-language_standards.md) —
  the `LENS_CONFIG`/`LANGUAGE_DEFINITIONS` tables the tiers consult.
- Module catalogs: [language_lens](../catalog/gitgalaxy/standards/language_lens.md).
- Related doc-concepts: [ecosystem-gravity-and-confidence-override](ecosystem-gravity-and-confidence-override.md),
  [identity-deception-and-extension-mismatch](identity-deception-and-extension-mismatch.md),
  [polyglot-handshake-detection](polyglot-handshake-detection.md),
  [guidestar-intent-vs-identity](guidestar-intent-vs-identity.md) — the upstream "Scout" whose
  manifest-derived prior is what earns a file its Tier 1 Roadmap Lock or Tier 3 Contextual Proof.

## Source
Extracted from `docs/wiki/02-05-language-lens.md`, kept in place.
