---
title: 'Module: tests/test_charmap_encoding.py'
type: catalog
provenance: extracted
module: tests/test_charmap_encoding.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_charmap_encoding`/
symbols:
  TestSubprocessEncoding.test_subprocess_called_with_utf8_encoding: TestSubprocessEncoding#test_subprocess_called_with_utf8_encoding().
  TestSubprocessEncoding.test_subprocess_does_not_use_text_true_without_encoding: TestSubprocessEncoding#test_subprocess_does_not_use_text_true_without_encoding().
  TestSubprocessEncoding.test_unicode_chars_survive_subprocess_roundtrip: TestSubprocessEncoding#test_unicode_chars_survive_subprocess_roundtrip().
  TestSubprocessEncoding._make_completed: TestSubprocessEncoding#_make_completed().
  TestSubprocessEncoding.test_call_llm_claude_cli_subprocess_encoding: TestSubprocessEncoding#test_call_llm_claude_cli_subprocess_encoding().
  TestSubstitutionValidation.test_read_files_produces_utf8_safe_prompt: TestSubstitutionValidation#test_read_files_produces_utf8_safe_prompt().
  TestSubstitutionValidation.test_cp1252_would_fail_but_utf8_succeeds: TestSubstitutionValidation#test_cp1252_would_fail_but_utf8_succeeds().
  TestSubstitutionValidation.test_subprocess_encoding_kwarg_in_extract_files_direct: TestSubstitutionValidation#test_subprocess_encoding_kwarg_in_extract_files_direct().
  _UNICODE_CONTENT: _UNICODE_CONTENT.
  TestSubstitutionValidation._UNICODE_CHARS: TestSubstitutionValidation#_UNICODE_CHARS.
  TestLoudChunkFailure.test_failure_count_in_merged_result: TestLoudChunkFailure#test_failure_count_in_merged_result().
  TestLoudChunkFailure.test_summary_printed_when_chunks_fail: TestLoudChunkFailure#test_summary_printed_when_chunks_fail().
  TestLoudChunkFailure.test_no_false_alarm_when_all_chunks_succeed: TestLoudChunkFailure#test_no_false_alarm_when_all_chunks_succeed().
  _ENVELOPE: _ENVELOPE.
  TestSubprocessEncoding: TestSubprocessEncoding#
  TestLoudChunkFailure: TestLoudChunkFailure#
  TestSubstitutionValidation: TestSubstitutionValidation#
---
# Module: [`tests/test_charmap_encoding.py`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py)

## Classes
### `TestLoudChunkFailure`
- def: [`tests/test_charmap_encoding.py:141`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L141)
- doc: extract_corpus_parallel must surface chunk failures loudly — either via
- signature: `class TestLoudChunkFailure:`
- members:
  - `test_failure_count_in_merged_result(self, monkeypatch, tmp_path)` — [`L147`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L147) — When chunks fail, extract_corpus_parallel must record failed_chunks > 0
  - `test_no_false_alarm_when_all_chunks_succeed(self, monkeypatch, tmp_path, capsys)` — [`L191`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L191) — When all chunks succeed, failed_chunks must be 0 and no failure
  - `test_summary_printed_when_chunks_fail(self, monkeypatch, tmp_path, capsys)` — [`L169`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L169) — A summary line must appear on stderr when ≥1 chunk fails.
- uses (calls/refs, reference-scoped): [`extract_corpus_parallel`](../graphify/llm.md#extract_corpus_parallel)

### `TestSubprocessEncoding`
- def: [`tests/test_charmap_encoding.py:57`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L57)
- doc: _call_claude_cli must pass encoding="utf-8" to subprocess.run so that
- signature: `class TestSubprocessEncoding:`
- members:
  - `_make_completed(self)` — [`L63`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L63) — Build a mock CompletedProcess with a valid JSON envelope.
  - `test_call_llm_claude_cli_subprocess_encoding(self, monkeypatch)` — [`L122`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L122) — _call_llm with backend='claude-cli' must also use encoding='utf-8'.
  - `test_subprocess_called_with_utf8_encoding(self, monkeypatch)` — [`L67`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L67) — subprocess.run must be invoked with encoding='utf-8'. — documented in [graphify-llm](../../concepts/graphify-llm.md)
  - `test_subprocess_does_not_use_text_true_without_encoding(self, monkeypatch)` — [`L80`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L80) — text=True without encoding= relies on the locale codec (cp1252 on Windows).
  - `test_unicode_chars_survive_subprocess_roundtrip(self, monkeypatch, tmp_path)` — [`L105`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L105) — Writing a file with → ✅ ≥ then passing its content through
- uses (calls/refs, reference-scoped): [`extract_files_direct`](../graphify/llm.md#extract_files_direct), [`_call_claude_cli`](../graphify/llm.md#_call_claude_cli), [`_call_llm`](../graphify/llm.md#_call_llm)  (2 test-only)

### `TestSubstitutionValidation`
- def: [`tests/test_charmap_encoding.py:220`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L220)
- doc: Exercises the same code path as the rsl-siege-manager reproduction
- signature: `class TestSubstitutionValidation:`
- members:
  - `test_cp1252_would_fail_but_utf8_succeeds(self, tmp_path)` — [`L250`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L250) — Demonstrate the exact failure mode that is now fixed.
  - `test_read_files_produces_utf8_safe_prompt(self, tmp_path)` — [`L238`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L238) — _read_files must return a string that encodes cleanly to UTF-8.
  - `test_subprocess_encoding_kwarg_in_extract_files_direct(self, monkeypatch, tmp_path)` — [`L282`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L282) — End-to-end path: write unicode file → extract_files_direct → subprocess.
- protocol/private: `_UNICODE_CHARS`[`L236`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L236)
- uses (calls/refs, reference-scoped): [`extract_files_direct`](../graphify/llm.md#extract_files_direct), [`_read_files`](../graphify/llm.md#_read_files)

## Module values
- `_ENVELOPE` — [`L30`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L30)
- `_UNICODE_CONTENT` — [`L28`](../../../../../raw/code/graphify/tests/test_charmap_encoding.py#L28)

