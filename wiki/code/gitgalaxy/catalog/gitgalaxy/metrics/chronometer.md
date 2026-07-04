---
title: 'Module: gitgalaxy/metrics/chronometer.py'
type: catalog
provenance: extracted
module: gitgalaxy/metrics/chronometer.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.metrics.chronometer`/Chronometer#
symbols:
  Chronometer._initialize_history_scan: _initialize_history_scan().
  Chronometer.get_file_history_metrics: get_file_history_metrics().
  Chronometer.repo_max_time: repo_max_time.
  Chronometer._determine_commit_bounds: _determine_commit_bounds().
  Chronometer._scan_git_history: _scan_git_history().
  Chronometer._stream_git_log: _stream_git_log().
  Chronometer.logger: logger.
  Chronometer: ''
  Chronometer.root: root.
  Chronometer.is_git_enabled: is_git_enabled.
  Chronometer.churn_map: churn_map.
  Chronometer.repo_min_time: repo_min_time.
  Chronometer.mtime_map: mtime_map.
  Chronometer.author_map: author_map.
  Chronometer._load_ignored_revs: _load_ignored_revs().
  Chronometer._survey_filesystem_mtimes: _survey_filesystem_mtimes().
  Chronometer.chrono_config: chrono_config.
  Chronometer.aperture_config: aperture_config.
  Chronometer.__init__: __init__().
---
# Module: [`gitgalaxy/metrics/chronometer.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py)

## Classes
### `Chronometer`
- def: [`gitgalaxy/metrics/chronometer.py:24`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L24) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
- doc: The GitGalaxy Chronometer.
- signature: `class Chronometer:`
- members:
  - `__init__(self, root_path: Path, parent_logger: Optional[logging.Logger] = None)` — [`L43`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L43) — Initializes the Time-Series Analyzer and ignites the Bulk Survey Pass.
  - `_determine_commit_bounds(self)` — [`L102`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L102) — [SIGNAL 1: ABSOLUTE BOUNDARIES] — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `_initialize_history_scan(self)` — [`L73`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L73) — Dispatches the survey engines to establish boundaries and churn cache. — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `_load_ignored_revs(self)` — [`L172`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L172) — Loads non-functional cosmetic commits to filter out of the churn math. — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `_scan_git_history(self)` — [`L190`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L190) — [BOUNDED HISTORY SCAN] — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `_stream_git_log(self, cmd: List[str], ignored_hashes: set, tracked_files: set, required_files: int, timeout_limit: float, start_time: float)` — [`L260`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L260) — Executes Git log via Popen stream, halting dynamically based on coverage or time. — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `_survey_filesystem_mtimes(self)` — [`L366`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L366) — OS-level fallback to populate mtime_map in non-Git environments. — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `get_file_history_metrics(self, rel_path: str)` — [`L377`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L377) — ======================================================================== — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `aperture_config` — [`L57`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L57) — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `author_map` — [`L62`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L62) — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `chrono_config` — [`L56`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L56) — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `churn_map` — [`L60`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L60) — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `is_git_enabled` — [`L53`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L53) — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `logger` — [`L46`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L46)
  - `mtime_map` — [`L61`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L61) — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `repo_max_time` — [`L66`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L66) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)
  - `repo_min_time` — [`L65`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L65) — documented in [gitgalaxy-metrics-chronometer](../../../concepts/gitgalaxy-metrics-chronometer.md)
  - `root` — [`L52`](../../../../../../raw/code/gitgalaxy/gitgalaxy/metrics/chronometer.py#L52)
- used by: [`used_tokens`](../galaxyscope.md#Orchestrator.used_tokens), [`_init_worker`](../galaxyscope.md#_init_worker), [`chronometer`](../galaxyscope.md#Orchestrator.chronometer)  (6 test-only)

