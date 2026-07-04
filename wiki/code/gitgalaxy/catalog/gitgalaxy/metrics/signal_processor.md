---
title: 'Module: gitgalaxy/metrics/signal_processor.py'
type: catalog
provenance: extracted
module: gitgalaxy/metrics/signal_processor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.metrics.signal_processor`/SignalProcessor#
symbols:
  SignalProcessor.calculate_risk_vector: calculate_risk_vector().
  SignalProcessor.SIGNAL_SCHEMA: SIGNAL_SCHEMA.
  SignalProcessor.RISK_SCHEMA: RISK_SCHEMA.
  SignalProcessor: ''
  SignalProcessor.summarize_galaxy_metrics: summarize_galaxy_metrics().
  SignalProcessor.generate_forensic_report: generate_forensic_report().
  SignalProcessor.logger: logger.
  SignalProcessor.risk_tuning: risk_tuning.
  SignalProcessor._get_context_multipliers: _get_context_multipliers().
  SignalProcessor.CONTEXT_VIOLATION_MATRIX: CONTEXT_VIOLATION_MATRIX.
  SignalProcessor.get_avg: get_avg().
  SignalProcessor._calc_safety: _calc_safety().
  SignalProcessor._calc_concurrency: _calc_concurrency().
  SignalProcessor._calc_state_flux: _calc_state_flux().
  SignalProcessor._calc_obscured_payload: _calc_obscured_payload().
  SignalProcessor._calc_logic_bomb: _calc_logic_bomb().
  SignalProcessor._calc_injection_surface: _calc_injection_surface().
  SignalProcessor._calc_memory_corruption: _calc_memory_corruption().
  SignalProcessor._rank_list: _rank_list().
  SignalProcessor.SCALER_IQRS: SCALER_IQRS.
  SignalProcessor._calculate_silo_risk: _calculate_silo_risk().
  SignalProcessor._normalize_temporal_metrics: _normalize_temporal_metrics().
  SignalProcessor._calc_cog_load: _calc_cog_load().
  SignalProcessor._calc_tech_debt: _calc_tech_debt().
  SignalProcessor._calc_documentation: _calc_documentation().
  SignalProcessor._calc_verification: _calc_verification().
  SignalProcessor._calc_graveyard: _calc_graveyard().
  SignalProcessor._calc_secrets_risk: _calc_secrets_risk().
  SignalProcessor._calc_algorithmic_dos: _calc_algorithmic_dos().
  SignalProcessor._get_locational_multipliers: _get_locational_multipliers().
  SignalProcessor.SCALER_MEDIANS: SCALER_MEDIANS.
  SignalProcessor.TIER_VARS: TIER_VARS.
  SignalProcessor._calc_raw_temporal_signals: _calc_raw_temporal_signals().
  SignalProcessor.get_cumulative_risk: get_cumulative_risk().
  SignalProcessor.get_val: get_val().
  SignalProcessor.is_paranoid: is_paranoid.
  SignalProcessor.asset_masks: asset_masks.
  SignalProcessor.ECOSYSTEMS: ECOSYSTEMS.
  SignalProcessor.NATIVE_WEIGHTS: NATIVE_WEIGHTS.
  SignalProcessor._classify_archetype: _classify_archetype().
  SignalProcessor._calc_ownership_entropy: _calc_ownership_entropy().
  SignalProcessor._sigmoid: _sigmoid().
  SignalProcessor.config: config.
  SignalProcessor.GLOBAL_ARCHETYPES: GLOBAL_ARCHETYPES.
  SignalProcessor.LANGUAGE_INFERENCE_MODELS: LANGUAGE_INFERENCE_MODELS.
  SignalProcessor.WEIGHT_DEFENSE: WEIGHT_DEFENSE.
  SignalProcessor.path_modifiers: path_modifiers.
  SignalProcessor.ECOSYSTEM_MISMATCH_WEIGHTS: ECOSYSTEM_MISMATCH_WEIGHTS.
  SignalProcessor._calc_civil_war: _calc_civil_war().
  SignalProcessor._calc_api_exposure: _calc_api_exposure().
  SignalProcessor._calc_spec_alignment: _calc_spec_alignment().
  SignalProcessor._generate_function_rankings: _generate_function_rankings().
  SignalProcessor._get_tier: _get_tier().
  SignalProcessor._get_dominant_lang: _get_dominant_lang().
  SignalProcessor.__init__: __init__().
  SignalProcessor.WEIGHT_RISK: WEIGHT_RISK.
  SignalProcessor.MASSIVE_FILE_THRESHOLD: MASSIVE_FILE_THRESHOLD.
  SignalProcessor.TESTING_RISK_FLOOR: TESTING_RISK_FLOOR.
---
# Module: [`gitgalaxy/metrics/signal_processor.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py)

## Classes
### `SignalProcessor`
- def: [`gitgalaxy/metrics/signal_processor.py:24`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L24) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
- doc: The GitGalaxy Signal Processor.
- signature: `class SignalProcessor:`
- members:
  - `__init__(self, aperture_config: Optional[Dict[str, Any]] = None, parent_logger: Optional[logging.Logger] = None)` — [`L49`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L49) — Initializes the signal processing engine with forensic constants and telemetry.
  - `_calc_algorithmic_dos(self, loc: int, raw_signals: Dict[str, int], mp: float, functions: List[Dict[str, Any]], popularity: int)` — [`L2174`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2174) — Calculates Algorithmic DoS Exposure based on Big-O depth, data gravity, and dependency bottlenecks.
  - `_calc_api_exposure(self, raw_signals: dict, total_loc: int, popularity: int = 0)` — [`L1685`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1685) — RISK: Publicly exposed surfaces (api).
  - `_calc_civil_war(self, raw_signals: Dict[str, int])` — [`L1332`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1332) — Calculates Formatting Inconsistencies (Tabs vs Spaces).
  - `_calc_concurrency(self, loc: int, raw_signals: Dict[str, int], irc: int, mp: float, functions: List[Dict[str, Any]] = None)` — [`L1713`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1713) — RISK: Threads/Async execution + Thread Starvation (O(N) Bombs). — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_calc_injection_surface(self, loc: int, raw_signals: Dict[str, int], mp: float, archetype: str)` — [`L1989`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1989) — Calculates Injection Surface Exposure (XSS, SQLi, RCE, SSTI). — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_calc_logic_bomb(self, loc: int, raw_signals: Dict[str, int], mp: float, archetype: str, global_drift: float, local_drift: float, max_big_o: int = 1)` — [`L1893`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1893) — Calculates Logic Bomb / Sabotage Exposure. — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_calc_memory_corruption(self, loc: int, raw_signals: Dict[str, int], mp: float, lang_id: str = "", archetype: str = "")` — [`L2052`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2052) — Calculates Memory Corruption Exposure (Buffer Overflows, UAF).
  - `_calc_obscured_payload(self, loc: int, raw_signals: Dict[str, int], mp: float, archetype: str, global_drift: float, local_drift: float)` — [`L1798`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1798) — Calculates Obscured Payload Exposure (Malicious Intent Density). — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_calc_ownership_entropy(self, authors: Dict[str, int])` — [`L1309`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1309) — Calculates Ownership Entropy (Shannon Entropy) for the file. — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_calc_raw_temporal_signals(self, temp: Dict[str, Any])` — [`L1285`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1285) — Calculates Stability (Age) and Raw Churn (Seismic Frequency). — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_calc_secrets_risk(self, loc: int, raw_signals: Dict[str, int], mp: float)` — [`L2127`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2127) — Calculates Secrets Risk Exposure (Credential Exposure).
  - `_calc_state_flux(self, loc: int, raw_signals: Dict[str, int], irc: int, mp: float)` — [`L1759`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1759) — RISK: State mutation (flux). — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_calc_verification(self, loc: int, rel_path: str, is_protected: bool, raw_signals: Dict[str, int], ot: float, fc: float, mp: float, functions: List[Dict[str, Any]], test_coverage_map: Dict[str, List[Dict[str, Any]]], umbrella_bonus: float = 0, popularity: int = 0)` — [`L1563`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1563) — Calculates Verification Risk Exposure by comparing structural function complexity
  - `_calculate_silo_risk(self, authors: dict)` — [`L200`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L200) — Calculates the Authorship Centralization risk of a file. — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_classify_archetype(self, scaled_vector: List[float], archetypes_dict: Dict[str, List[float]])` — [`L127`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L127) — Dynamically calculates the Euclidean Distance for any provided K-Means dictionary. — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_get_context_multipliers(self, file_lang: str, folder_lang: str)` — [`L156`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L156) — Calculates risk multipliers by comparing an asset's language to its directory environment. — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_get_locational_multipliers(self, path: str)` — [`L2385`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2385) — Matches path against regex configurations and extracts applicable Modifiers. — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_normalize_temporal_metrics(self, parsed_files: List[Dict[str, Any]])` — [`L1250`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1250) — [PASS 2] Normalizes churn using a Logarithmic Curve for better UI gradients. — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `_rank_list(self, parsed_files: List[Dict[str, Any]], key_path: List[Any])` — [`L2424`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2424) — Extracts top and bottom ranks safely navigating dictionaries and lists.
  - `_sigmoid(self, density: float, threshold: float, slope: float)` — [`L1791`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1791) — Safely calculates the sigmoid curve with overflow protection for extreme densities. — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `calculate_risk_vector(self, meta: Dict[str, Any], raw_signals: Dict[str, int], umbrella_bonus: float = 0)` — [`L218`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L218) — Calculates risk exposure, temporal analysis, and per-file structural impact. — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `generate_forensic_report(self, parsed_files: List[Dict[str, Any]])` — [`L2248`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2248) — [FORENSIC RANKING] Generates Top/Bottom 3 for dynamically indexed exposures. — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `get_avg(metric_name)` — [`L874`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L874)
  - `get_cumulative_risk(f)` — [`L2276`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2276)
  - `get_val(f)` — [`L2427`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2427)
  - `summarize_galaxy_metrics(self, parsed_files: List[Dict[str, Any]], unparsable_files: List[Dict[str, Any]])` — [`L857`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L857) — [GLOBAL SYNTHESIS] Executes Pass 2 Normalization and aggregates health metrics. — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `CONTEXT_VIOLATION_MATRIX` — [`L123`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L123) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `ECOSYSTEMS` — [`L106`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L106) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `ECOSYSTEM_MISMATCH_WEIGHTS` — [`L110`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L110) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `GLOBAL_ARCHETYPES` — [`L75`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L75) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `LANGUAGE_INFERENCE_MODELS` — [`L78`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L78) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `MASSIVE_FILE_THRESHOLD` — [`L92`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L92)
  - `NATIVE_WEIGHTS` — [`L107`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L107) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `RISK_SCHEMA` — [`L47`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L47) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `SCALER_IQRS` — [`L71`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L71) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `SCALER_MEDIANS` — [`L70`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L70) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `SIGNAL_SCHEMA` — [`L44`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L44) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `TESTING_RISK_FLOOR` — [`L93`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L93)
  - `TIER_VARS` — [`L84`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L84) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `WEIGHT_DEFENSE` — [`L83`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L83)
  - `WEIGHT_RISK` — [`L82`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L82)
  - `asset_masks` — [`L97`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L97) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `config` — [`L63`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L63)
  - `is_paranoid` — [`L99`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L99)
  - `logger` — [`L56`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L56)
  - `path_modifiers` — [`L96`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L96) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `risk_tuning` — [`L98`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L98) — documented in [gitgalaxy-metrics-signal_processor](../../../concepts/gitgalaxy-metrics-signal_processor.md)
- protocol/private: `_calc_cog_load`[`L1352`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1352), `_calc_documentation`[`L1499`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1499), `_calc_graveyard`[`L1668`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1668), `_calc_safety`[`L1421`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1421), `_calc_spec_alignment`[`L1786`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1786), `_calc_tech_debt`[`L1461`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L1461), `_generate_function_rankings`[`L2458`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2458), `_get_dominant_lang`[`L2486`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2486), `_get_tier`[`L2477`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/signal_processor.py#L2477)
- uses (calls/refs, reference-scoped): [`RECORDING_SCHEMAS`](../standards/analysis_lens.md#RECORDING_SCHEMAS)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline), [`execute_incremental_scan`](../galaxyscope.md#Orchestrator.execute_incremental_scan), [`used_tokens`](../galaxyscope.md#Orchestrator.used_tokens), [`_init_worker`](../galaxyscope.md#_init_worker), [`_process_file_worker`](../galaxyscope.md#_process_file_worker), [`processor`](../galaxyscope.md#Orchestrator.processor)  (3 test-only)

