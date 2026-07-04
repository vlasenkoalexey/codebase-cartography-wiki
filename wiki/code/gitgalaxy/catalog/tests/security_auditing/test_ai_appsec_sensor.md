---
title: 'Module: tests/security_auditing/test_ai_appsec_sensor.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_ai_appsec_sensor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_ai_appsec_sensor`/test_
symbols:
  test_autonomous_execution_vector_detection: autonomous_execution_vector_detection().
  test_over_permissioned_agent_detection: over_permissioned_agent_detection().
  test_exfiltration_vector_detection: exfiltration_vector_detection().
  test_safe_baseline: safe_baseline().
---
# Module: [`tests/security_auditing/test_ai_appsec_sensor.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_ai_appsec_sensor.py)

## Functions
- `test_autonomous_execution_vector_detection()` — [`L8`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_ai_appsec_sensor.py#L8) — Proves that an LLM directly wired to OS execution (eval/subprocess)
- `test_exfiltration_vector_detection()` — [`L69`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_ai_appsec_sensor.py#L69) — Proves that an LLM with access to both raw network sockets and hardcoded
- `test_over_permissioned_agent_detection()` — [`L38`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_ai_appsec_sensor.py#L38) — Proves that an AI agent given autonomous tools, write-access to complex
- `test_safe_baseline()` — [`L101`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_ai_appsec_sensor.py#L101) — Proves that a properly sandboxed AI integration (e.g., an LLM script with

