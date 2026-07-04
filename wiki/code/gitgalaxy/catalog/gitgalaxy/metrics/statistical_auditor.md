---
title: 'Module: gitgalaxy/metrics/statistical_auditor.py'
type: catalog
provenance: extracted
module: gitgalaxy/metrics/statistical_auditor.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.metrics.statistical_auditor`/StatisticalAuditor#
symbols:
  StatisticalAuditor.logger: logger.
  StatisticalAuditor.audit: audit().
  StatisticalAuditor: ''
  StatisticalAuditor._is_dead_code: _is_dead_code().
  StatisticalAuditor._is_threat: _is_threat().
  StatisticalAuditor._format_for_exclusion: _format_for_exclusion().
  StatisticalAuditor.lang_defs: lang_defs.
  StatisticalAuditor.SIGNAL_KEYS: SIGNAL_KEYS.
  StatisticalAuditor._is_highly_blended: _is_highly_blended().
  StatisticalAuditor.__init__: __init__().
---
# Module: [`gitgalaxy/metrics/statistical_auditor.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py)

## Classes
### `StatisticalAuditor`
- def: [`gitgalaxy/metrics/statistical_auditor.py:21`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py#L21)
- doc: GitGalaxy Statistical Auditor.
- signature: `class StatisticalAuditor:`
- members:
  - `__init__(self, parent_logger: Optional[logging.Logger] = None, lang_defs: Optional[Dict[str, Any]] = None)` — [`L35`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py#L35) — Initializes the statistical auditor and synchronizes telemetry.
  - `_format_for_exclusion(self, artifact: Dict[str, Any], reason: str)` — [`L487`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py#L487) — Formats an audited artifact to match the Orchestrator's Exclusion Queue schema.
  - `_is_dead_code(self, artifact: Dict[str, Any])` — [`L465`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py#L465) — Determines if an artifact is predominantly dead code or comments.
  - `_is_highly_blended(self, artifact: Dict[str, Any])` — [`L451`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py#L451) — Determines if a file is a Polyglot where the primary language is < 80% of the mass.
  - `_is_threat(self, artifact: Dict[str, Any])` — [`L505`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py#L505) — Determines if an artifact contains active security threat signatures.
  - `audit(self, parsed_files: List[Dict[str, Any]])` — [`L90`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py#L90) — Executes statistical gating to identify data-dumps and structural outliers. — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `SIGNAL_KEYS` — [`L55`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py#L55)
  - `lang_defs` — [`L52`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py#L52)
  - `logger` — [`L43`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/statistical_auditor.py#L43)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline), [`execute_incremental_scan`](../galaxyscope.md#Orchestrator.execute_incremental_scan), [`auditor`](../galaxyscope.md#Orchestrator.auditor)  (3 test-only)

