---
title: "\"Delta Missions\" vs. execute_incremental_scan — a doc claim the code contradicts"
type: doc-concept
provenance: doc
source: docs/wiki/02-02-optical-orchestration.md
updated: 2026-07-04
status: fresh
---
# "Delta Missions" vs. execute_incremental_scan — a doc claim the code contradicts

## Definition
`02-02-optical-orchestration.md` states, in the present tense and without qualification: "For rapid
continuous integration, the GalaxyScope supports `execute_delta_mission`. Rather than re-scanning tens
of thousands of files, the chassis rehydrates the previous scan's state directly into RAM, surgically
processes only the added/modified files through the Optical Pipeline (Pass 1), and then instantly
recalculates the entire Network Graph and ML Inference (Passes 2-7) in a fraction of the time." This
reads as a shipped, CI-friendly incremental-rescan feature.

## In gitgalaxy (grounded)
Two things are wrong with this claim as stated, both verifiable directly against the pinned source:

1. **The method is misnamed.** No symbol called `execute_delta_mission` exists anywhere in
   `galaxyscope.py` or the rest of the pinned repository. The method that actually implements the
   behavior the doc describes is [`execute_incremental_scan`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator.execute_incremental_scan) —
   different name, same described mechanism (evict changed entries from `ram_cache`, re-extract only
   the changed set, then recompute dependency/network/risk globally over the surviving cache).
2. **It is not reachable.** The [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) page's
   Open Questions section documents, from a repo-wide search of both production source and tests, that
   [`execute_incremental_scan`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator.execute_incremental_scan)
   has **no call site anywhere in this codebase** — [`main`](../catalog/gitgalaxy/galaxyscope.md#main)
   parses no CLI flag that routes to it, and no test exercises it. Its own body does not compute a git
   diff; it receives `added`/`modified`/`deleted` as plain arguments from an external caller that,
   per that page's finding, does not exist in this repository. The method is fully implemented — the
   doc's mechanism description is accurate to what the code *would do if called* — but as of this
   pinned commit it is dead scaffolding, not a supported, invokable feature.

Even taken as a description of the method's own logic (setting aside reachability), the doc's "instant"
framing is itself an overstatement the code's own docstring pushes back on: per the orchestrator page,
`execute_incremental_scan` still "re-runs [`_resolve_dependency_graph`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator._resolve_dependency_graph),
[`build_dependency_graph`](../catalog/gitgalaxy/core/network_risk_sensor.md#NetworkRiskSensor.build_dependency_graph),
and the risk/network recompute over the *entire* surviving `ram_cache`" — its own docstring calls this
the "Ripple Effect." So even in the counterfactual where it were wired to a caller, only file
*extraction* (Pass 1) is surgical; graph/risk recomputation (the doc's "Passes 2-7") is still
whole-repository, not incremental, work.

## Why it matters / when it applies
This is a concrete, source-verifiable contradiction between what gitgalaxy's own documentation claims
is a shipped capability and what a repo-wide search of the pinned commit shows is actually reachable —
exactly the kind of claim this wiki's grounding discipline exists to catch rather than silently repeat.
For a user deciding whether gitgalaxy fits a CI/CD incremental-scan use case, the accurate answer (per
this pinned commit) is: no, despite the doc's "the GalaxyScope supports `execute_delta_mission`"
framing, there is no supported way to invoke it — a full [`execute_pipeline`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator.execute_pipeline)
run is the only reachable path in this version. It also matters for cross-tool comparison in this
survey: unlike wikify-repo's `ingest --ref`-driven delta rebuild or graphify's content-addressed
incremental cache — both wired, reachable code paths — gitgalaxy has no working equivalent, despite
first-party documentation describing one in the present tense.

## Connections
- Code concepts: [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) — the page whose Open
  Questions section this finding is grounded in.
- Module catalogs: [galaxyscope](../catalog/gitgalaxy/galaxyscope.md), [network_risk_sensor](../catalog/gitgalaxy/core/network_risk_sensor.md).
- Related doc-concepts: [optical-pipeline-metaphor](optical-pipeline-metaphor.md) — the same doc's other
  claims about phase numbering and module names, checked the same way.

## Source
Extracted from `docs/wiki/02-02-optical-orchestration.md`, kept in place.
