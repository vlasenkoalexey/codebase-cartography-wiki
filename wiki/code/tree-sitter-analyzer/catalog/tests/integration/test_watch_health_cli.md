---
title: 'Module: tests/integration/test_watch_health_cli.py'
type: catalog
provenance: extracted
module: tests/integration/test_watch_health_cli.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.test_watch_health_cli`/
symbols:
  test_file_modify_triggers_reevaluation: test_file_modify_triggers_reevaluation().
  test_cli_args_flow_into_runner_config: test_cli_args_flow_into_runner_config().
  _create_parser: _create_parser().
  _spawn_runner: _spawn_runner().
  _spawn_runner._FunctionRunner.start: _spawn_runner()._FunctionRunner#start().
  _spawn_runner._FunctionRunner.stop: _spawn_runner()._FunctionRunner#stop().
  test_watch_health_daemon_starts_and_stops_clean_on_sigint: test_watch_health_daemon_starts_and_stops_clean_on_sigint().
  _FunctionRunner._thread: _FunctionRunner#_thread.
  _spawn_runner._FunctionRunner._go: _spawn_runner()._FunctionRunner#_go().
  _import_runner: _import_runner().
  test_watch_health_cli_flag_parsed: test_watch_health_cli_flag_parsed().
  test_watch_health_all_siblings_parsed: test_watch_health_all_siblings_parsed().
  test_threshold_grade_rejects_invalid_values: test_threshold_grade_rejects_invalid_values().
  _FunctionRunner._stop_event: _FunctionRunner#_stop_event.
  _spawn_runner._FunctionRunner: _spawn_runner()._FunctionRunner#
  pytestmark: pytestmark.
  _spawn_runner._FunctionRunner.__init__: _spawn_runner()._FunctionRunner#__init__().
---
# Module: [`tests/integration/test_watch_health_cli.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py)

## Classes
### `_FunctionRunner`
- def: [`tests/integration/test_watch_health_cli.py:154`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L154)
- signature: `class _FunctionRunner:`
- members:
  - `start(self)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L159)
  - `stop(self, timeout: float = 5)` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L166)
- protocol/private: `__init__`[`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L155), `_go`[`L160`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L160), `_stop_event`[`L157`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L157), `_thread`[`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L156)
- used by: (1 test-only callers)

## Functions
- `_create_parser()` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L44)
- `_import_runner()` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L52) — Find the watch-health runner entrypoint.
- `_spawn_runner(runner_target, project_root: Path, **kwargs)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L136) — Instantiate the runner (class or factory) and return an object that
- `test_cli_args_flow_into_runner_config(tmp_path: Path)` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L315) — Args parsed from CLI → runner accepts them as kwargs.
- `test_file_modify_triggers_reevaluation(tmp_path: Path)` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L231) — Modifying a watched file → after debounce, HealthHistory has a new row.
- `test_threshold_grade_rejects_invalid_values()` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L126) — --threshold-grade must constrain to A|B|C|D|F.
- `test_watch_health_all_siblings_parsed(tmp_path: Path)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L82) — All --watch-health sibling flags must parse without errors.
- `test_watch_health_cli_flag_parsed()` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L72) — --watch-health and --threshold-grade are recognized by the argparse builder.
- `test_watch_health_daemon_starts_and_stops_clean_on_sigint(tmp_path: Path)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L174) — Daemon starts in a background thread, stops cleanly on .stop(),

## Module values
- `pytestmark` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/integration/test_watch_health_cli.py#L38)

