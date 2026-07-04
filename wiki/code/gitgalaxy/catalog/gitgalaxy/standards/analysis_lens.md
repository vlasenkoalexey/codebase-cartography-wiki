---
title: 'Module: gitgalaxy/standards/analysis_lens.py'
type: catalog
provenance: extracted
module: gitgalaxy/standards/analysis_lens.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.standards.analysis_lens`/
symbols:
  ThreatPolicy: ThreatPolicy#
  ThreatPolicy.get_policy: ThreatPolicy#get_policy().
  RECORDING_SCHEMAS: RECORDING_SCHEMAS.
  AI_THREAT_THRESHOLD: AI_THREAT_THRESHOLD.
  ThreatPolicy.PROFILES: ThreatPolicy#PROFILES.
  ASSET_MASKS: ASSET_MASKS.
  PATH_MODIFIERS: PATH_MODIFIERS.
  ENGINE_CONSTANTS: ENGINE_CONSTANTS.
  FIDELITY_TIERS: FIDELITY_TIERS.
  RISK_EQUATION_TUNING: RISK_EQUATION_TUNING.
  LANGUAGE_SECURITY_PROFILES: LANGUAGE_SECURITY_PROFILES.
  GENERAL_FUNCTION_INFERENCE_MODEL: GENERAL_FUNCTION_INFERENCE_MODEL.
  GENERAL_FILE_INFERENCE_MODEL: GENERAL_FILE_INFERENCE_MODEL.
  SPECIFIC_FILE_INFERENCE_MODEL: SPECIFIC_FILE_INFERENCE_MODEL.
  GENERAL_REPO_INFERENCE_MODEL: GENERAL_REPO_INFERENCE_MODEL.
---
# Module: [`gitgalaxy/standards/analysis_lens.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py)

## Classes
### `ThreatPolicy`
- def: [`gitgalaxy/standards/analysis_lens.py:31`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L31) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
- doc: Defines the threshold at which a structural anomaly becomes a critical threat.
- signature: `class ThreatPolicy:`
- members:
  - `get_policy(mode="baseline")` — [`L54`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L54) — Returns the specific threat thresholds based on the deployment mode. — documented in [gitgalaxy-standards-analysis_lens](../../../concepts/gitgalaxy-standards-analysis_lens.md)
  - `PROFILES` — [`L34`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L34) — documented in [gitgalaxy-standards-analysis_lens](../../../concepts/gitgalaxy-standards-analysis_lens.md)
- used by: [`main`](../tools/supply_chain_security/vault_sentinel.md#main), [`main`](../tools/compliance/sbom_generator.md#main), [`main`](../galaxyscope.md#main), [`_init_worker`](../galaxyscope.md#_init_worker), [`run_firewall_audit`](../tools/supply_chain_security/supply_chain_firewall.md#run_firewall_audit), [`db_recorder`](../galaxyscope.md#Orchestrator.db_recorder)

## Module values
- `AI_THREAT_THRESHOLD` — [`L28`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L28) — documented in [gitgalaxy-standards-analysis_lens](../../../concepts/gitgalaxy-standards-analysis_lens.md)
- `ASSET_MASKS` — [`L123`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L123)
- `ENGINE_CONSTANTS` — [`L63`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L63)
- `FIDELITY_TIERS` — [`L77`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L77)
- `GENERAL_FILE_INFERENCE_MODEL` — [`L2235`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L2235)
- `GENERAL_FUNCTION_INFERENCE_MODEL` — [`L1333`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L1333)
- `GENERAL_REPO_INFERENCE_MODEL` — [`L8176`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L8176)
- `LANGUAGE_SECURITY_PROFILES` — [`L860`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L860)
- `PATH_MODIFIERS` — [`L250`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L250)
- `RECORDING_SCHEMAS` — [`L1044`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L1044) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
- `RISK_EQUATION_TUNING` — [`L743`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L743)
- `SPECIFIC_FILE_INFERENCE_MODEL` — [`L4581`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/analysis_lens.py#L4581)

