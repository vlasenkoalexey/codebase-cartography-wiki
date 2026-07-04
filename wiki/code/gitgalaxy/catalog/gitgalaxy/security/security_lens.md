---
title: 'Module: gitgalaxy/security/security_lens.py'
type: catalog
provenance: extracted
module: gitgalaxy/security/security_lens.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.security.security_lens`/SecurityLens#
symbols:
  SecurityLens: ''
  SecurityLens.scan_content: scan_content().
  SecurityLens.THREAT_SIGNATURES: THREAT_SIGNATURES.
  SecurityLens.scan_binary: scan_binary().
  SecurityLens.policy: policy.
  SecurityLens.evaluate_risk: evaluate_risk().
  SecurityLens.string_extractor: string_extractor.
  SecurityLens.auto_gen_shield: auto_gen_shield.
  SecurityLens.MAGIC_BYTES: MAGIC_BYTES.
  SecurityLens.THREAT_HEADERS: THREAT_HEADERS.
  SecurityLens._calculate_shannon_entropy: _calculate_shannon_entropy().
  SecurityLens.__init__: __init__().
---
# Module: [`gitgalaxy/security/security_lens.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py)

## Classes
### `SecurityLens`
- def: [`gitgalaxy/security/security_lens.py:16`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L16) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
- doc: Static Application Security Testing (SAST) Engine.
- signature: `class SecurityLens:`
- members:
  - `_calculate_shannon_entropy(self, data: str)` — [`L183`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L183) — Calculates the Shannon Entropy of a string to identify base64/encrypted blobs. — documented in [gitgalaxy-security-security_lens](../../../concepts/gitgalaxy-security-security_lens.md)
  - `evaluate_risk(self, aggregated_hits, total_loc, network_metrics=None)` — [`L363`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L363) — Evaluates vulnerability risk with Network Centrality awareness.
  - `scan_binary(self, raw_bytes: bytes, ext: str)` — [`L430`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L430) — Binary Magic Byte & Entropy Analyzer. — documented in [gitgalaxy-security-security_lens](../../../concepts/gitgalaxy-security-security_lens.md)
  - `scan_content(self, content: str, loc: int)` — [`L198`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L198) — Executes primary regex scanning, entropy calculation, and multi-line data flow taint tracking. — documented in [gitgalaxy-security-security_lens](../../../concepts/gitgalaxy-security-security_lens.md)
  - `MAGIC_BYTES` — [`L51`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L51) — documented in [gitgalaxy-security-security_lens](../../../concepts/gitgalaxy-security-security_lens.md)
  - `THREAT_HEADERS` — [`L61`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L61) — documented in [gitgalaxy-security-security_lens](../../../concepts/gitgalaxy-security-security_lens.md)
  - `THREAT_SIGNATURES` — [`L72`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L72) — documented in [gitgalaxy-security-security_lens](../../../concepts/gitgalaxy-security-security_lens.md)
  - `auto_gen_shield` — [`L44`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L44) — documented in [gitgalaxy-security-security_lens](../../../concepts/gitgalaxy-security-security_lens.md)
  - `policy` — [`L29`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L29)
  - `string_extractor` — [`L40`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L40) — documented in [gitgalaxy-security-security_lens](../../../concepts/gitgalaxy-security-security_lens.md)
- protocol/private: `__init__`[`L25`](../../../../../../raw/code/gitgalaxy/gitgalaxy/security/security_lens.py#L25)
- used by: [`main`](../tools/supply_chain_security/vault_sentinel.md#main), [`main`](../tools/supply_chain_security/binary_anomaly_detector.md#main), [`main`](../tools/compliance/sbom_generator.md#main), [`run_xray_audit`](../tools/supply_chain_security/binary_anomaly_detector.md#run_xray_audit), [`_init_worker`](../galaxyscope.md#_init_worker), [`run_firewall_audit`](../tools/supply_chain_security/supply_chain_firewall.md#run_firewall_audit), [`security_analyzer`](../galaxyscope.md#Orchestrator.security_analyzer)  (1 test-only)

