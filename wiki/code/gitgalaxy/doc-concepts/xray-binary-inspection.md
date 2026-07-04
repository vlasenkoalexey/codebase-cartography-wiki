---
title: The X-Ray Binary Sensor — 8KB header/entropy triage, described as part of the Aperture Filter
type: doc-concept
provenance: doc
source: docs/wiki/02-03-aperture-filter.md
updated: 2026-07-04
status: fresh
---
# The X-Ray Binary Sensor — 8KB header/entropy triage, described as part of the Aperture Filter

## Definition
`02-03-aperture-filter.md` describes an "X-Ray Binary Sensor" as one of the Aperture Filter's own
capabilities: "When a file is flagged as a binary or blacklisted asset, it isn't simply discarded. The
X-Ray sensor intercepts the first 8KB of the payload and scans for embedded execution headers, magic
byte mismatches, or extreme cryptographic entropy. If the binary is weaponized or contains AI model
weights, it is promoted to a 'Supernova' on the 3D map. If it is inert, it is relegated to Dark
Matter." The doc's Data Classification Matrix lists this under the same table as the rest of the
Aperture Filter's Wavelength categories.

## In gitgalaxy (grounded)
No 8KB-read, magic-byte, or entropy logic exists in `gitgalaxy/core/aperture.py` — a direct search of
that file for these terms comes up empty. The described behavior is real, but it lives in a separate,
independently-invocable security tool: [`run_xray_audit`](../catalog/gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.md#run_xray_audit)
and its standalone [`main`](../catalog/gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.md#main)
in `gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.py`. Both functions read "only the
first 8KB of the file" (`f.read(8192)`) — matching the doc's number exactly — specifically, per that
file's own comment, because "this is sufficient to capture magic bytes, execution headers, and enough
string data for an accurate entropy calculation, completely preventing Out-Of-Memory (OOM) crashes on
huge files." The module's own CLI banner even uses the doc's language verbatim: "Binary Anomaly
Detector: Entropy & Magic Byte Scanner." Shannon entropy above `4.8` is the threshold that flags a
payload as "mathematically dense/encrypted." This is the tool the [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md)
page's Phase 10 already documents `run_xray_audit` being called from as one of three independently
importable security audits `execute_pipeline` runs as plain library functions.

So the doc's placement of "X-Ray Binary Sensor" inside the Aperture Filter chapter is a framing choice,
not a code fact: [`ApertureFilter`](../concepts/gitgalaxy-core-aperture.md) is what decides a file is
`binary_payload`/blacklisted in the first place, but the actual X-ray header/entropy inspection the
doc describes is a downstream, separately-run audit over files the Aperture Filter (or a standalone
CLI invocation) has already flagged — the two modules are sequential collaborators, not one class.

## Why it matters / when it applies
This is a case where the doc's organizing metaphor (grouping every triage decision under "the
telescope's filters") is a reasonable narrative simplification but obscures a real module boundary: a
reader trying to find "the X-Ray sensor" in `aperture.py` will not find it there. It also connects
directly to [supernova-injection](supernova-injection.md): the promotion described here ("promoted to
a 'Supernova'... if inert, relegated to Dark Matter") is the same force-onto-the-map pattern that page
documents for the Aperture Filter's own secrets shunt — this doc-concept is the grounding for the
"X-Ray Anomalies" row of that pattern specifically.

## Connections
- Code concepts: [The Aperture Filter](../concepts/gitgalaxy-core-aperture.md) — decides a file is
  binary/blacklisted before this sensor ever runs; [GalaxyScope orchestrator](../concepts/gitgalaxy-galaxyscope.md) —
  Phase 10 calls `run_xray_audit` as one of three ecosystem security audits.
- Module catalogs: [binary_anomaly_detector](../catalog/gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.md),
  [aperture](../catalog/gitgalaxy/core/aperture.md).
- Related doc-concepts: [supernova-injection](supernova-injection.md), [optical-pipeline-metaphor](optical-pipeline-metaphor.md).

## Source
Extracted from `docs/wiki/02-03-aperture-filter.md`, kept in place.
