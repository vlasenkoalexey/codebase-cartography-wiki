---
title: 'Module: tests/security_auditing/test_sbom_generator.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_sbom_generator.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_sbom_generator`/test_
symbols:
  test_universal_manifest_slicer_all_ecosystems: universal_manifest_slicer_all_ecosystems().
  test_locate_physical_package: locate_physical_package().
  test_zero_trust_sbom_generation_anomalies: zero_trust_sbom_generation_anomalies().
  test_sbom_generator_system_exits: sbom_generator_system_exits().
  test_zero_trust_sbom_clean_run: zero_trust_sbom_clean_run().
  test_zero_trust_sbom_generation_anomalies.conditional_open: zero_trust_sbom_generation_anomalies().conditional_open().
---
# Module: [`tests/security_auditing/test_sbom_generator.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_sbom_generator.py)

## Functions
- `conditional_open(file, *args, **kwargs)` — [`L193`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_sbom_generator.py#L193)
- `test_locate_physical_package(tmp_path)` — [`L94`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_sbom_generator.py#L94) — Proves the physical cartography logic accurately hunts down packages based on ecosystem norms.
- `test_sbom_generator_system_exits(tmp_path)` — [`L136`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_sbom_generator.py#L136) — Proves the orchestrator aborts gracefully if the target is invalid or empty.
- `test_universal_manifest_slicer_all_ecosystems(tmp_path)` — [`L12`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_sbom_generator.py#L12) — Proves regex and parsing logic flawlessly extracts dependencies across all 7 supported ecosystems.
- `test_zero_trust_sbom_clean_run(mock_detector_class, mock_security_class, tmp_path)` — [`L231`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_sbom_generator.py#L231) — Proves the generator successfully outputs a VERIFIED_SAFE SBOM status.
- `test_zero_trust_sbom_generation_anomalies(mock_detector_class, mock_security_class, tmp_path)` — [`L159`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_sbom_generator.py#L159) — Proves the physical audit detects malware, missing files, and survives OS exceptions.

