---
title: 'Module: tests/test_transcribe.py'
type: catalog
provenance: extracted
module: tests/test_transcribe.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_transcribe`/test_
symbols:
  test_video_extensions_set: video_extensions_set().
  test_build_whisper_prompt_no_nodes: build_whisper_prompt_no_nodes().
  test_build_whisper_prompt_env_override: build_whisper_prompt_env_override().
  test_build_whisper_prompt_returns_topic_string: build_whisper_prompt_returns_topic_string().
  test_build_whisper_prompt_nodes_without_labels: build_whisper_prompt_nodes_without_labels().
  test_transcribe_uses_cache: transcribe_uses_cache().
  test_transcribe_force_reruns: transcribe_force_reruns().
  test_transcribe_missing_faster_whisper: transcribe_missing_faster_whisper().
  test_transcribe_all_empty: transcribe_all_empty().
  test_transcribe_all_uses_cache: transcribe_all_uses_cache().
  test_transcribe_all_skips_failed: transcribe_all_skips_failed().
  test_transcribe_all_skips_failed.raise_import: transcribe_all_skips_failed().raise_import().
---
# Module: [`tests/test_transcribe.py`](../../../../../raw/code/graphify/tests/test_transcribe.py)

## Functions
- `raise_import(*args, **kwargs)` — [`L141`](../../../../../raw/code/graphify/tests/test_transcribe.py#L141)
- `test_build_whisper_prompt_env_override(monkeypatch)` — [`L40`](../../../../../raw/code/graphify/tests/test_transcribe.py#L40) — GRAPHIFY_WHISPER_PROMPT env var short-circuits LLM call.
- `test_build_whisper_prompt_no_nodes()` — [`L34`](../../../../../raw/code/graphify/tests/test_transcribe.py#L34) — Empty god_nodes returns fallback prompt.
- `test_build_whisper_prompt_nodes_without_labels()` — [`L57`](../../../../../raw/code/graphify/tests/test_transcribe.py#L57) — Nodes missing 'label' keys are safely skipped.
- `test_build_whisper_prompt_returns_topic_string()` — [`L47`](../../../../../raw/code/graphify/tests/test_transcribe.py#L47) — Returns a topic-based prompt from god node labels — no LLM call.
- `test_transcribe_all_empty()` — [`L117`](../../../../../raw/code/graphify/tests/test_transcribe.py#L117) — Empty input returns empty list without error.
- `test_transcribe_all_skips_failed(tmp_path)` — [`L136`](../../../../../raw/code/graphify/tests/test_transcribe.py#L136) — transcribe_all() warns and skips files that fail to transcribe.
- `test_transcribe_all_uses_cache(tmp_path)` — [`L122`](../../../../../raw/code/graphify/tests/test_transcribe.py#L122) — transcribe_all() returns cached paths for already-transcribed files.
- `test_transcribe_force_reruns(tmp_path)` — [`L81`](../../../../../raw/code/graphify/tests/test_transcribe.py#L81) — force=True re-transcribes even when cache exists.
- `test_transcribe_missing_faster_whisper(tmp_path)` — [`L103`](../../../../../raw/code/graphify/tests/test_transcribe.py#L103) — ImportError propagates when faster_whisper is not installed.
- `test_transcribe_uses_cache(tmp_path)` — [`L68`](../../../../../raw/code/graphify/tests/test_transcribe.py#L68) — If transcript already exists, transcribe() returns cached path without running Whisper.
- `test_video_extensions_set()` — [`L22`](../../../../../raw/code/graphify/tests/test_transcribe.py#L22)

