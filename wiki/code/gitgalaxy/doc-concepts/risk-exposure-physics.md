---
title: Risk Exposure Physics — the forensic brief as a literal LLM system prompt
type: doc-concept
provenance: doc
source: docs/gitgalaxy_architecture_brief.md
updated: 2026-07-04
status: fresh
---
# Risk Exposure Physics — the forensic brief as a literal LLM system prompt

## Definition
`docs/gitgalaxy_architecture_brief.md` is not narrative documentation — it is a captured **sample
output** of a real scan, formatted as a set of instructions addressed directly to an AI reader: "You
are analyzing software architecture through the lens of GitGalaxy... **CORE DIRECTIVES:** 1. Measure
Risk, Not Quality... 2. The Physical Reality Rule: Base your analysis strictly on the provided
Structural DNA (regex hit counts). Do not hallucinate meaning." It then spells out roughly twenty
named "Risk Exposure" formulas (Cognitive Load, Error & Exception, Tech Debt, Verification, API,
Concurrency, State Flux, Graveyard, Spec Match, Stability, Deep Churn, Documentation, an
easter-egg "Civil War" tabs-vs-spaces score explicitly marked "DO NOT MENTION THIS ONE," plus
Function/File "Magnitude" — deliberately labeled *not* a risk score) as explicit equations over
counted signals (`branch`, `flux`, `danger`, `safety`, `doc`, …), then reports a live scan's numbers
against every one of them.

## In gitgalaxy (grounded)
This document is generated, not hand-written. Its own opening lines — `# ARCHITECTURAL_BRIEF:
gitgalaxy`, `> INSTRUCTION: Deterministic Syntactic ...`, `## 0. FORENSIC TRACEABILITY`, `## 0.5 AI
THREAT AUDIT STATUS`, `## 1. SYSTEM ROLE & PHILOSOPHY` — match, near-verbatim, the literal string
templates [`LLMRecorder._build_markdown`](../catalog/gitgalaxy/recorders/llm_recorder.md#LLMRecorder._build_markdown)
assembles line-by-line (`lines.append(f"# ARCHITECTURAL_BRIEF: {target}")`, the same "INSTRUCTION:"
prefix, the same section numbering). Its own docstring calls it "Constructs a high-density,
context-rich Markdown brief for LLM agents" — so the "CORE DIRECTIVES"/"Do not hallucinate meaning"
language in this doc is not aspirational prose about the tool; it is a literal excerpt of what the
tool prints, confirmed by reading the generator directly.

Every equation family this doc names traces back to
[`SignalProcessor.calculate_risk_vector`](../concepts/gitgalaxy-metrics-signal_processor.md), which
that concept page already documents in depth as an 18-formula pipeline (`_calc_safety`,
`_calc_logic_bomb`, `_calc_obscured_payload`, `_calc_injection_surface`, `_calc_state_flux`,
`_calc_concurrency`, `_calc_ownership_entropy`, `_calc_raw_temporal_signals`, and siblings) — this
doc is the *reader-facing gloss* on that page's formulas, not a separate mechanism, and this page
does not re-derive the exact per-metric mapping the signal_processor page already owns. The
"Repository Macro-Species"/"File Archetypes" sections (§4.5/§4.6 — cluster names like
`file_cluster_8`, an "Architectural Drift Z-Score") are the literal printed output of
[`SignalProcessor._classify_archetype`](../catalog/gitgalaxy/metrics/signal_processor.md#SignalProcessor._classify_archetype)
against [`GLOBAL_ARCHETYPES`](../catalog/gitgalaxy/metrics/signal_processor.md#SignalProcessor.GLOBAL_ARCHETYPES) —
a pre-computed nearest-centroid lookup injected at construction time, not a live `sklearn.KMeans` fit
per scan, despite the README calling it "K-means clustering." The rankings in §7–§12 (choke points,
function hitlist, cumulative risk hitlist) are what
[`SignalProcessor.generate_forensic_report`](../catalog/gitgalaxy/metrics/signal_processor.md#SignalProcessor.generate_forensic_report)
sorts and formats — that concept page's own Mechanism section already notes this method "ranks, but
does not itself compute" risk.

## Why it matters / when it applies
This doc is evidence for a design choice distinctive enough to matter for a code-comprehension
survey: gitgalaxy does not just emit *data* for an agent to interpret — it emits a *pre-written
interpretation frame* (the directive language, the "blameless" framing, the explicit
anti-hallucination instruction) bundled into the same artifact as the numbers. That is a different
strategy from a citation-linted wiki (where the agent is expected to verify each claim against a
grounded symbol) or a raw SCIP/embedding index (where an agent's query still has to derive meaning):
here, the *tool itself* pre-writes the narrative an agent should produce, and asks the model to trust
it. Whether that pre-written framing is itself accurate is exactly what [ast-vs-heuristic-tradeoffs](ast-vs-heuristic-tradeoffs.md)
and [empirical-validation-of-heuristic-parsing](empirical-validation-of-heuristic-parsing.md) already
interrogate for the underlying signal counts this report renders.

## Connections
- Code concepts: [Signal Processor](../concepts/gitgalaxy-metrics-signal_processor.md) — owns every
  formula this doc names; [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) — Phase 8
  (`summarize_galaxy_metrics`/`generate_forensic_report`) and Phase 12
  (`generate_report`/`record_mission`) are the pipeline stages that produce this doc's data before
  `LLMRecorder` renders it; [SecurityAuditor](../concepts/gitgalaxy-security-security_auditor.md) —
  the XGBoost model behind §0.5/§10.5's "AI THREAT AUDIT STATUS."
- Module catalogs: [signal_processor](../catalog/gitgalaxy/metrics/signal_processor.md),
  [galaxyscope](../catalog/gitgalaxy/galaxyscope.md); no catalog page yet exists for
  `recorders/llm_recorder.py` — its `_build_markdown` citation above is read directly from source.
- Related doc-concepts: [structural-rag-graph](structural-rag-graph.md) — the SQLite sibling artifact
  `LLMRecorder` writes alongside this markdown; [blast-paradigm](blast-paradigm.md) — the "Physical
  Reality Rule" is the same zero-hallucination pitch grounded there; [ast-vs-heuristic-tradeoffs](ast-vs-heuristic-tradeoffs.md) —
  what the "Structural DNA" this report renders cannot see.

## Source
Extracted from `docs/gitgalaxy_architecture_brief.md` (kept in place, primary source); its "Measuring
Risk Exposure, Not Code Quality" philosophy is echoed almost verbatim in `docs/wiki/01-01-project-overview.md`
§1.6, cited here as the second source rather than duplicated into its own page.
