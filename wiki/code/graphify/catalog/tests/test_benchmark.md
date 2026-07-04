---
title: 'Module: tests/test_benchmark.py'
type: catalog
provenance: extracted
module: tests/test_benchmark.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_benchmark`/
symbols:
  _make_graph: _make_graph().
  test_print_benchmark_no_crash: test_print_benchmark_no_crash().
  test_print_benchmark_survives_cp1252_stdout: test_print_benchmark_survives_cp1252_stdout().
  _write_graph: _write_graph().
  test_run_benchmark_returns_reduction: test_run_benchmark_returns_reduction().
  test_run_benchmark_corpus_tokens_proportional: test_run_benchmark_corpus_tokens_proportional().
  test_run_benchmark_per_question_list: test_run_benchmark_per_question_list().
  test_run_benchmark_estimates_corpus_if_no_words: test_run_benchmark_estimates_corpus_if_no_words().
  test_run_benchmark_includes_node_edge_counts: test_run_benchmark_includes_node_edge_counts().
  test_run_benchmark_rejects_oversized_graph: test_run_benchmark_rejects_oversized_graph().
  test_query_returns_positive_for_matching_question: test_query_returns_positive_for_matching_question().
  test_query_returns_zero_for_no_match: test_query_returns_zero_for_no_match().
  test_query_bfs_expands_neighbors: test_query_bfs_expands_neighbors().
  test_run_benchmark_error_on_empty_graph: test_run_benchmark_error_on_empty_graph().
  test_safe_returns_unicode_when_encodable: test_safe_returns_unicode_when_encodable().
  test_safe_falls_back_when_unencodable: test_safe_falls_back_when_unencodable().
  test_query_keeps_short_non_english_terms: test_query_keeps_short_non_english_terms().
  test_print_benchmark_error_message: test_print_benchmark_error_message().
---
# Module: [`tests/test_benchmark.py`](../../../../../raw/code/graphify/tests/test_benchmark.py)

## Functions
- `_make_graph()` — [`L11`](../../../../../raw/code/graphify/tests/test_benchmark.py#L11)
- `_write_graph(G: nx.Graph, path)` — [`L25`](../../../../../raw/code/graphify/tests/test_benchmark.py#L25)
- `test_print_benchmark_error_message(capsys)` — [`L123`](../../../../../raw/code/graphify/tests/test_benchmark.py#L123)
- `test_print_benchmark_no_crash(tmp_path, capsys)` — [`L113`](../../../../../raw/code/graphify/tests/test_benchmark.py#L113)
- `test_print_benchmark_survives_cp1252_stdout(tmp_path, monkeypatch, capsys)` — [`L154`](../../../../../raw/code/graphify/tests/test_benchmark.py#L154) — Regression: U+2500 / U+2192 used to crash with UnicodeEncodeError on cp1252.
- `test_query_bfs_expands_neighbors()` — [`L42`](../../../../../raw/code/graphify/tests/test_benchmark.py#L42)
- `test_query_keeps_short_non_english_terms()` — [`L50`](../../../../../raw/code/graphify/tests/test_benchmark.py#L50)
- `test_query_returns_positive_for_matching_question()` — [`L32`](../../../../../raw/code/graphify/tests/test_benchmark.py#L32)
- `test_query_returns_zero_for_no_match()` — [`L37`](../../../../../raw/code/graphify/tests/test_benchmark.py#L37)
- `test_run_benchmark_corpus_tokens_proportional(tmp_path)` — [`L67`](../../../../../raw/code/graphify/tests/test_benchmark.py#L67)
- `test_run_benchmark_error_on_empty_graph(tmp_path)` — [`L95`](../../../../../raw/code/graphify/tests/test_benchmark.py#L95)
- `test_run_benchmark_estimates_corpus_if_no_words(tmp_path)` — [`L88`](../../../../../raw/code/graphify/tests/test_benchmark.py#L88)
- `test_run_benchmark_includes_node_edge_counts(tmp_path)` — [`L102`](../../../../../raw/code/graphify/tests/test_benchmark.py#L102)
- `test_run_benchmark_per_question_list(tmp_path)` — [`L76`](../../../../../raw/code/graphify/tests/test_benchmark.py#L76)
- `test_run_benchmark_rejects_oversized_graph(monkeypatch, tmp_path)` — [`L175`](../../../../../raw/code/graphify/tests/test_benchmark.py#L175) — #F4: run_benchmark must refuse to read a graph.json that exceeds
- `test_run_benchmark_returns_reduction(tmp_path)` — [`L59`](../../../../../raw/code/graphify/tests/test_benchmark.py#L59)
- `test_safe_falls_back_when_unencodable()` — [`L144`](../../../../../raw/code/graphify/tests/test_benchmark.py#L144)
- `test_safe_returns_unicode_when_encodable()` — [`L134`](../../../../../raw/code/graphify/tests/test_benchmark.py#L134)

