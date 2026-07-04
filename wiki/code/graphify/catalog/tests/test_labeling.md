---
title: 'Module: tests/test_labeling.py'
type: catalog
provenance: extracted
module: tests/test_labeling.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_labeling`/
symbols:
  _graph: _graph().
  test_label_communities_happy_path: test_label_communities_happy_path().
  test_label_communities_passes_model_override: test_label_communities_passes_model_override().
  test_label_communities_batches_when_over_batch_size: test_label_communities_batches_when_over_batch_size().
  test_label_communities_partial_batch_failure_keeps_successful_batches: test_label_communities_partial_batch_failure_keeps_successful_batches().
  test_label_communities_all_batches_fail_raises: test_label_communities_all_batches_fail_raises().
  test_label_communities_max_communities_caps_total: test_label_communities_max_communities_caps_total().
  test_label_communities_parallel_matches_sequential: test_label_communities_parallel_matches_sequential().
  test_label_communities_batch_size_controls_batch_count: test_label_communities_batch_size_controls_batch_count().
  test_label_communities_runs_batches_concurrently: test_label_communities_runs_batches_concurrently().
  test_label_communities_forces_serial_for_ollama: test_label_communities_forces_serial_for_ollama().
  test_label_cli_passes_model_override: test_label_cli_passes_model_override().
  test_label_cli_missing_only_preserves_existing_labels: test_label_cli_missing_only_preserves_existing_labels().
  test_label_communities_partial_reply_fills_placeholder: test_label_communities_partial_reply_fills_placeholder().
  test_label_communities_strips_code_fences: test_label_communities_strips_code_fences().
  test_label_communities_malformed_raises: test_label_communities_malformed_raises().
  test_generate_community_labels_degrades_on_error: test_generate_community_labels_degrades_on_error().
  test_generate_community_labels_no_backend: test_generate_community_labels_no_backend().
  test_generate_community_labels_success: test_generate_community_labels_success().
  test_gods_as_dicts_do_not_crash: test_gods_as_dicts_do_not_crash().
  test_empty_communities_returns_placeholders: test_empty_communities_returns_placeholders().
  _peak_tracker: _peak_tracker().
  _wide_graph: _wide_graph().
  _many_communities: _many_communities().
  test_label_communities_happy_path.fake_call: test_label_communities_happy_path().fake_call().
  test_label_communities_passes_model_override.fake_call: test_label_communities_passes_model_override().fake_call().
  test_label_cli_passes_model_override.fake_generate: test_label_cli_passes_model_override().fake_generate().
  test_label_cli_missing_only_preserves_existing_labels.fake_generate: test_label_cli_missing_only_preserves_existing_labels().fake_generate().
  test_empty_communities_returns_placeholders.fake_call: test_empty_communities_returns_placeholders().fake_call().
  test_label_communities_batches_when_over_batch_size.fake_call: test_label_communities_batches_when_over_batch_size().fake_call().
  test_label_communities_partial_batch_failure_keeps_successful_batches.fake_call: test_label_communities_partial_batch_failure_keeps_successful_batches().fake_call().
  test_label_communities_all_batches_fail_raises.always_fail: test_label_communities_all_batches_fail_raises().always_fail().
  test_label_communities_max_communities_caps_total.fake_call: test_label_communities_max_communities_caps_total().fake_call().
  test_label_communities_parallel_matches_sequential.fake_batch: test_label_communities_parallel_matches_sequential().fake_batch().
  test_label_communities_batch_size_controls_batch_count.fake_batch: test_label_communities_batch_size_controls_batch_count().fake_batch().
  _peak_tracker.fake_batch: _peak_tracker().fake_batch().
---
# Module: [`tests/test_labeling.py`](../../../../../raw/code/graphify/tests/test_labeling.py)

## Functions
- `_graph()` — [`L15`](../../../../../raw/code/graphify/tests/test_labeling.py#L15)
- `_many_communities(n)` — [`L343`](../../../../../raw/code/graphify/tests/test_labeling.py#L343)
- `_peak_tracker()` — [`L381`](../../../../../raw/code/graphify/tests/test_labeling.py#L381)
- `_wide_graph(n_communities: int)` — [`L251`](../../../../../raw/code/graphify/tests/test_labeling.py#L251)
- `always_fail(prompt, *, backend, max_tokens=200)` — [`L310`](../../../../../raw/code/graphify/tests/test_labeling.py#L310)
- `fake_batch(batch_cids, batch_lines, *, backend, model=None)` — [`L357`](../../../../../raw/code/graphify/tests/test_labeling.py#L357)
- `fake_batch(batch_cids, batch_lines, *, backend, model=None)` — [`L370`](../../../../../raw/code/graphify/tests/test_labeling.py#L370)
- `fake_batch(batch_cids, batch_lines, *, backend, model=None)` — [`L385`](../../../../../raw/code/graphify/tests/test_labeling.py#L385)
- `fake_call(prompt, *, backend, max_tokens=200)` — [`L31`](../../../../../raw/code/graphify/tests/test_labeling.py#L31)
- `fake_call(prompt, *, backend, max_tokens=200, model=None)` — [`L50`](../../../../../raw/code/graphify/tests/test_labeling.py#L50)
- `fake_call(p, *, backend, max_tokens=200)` — [`L232`](../../../../../raw/code/graphify/tests/test_labeling.py#L232)
- `fake_call(prompt, *, backend, max_tokens=200)` — [`L266`](../../../../../raw/code/graphify/tests/test_labeling.py#L266)
- `fake_call(prompt, *, backend, max_tokens=200)` — [`L288`](../../../../../raw/code/graphify/tests/test_labeling.py#L288)
- `fake_call(prompt, *, backend, max_tokens=200)` — [`L325`](../../../../../raw/code/graphify/tests/test_labeling.py#L325)
- `fake_generate(G, communities, *, backend=None, model=None, gods=None, quiet=False, max_concurrency=4, batch_size=100)` — [`L84`](../../../../../raw/code/graphify/tests/test_labeling.py#L84)
- `fake_generate(G, communities, *, backend=None, model=None, gods=None, quiet=False, max_concurrency=4, batch_size=100)` — [`L145`](../../../../../raw/code/graphify/tests/test_labeling.py#L145)
- `test_empty_communities_returns_placeholders(monkeypatch)` — [`L228`](../../../../../raw/code/graphify/tests/test_labeling.py#L228)
- `test_generate_community_labels_degrades_on_error(monkeypatch)` — [`L192`](../../../../../raw/code/graphify/tests/test_labeling.py#L192)
- `test_generate_community_labels_no_backend(monkeypatch)` — [`L201`](../../../../../raw/code/graphify/tests/test_labeling.py#L201)
- `test_generate_community_labels_success(monkeypatch)` — [`L209`](../../../../../raw/code/graphify/tests/test_labeling.py#L209)
- `test_gods_as_dicts_do_not_crash(monkeypatch)` — [`L218`](../../../../../raw/code/graphify/tests/test_labeling.py#L218) — god_nodes() returns list[dict] with an 'id' key, not bare ids.
- `test_label_cli_missing_only_preserves_existing_labels(tmp_path, monkeypatch)` — [`L123`](../../../../../raw/code/graphify/tests/test_labeling.py#L123)
- `test_label_cli_passes_model_override(tmp_path, monkeypatch)` — [`L67`](../../../../../raw/code/graphify/tests/test_labeling.py#L67)
- `test_label_communities_all_batches_fail_raises(monkeypatch)` — [`L307`](../../../../../raw/code/graphify/tests/test_labeling.py#L307)
- `test_label_communities_batch_size_controls_batch_count(monkeypatch)` — [`L366`](../../../../../raw/code/graphify/tests/test_labeling.py#L366)
- `test_label_communities_batches_when_over_batch_size(monkeypatch)` — [`L262`](../../../../../raw/code/graphify/tests/test_labeling.py#L262)
- `test_label_communities_forces_serial_for_ollama(monkeypatch)` — [`L405`](../../../../../raw/code/graphify/tests/test_labeling.py#L405) — ollama/claude-cli must stay serial regardless of --max-concurrency.
- `test_label_communities_happy_path(monkeypatch)` — [`L26`](../../../../../raw/code/graphify/tests/test_labeling.py#L26)
- `test_label_communities_malformed_raises(monkeypatch)` — [`L184`](../../../../../raw/code/graphify/tests/test_labeling.py#L184)
- `test_label_communities_max_communities_caps_total(monkeypatch)` — [`L319`](../../../../../raw/code/graphify/tests/test_labeling.py#L319)
- `test_label_communities_parallel_matches_sequential(monkeypatch)` — [`L353`](../../../../../raw/code/graphify/tests/test_labeling.py#L353) — Concurrency must not change the result: same cid->name map either way.
- `test_label_communities_partial_batch_failure_keeps_successful_batches(monkeypatch)` — [`L284`](../../../../../raw/code/graphify/tests/test_labeling.py#L284)
- `test_label_communities_partial_reply_fills_placeholder(monkeypatch)` — [`L165`](../../../../../raw/code/graphify/tests/test_labeling.py#L165)
- `test_label_communities_passes_model_override(monkeypatch)` — [`L46`](../../../../../raw/code/graphify/tests/test_labeling.py#L46)
- `test_label_communities_runs_batches_concurrently(monkeypatch)` — [`L397`](../../../../../raw/code/graphify/tests/test_labeling.py#L397)
- `test_label_communities_strips_code_fences(monkeypatch)` — [`L174`](../../../../../raw/code/graphify/tests/test_labeling.py#L174)

