---
title: 'Module: tests/test_minhash.py'
type: catalog
provenance: extracted
module: tests/test_minhash.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_minhash`/
symbols:
  _minhash_for: _minhash_for().
  test_near_duplicates_are_candidates: test_near_duplicates_are_candidates().
  test_unrelated_strings_not_candidates: test_unrelated_strings_not_candidates().
  test_query_always_returns_self: test_query_always_returns_self().
  test_duplicate_insert_raises: test_duplicate_insert_raises().
  test_identical_texts_produce_identical_hashvalues: test_identical_texts_produce_identical_hashvalues().
  test_similar_texts_share_most_hashvalues: test_similar_texts_share_most_hashvalues().
  test_unrelated_texts_share_few_hashvalues: test_unrelated_texts_share_few_hashvalues().
  test_update_mutates_hashvalues: test_update_mutates_hashvalues().
  test_optimal_params_within_budget: test_optimal_params_within_budget().
  test_optimal_params_cached: test_optimal_params_cached().
  test_dedup_import_does_not_pull_scipy_or_numpy_testing: test_dedup_import_does_not_pull_scipy_or_numpy_testing().
---
# Module: [`tests/test_minhash.py`](../../../../../raw/code/graphify/tests/test_minhash.py)

## Functions
- `_minhash_for(text: str, num_perm: int = 128)` — [`L8`](../../../../../raw/code/graphify/tests/test_minhash.py#L8) — documented in [graphify-_minhash](../../concepts/graphify-_minhash.md)
- `test_dedup_import_does_not_pull_scipy_or_numpy_testing()` — [`L95`](../../../../../raw/code/graphify/tests/test_minhash.py#L95)
- `test_duplicate_insert_raises()` — [`L71`](../../../../../raw/code/graphify/tests/test_minhash.py#L71)
- `test_identical_texts_produce_identical_hashvalues()` — [`L17`](../../../../../raw/code/graphify/tests/test_minhash.py#L17)
- `test_near_duplicates_are_candidates()` — [`L46`](../../../../../raw/code/graphify/tests/test_minhash.py#L46)
- `test_optimal_params_cached()` — [`L87`](../../../../../raw/code/graphify/tests/test_minhash.py#L87)
- `test_optimal_params_within_budget()` — [`L81`](../../../../../raw/code/graphify/tests/test_minhash.py#L81)
- `test_query_always_returns_self()` — [`L64`](../../../../../raw/code/graphify/tests/test_minhash.py#L64)
- `test_similar_texts_share_most_hashvalues()` — [`L23`](../../../../../raw/code/graphify/tests/test_minhash.py#L23)
- `test_unrelated_strings_not_candidates()` — [`L55`](../../../../../raw/code/graphify/tests/test_minhash.py#L55)
- `test_unrelated_texts_share_few_hashvalues()` — [`L30`](../../../../../raw/code/graphify/tests/test_minhash.py#L30)
- `test_update_mutates_hashvalues()` — [`L37`](../../../../../raw/code/graphify/tests/test_minhash.py#L37)

