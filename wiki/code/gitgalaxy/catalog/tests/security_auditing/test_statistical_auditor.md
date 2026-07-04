---
title: 'Module: tests/security_auditing/test_statistical_auditor.py'
type: catalog
provenance: extracted
module: tests/security_auditing/test_statistical_auditor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.security_auditing.test_statistical_auditor`/
symbols:
  auditor: auditor().
  test_auditor_consensus_engine: test_auditor_consensus_engine().
  test_auditor_c_family_header_fallback: test_auditor_c_family_header_fallback().
  MOCK_LANG_DEFS: MOCK_LANG_DEFS.
  test_auditor_zero_density_threshold: test_auditor_zero_density_threshold().
  test_auditor_packed_payload_guard: test_auditor_packed_payload_guard().
  test_auditor_threat_quarantine_guard: test_auditor_threat_quarantine_guard().
  test_auditor_low_sample_threshold_guard: test_auditor_low_sample_threshold_guard().
  test_auditor_dead_code_bypass: test_auditor_dead_code_bypass().
  test_auditor_statistical_mad_outliers: test_auditor_statistical_mad_outliers().
  test_auditor_inert_data_bypass: test_auditor_inert_data_bypass().
---
# Module: [`tests/security_auditing/test_statistical_auditor.py`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py)

## Functions
- `auditor()` — [`L26`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L26) — Initializes the Statistical Auditor with controlled definitions.
- `test_auditor_c_family_header_fallback(auditor)` — [`L255`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L255) — Proves that if an ambiguous header file (.h) lacks a direct 80% consensus match,
- `test_auditor_consensus_engine(auditor)` — [`L34`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L34) — Proves that the engine uses the ecosystem's confident files to rescue
- `test_auditor_dead_code_bypass(auditor)` — [`L188`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L188) — Proves that a file heavily weighted with comments/dead code that triggers
- `test_auditor_inert_data_bypass(auditor)` — [`L288`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L288) — Proves that data formats with no active logic signals (like JSON)
- `test_auditor_low_sample_threshold_guard(auditor)` — [`L157`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L157) — Proves that a tiny population (1 file) with a weak confidence tier gets
- `test_auditor_packed_payload_guard(auditor)` — [`L102`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L102) — Proves that a file with >3.0 signals per line is relegated as obscured noise.
- `test_auditor_statistical_mad_outliers(auditor)` — [`L214`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L214) — Creates a mathematically significant population (N=50) to build a baseline,
- `test_auditor_threat_quarantine_guard(auditor)` — [`L129`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L129) — Proves that a file failing the Zero-Density Threshold is forcefully saved onto the map
- `test_auditor_zero_density_threshold(auditor)` — [`L73`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L73) — Proves that a massive file with 0 structural logic is relegated to the Exclusion Queue,

## Module values
- `MOCK_LANG_DEFS` — [`L13`](../../../../../../raw/code/gitgalaxy/tests/security_auditing/test_statistical_auditor.py#L13)

