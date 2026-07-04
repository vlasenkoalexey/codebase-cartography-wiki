---
title: 'Module: tests/test_label_retry.py'
type: catalog
provenance: extracted
module: tests/test_label_retry.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_label_retry`/test_label_batch_recovers_via_split_on_invalid_json().
symbols:
  test_label_batch_recovers_via_split_on_invalid_json: ''
  test_label_batch_recovers_via_split_on_invalid_json.fake_call_llm: fake_call_llm().
---
# Module: [`tests/test_label_retry.py`](../../../../../raw/code/graphify/tests/test_label_retry.py)

## Functions
- `fake_call_llm(prompt: str, **_kwargs)` — [`L28`](../../../../../raw/code/graphify/tests/test_label_retry.py#L28) — First call (4 communities): returns broken JSON to trigger retry.
- `test_label_batch_recovers_via_split_on_invalid_json(monkeypatch)` — [`L12`](../../../../../raw/code/graphify/tests/test_label_retry.py#L12) — Demonstrates the bug fix.

