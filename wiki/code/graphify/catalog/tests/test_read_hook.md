---
title: 'Module: tests/test_read_hook.py'
type: catalog
provenance: extracted
module: tests/test_read_hook.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_read_hook`/
symbols:
  _run: _run().
  CMD: CMD.
  test_matcher_targets_read_and_glob: test_matcher_targets_read_and_glob().
  test_silent_without_graph: test_silent_without_graph().
  test_nudges_on_source_read_with_graph: test_nudges_on_source_read_with_graph().
  test_nudge_payload_is_valid_pretooluse_json: test_nudge_payload_is_valid_pretooluse_json().
  test_silent_on_graphify_out_targets: test_silent_on_graphify_out_targets().
  test_silent_on_non_source_files: test_silent_on_non_source_files().
  test_glob_pattern_nudges: test_glob_pattern_nudges().
  test_nudges_on_framework_source: test_nudges_on_framework_source().
  test_astro_glob_nudges: test_astro_glob_nudges().
  test_silent_on_json_config: test_silent_on_json_config().
  test_nudges_on_multi_dot_source: test_nudges_on_multi_dot_source().
  test_windows_path_nudges: test_windows_path_nudges().
  test_silent_when_extension_is_on_a_directory_segment: test_silent_when_extension_is_on_a_directory_segment().
  test_fails_open_on_malformed_stdin: test_fails_open_on_malformed_stdin().
  test_never_blocks: test_never_blocks().
---
# Module: [`tests/test_read_hook.py`](../../../../../raw/code/graphify/tests/test_read_hook.py)

## Functions
- `_run(tool_input, cwd, *, graph: bool)` — [`L17`](../../../../../raw/code/graphify/tests/test_read_hook.py#L17)
- `test_astro_glob_nudges(tmp_path)` — [`L72`](../../../../../raw/code/graphify/tests/test_read_hook.py#L72)
- `test_fails_open_on_malformed_stdin(tmp_path)` — [`L105`](../../../../../raw/code/graphify/tests/test_read_hook.py#L105)
- `test_glob_pattern_nudges(tmp_path)` — [`L60`](../../../../../raw/code/graphify/tests/test_read_hook.py#L60)
- `test_matcher_targets_read_and_glob()` — [`L27`](../../../../../raw/code/graphify/tests/test_read_hook.py#L27)
- `test_never_blocks(tmp_path)` — [`L115`](../../../../../raw/code/graphify/tests/test_read_hook.py#L115) — A nudge is additionalContext only - the hook must exit 0, never deny.
- `test_nudge_payload_is_valid_pretooluse_json(tmp_path)` — [`L41`](../../../../../raw/code/graphify/tests/test_read_hook.py#L41)
- `test_nudges_on_framework_source(tmp_path)` — [`L65`](../../../../../raw/code/graphify/tests/test_read_hook.py#L65) — .astro/.vue/.svelte are real source types and must nudge (regression).
- `test_nudges_on_multi_dot_source(tmp_path)` — [`L84`](../../../../../raw/code/graphify/tests/test_read_hook.py#L84) — A real trailing extension must win on multi-dot names (the segment split):
- `test_nudges_on_source_read_with_graph(tmp_path)` — [`L36`](../../../../../raw/code/graphify/tests/test_read_hook.py#L36)
- `test_silent_on_graphify_out_targets(tmp_path)` — [`L48`](../../../../../raw/code/graphify/tests/test_read_hook.py#L48) — Reading the graph's own report must not start a go-read-the-graph loop.
- `test_silent_on_json_config(tmp_path)` — [`L77`](../../../../../raw/code/graphify/tests/test_read_hook.py#L77) — Config files must stay silent: '.json' must not match the '.js' extension.
- `test_silent_on_non_source_files(tmp_path)` — [`L54`](../../../../../raw/code/graphify/tests/test_read_hook.py#L54)
- `test_silent_when_extension_is_on_a_directory_segment(tmp_path)` — [`L98`](../../../../../raw/code/graphify/tests/test_read_hook.py#L98) — An extension that sits on a directory component, not the final segment,
- `test_silent_without_graph(tmp_path)` — [`L31`](../../../../../raw/code/graphify/tests/test_read_hook.py#L31)
- `test_windows_path_nudges(tmp_path)` — [`L92`](../../../../../raw/code/graphify/tests/test_read_hook.py#L92) — Backslash-separated paths split on the real final segment, then its ext.

## Module values
- `CMD` — [`L14`](../../../../../raw/code/graphify/tests/test_read_hook.py#L14)

