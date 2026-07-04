---
title: 'Module: tests/test_office_limits.py'
type: catalog
provenance: extracted
module: tests/test_office_limits.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_office_limits`/
symbols:
  test_converters_return_empty_for_bomb: test_converters_return_empty_for_bomb().
  test_zip_ratio_bomb_rejected: test_zip_ratio_bomb_rejected().
  test_legit_zip_passes: test_legit_zip_passes().
  _write_zip: _write_zip().
  test_file_within_size_cap: test_file_within_size_cap().
  test_non_zip_rejected: test_non_zip_rejected().
  test_legit_multi_member_passes_streaming: test_legit_multi_member_passes_streaming().
  test_streaming_ceiling_rejects_oversized_actual: test_streaming_ceiling_rejects_oversized_actual().
  test_pdf_over_cap_returns_empty: test_pdf_over_cap_returns_empty().
---
# Module: [`tests/test_office_limits.py`](../../../../../raw/code/graphify/tests/test_office_limits.py)

## Functions
- `_write_zip(path, name, payload)` — [`L12`](../../../../../raw/code/graphify/tests/test_office_limits.py#L12)
- `test_converters_return_empty_for_bomb(tmp_path)` — [`L45`](../../../../../raw/code/graphify/tests/test_office_limits.py#L45) — The live converters bail out (return "") on a bomb before parsing.
- `test_file_within_size_cap(tmp_path)` — [`L17`](../../../../../raw/code/graphify/tests/test_office_limits.py#L17)
- `test_legit_multi_member_passes_streaming(tmp_path)` — [`L54`](../../../../../raw/code/graphify/tests/test_office_limits.py#L54) — A normal multi-member office zip passes the streaming-ceiling pass.
- `test_legit_zip_passes(tmp_path)` — [`L33`](../../../../../raw/code/graphify/tests/test_office_limits.py#L33)
- `test_non_zip_rejected(tmp_path)` — [`L39`](../../../../../raw/code/graphify/tests/test_office_limits.py#L39)
- `test_pdf_over_cap_returns_empty(tmp_path, monkeypatch)` — [`L81`](../../../../../raw/code/graphify/tests/test_office_limits.py#L81) — A PDF larger than the raw cap is skipped before pypdf opens it.
- `test_streaming_ceiling_rejects_oversized_actual(tmp_path, monkeypatch)` — [`L64`](../../../../../raw/code/graphify/tests/test_office_limits.py#L64) — With a low decompressed cap, content whose actual bytes exceed it is rejected.
- `test_zip_ratio_bomb_rejected(tmp_path)` — [`L25`](../../../../../raw/code/graphify/tests/test_office_limits.py#L25) — A tiny file that expands far past the ratio threshold is rejected.

