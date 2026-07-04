---
title: "Intent vs. Identity — GuideStar the Scout, Language Lens the Scientist"
type: doc-concept
provenance: doc
source: docs/wiki/02-04-guidestar-protocol.md
updated: 2026-07-04
status: fresh
---
# Intent vs. Identity — GuideStar the Scout, Language Lens the Scientist

## Definition
`02-04-guidestar-protocol.md` frames the whole GuideStar/Language-Lens split as a two-role
"Handover": "**GuideStar (The Scout):** Identifies **Intent** (Why this file exists). It says: 'I
found this file referenced in a Makefile and it has a known C-extension; I predict it is a C-target
with 0.90 confidence.' **Language Lens (The Scientist):** Identifies **Identity** (What this file
is). It updates the prior for the 'Standard Galaxy'... and performs the atomic scan to verify all
claims." The doc calls the resulting property a "Scan Once" efficiency, and separately documents a
strict four-step precedence order a *reader* of the resulting locks should follow: "Exact Filename
Match → Relative Path Match → Pattern Match (`.gitattributes`) → Sector Bias."

## In gitgalaxy (grounded)
The [GuideStar Protocol](../concepts/gitgalaxy-core-guidestar_lens.md) code concept page already
derives and cites this exact division of labor from the source's own docstrings — it is not a new
claim this doc adds, but the doc's plain-language "Scout"/"Scientist" framing is worth keeping
alongside the code concept's more mechanism-level description of the same split: GuideStar's
[`scan_project_config`](../catalog/gitgalaxy/core/guidestar_lens.md#GuideStarLens.scan_project_config)
only ever produces a *prior* — an [`intent_locks`](../catalog/gitgalaxy/core/guidestar_lens.md#GuideStarLens.intent_locks)
entry with a `lang_id`/`intensity`/`source_proof` — from manifest and `.gitattributes` evidence,
before any file content is inspected. The "atomic scan" the doc attributes to the Language Lens is a
separate module ([Language lens](../concepts/gitgalaxy-standards-language_lens.md)) not in this
packet's own subgraph, but the [GuideStar Protocol](../concepts/gitgalaxy-core-guidestar_lens.md)
page's Design rationale section independently confirms the same "Scan Once" motivation from
`GuideStarLens`'s own docstrings.

The doc's four-step read-order (`Exact Filename Match → Relative Path Match → Pattern Match → Sector
Bias`) is a genuinely new, specific detail this doc supplies that the code concept page could **not**
ground to a symbol: that page's own Open Questions section states plainly that "the read-side lookup
that later consumers use to resolve a file's final intent status... is not itself a symbol in this
packet's subgraph, so its exact precedence logic is described from the project's own docs rather than
cited to a method here." This doc-concept page is the source of that description — the four-tier order
is asserted by `docs/wiki/02-04-guidestar-protocol.md` itself, not verified against a cited method, and
should be read with that caveat.

## Why it matters / when it applies
This doc is the cleanest standalone statement of *why* GitGalaxy bothers with a two-pass
manifest-then-content design at all, rather than just running the (more expensive) content-level
Language Lens scan on every file unconditionally: cheap, project-declared evidence collected once up
front lets the expensive per-file identity work trust a pre-computed prior instead of guessing from
scratch. The doc's Evidence Hierarchy section (Tier 1 `.gitattributes` at 0.99, Tier 2 manifest
entries at 0.95/0.85, Tier 3 sector bias/Makefile targets at 0.75/0.70) reproduces, in prose, the exact
confidence values the [GuideStar Protocol](../concepts/gitgalaxy-core-guidestar_lens.md) page already
cites to [`_inject_intent_lock`](../catalog/gitgalaxy/core/guidestar_lens.md#GuideStarLens._inject_intent_lock)/[`_inject_pattern_lock`](../catalog/gitgalaxy/core/guidestar_lens.md#GuideStarLens._inject_pattern_lock) —
useful confirmation that the doc and the code agree here, in contrast to the numbering/naming drift
found in the pipeline-overview and optical-orchestration docs (see [The optical pipeline
metaphor](optical-pipeline-metaphor.md)).

## Connections
- Code concepts: [The GuideStar Protocol](../concepts/gitgalaxy-core-guidestar_lens.md) — the deep page
  on `GuideStarLens`'s mechanism, evidence tiers, and the same Open Question this page resolves with a
  doc citation; [Language lens](../concepts/gitgalaxy-standards-language_lens.md) — the "Scientist" half
  of this handover, not previously cross-linked from the GuideStar concept page; [The Aperture
  Filter](../concepts/gitgalaxy-core-aperture.md) — the direct consumer of GuideStar's intent locks via
  its `has_intent` parameter.
- Module catalogs: [guidestar_lens](../catalog/gitgalaxy/core/guidestar_lens.md).
- Related doc-concepts: [optical-pipeline-metaphor](optical-pipeline-metaphor.md).

## Source
Extracted from `docs/wiki/02-04-guidestar-protocol.md`, kept in place.
