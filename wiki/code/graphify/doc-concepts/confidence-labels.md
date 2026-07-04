---
title: Confidence labels and scores
type: doc-concept
provenance: doc
source: ARCHITECTURE.md
updated: 2026-07-04
status: fresh
---
# Confidence labels and scores

## Definition
Every edge in the graph carries one of three confidence labels so a reader always knows what was found versus guessed. `EXTRACTED` means the relationship is explicit in the source (an import, a direct call). `INFERRED` means it is a reasonable deduction (a call-graph second pass, co-occurrence), and it also carries a `confidence_score` (0.0–1.0). `AMBIGUOUS` means uncertain — flagged for human review in `GRAPH_REPORT.md`. EXTRACTED edges are always score 1.0; INFERRED edges use a discrete rubric (0.95 near-certain, 0.85 strong, 0.75 reasonable, 0.65 weak, 0.55 speculative).

## In graphify (grounded)
- The allowed label set is enforced at validation time by [`VALID_CONFIDENCES`](../catalog/graphify/validate.md#VALID_CONFIDENCES) inside [`validate_extraction`](../catalog/graphify/validate.md#validate_extraction).
- INFERRED `calls` edges are produced by the call-graph second pass [`walk_calls`](../catalog/graphify/extract.md#_extract_generic.walk_calls) and semantic reference edges via [`_semantic_reference_edge`](../catalog/graphify/extract.md#_semantic_reference_edge) in `extract.py`.
- Confidence flows into the report and export layers: the export path resolves per-edge scores against [`_CONFIDENCE_SCORE_DEFAULTS`](../catalog/graphify/export.md#_CONFIDENCE_SCORE_DEFAULTS) and picks a [`_dominant_confidence`](../catalog/graphify/export.md#to_obsidian._dominant_confidence); AMBIGUOUS edges are surfaced for review by [`generate`](../catalog/graphify/report.md#generate).

## Why it matters / when it applies
Confidence tagging is what keeps the graph honest as a comprehension aid: an agent (or human) reading a relationship can weight it, and the noisiest inferences are quarantined rather than presented as fact. It is the same EXTRACTED/INFERRED/AMBIGUOUS vocabulary that appears in the report's confidence tags.

## Connections
- Code concepts: [analyze](../concepts/graphify-analyze.md), [extract](../concepts/graphify-extract.md)
- Module catalogs: [validate](../catalog/graphify/validate.md), [extract](../catalog/graphify/extract.md), [export](../catalog/graphify/export.md), [report](../catalog/graphify/report.md)
- Related doc-concepts: [extraction-schema](extraction-schema.md), [god-nodes-report](god-nodes-report.md)

## Source
Extracted from `ARCHITECTURE.md` and `docs/how-it-works.md` (kept in place) — both document the same three-label scheme; the numeric rubric comes from `docs/how-it-works.md`.
