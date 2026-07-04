---
title: 'Module: gitgalaxy/galaxyscope.py'
type: catalog
provenance: extracted
module: gitgalaxy/galaxyscope.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.galaxyscope`/
symbols:
  Orchestrator.execute_pipeline: Orchestrator#execute_pipeline().
  logger: logger.
  Orchestrator.execute_incremental_scan: Orchestrator#execute_incremental_scan().
  Orchestrator.used_tokens: Orchestrator#used_tokens.
  Orchestrator._extract_features_parallel: Orchestrator#_extract_features_parallel().
  Orchestrator.root: Orchestrator#root.
  Orchestrator._build_file_census: Orchestrator#_build_file_census().
  main: main().
  _init_worker: _init_worker().
  Orchestrator._fallback_filesystem_walk: Orchestrator#_fallback_filesystem_walk().
  Orchestrator.ram_cache: Orchestrator#ram_cache.
  Orchestrator._resolve_dependency_graph: Orchestrator#_resolve_dependency_graph().
  Orchestrator.ext_tally: Orchestrator#ext_tally.
  _worker_state: _worker_state.
  Orchestrator.config: Orchestrator#config.
  Orchestrator.db_recorder: Orchestrator#db_recorder.
  Orchestrator.splicing_telemetry: Orchestrator#splicing_telemetry.
  Orchestrator.parsed_files: Orchestrator#parsed_files.
  _process_file_worker: _process_file_worker().
  Orchestrator.unparsable_files: Orchestrator#unparsable_files.
  Orchestrator._inspect_path: Orchestrator#_inspect_path().
  Orchestrator._prepare_target: Orchestrator#_prepare_target().
  Orchestrator._record_anomaly: Orchestrator#_record_anomaly().
  Orchestrator.stem_map: Orchestrator#stem_map.
  Orchestrator.guidestar: Orchestrator#guidestar.
  Orchestrator.gpu_recorder: Orchestrator#gpu_recorder.
  Orchestrator.processor: Orchestrator#processor.
  Orchestrator.chronometer: Orchestrator#chronometer.
  Orchestrator.network_sensor: Orchestrator#network_sensor.
  Orchestrator.cleanup: Orchestrator#cleanup().
  Orchestrator.temp_dir: Orchestrator#temp_dir.
  Orchestrator.auditor: Orchestrator#auditor.
  Orchestrator.model_auditor: Orchestrator#model_auditor.
  Orchestrator.census: Orchestrator#census.
  Orchestrator.popularity_scores: Orchestrator#popularity_scores.
  Orchestrator._calculate_risk_exposures: Orchestrator#_calculate_risk_exposures().
  Orchestrator.spatial_mapper: Orchestrator#spatial_mapper.
  Orchestrator.audit_recorder: Orchestrator#audit_recorder.
  Orchestrator.llm_recorder: Orchestrator#llm_recorder.
  HAS_PYYAML: HAS_PYYAML.
  Orchestrator.version: Orchestrator#version.
  Orchestrator._levenshtein: Orchestrator#_levenshtein().
  Orchestrator._get_git_audit: Orchestrator#_get_git_audit().
  Orchestrator.neighborhood_tracker: Orchestrator#neighborhood_tracker.
  Orchestrator.file_speed_telemetry: Orchestrator#file_speed_telemetry.
  Orchestrator._summarize_anomalies: Orchestrator#_summarize_anomalies().
  Orchestrator._render_file_speed_chart: Orchestrator#_render_file_speed_chart().
  Orchestrator._render_splicing_chart: Orchestrator#_render_splicing_chart().
  Orchestrator.git_tracked_files: Orchestrator#git_tracked_files.
  Orchestrator.security_analyzer: Orchestrator#security_analyzer.
  Orchestrator.anomalies: Orchestrator#anomalies.
  Orchestrator.MICRO_MASS_BYTES: Orchestrator#MICRO_MASS_BYTES.
  Orchestrator.MICRO_MASS_GRACE_LIMIT: Orchestrator#MICRO_MASS_GRACE_LIMIT.
  Orchestrator._get_deletes: Orchestrator#_get_deletes().
  execution_timeout_failsafe: execution_timeout_failsafe().
  Orchestrator: Orchestrator#
  Orchestrator.__init__: Orchestrator#__init__().
---
# Module: [`gitgalaxy/galaxyscope.py`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py)

## Classes
### `Orchestrator`
- def: [`gitgalaxy/galaxyscope.py:561`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L561)
- doc: Orchestrator Core: The GitGalaxy Central Processing Core.
- signature: `class Orchestrator:`
- members:
  - `_build_file_census(self)` — [`L998`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L998) — Phase 0: Building the Census via Git Authority with Fallback. — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `_calculate_risk_exposures(self)` — [`L1519`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1519) — Phase 3: Universal Exposure Framework & Signal Processing.
  - `_extract_features_parallel(self)` — [`L1113`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1113) — Phase 1: Parallel Extraction & Asset Filtering via Multi-Core Map-Reduce. — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `_fallback_filesystem_walk(self)` — [`L1063`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1063) — Standard OS-level filesystem walk for non-Git projects or ZIP archives. — documented in [gitgalaxy-core-aperture](../../concepts/gitgalaxy-core-aperture.md)
  - `_get_git_audit(self)` — [`L2012`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L2012) — Extracts forensic Git metadata (Commit SHA, Branch, Remote URL, Date) via subprocess.
  - `_prepare_target(self, target_input: Union[str, Path])` — [`L1843`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1843) — Validates the user's target input and constructs an ephemeral extraction environment if necessary.
  - `_record_anomaly(self, path: Union[str, Path], message: str)` — [`L1882`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1882) — Records failure telemetry.
  - `_render_file_speed_chart(self)` — [`L1943`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1943) — Generates a terminal ASCII chart for macro file phases.
  - `_render_splicing_chart(self)` — [`L1969`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1969) — Generates a terminal ASCII chart for regex and file performance.
  - `_resolve_dependency_graph(self)` — [`L1254`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1254) — Pass 1.5: Optimized relational token aggregation & Fuzzy Suffix Matching. — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `_summarize_anomalies(self, total_unparsable: List[Dict[str, Any]])` — [`L1888`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1888) — Bridges isolated worker failures back to the main thread's forensic ledger.
  - `cleanup(self)` — [`L1868`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1868) — Executes a mandatory garbage collection routine to securely purge any ephemeral environments.
  - `execute_incremental_scan(self, ram_cache: Dict[str, Any], added: List[str], modified: List[str], deleted: List[str], db_output_path: str)` — [`L2067`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L2067) — Executes a high-efficiency 'Continuous Delta' scan for CI/CD environments. — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `execute_pipeline(self, output_file: str = "galaxy.json")` — [`L676`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L676) — Executes the synthesis protocol with a multi-recorder exit strategy. — documented in [gitgalaxy-core-guidestar_lens](../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `MICRO_MASS_BYTES` — [`L660`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L660)
  - `MICRO_MASS_GRACE_LIMIT` — [`L661`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L661)
  - `anomalies` — [`L652`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L652)
  - `audit_recorder` — [`L624`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L624)
  - `auditor` — [`L613`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L613)
  - `census` — [`L647`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L647)
  - `chronometer` — [`L606`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L606)
  - `config` — [`L587`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L587) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `db_recorder` — [`L628`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L628) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `ext_tally` — [`L654`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L654) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `file_speed_telemetry` — [`L671`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L671)
  - `git_tracked_files` — [`L655`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L655)
  - `gpu_recorder` — [`L622`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L622) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `guidestar` — [`L603`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L603)
  - `llm_recorder` — [`L626`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L626)
  - `model_auditor` — [`L640`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L640) — documented in [gitgalaxy-security-security_auditor](../../concepts/gitgalaxy-security-security_auditor.md)
  - `neighborhood_tracker` — [`L662`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L662)
  - `network_sensor` — [`L616`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L616)
  - `parsed_files` — [`L650`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L650) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `popularity_scores` — [`L653`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L653)
  - `processor` — [`L610`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L610) — documented in [gitgalaxy-metrics-signal_processor](../../concepts/gitgalaxy-metrics-signal_processor.md)
  - `ram_cache` — [`L649`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L649) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `root` — [`L590`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L590)
  - `security_analyzer` — [`L637`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L637) — documented in [gitgalaxy-security-security_lens](../../concepts/gitgalaxy-security-security_lens.md)
  - `spatial_mapper` — [`L607`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L607)
  - `splicing_telemetry` — [`L664`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L664) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `stem_map` — [`L648`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L648) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `temp_dir` — [`L589`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L589)
  - `unparsable_files` — [`L651`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L651) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `used_tokens` — [`L1556`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1556) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)
  - `version` — [`L588`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L588)
- protocol/private: `__init__`[`L581`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L581), `_get_deletes`[`L1438`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1438), `_inspect_path`[`L1008`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1008), `_levenshtein`[`L1424`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L1424)
- uses (calls/refs, reference-scoped): [`logger`](galaxyscope.md#logger), [`calculate_risk_vector`](metrics/signal_processor.md#SignalProcessor.calculate_risk_vector), [`SIGNAL_SCHEMA`](metrics/signal_processor.md#SignalProcessor.SIGNAL_SCHEMA), [`RISK_SCHEMA`](metrics/signal_processor.md#SignalProcessor.RISK_SCHEMA), [`record_mission`](recorders/gpu_recorder.md#GPURecorder.record_mission), [`run_xray_audit`](tools/supply_chain_security/binary_anomaly_detector.md#run_xray_audit), [`_init_worker`](galaxyscope.md#_init_worker), [`map_repository`](core/spatial_mapper.md#SpatialMapper.map_repository), [`run_firewall_audit`](tools/supply_chain_security/supply_chain_firewall.md#run_firewall_audit), [`audit_repository`](security/security_auditor.md#SecurityAuditor.audit_repository), [`evaluate_path_integrity`](core/aperture.md#ApertureFilter.evaluate_path_integrity), [`get_file_history_metrics`](metrics/chronometer.md#Chronometer.get_file_history_metrics), [`SignalProcessor`](metrics/signal_processor.md#SignalProcessor), [`scan_project_config`](core/guidestar_lens.md#GuideStarLens.scan_project_config), [`audit`](metrics/statistical_auditor.md#StatisticalAuditor.audit), [`HAS_NETWORKX`](core/network_risk_sensor.md#HAS_NETWORKX), [`summarize_galaxy_metrics`](metrics/signal_processor.md#SignalProcessor.summarize_galaxy_metrics), [`generate_forensic_report`](metrics/signal_processor.md#SignalProcessor.generate_forensic_report), [`Chronometer`](metrics/chronometer.md#Chronometer), [`SecurityAuditor`](security/security_auditor.md#SecurityAuditor), [`ThreatPolicy`](standards/analysis_lens.md#ThreatPolicy), [`SecurityLens`](security/security_lens.md#SecurityLens), [`get_policy`](standards/analysis_lens.md#ThreatPolicy.get_policy), [`HAS_TIKTOKEN`](core/detector.md#HAS_TIKTOKEN), [`build_resolution_map`](security/manifest_parser.md#ManifestParser.build_resolution_map), [`run_api_audit`](tools/network_auditing/full_api_network_map.md#run_api_audit), [`build_dependency_graph`](core/network_risk_sensor.md#NetworkRiskSensor.build_dependency_graph), [`record_mission`](recorders/record_keeper.md#RecordKeeper.record_mission), [`ApertureFilter`](core/aperture.md#ApertureFilter), [`APERTURE_CONFIG`](standards/gitgalaxy_config.md#APERTURE_CONFIG), [`_process_file_worker`](galaxyscope.md#_process_file_worker), [`generate_report`](recorders/audit_recorder.md#AuditRecorder.generate_report), [`get_intent_status`](core/guidestar_lens.md#GuideStarLens.get_intent_status), [`ML_AVAILABLE`](security/security_auditor.md#ML_AVAILABLE), [`audit_model`](metrics/tensor_scanner.md#TensorScanner.audit_model), [`evaluate_ecosystem`](tools/ai_guardrails/dev_agent_firewall.md#DevAgentFirewall.evaluate_ecosystem), [`generate_artifacts`](recorders/llm_recorder.md#LLMRecorder.generate_artifacts), [`DevAgentFirewall`](tools/ai_guardrails/dev_agent_firewall.md#DevAgentFirewall), [`hunt_threats`](tools/ai_guardrails/ai_appsec_sensor.md#AIAppSecSensor.hunt_threats), [`AIAppSecSensor`](tools/ai_guardrails/ai_appsec_sensor.md#AIAppSecSensor)  (+15 more)
- used by: [`main`](galaxyscope.md#main)

## Functions
- `_init_worker(root_str: str, config: Dict[str, Any], ext_tally: Dict[str, int], log_level: int, git_tracked: Set[str], census: Set[str])` — [`L90`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L90) — Initializes the CPU-bound optical modules within the worker process's isolated memory. — documented in [gitgalaxy-core-detector](../../concepts/gitgalaxy-core-detector.md)
- `_process_file_worker(rel_path: str)` — [`L171`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L171) — Processes a single file path using the worker's cached hardware modules. — documented in [gitgalaxy-metrics-signal_processor](../../concepts/gitgalaxy-metrics-signal_processor.md)
- `execution_timeout_failsafe(signum, frame)` — [`L79`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L79) — Hardware-level OS interrupt for Catastrophic Backtracking (ReDoS) protection.
- `main()` — [`L2175`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L2175) — documented in [gitgalaxy-galaxyscope](../../concepts/gitgalaxy-galaxyscope.md)

## Module values
- `HAS_PYYAML` — [`L68`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L68)
- `_worker_state` — [`L77`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L77)
- `logger` — [`L70`](../../../../../raw/code/gitgalaxy/gitgalaxy/galaxyscope.py#L70)

