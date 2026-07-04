---
title: The optical pipeline metaphor — GalaxyScope as a telescope, not a scanner
type: doc-concept
provenance: doc
source: docs/wiki/02-01-pipeline-overview.md, docs/wiki/02-02-optical-orchestration.md
updated: 2026-07-04
status: fresh
---
# The optical pipeline metaphor — GalaxyScope as a telescope, not a scanner

## Definition
Both docs frame GitGalaxy's entire pipeline as a physical optical instrument rather than a
conventional "scanner": "Just as light flows through a telescope, data flows through our
GalaxyScope." Every stage gets an instrument name — aperture, guidestar, lens, prism, detector,
signal processor, auditor, recorder — and the `Orchestrator` class itself is cast as "the GalaxyScope
Chassis," the "physical chassis that houses and synchronizes every optical module." The docs are
explicit that the metaphor is meant to be generative, not decorative: "I hope this architecture
inspires people to build better versions of these things and view data analysis through the lens of
scientific instrumentation."

## In gitgalaxy (grounded)
The doc's module table maps one-to-one onto real modules already documented elsewhere in this silo,
but grounding it against the pinned source surfaces two places where the *doc's own names* have
drifted from the code:

| Doc's "optical" name | Doc's claimed module | Actual module / symbol |
| :--- | :--- | :--- |
| The Adaptive Light Path System | `galaxyscope.py` | [`Orchestrator`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator) — see [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) |
| The Aperture Filter | `aperture.py` | [`ApertureFilter`](../catalog/gitgalaxy/core/aperture.md#ApertureFilter) — see [The Aperture Filter](../concepts/gitgalaxy-core-aperture.md) |
| The GuideStar Protocol | `guidestar_lens.py` | [`GuideStarLens`](../catalog/gitgalaxy/core/guidestar_lens.md#GuideStarLens) — see [The GuideStar Protocol](../concepts/gitgalaxy-core-guidestar_lens.md) |
| The Language Lens | `language_lens.py` | see [Language lens](../concepts/gitgalaxy-standards-language_lens.md) |
| The Prism | `prism.py` | [`Prism.split_streams`](../catalog/gitgalaxy/core/prism.md#Prism.split_streams) — see [The Prism](../concepts/gitgalaxy-core-prism.md) |
| The Primary Detector | `detector.py` | [`StructuralExtractor.splice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.splice) — see [The Detector](../concepts/gitgalaxy-core-detector.md) |
| The Signal Processor | `signal_processor.py` | see [Signal Processor](../concepts/gitgalaxy-metrics-signal_processor.md) |
| **The Spectral Auditor** | **`spectral_auditor.py`** | no such file exists in the pinned source; the statistical Z-score auditor the doc describes is [`StatisticalAuditor.audit`](../catalog/gitgalaxy/metrics/statistical_auditor.md#StatisticalAuditor.audit) in `gitgalaxy/metrics/statistical_auditor.py` |
| The Chronometer | `chronometer.py` | see [Chronometer](../concepts/gitgalaxy-metrics-chronometer.md) |
| The Network Risk Sensor | `network_risk_sensor.py` | [`NetworkRiskSensor.build_dependency_graph`](../catalog/gitgalaxy/core/network_risk_sensor.md#NetworkRiskSensor.build_dependency_graph) |
| The Security Lens | `security_lens.py` | see [SecurityLens](../concepts/gitgalaxy-security-security_lens.md) |
| The AI AppSec Sensor | `ai_appsec_sensor.py` | [`AIAppSecSensor`](../catalog/gitgalaxy/tools/ai_guardrails/ai_appsec_sensor.md#AIAppSecSensor) in `gitgalaxy/tools/ai_guardrails/ai_appsec_sensor.py` — matches |
| The Dev Agent Firewall | `dev_agent_firewall.py` | [`DevAgentFirewall`](../catalog/gitgalaxy/tools/ai_guardrails/dev_agent_firewall.md#DevAgentFirewall) in `gitgalaxy/tools/ai_guardrails/dev_agent_firewall.py` — matches |
| **The Neural Auditor** | **`neural_auditor.py`** | no such file exists; the `.safetensors`/`.gguf` weight-inspection logic the doc describes is [`TensorScanner`](../catalog/gitgalaxy/metrics/tensor_scanner.md#TensorScanner) in `gitgalaxy/metrics/tensor_scanner.py`, invoked from within [`_calculate_risk_exposures`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator._calculate_risk_exposures) |
| The Security Auditor | `security_auditor.py` | see [SecurityAuditor](../concepts/gitgalaxy-security-security_auditor.md) |
| The Audit / Record / LLM / GPU Recorders | `audit_recorder.py` / `record_keeper.py` / `llm_recorder.py` / `gpu_recorder.py` | [`AuditRecorder.generate_report`](../catalog/gitgalaxy/recorders/audit_recorder.md#AuditRecorder.generate_report), [`RecordKeeper.record_mission`](../catalog/gitgalaxy/recorders/record_keeper.md#RecordKeeper.record_mission), [`LLMRecorder`](../catalog/gitgalaxy/recorders/llm_recorder.md#LLMRecorder), [`GPURecorder.record_mission`](../catalog/gitgalaxy/recorders/gpu_recorder.md#GPURecorder.record_mission) |

`spectral_auditor.py`/`neural_auditor.py` read as either stale filenames from an earlier refactor or
aspirational names that never matched a file on disk — either way, the doc's own module table is not
fully in sync with the pinned commit, in two out of nineteen rows.

The phase choreography in `02-02-optical-orchestration.md` shows the same kind of drift, one level
deeper. The doc numbers phases 0, 1, 1.5, 2, 3, 3.5, 4, 5, 6, 7.8, 8-9, and assigns **Phase 3** to
Network Topology and **Phase 7.8** to ML Threat Hunting. But [`execute_pipeline`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator.execute_pipeline)'s
*own* docstring — already quoted on the [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md)
page — states "Network Topology (Phase 4) is required before XGBoost Inference (Phase 9)," i.e. the
code's internal phase numbers for those same two stages are **4** and **9**, not 3 and 7.8. The two
numbering schemes agree on relative order (topology before ML inference) but disagree on the actual
phase indices, which suggests the doc's phase list was written or revised independently of the
docstring rather than generated from it. Neither the doc's Phase 2 "Domain Ontologies"/"Global Test
Umbrella" step nor its Phase 1.5 "Typosquatting Radar" have their own named symbol — both run inside
[`_resolve_dependency_graph`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator._resolve_dependency_graph)
(the Levenshtein-distance typosquat check) and
[`_calculate_risk_exposures`](../catalog/gitgalaxy/galaxyscope.md#Orchestrator._calculate_risk_exposures)
(the folder-level "Domain Ontologies" and "Global Test Umbrella" calculations) respectively, alongside
the risk-vector work those methods already do.

## Why it matters / when it applies
For this survey, the metaphor itself is the doc's real contribution — it's the maintainers' own
mental model for *why* the pipeline is a strict linear sequence of independent, swappable stages
("Just as different telescopes can have different lenses and prisms to see different things"), which
is the same hub-and-spoke, phase-ordered design the [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md)
page derives independently from the code's own docstrings. But the metaphor's *literal* module-name
and phase-number claims are exactly the kind of prose detail this project's grounding discipline
exists to check — and here checking them surfaces real drift between the docs and the pinned commit,
not just a difference in framing. That is itself a useful data point about heuristic/non-typed tools
in general: without a citation linter gating the docs the way this wiki's own finalizer gates its
synthesis, stale filenames and inconsistent phase numbers can ship in first-party documentation
undetected.

## Connections
- Code concepts: [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) — the `Orchestrator`
  this whole metaphor describes; [The Aperture Filter](../concepts/gitgalaxy-core-aperture.md),
  [The GuideStar Protocol](../concepts/gitgalaxy-core-guidestar_lens.md), [The Prism](../concepts/gitgalaxy-core-prism.md),
  [The Detector](../concepts/gitgalaxy-core-detector.md), [Signal Processor](../concepts/gitgalaxy-metrics-signal_processor.md),
  [Chronometer](../concepts/gitgalaxy-metrics-chronometer.md), [SecurityLens](../concepts/gitgalaxy-security-security_lens.md),
  [SecurityAuditor](../concepts/gitgalaxy-security-security_auditor.md), [Language lens](../concepts/gitgalaxy-standards-language_lens.md) —
  every stage the metaphor names.
- Module catalogs: [galaxyscope](../catalog/gitgalaxy/galaxyscope.md), [statistical_auditor](../catalog/gitgalaxy/metrics/statistical_auditor.md),
  [tensor_scanner](../catalog/gitgalaxy/metrics/tensor_scanner.md), [network_risk_sensor](../catalog/gitgalaxy/core/network_risk_sensor.md),
  [ai_appsec_sensor](../catalog/gitgalaxy/tools/ai_guardrails/ai_appsec_sensor.md), [dev_agent_firewall](../catalog/gitgalaxy/tools/ai_guardrails/dev_agent_firewall.md),
  [audit_recorder](../catalog/gitgalaxy/recorders/audit_recorder.md), [record_keeper](../catalog/gitgalaxy/recorders/record_keeper.md),
  [gpu_recorder](../catalog/gitgalaxy/recorders/gpu_recorder.md), [llm_recorder](../catalog/gitgalaxy/recorders/llm_recorder.md).
- Related doc-concepts: [blast-paradigm](blast-paradigm.md), [supernova-injection](supernova-injection.md),
  [delta-mission-vs-incremental-scan](delta-mission-vs-incremental-scan.md), [domain-dialect-patching](domain-dialect-patching.md),
  [neighborhood-micro-mass-quota](neighborhood-micro-mass-quota.md).

## Source
Extracted from `docs/wiki/02-01-pipeline-overview.md` and `docs/wiki/02-02-optical-orchestration.md`,
kept in place.
