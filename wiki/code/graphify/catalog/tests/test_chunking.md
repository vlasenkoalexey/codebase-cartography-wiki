---
title: 'Module: tests/test_chunking.py'
type: catalog
provenance: extracted
module: tests/test_chunking.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_chunking`/
symbols:
  test_estimate_file_tokens_uses_tiktoken_when_available: test_estimate_file_tokens_uses_tiktoken_when_available().
  test_estimate_file_tokens_falls_back_to_chars_when_no_tokenizer: test_estimate_file_tokens_falls_back_to_chars_when_no_tokenizer().
  _stub_with_finish: _stub_with_finish().
  _stub_chunk_result: _stub_chunk_result().
  test_corpus_parallel_runs_chunks_concurrently: test_corpus_parallel_runs_chunks_concurrently().
  test_corpus_parallel_sequential_when_max_concurrency_is_one: test_corpus_parallel_sequential_when_max_concurrency_is_one().
  test_corpus_parallel_merge_order_is_submission_order_not_completion: test_corpus_parallel_merge_order_is_submission_order_not_completion().
  test_corpus_parallel_continues_after_chunk_failure: test_corpus_parallel_continues_after_chunk_failure().
  test_corpus_parallel_legacy_mode_when_token_budget_is_none: test_corpus_parallel_legacy_mode_when_token_budget_is_none().
  test_corpus_parallel_token_budget_default_packs_files: test_corpus_parallel_token_budget_default_packs_files().
  test_adaptive_retry_returns_directly_when_not_truncated: test_adaptive_retry_returns_directly_when_not_truncated().
  test_adaptive_retry_splits_when_finish_reason_length: test_adaptive_retry_splits_when_finish_reason_length().
  test_adaptive_retry_recurses_for_persistent_truncation: test_adaptive_retry_recurses_for_persistent_truncation().
  test_adaptive_retry_caps_at_max_depth: test_adaptive_retry_caps_at_max_depth().
  test_adaptive_retry_single_file_truncation_does_not_recurse: test_adaptive_retry_single_file_truncation_does_not_recurse().
  test_corpus_parallel_uses_adaptive_retry: test_corpus_parallel_uses_adaptive_retry().
  test_corpus_parallel_runs_chunks_concurrently.slow_extract: test_corpus_parallel_runs_chunks_concurrently().slow_extract().
  test_corpus_parallel_sequential_when_max_concurrency_is_one.record: test_corpus_parallel_sequential_when_max_concurrency_is_one().record().
  test_corpus_parallel_continues_after_chunk_failure.maybe_fail: test_corpus_parallel_continues_after_chunk_failure().maybe_fail().
  test_corpus_parallel_legacy_mode_when_token_budget_is_none.record: test_corpus_parallel_legacy_mode_when_token_budget_is_none().record().
  test_corpus_parallel_token_budget_default_packs_files.record: test_corpus_parallel_token_budget_default_packs_files().record().
  test_adaptive_retry_returns_directly_when_not_truncated.stub: test_adaptive_retry_returns_directly_when_not_truncated().stub().
  test_adaptive_retry_splits_when_finish_reason_length.stub: test_adaptive_retry_splits_when_finish_reason_length().stub().
  test_adaptive_retry_recurses_for_persistent_truncation.stub: test_adaptive_retry_recurses_for_persistent_truncation().stub().
  test_adaptive_retry_caps_at_max_depth.always_truncate: test_adaptive_retry_caps_at_max_depth().always_truncate().
  test_adaptive_retry_single_file_truncation_does_not_recurse.stub: test_adaptive_retry_single_file_truncation_does_not_recurse().stub().
  test_corpus_parallel_uses_adaptive_retry.stub: test_corpus_parallel_uses_adaptive_retry().stub().
  test_pack_chunks_packs_small_files_together: test_pack_chunks_packs_small_files_together().
  test_pack_chunks_starts_new_chunk_when_budget_would_overflow: test_pack_chunks_starts_new_chunk_when_budget_would_overflow().
  test_pack_chunks_groups_by_directory: test_pack_chunks_groups_by_directory().
  test_pack_chunks_oversized_file_gets_its_own_chunk: test_pack_chunks_oversized_file_gets_its_own_chunk().
  test_pack_chunks_rejects_non_positive_budget: test_pack_chunks_rejects_non_positive_budget().
  test_corpus_parallel_merge_order_is_submission_order_not_completion.latency_skewed: test_corpus_parallel_merge_order_is_submission_order_not_completion().latency_skewed().
  no_tokenizer: no_tokenizer().
---
# Module: [`tests/test_chunking.py`](../../../../../raw/code/graphify/tests/test_chunking.py)

## Functions
- `_stub_chunk_result(file_count: int, idx: int)` — [`L142`](../../../../../raw/code/graphify/tests/test_chunking.py#L142) — Build a deterministic fake extraction result for a chunk.
- `_stub_with_finish(file_count: int, finish_reason: str = "stop")` — [`L329`](../../../../../raw/code/graphify/tests/test_chunking.py#L329) — Build a stub extraction result with a controllable finish_reason.
- `always_truncate(chunk, **kwargs)` — [`L428`](../../../../../raw/code/graphify/tests/test_chunking.py#L428)
- `latency_skewed(chunk, **kwargs)` — [`L216`](../../../../../raw/code/graphify/tests/test_chunking.py#L216)
- `maybe_fail(chunk, **kwargs)` — [`L263`](../../../../../raw/code/graphify/tests/test_chunking.py#L263)
- `no_tokenizer()` — [`L10`](../../../../../raw/code/graphify/tests/test_chunking.py#L10) — Force the chars/4 fallback so packing math is deterministic regardless
- `record(chunk, **kwargs)` — [`L191`](../../../../../raw/code/graphify/tests/test_chunking.py#L191)
- `record(chunk, **kwargs)` — [`L291`](../../../../../raw/code/graphify/tests/test_chunking.py#L291)
- `record(chunk, **kwargs)` — [`L315`](../../../../../raw/code/graphify/tests/test_chunking.py#L315)
- `slow_extract(chunk, **kwargs)` — [`L163`](../../../../../raw/code/graphify/tests/test_chunking.py#L163)
- `stub(chunk, **kwargs)` — [`L351`](../../../../../raw/code/graphify/tests/test_chunking.py#L351)
- `stub(chunk, **kwargs)` — [`L375`](../../../../../raw/code/graphify/tests/test_chunking.py#L375)
- `stub(chunk, **kwargs)` — [`L401`](../../../../../raw/code/graphify/tests/test_chunking.py#L401)
- `stub(chunk, **kwargs)` — [`L452`](../../../../../raw/code/graphify/tests/test_chunking.py#L452)
- `stub(chunk, **kwargs)` — [`L478`](../../../../../raw/code/graphify/tests/test_chunking.py#L478)
- `test_adaptive_retry_caps_at_max_depth(tmp_path, capsys)` — [`L417`](../../../../../raw/code/graphify/tests/test_chunking.py#L417) — If everything truncates, retries stop at max_depth — partial result
- `test_adaptive_retry_recurses_for_persistent_truncation(tmp_path)` — [`L390`](../../../../../raw/code/graphify/tests/test_chunking.py#L390) — When even the half-chunk truncates, split again. With 8 files and a
- `test_adaptive_retry_returns_directly_when_not_truncated(tmp_path)` — [`L341`](../../../../../raw/code/graphify/tests/test_chunking.py#L341) — No retry when finish_reason='stop' — single call, result passes through.
- `test_adaptive_retry_single_file_truncation_does_not_recurse(tmp_path, capsys)` — [`L443`](../../../../../raw/code/graphify/tests/test_chunking.py#L443) — A single file that truncates can't be split further — surface a
- `test_adaptive_retry_splits_when_finish_reason_length(tmp_path)` — [`L364`](../../../../../raw/code/graphify/tests/test_chunking.py#L364) — finish_reason='length' triggers split-in-half. Both halves succeed
- `test_corpus_parallel_continues_after_chunk_failure(tmp_path, capsys)` — [`L251`](../../../../../raw/code/graphify/tests/test_chunking.py#L251) — A single chunk raising should be logged but not abort the run.
- `test_corpus_parallel_legacy_mode_when_token_budget_is_none(tmp_path)` — [`L280`](../../../../../raw/code/graphify/tests/test_chunking.py#L280) — token_budget=None should fall back to legacy fixed-count chunking.
- `test_corpus_parallel_merge_order_is_submission_order_not_completion(tmp_path)` — [`L204`](../../../../../raw/code/graphify/tests/test_chunking.py#L204) — #1632: merged node/edge order must be deterministic (submission order),
- `test_corpus_parallel_runs_chunks_concurrently(tmp_path)` — [`L153`](../../../../../raw/code/graphify/tests/test_chunking.py#L153) — With max_concurrency > 1, total wall time should be ~max(chunk times),
- `test_corpus_parallel_sequential_when_max_concurrency_is_one(tmp_path)` — [`L180`](../../../../../raw/code/graphify/tests/test_chunking.py#L180) — max_concurrency=1 should run sequentially (no thread pool).
- `test_corpus_parallel_token_budget_default_packs_files(tmp_path)` — [`L304`](../../../../../raw/code/graphify/tests/test_chunking.py#L304) — With the default token_budget, many tiny files pack into one chunk.
- `test_corpus_parallel_uses_adaptive_retry(tmp_path)` — [`L466`](../../../../../raw/code/graphify/tests/test_chunking.py#L466) — End-to-end: extract_corpus_parallel routes through adaptive retry,
- `test_estimate_file_tokens_falls_back_to_chars_when_no_tokenizer(tmp_path)` — [`L127`](../../../../../raw/code/graphify/tests/test_chunking.py#L127) — Without tiktoken installed, the estimator falls back to chars/4.
- `test_estimate_file_tokens_uses_tiktoken_when_available(tmp_path)` — [`L110`](../../../../../raw/code/graphify/tests/test_chunking.py#L110) — When tiktoken is installed, the estimator should call into it for
- `test_pack_chunks_groups_by_directory(tmp_path)` — [`L58`](../../../../../raw/code/graphify/tests/test_chunking.py#L58) — Files in the same directory should land in the same chunk when they fit.
- `test_pack_chunks_oversized_file_gets_its_own_chunk(tmp_path, no_tokenizer)` — [`L86`](../../../../../raw/code/graphify/tests/test_chunking.py#L86) — A file larger than the budget can't be split — it goes alone in a chunk.
- `test_pack_chunks_packs_small_files_together(tmp_path)` — [`L22`](../../../../../raw/code/graphify/tests/test_chunking.py#L22) — Many small files should land in a single chunk, not one chunk per file.
- `test_pack_chunks_rejects_non_positive_budget(tmp_path)` — [`L100`](../../../../../raw/code/graphify/tests/test_chunking.py#L100)
- `test_pack_chunks_starts_new_chunk_when_budget_would_overflow(tmp_path, no_tokenizer)` — [`L37`](../../../../../raw/code/graphify/tests/test_chunking.py#L37) — When the next file would push the chunk past the budget, start a new chunk.

