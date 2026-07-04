---
title: 'Module: tests/test_cli.py'
type: catalog
provenance: extracted
module: tests/test_cli.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `tests.test_cli`/
symbols:
  test_finalize_emits_catalogs_before_lint: test_finalize_emits_catalogs_before_lint().
  SLUG: SLUG.
  _prepare: _prepare().
  test_plan_models_prepare_agenda: test_plan_models_prepare_agenda().
  test_top_index_reports_connection_status: test_top_index_reports_connection_status().
  test_finalize_lint_gate_fails_on_dead_citation: test_finalize_lint_gate_fails_on_dead_citation().
  project: project().
  test_plan_is_a_dry_run_never_indexes: test_plan_is_a_dry_run_never_indexes().
  runner: runner.
  test_prepare_writes_packet_for_config_concept: test_prepare_writes_packet_for_config_concept().
  _git: _git().
  FIXTURE: FIXTURE.
  test_plan_models_prepare_agenda.agenda_line: test_plan_models_prepare_agenda().agenda_line().
---
# Module: [`tests/test_cli.py`](../../../../../raw/code/wikify-repo/tests/test_cli.py)

## Functions
- `_git(repo: Path, *args: str)` — [`L30`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L30)
- `_prepare(root: Path)` — [`L60`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L60)
- `agenda_line(out: str)` — [`L84`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L84)
- `project(tmp_path)` — [`L38`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L38) — A project root + a committed source repo, index pre-seeded (no scip-python).
- `test_finalize_emits_catalogs_before_lint(project)` — [`L101`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L101) — A concept page cites ``../catalog/<module>.md#<anchor>`` — with no catalog
- `test_finalize_lint_gate_fails_on_dead_citation(project)` — [`L153`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L153) — The citation linter is a hard build gate: a citation whose anchor does not
- `test_plan_is_a_dry_run_never_indexes(project, tmp_path)` — [`L91`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L91) — Without a cached index, ``plan`` must refuse (exit 2) — not silently run
- `test_plan_models_prepare_agenda(project)` — [`L75`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L75) — Regression: ``plan`` once diffed the raw config only (no discovery), so its
- `test_prepare_writes_packet_for_config_concept(project)` — [`L65`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L65)
- `test_top_index_reports_connection_status(project)` — [`L129`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L129) — The top catalog's Connection column is derived from the silo pages: a

## Module values
- `FIXTURE` — [`L24`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L24)
- `SLUG` — [`L25`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L25)
- `runner` — [`L27`](../../../../../raw/code/wikify-repo/tests/test_cli.py#L27)

