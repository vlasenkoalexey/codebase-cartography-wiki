---
title: 'Module: tests/test_ollama.py'
type: catalog
provenance: extracted
module: tests/test_ollama.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_ollama`/test_
symbols:
  test_ollama_alias_resolving_to_link_local_blocked: ollama_alias_resolving_to_link_local_blocked().
  test_ollama_blocks_link_local_and_metadata: ollama_blocks_link_local_and_metadata().
  test_ollama_loopback_and_lan_do_not_raise: ollama_loopback_and_lan_do_not_raise().
  test_ollama_warn_false_still_hard_blocks_but_stays_quiet: ollama_warn_false_still_hard_blocks_but_stays_quiet().
  test_ollama_in_backends: ollama_in_backends().
  test_detect_backend_ollama: detect_backend_ollama().
  test_detect_backend_kimi_beats_ollama: detect_backend_kimi_beats_ollama().
  test_detect_backend_claude_beats_ollama: detect_backend_claude_beats_ollama().
  test_detect_backend_none_without_envvars: detect_backend_none_without_envvars().
  test_ollama_api_key_sentinel: ollama_api_key_sentinel().
  test_ollama_alias_resolving_to_link_local_blocked.fake_getaddrinfo: ollama_alias_resolving_to_link_local_blocked().fake_getaddrinfo().
---
# Module: [`tests/test_ollama.py`](../../../../../raw/code/graphify/tests/test_ollama.py)

## Functions
- `fake_getaddrinfo(host, *a, **k)` — [`L33`](../../../../../raw/code/graphify/tests/test_ollama.py#L33)
- `test_detect_backend_claude_beats_ollama(monkeypatch)` — [`L72`](../../../../../raw/code/graphify/tests/test_ollama.py#L72)
- `test_detect_backend_kimi_beats_ollama(monkeypatch)` — [`L65`](../../../../../raw/code/graphify/tests/test_ollama.py#L65)
- `test_detect_backend_none_without_envvars(monkeypatch)` — [`L83`](../../../../../raw/code/graphify/tests/test_ollama.py#L83)
- `test_detect_backend_ollama(monkeypatch)` — [`L58`](../../../../../raw/code/graphify/tests/test_ollama.py#L58)
- `test_ollama_alias_resolving_to_link_local_blocked(monkeypatch)` — [`L29`](../../../../../raw/code/graphify/tests/test_ollama.py#L29) — A hostname that RESOLVES to a link-local IP is blocked, not just literals (F3).
- `test_ollama_api_key_sentinel(monkeypatch)` — [`L90`](../../../../../raw/code/graphify/tests/test_ollama.py#L90) — extract_files_direct with backend=ollama and no OLLAMA_API_KEY should use sentinel 'ollama' not raise.
- `test_ollama_blocks_link_local_and_metadata(url)` — [`L15`](../../../../../raw/code/graphify/tests/test_ollama.py#L15) — Link-local / cloud-metadata Ollama targets fail closed (F3).
- `test_ollama_in_backends()` — [`L51`](../../../../../raw/code/graphify/tests/test_ollama.py#L51)
- `test_ollama_loopback_and_lan_do_not_raise(capsys)` — [`L21`](../../../../../raw/code/graphify/tests/test_ollama.py#L21) — Loopback is silent; a general LAN host warns but is allowed (F3).
- `test_ollama_warn_false_still_hard_blocks_but_stays_quiet(capsys)` — [`L41`](../../../../../raw/code/graphify/tests/test_ollama.py#L41) — warn=False suppresses the LAN warning but never the metadata hard-block (F3).

