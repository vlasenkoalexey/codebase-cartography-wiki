---
title: 'Module: tests/test_id_normalization_contract.py'
type: catalog
provenance: extracted
module: tests/test_id_normalization_contract.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_id_normalization_contract`/
symbols:
  test_both_callers_share_one_implementation: test_both_callers_share_one_implementation().
  test_make_id_matches_normalize_id: test_make_id_matches_normalize_id().
  test_normalize_id_is_idempotent: test_normalize_id_is_idempotent().
  test_make_id_joins_then_normalizes: test_make_id_joins_then_normalizes().
  test_normalized_ids_are_safe_node_ids: test_normalized_ids_are_safe_node_ids().
  test_property_make_id_equals_normalize_id: test_property_make_id_equals_normalize_id().
  CONTRACT_CASES: CONTRACT_CASES.
  test_unicode_identifiers_do_not_collapse_to_empty: test_unicode_identifiers_do_not_collapse_to_empty().
  test_property_normalize_id_idempotent: test_property_normalize_id_idempotent().
  hypothesis: hypothesis.
---
# Module: [`tests/test_id_normalization_contract.py`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py)

## Functions
- `test_both_callers_share_one_implementation()` — [`L87`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py#L87) — Guard against re-forking: the two public callers must resolve to the same
- `test_make_id_joins_then_normalizes()` — [`L60`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py#L60) — Multi-part make_id == normalize_id of the joined parts (the builder only
- `test_make_id_matches_normalize_id(raw)` — [`L46`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py#L46) — The AST id-maker and the builder's reconciler must agree, char for char.
- `test_normalize_id_is_idempotent(raw)` — [`L55`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py#L55)
- `test_normalized_ids_are_safe_node_ids()` — [`L78`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py#L78) — Output is lowercase and contains no path/punctuation separators.
- `test_property_make_id_equals_normalize_id(s)` — [`L112`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py#L112)
- `test_property_normalize_id_idempotent(s)` — [`L117`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py#L117)
- `test_unicode_identifiers_do_not_collapse_to_empty()` — [`L70`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py#L70) — #811: non-ASCII identifiers must yield distinct, non-empty IDs rather than

## Module values
- `CONTRACT_CASES` — [`L27`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py#L27)
- `hypothesis` — [`L106`](../../../../../raw/code/graphify/tests/test_id_normalization_contract.py#L106)

