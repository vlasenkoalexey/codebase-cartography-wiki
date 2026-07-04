---
title: 'Module: tests/core_engine/test_aperture.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_aperture.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_aperture`/
symbols:
  test_aperture_gitignore_and_contraband: test_aperture_gitignore_and_contraband().
  filter_engine: filter_engine().
  MOCK_REGISTRY: MOCK_REGISTRY.
  MOCK_CONFIG: MOCK_CONFIG.
  test_aperture_lead_shield: test_aperture_lead_shield().
  test_aperture_semantic_path_and_intent: test_aperture_semantic_path_and_intent().
  test_aperture_auto_gen_shield: test_aperture_auto_gen_shield().
  test_aperture_embedded_hex_shield: test_aperture_embedded_hex_shield().
  test_aperture_infrared_saturation_gate: test_aperture_infrared_saturation_gate().
  test_aperture_system_guardrails: test_aperture_system_guardrails().
  test_aperture_binary_and_monolith_shields: test_aperture_binary_and_monolith_shields().
  test_aperture_machine_gen_and_monotony: test_aperture_machine_gen_and_monotony().
  test_aperture_declarative_blob_shield: test_aperture_declarative_blob_shield().
  test_aperture_comma_density_shield: test_aperture_comma_density_shield().
---
# Module: [`tests/core_engine/test_aperture.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py)

## Functions
- `filter_engine(tmp_path)` — [`L30`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L30) — Initializes the Aperture Filter with a temporary directory.
- `test_aperture_auto_gen_shield(filter_engine, tmp_path)` — [`L95`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L95) — Proves the engine detects machine-generated signatures and dynamically
- `test_aperture_binary_and_monolith_shields(filter_engine, tmp_path)` — [`L216`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L216) — Ensures opaque binaries (null bytes) and >30,000 LOC monoliths are blocked.
- `test_aperture_comma_density_shield(filter_engine, tmp_path)` — [`L297`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L297) — Proves that massive data arrays compiled into source code are detected
- `test_aperture_declarative_blob_shield(filter_engine, tmp_path)` — [`L270`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L270) — Ensures massive vector or declarative files are suppressed unless they
- `test_aperture_embedded_hex_shield(filter_engine, tmp_path)` — [`L134`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L134) — Proves that massive C-header data payloads (hex arrays) are dropped to protect
- `test_aperture_gitignore_and_contraband(tmp_path)` — [`L315`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L315) — Proves that the engine correctly loads .gitignore patterns at runtime and
- `test_aperture_infrared_saturation_gate(filter_engine, tmp_path)` — [`L158`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L158) — Proves that absurdly long lines of code (minified JS) are shunted to Infrared,
- `test_aperture_lead_shield(filter_engine, tmp_path)` — [`L42`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L42) — Proves that critical leaks and AI model weights bypass standard optical
- `test_aperture_machine_gen_and_monotony(filter_engine, tmp_path)` — [`L243`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L243) — Tests the engine's ability to identify machine-generated files via headers
- `test_aperture_semantic_path_and_intent(filter_engine, tmp_path)` — [`L67`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L67) — Proves that infrastructure paths (vendor/build/test) are blocked by default,
- `test_aperture_system_guardrails(filter_engine, tmp_path)` — [`L183`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L183) — Tests edge cases regarding OS-level errors and protocol violations.

## Module values
- `MOCK_CONFIG` — [`L18`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L18)
- `MOCK_REGISTRY` — [`L9`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_aperture.py#L9)

