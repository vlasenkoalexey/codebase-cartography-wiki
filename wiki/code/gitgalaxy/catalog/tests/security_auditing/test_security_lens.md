---
title: 'Module: tests/security_auditing/test_security_lens.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_security_lens.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_security_lens`/
symbols:
  lens: lens().
  test_sast_vulnerability_signatures: test_sast_vulnerability_signatures().
  test_obfuscation_entropy_detection: test_obfuscation_entropy_detection().
  test_data_flow_taint_tracking: test_data_flow_taint_tracking().
  test_auto_gen_shield_bypasses: test_auto_gen_shield_bypasses().
  test_evaluate_risk_network_centrality: test_evaluate_risk_network_centrality().
  test_evaluate_risk_prompt_injection_isolation: test_evaluate_risk_prompt_injection_isolation().
  test_binary_magic_byte_scanner: test_binary_magic_byte_scanner().
  test_comprehensive_risk_evaluation_coverage: test_comprehensive_risk_evaluation_coverage().
---
# Module: [`tests/security_auditing/test_security_lens.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_lens.py)

## Functions
- `lens()` — [`L9`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_lens.py#L9) — Initializes the Security Lens with default policy thresholds. — documented in [gitgalaxy-security-security_lens](../../../concepts/gitgalaxy-security-security_lens.md)
- `test_auto_gen_shield_bypasses(lens)` — [`L113`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_lens.py#L113) — Proves that machine generated code bypasses taint tracking and homoglyph
- `test_binary_magic_byte_scanner(lens)` — [`L186`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_lens.py#L186) — Proves the X-Ray scanner detects Magic Byte mismatches, embedded execution
- `test_comprehensive_risk_evaluation_coverage(lens)` — [`L214`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_lens.py#L214) — Triggers every remaining catastrophic threshold, empty state fallback,
- `test_data_flow_taint_tracking(lens)` — [`L74`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_lens.py#L74) — Proves the engine can track multi-line taint from I/O sinks to execution
- `test_evaluate_risk_network_centrality(lens)` — [`L141`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_lens.py#L141) — Proves the Network Centrality multiplier correctly amplifies threshold policies
- `test_evaluate_risk_prompt_injection_isolation(lens)` — [`L166`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_lens.py#L166) — Proves that Prompt Injections that do NOT result in RCE are scored independently,
- `test_obfuscation_entropy_detection(lens)` — [`L52`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_lens.py#L52) — Proves the string extractor drops small strings but accurately calculates
- `test_sast_vulnerability_signatures(lens)` — [`L17`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_security_lens.py#L17) — Proves the engine detects specific logic bombs, steganographic imports, prototype

