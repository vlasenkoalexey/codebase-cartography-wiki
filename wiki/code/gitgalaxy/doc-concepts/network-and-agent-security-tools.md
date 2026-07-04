---
title: Network and AI-agent guardrail tools — Spokes that consume the Hub's own risk graph
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Network and AI-agent guardrail tools — Spokes that consume the Hub's own risk graph

## Definition
Three more README-listed tool clusters round out the "Enterprise Codebase Tools" suite: an "API
Security & Shadow API Detection" tool that "uses structural regex to find active physical routing
logic... and applies set theory against official OpenAPI/Swagger documentation to isolate critical
Shadow APIs and outdated Ghost APIs"; a "High-Speed PII Detection & Log Analysis" scanner that "hunts
and masks PII... and uses static architecture maps to prove exact runtime execution frequencies with
ASCII time-series histograms"; and "AI Agent Guardrails & Codebase Protection," which "evaluates
token mass and blast radius to restrict autonomous coding agents from modifying dangerous or
context-token-draining files."

## In gitgalaxy (grounded)
Each claim maps to a real function, and one of them is the clearest place in the repository where a
downstream Spoke literally reads the Hub's own graph-derived metrics:
- **Shadow/Ghost API detection is literal set difference.** [`map_physical_codebase`](../catalog/gitgalaxy/tools/network_auditing/full_api_network_map.md#map_physical_codebase)
  extracts routing endpoints from source, [`parse_official_swagger`](../catalog/gitgalaxy/tools/network_auditing/full_api_network_map.md#parse_official_swagger)
  (fed by [`auto_discover_swagger`](../catalog/gitgalaxy/tools/network_auditing/full_api_network_map.md#auto_discover_swagger))
  extracts the documented set, and `main`'s own logic is exactly `shadow_apis = physical_endpoints -
  approved_apis` / `ghost_apis = approved_apis - physical_endpoints` — plain Python set arithmetic, not
  a metaphor for "set theory." [`run_api_audit`](../catalog/gitgalaxy/tools/network_auditing/full_api_network_map.md#run_api_audit)
  (already cited from [the COBOL Refractor Controller page](../concepts/gitgalaxy-cobol_refractor_controller.md))
  is the library entry point `Orchestrator.execute_pipeline`'s Phase 10 calls.
- **PII masking and the histogram are both real, separate functions.** [`mask_pii`](../catalog/gitgalaxy/tools/terabyte_log_scanning/pii_leak_hunter.md#mask_pii)
  is the masking pass; [`draw_ascii_histogram`](../catalog/gitgalaxy/tools/terabyte_log_scanning/pii_leak_hunter.md#draw_ascii_histogram)
  is, specifically, the function behind the README's "ASCII time-series histograms" line — the claim
  names a real, separately-testable function rather than a generic logging feature.
- **The AI-agent firewall reads the dependency graph's own PageRank output.** [`DevAgentFirewall.evaluate_ecosystem`](../catalog/gitgalaxy/tools/ai_guardrails/dev_agent_firewall.md#DevAgentFirewall.evaluate_ecosystem)
  pulls `token_mass` and `network_metrics["normalized_blast_radius"]` — the exact field
  `NetworkRiskSensor.build_dependency_graph` (see [structural-rag-graph](structural-rag-graph.md))
  writes as `pagerank * 1000` — straight out of each file's `telemetry` dict to decide which files an
  autonomous coding agent should be restricted from touching. This is the one place in the codebase
  where "blast radius" is not just a report column; a downstream tool makes a live decision from it.
- **A separate sensor, not the same class, watches for AI-specific weaponization.** [`AIAppSecSensor.hunt_threats`](../catalog/gitgalaxy/tools/ai_guardrails/ai_appsec_sensor.md#AIAppSecSensor.hunt_threats)
  reads `ai_orchestrator`/`llm_api`/`ai_tools` telemetry counts to flag "Autonomous Execution Vectors"
  — a distinct class from `DevAgentFirewall`, despite the README bundling both under one "AI Agent
  Guardrails" heading.

## Why it matters / when it applies
`DevAgentFirewall.evaluate_ecosystem` is the strongest evidence in this survey's gitgalaxy silo that
the Hub-and-Spoke architecture (`docs/wiki/01-01-project-overview.md` §1.3) is a real data dependency,
not just an org-chart metaphor: a Spoke tool's safety decision is a direct function of a metric the
Hub's `NetworkRiskSensor` graph computed. It also grounds a specific README claim — "evaluates token
mass and blast radius" — down to the exact two dict keys the code reads, which is a stronger check
than most of this doc's more general performance/scale claims allow.

## Connections
- Code concepts: none of these three tools has its own code-concept page yet in this silo; the
  closest existing pages are [The Aperture Filter](../concepts/gitgalaxy-core-aperture.md) (the file
  gate every scan shares) and [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) (Phase
  10, where `run_api_audit` is wired in).
- Module catalogs: no catalog page yet exists for `tools/network_auditing/full_api_network_map.py`,
  `tools/terabyte_log_scanning/pii_leak_hunter.py`, or `tools/ai_guardrails/*.py`; the symbols cited
  above are read directly from source.
- Related doc-concepts: [structural-rag-graph](structural-rag-graph.md) — the `NetworkRiskSensor`
  graph `DevAgentFirewall` consumes; [supply-chain-and-compliance-tools](supply-chain-and-compliance-tools.md) —
  the sibling tool cluster (SBOM, firewall, X-Ray, vault sentinel).

## Source
Extracted from `README.md` §"Enterprise Codebase Tools & Use Cases" (kept in place).
