---
title: 'Module: tests/test_extract_cli.py'
type: catalog
provenance: extracted
module: tests/test_extract_cli.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_extract_cli`/
symbols:
  test_extract_exits_nonzero_when_all_semantic_chunks_fail: test_extract_exits_nonzero_when_all_semantic_chunks_fail().
  test_extract_succeeds_when_at_least_one_chunk_completes: test_extract_succeeds_when_at_least_one_chunk_completes().
  test_extract_codeonly_succeeds_without_api_key: test_extract_codeonly_succeeds_without_api_key().
  test_extract_out_keeps_project_root_clean: test_extract_out_keeps_project_root_clean().
  test_extract_without_key_still_errors_when_docs_present: test_extract_without_key_still_errors_when_docs_present().
  _make_corpus: _make_corpus().
  _clear_backend_keys: _clear_backend_keys().
  test_extract_timing_flag_emits_stage_timings: test_extract_timing_flag_emits_stage_timings().
  _code_only_corpus: _code_only_corpus().
  test_extract_exits_nonzero_when_all_semantic_chunks_fail._all_chunks_failed: test_extract_exits_nonzero_when_all_semantic_chunks_fail()._all_chunks_failed().
  test_extract_succeeds_when_at_least_one_chunk_completes._one_chunk_succeeded: test_extract_succeeds_when_at_least_one_chunk_completes()._one_chunk_succeeded().
---
# Module: [`tests/test_extract_cli.py`](../../../../../raw/code/graphify/tests/test_extract_cli.py)

## Functions
- `_all_chunks_failed(paths, **kwargs)` — [`L42`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L42)
- `_clear_backend_keys(monkeypatch)` — [`L135`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L135) — Clear every env var that detect_backend() or _get_backend_api_key() reads.
- `_code_only_corpus(tmp_path)` — [`L126`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L126) — A corpus with only code — no docs/papers/images.
- `_make_corpus(tmp_path)` — [`L9`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L9) — Minimal corpus: one Go code file + one Markdown doc.
- `_one_chunk_succeeded(paths, **kwargs)` — [`L90`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L90)
- `test_extract_codeonly_succeeds_without_api_key(monkeypatch, tmp_path)` — [`L148`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L148) — A code-only corpus must run with no LLM API key.
- `test_extract_exits_nonzero_when_all_semantic_chunks_fail(monkeypatch, tmp_path, capsys)` — [`L20`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L20) — When every semantic chunk errors (e.g. backend SDK not installed),
- `test_extract_out_keeps_project_root_clean(monkeypatch, tmp_path)` — [`L175`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L175) — `extract --out DIR` routes every artifact to DIR/graphify-out/ and the
- `test_extract_succeeds_when_at_least_one_chunk_completes(monkeypatch, tmp_path)` — [`L81`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L81) — Sanity counter-test: a successful chunk run keeps exit 0. Confirms the
- `test_extract_timing_flag_emits_stage_timings(monkeypatch, tmp_path, capsys)` — [`L240`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L240) — --timing prints per-stage `[graphify timing]` lines to stderr (#1490); omitting
- `test_extract_without_key_still_errors_when_docs_present(monkeypatch, tmp_path, capsys)` — [`L212`](../../../../../raw/code/graphify/tests/test_extract_cli.py#L212) — Key requirement still fires when semantic work is needed.

