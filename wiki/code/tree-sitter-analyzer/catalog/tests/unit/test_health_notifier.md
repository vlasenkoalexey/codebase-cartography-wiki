---
title: 'Module: tests/unit/test_health_notifier.py'
type: catalog
provenance: extracted
module: tests/unit/test_health_notifier.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_health_notifier`/
symbols:
  test_stacked_channels_dispatch_to_all: test_stacked_channels_dispatch_to_all().
  test_stacked_channel_failure_does_not_stop_siblings: test_stacked_channel_failure_does_not_stop_siblings().
  _import_notifier_module: _import_notifier_module().
  test_webhook_notifier_stub_raises_not_implemented: test_webhook_notifier_stub_raises_not_implemented().
  test_stdout_notifier_writes_one_line_per_event: test_stdout_notifier_writes_one_line_per_event().
  test_stdout_notifier_handles_cold_start_event: test_stdout_notifier_handles_cold_start_event().
  test_file_notifier_appends_jsonl: test_file_notifier_appends_jsonl().
  test_file_notifier_does_not_overwrite_existing_records: test_file_notifier_does_not_overwrite_existing_records().
  test_file_notifier_creates_parent_directory: test_file_notifier_creates_parent_directory().
  test_shell_notifier_substitutes_template_tokens: test_shell_notifier_substitutes_template_tokens().
  test_shell_notifier_supports_string_template_dollar_syntax: test_shell_notifier_supports_string_template_dollar_syntax().
  test_shell_notifier_handles_unknown_tokens_safely: test_shell_notifier_handles_unknown_tokens_safely().
  test_module_exposes_build_notifier_factory: test_module_exposes_build_notifier_factory().
  test_stacked_channel_failure_does_not_stop_siblings._Boom: test_stacked_channel_failure_does_not_stop_siblings()._Boom#
  pytestmark: pytestmark.
  sample_event: sample_event().
  test_stacked_channel_failure_does_not_stop_siblings._Boom.dispatch: test_stacked_channel_failure_does_not_stop_siblings()._Boom#dispatch().
---
# Module: [`tests/unit/test_health_notifier.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py)

## Classes
### `_Boom`
- def: [`tests/unit/test_health_notifier.py:300`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L300)
- signature: `class _Boom:`
- members:
  - `dispatch(self, event)` — [`L301`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L301)
- used by: (1 test-only callers)

## Functions
- `_import_notifier_module()` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L51)
- `sample_event()` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L61)
- `test_file_notifier_appends_jsonl(tmp_path: Path, sample_event)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L115) — FileNotifier(path) appends one JSONL record per dispatch.
- `test_file_notifier_creates_parent_directory(tmp_path: Path, sample_event)` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L154) — FileNotifier auto-creates missing parent dirs (best-effort).
- `test_file_notifier_does_not_overwrite_existing_records(tmp_path: Path, sample_event)` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L136) — A second FileNotifier instance pointed at the same file must append,
- `test_module_exposes_build_notifier_factory()` — [`L318`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L318) — The module should expose a factory that maps CLI channel strings to
- `test_shell_notifier_handles_unknown_tokens_safely(sample_event)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L226) — An unknown token in the template must not crash and must not leak shell
- `test_shell_notifier_substitutes_template_tokens(sample_event)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L168) — Template tokens substituted via string.Template, NOT shell expansion.
- `test_shell_notifier_supports_string_template_dollar_syntax(sample_event)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L204) — Spec calls out `string.Template`. Some impls may use $token instead of
- `test_stacked_channel_failure_does_not_stop_siblings(tmp_path: Path, capsys, sample_event)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L290) — If one channel raises, the others must still receive the event.
- `test_stacked_channels_dispatch_to_all(tmp_path: Path, capsys, sample_event)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L270) — A composite notifier (stdout + file) sends each event to both backends.
- `test_stdout_notifier_handles_cold_start_event(capsys)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L92) — previous_grade may be None on cold start — must not crash.
- `test_stdout_notifier_writes_one_line_per_event(capsys, sample_event)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L75) — StdoutNotifier writes a single human-readable line per event,
- `test_webhook_notifier_stub_raises_not_implemented(sample_event)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L243) — Webhook is a stub for MVP. Spec hedges between 'raises' and 'logs +

## Module values
- `pytestmark` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_health_notifier.py#L45)

