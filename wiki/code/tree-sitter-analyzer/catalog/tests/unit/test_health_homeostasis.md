---
title: 'Module: tests/unit/test_health_homeostasis.py'
type: catalog
provenance: extracted
module: tests/unit/test_health_homeostasis.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_health_homeostasis`/
symbols:
  test_threshold_filter_suppresses_jitter_above_threshold: test_threshold_filter_suppresses_jitter_above_threshold().
  make_loop._make: make_loop()._make().
  _FakeScorer.score_file: _FakeScorer#score_file().
  _import_loop: _import_loop().
  _import_history: _import_history().
  _import_ordering: _import_ordering().
  history: history().
  make_loop: make_loop().
  test_classifier_grade_ordering: test_classifier_grade_ordering().
  _FakeScorer: _FakeScorer#
  _FakeScorer.table: _FakeScorer#table.
  _FakeScorer.calls: _FakeScorer#calls.
  pytestmark: pytestmark.
  _FakeScorer.__init__: _FakeScorer#__init__().
  project_root: project_root().
  notifier: notifier().
  test_loop_alerts_on_grade_drop: test_loop_alerts_on_grade_drop().
  test_loop_silent_on_grade_improvement: test_loop_silent_on_grade_improvement().
  test_loop_silent_on_grade_unchanged: test_loop_silent_on_grade_unchanged().
  test_loop_alerts_on_first_drop_below_threshold_edge_trigger: test_loop_alerts_on_first_drop_below_threshold_edge_trigger().
  test_loop_no_alert_when_already_below_threshold_no_drop: test_loop_no_alert_when_already_below_threshold_no_drop().
  test_loop_no_alert_on_level_repeat_below_threshold: test_loop_no_alert_on_level_repeat_below_threshold().
  test_cold_start_alerts_only_below_threshold: test_cold_start_alerts_only_below_threshold().
  test_cold_start_at_threshold_alerts: test_cold_start_at_threshold_alerts().
  test_cooldown_suppresses_repeat_alerts_same_file: test_cooldown_suppresses_repeat_alerts_same_file().
  test_cooldown_does_not_cross_files: test_cooldown_does_not_cross_files().
  test_cooldown_expires_allows_new_alert: test_cooldown_expires_allows_new_alert().
  test_alert_event_contains_template_tokens: test_alert_event_contains_template_tokens().
---
# Module: [`tests/unit/test_health_homeostasis.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py)

## Classes
### `_FakeScorer`
- def: [`tests/unit/test_health_homeostasis.py:74`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L74)
- doc: Minimal stand-in for HealthScorer. Maps file→(total, grade) per call.
- signature: `class _FakeScorer:`
- members:
  - `score_file(self, file_path: str)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L81)
  - `calls` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L79)
  - `table` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L78)
- protocol/private: `__init__`[`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L77)
- used by: (2 test-only callers)

## Functions
- `_import_history()` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L53)
- `_import_loop()` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L45)
- `_import_ordering()` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L59) — Optional helper: classifier ordering function.
- `_make(threshold_grade: str = "C", cooldown: float = 0, scorer_table: dict[str, tuple[float, str]] | None = None)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L121)
- `history(project_root: str)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L100)
- `make_loop(history, notifier)` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L118) — Factory: build a loop with mocked scorer + given threshold/cooldown.
- `notifier()` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L110) — Mock notifier with .dispatch(event_dict).
- `project_root(tmp_path: Path)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L94)
- `test_alert_event_contains_template_tokens(make_loop, history, notifier)` — [`L406`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L406) — Emitted event dict must include the tokens the Notifier needs:
- `test_classifier_grade_ordering()` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L142) — Spec: A < B < C < D < F (A is best, F is worst).
- `test_cold_start_alerts_only_below_threshold(make_loop, notifier)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L265) — No prior row; threshold=C.
- `test_cold_start_at_threshold_alerts(make_loop, notifier)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L290) — threshold=C; no prior row; now=C → 1 alert (<= threshold edge fires).
- `test_cooldown_does_not_cross_files(make_loop, history, notifier)` — [`L325`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L325) — Cooldown is per-file. fileA cooldown does not suppress fileB alert.
- `test_cooldown_expires_allows_new_alert(make_loop, history, notifier)` — [`L345`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L345) — After cooldown window elapses, a new alert is allowed for the same file.
- `test_cooldown_suppresses_repeat_alerts_same_file(make_loop, history, notifier)` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L307) — 5 calls within cooldown window for the same alert-worthy file → 1 alert.
- `test_loop_alerts_on_first_drop_below_threshold_edge_trigger(make_loop, history, notifier)` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L211) — threshold=C; prev=B (above), now=D (below) → 1 alert.
- `test_loop_alerts_on_grade_drop(make_loop, history, notifier)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L165) — History has file→B. Recompute yields file→D. Expect 1 alert.
- `test_loop_no_alert_on_level_repeat_below_threshold(make_loop, history, notifier)` — [`L247`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L247) — threshold=C; prev=F, now=F → 0 alerts. Level-only entries suppressed.
- `test_loop_no_alert_when_already_below_threshold_no_drop(make_loop, history, notifier)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L226) — threshold=C; prev=D (already below), now=F (still below, but worse).
- `test_loop_silent_on_grade_improvement(make_loop, history, notifier)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L182) — History has file→D. Recompute yields file→B. Expect 0 alerts.
- `test_loop_silent_on_grade_unchanged(make_loop, history, notifier)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L195) — History has file→C. Recompute yields file→C (level repeat). Expect 0 alerts.
- `test_threshold_filter_suppresses_jitter_above_threshold(history, notifier)` — [`L368`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L368) — threshold=C; chain B→A→B → 0 alerts (all hovering above threshold).

## Module values
- `pytestmark` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_homeostasis.py#L39)

