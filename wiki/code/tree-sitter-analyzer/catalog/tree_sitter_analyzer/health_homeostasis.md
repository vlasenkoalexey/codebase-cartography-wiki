---
title: 'Module: tree_sitter_analyzer/health_homeostasis.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/health_homeostasis.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.health_homeostasis`/
symbols:
  HealthHomeostasisLoop._process_one: HealthHomeostasisLoop#_process_one().
  run_watch_health: run_watch_health().
  HealthHomeostasisLoop._should_alert: HealthHomeostasisLoop#_should_alert().
  HealthHomeostasisLoop.on_sync_callback: HealthHomeostasisLoop#on_sync_callback().
  HealthHomeostasisLoop.__init__: HealthHomeostasisLoop#__init__().
  GRADE_ORDER.GRADE_ORDER: GRADE_ORDER.GRADE_ORDER.
  HealthHomeostasisLoop._in_cooldown: HealthHomeostasisLoop#_in_cooldown().
  run_watch_health._on_sync: run_watch_health()._on_sync().
  WatchHealthRunner._go: WatchHealthRunner#_go().
  WatchHealthRunner.start: WatchHealthRunner#start().
  WatchHealthRunner._thread: WatchHealthRunner#_thread.
  is_worse_grade: is_worse_grade().
  _at_or_below: _at_or_below().
  WatchHealthRunner.stop: WatchHealthRunner#stop().
  _VALID_GRADES: _VALID_GRADES.
  logger: logger.
  _strictly_above: _strictly_above().
  HealthHomeostasisLoop._build_event: HealthHomeostasisLoop#_build_event().
  _build_recommendation: _build_recommendation().
  _extract_changed_files: _extract_changed_files().
  HealthHomeostasisLoop: HealthHomeostasisLoop#
  WatchHealthRunner._stop_event: WatchHealthRunner#_stop_event.
  HealthHomeostasisLoop.threshold_grade: HealthHomeostasisLoop#threshold_grade().
  _ScorerLike: _ScorerLike#
  HealthHomeostasisLoop._threshold_grade: HealthHomeostasisLoop#_threshold_grade.
  HealthHomeostasisLoop._cooldown: HealthHomeostasisLoop#_cooldown.
  HealthHomeostasisLoop._history: HealthHomeostasisLoop#_history.
  HealthHomeostasisLoop._last_alert: HealthHomeostasisLoop#_last_alert.
  HealthHomeostasisLoop._lock: HealthHomeostasisLoop#_lock.
  _extract_changed_files._to_abs: _extract_changed_files()._to_abs().
  _ScorerLike.score_file: _ScorerLike#score_file().
  _NotifierLike: _NotifierLike#
  _NotifierLike.dispatch: _NotifierLike#dispatch().
  HealthHomeostasisLoop._notifier: HealthHomeostasisLoop#_notifier.
  HealthHomeostasisLoop._scorer: HealthHomeostasisLoop#_scorer.
  HealthHomeostasisLoop._clock: HealthHomeostasisLoop#_clock.
  WatchHealthRunner._kwargs: WatchHealthRunner#_kwargs.
  WatchHealthRunner: WatchHealthRunner#
  WatchHealthRunner.__init__: WatchHealthRunner#__init__().
---
# Module: [`tree_sitter_analyzer/health_homeostasis.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py)

## Classes
### `HealthHomeostasisLoop`
- def: [`tree_sitter_analyzer/health_homeostasis.py:81`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L81)
- doc: Stateful classifier that decides which file changes deserve alerts.
- signature: `class HealthHomeostasisLoop:`
- members:
  - `_should_alert(self, prev_grade: str | None, new_grade: str)` — [`L180`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L180) — Apply the two-rule classifier — see module docstring.
  - `on_sync_callback(self, changed_files: set[str] | list[str])` — [`L122`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L122) — For each changed file: rescore, classify, alert + persist.
  - `threshold_grade(self)` — [`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L117)
- protocol/private: `__init__`[`L91`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L91), `_build_event`[`L224`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L224), `_clock`[`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L111), `_cooldown`[`L107`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L107), `_history`[`L108`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L108), `_in_cooldown`[`L215`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L215), `_last_alert`[`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L113), `_lock`[`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L114), `_notifier`[`L109`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L109), `_process_one`[`L139`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L139), `_scorer`[`L110`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L110), `_threshold_grade`[`L106`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L106)
- uses (calls/refs, reference-scoped): [`append`](_health_history.md#HealthHistory.append), [`HealthHistory`](_health_history.md#HealthHistory), [`last`](_health_history.md#HealthHistory.last), [`GRADE_ORDER`](health_homeostasis.md#GRADE_ORDER.GRADE_ORDER), [`_at_or_below`](health_homeostasis.md#_at_or_below), [`is_worse_grade`](health_homeostasis.md#is_worse_grade), [`_VALID_GRADES`](health_homeostasis.md#_VALID_GRADES), [`logger`](health_homeostasis.md#logger), [`_build_recommendation`](health_homeostasis.md#_build_recommendation), [`_strictly_above`](health_homeostasis.md#_strictly_above), [`_ScorerLike`](health_homeostasis.md#_ScorerLike), [`_NotifierLike`](health_homeostasis.md#_NotifierLike), [`dispatch`](health_homeostasis.md#_NotifierLike.dispatch), [`score_file`](health_homeostasis.md#_ScorerLike.score_file)
- used by: [`run_watch_health`](health_homeostasis.md#run_watch_health), [`_on_sync`](health_homeostasis.md#run_watch_health._on_sync)  (2 test-only)

### `WatchHealthRunner`
- def: [`tree_sitter_analyzer/health_homeostasis.py:415`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L415)
- doc: Threaded wrapper around `run_watch_health`.
- signature: `class WatchHealthRunner:`
- members:
  - `start(self)` — [`L453`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L453)
  - `stop(self, timeout: float = 5)` — [`L468`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L468)
- protocol/private: `__init__`[`L422`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L422), `_go`[`L458`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L458), `_kwargs`[`L437`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L437), `_stop_event`[`L450`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L450), `_thread`[`L451`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L451)
- uses (calls/refs, reference-scoped): [`run_watch_health`](health_homeostasis.md#run_watch_health)

### `_NotifierLike`  ·  implements/extends Protocol
- def: [`tree_sitter_analyzer/health_homeostasis.py:74`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L74)
- signature: `class _NotifierLike(Protocol):`
- members:
  - `dispatch(self, event: dict[str, Any])` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L75)
- used by: [`_process_one`](health_homeostasis.md#HealthHomeostasisLoop._process_one), [`__init__`](health_homeostasis.md#HealthHomeostasisLoop.__init__)

### `_ScorerLike`  ·  implements/extends Protocol
- def: [`tree_sitter_analyzer/health_homeostasis.py:68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L68)
- doc: Duck-typed scorer; matches `HealthScorer`.
- signature: `class _ScorerLike(Protocol):`
- members:
  - `score_file(self, file_path: str)` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L71)
- used by: [`_process_one`](health_homeostasis.md#HealthHomeostasisLoop._process_one), [`__init__`](health_homeostasis.md#HealthHomeostasisLoop.__init__)

## Functions
- `_at_or_below(grade: str, threshold: str)` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L55) — True iff ``grade`` is at or below the threshold (worse-or-equal).
- `_build_recommendation(new_grade: str, prev_grade: str | None)` — [`L246`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L246) — One-liner action hint, used in the template payload.
- `_extract_changed_files(sync_result: dict[str, Any], *, project_root: str | Path | None = None)` — [`L346`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L346) — Pull changed file paths out of an ``IncrementalSync.SyncResult.to_dict()``.
- `_on_sync(result: dict[str, Any])` — [`L306`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L306)
- `_strictly_above(grade: str, threshold: str)` — [`L60`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L60) — True iff ``grade`` is strictly better than the threshold.
- `_to_abs(rel_or_abs: str)` — [`L371`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L371)
- `is_worse_grade(new_grade: str, prev_grade: str)` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L50) — True iff ``new_grade`` is strictly worse than ``prev_grade``.
- `run_watch_health(*, project_root: str | Path, threshold_grade: str = "C", interval: float = 5, debounce: float = 0.5, cooldown: float = 0, history_keep: int = 50, notify_channels: list[str] | None = None, notify_file: str | Path | None = None, on_degradation: str | None = None, webhook_url: str | None = None, backend: str = "poll", stop_event: threading.Event | None = None)` — [`L260`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L260) — Blocking entrypoint: spin up the daemon and the homeostasis loop.

## Module values
- `GRADE_ORDER` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L43)
- `_VALID_GRADES` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L44)
- `logger` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_homeostasis.py#L39)

