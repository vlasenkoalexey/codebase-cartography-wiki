---
title: 'Module: tests/test_claude_cli_backend.py'
type: catalog
provenance: extracted
module: tests/test_claude_cli_backend.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_claude_cli_backend`/
symbols:
  test_windows_prefers_claude_cmd_over_bare_claude: test_windows_prefers_claude_cmd_over_bare_claude().
  test_windows_falls_back_to_bare_claude_when_cmd_missing: test_windows_falls_back_to_bare_claude_when_cmd_missing().
  test_simple_completion_resolves_cmd_shim_on_windows: test_simple_completion_resolves_cmd_shim_on_windows().
  _ENVELOPE: _ENVELOPE.
  test_finish_reason_length_on_max_tokens: test_finish_reason_length_on_max_tokens().
  test_backend_registered_with_zero_cost: test_backend_registered_with_zero_cost().
  test_non_windows_uses_bare_claude: test_non_windows_uses_bare_claude().
  fake_claude: fake_claude().
  test_returns_parsed_nodes_and_edges: test_returns_parsed_nodes_and_edges().
  test_token_accounting_includes_cache: test_token_accounting_includes_cache().
  test_raises_when_cli_missing: test_raises_when_cli_missing().
  test_raises_on_nonzero_exit: test_raises_on_nonzero_exit().
  test_raises_on_garbage_envelope: test_raises_on_garbage_envelope().
  test_extract_files_direct_dispatches_to_claude_cli: test_extract_files_direct_dispatches_to_claude_cli().
  test_no_session_persistence_flag_in_subprocess: test_no_session_persistence_flag_in_subprocess().
  test_no_system_prompt_flag_in_subprocess: test_no_system_prompt_flag_in_subprocess().
  test_extraction_instructions_ride_in_user_turn: test_extraction_instructions_ride_in_user_turn().
  test_user_turn_preserves_untrusted_source_guardrails: test_user_turn_preserves_untrusted_source_guardrails().
  test_windows_raises_when_neither_cmd_nor_bare_claude_present: test_windows_raises_when_neither_cmd_nor_bare_claude_present().
  test_resolve_api_timeout_default: test_resolve_api_timeout_default().
  test_resolve_api_timeout_env_override: test_resolve_api_timeout_env_override().
  test_resolve_api_timeout_ignores_invalid: test_resolve_api_timeout_ignores_invalid().
  test_resolve_api_timeout_ignores_nonpositive: test_resolve_api_timeout_ignores_nonpositive().
  test_claude_cli_extraction_honours_timeout: test_claude_cli_extraction_honours_timeout().
  test_call_llm_claude_cli_branch_honours_timeout: test_call_llm_claude_cli_branch_honours_timeout().
  test_windows_prefers_claude_cmd_over_bare_claude.fake_which: test_windows_prefers_claude_cmd_over_bare_claude().fake_which().
  test_windows_falls_back_to_bare_claude_when_cmd_missing.fake_which: test_windows_falls_back_to_bare_claude_when_cmd_missing().fake_which().
  test_simple_completion_resolves_cmd_shim_on_windows.fake_run: test_simple_completion_resolves_cmd_shim_on_windows().fake_run().
  test_simple_completion_resolves_cmd_shim_on_windows.fake_which: test_simple_completion_resolves_cmd_shim_on_windows().fake_which().
---
# Module: [`tests/test_claude_cli_backend.py`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py)

## Functions
- `fake_claude(monkeypatch)` — [`L44`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L44)
- `fake_run(args, **kwargs)` — [`L278`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L278)
- `fake_which(name)` — [`L168`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L168)
- `fake_which(name)` — [`L195`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L195)
- `fake_which(name)` — [`L285`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L285)
- `test_backend_registered_with_zero_cost()` — [`L106`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L106)
- `test_call_llm_claude_cli_branch_honours_timeout(monkeypatch, fake_claude)` — [`L264`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L264)
- `test_claude_cli_extraction_honours_timeout(monkeypatch, fake_claude)` — [`L258`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L258)
- `test_extract_files_direct_dispatches_to_claude_cli(tmp_path, fake_claude)` — [`L98`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L98)
- `test_extraction_instructions_ride_in_user_turn(fake_claude)` — [`L136`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L136) — The full extraction schema, an explicit imperative, and the source must
- `test_finish_reason_length_on_max_tokens(monkeypatch)` — [`L66`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L66)
- `test_no_session_persistence_flag_in_subprocess(fake_claude)` — [`L114`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L114)
- `test_no_system_prompt_flag_in_subprocess(fake_claude)` — [`L128`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L128) — --system-prompt must NOT be used: the CLI ignores its 'raw JSON only'
- `test_non_windows_uses_bare_claude(monkeypatch)` — [`L220`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L220) — On non-Windows platforms, behaviour is unchanged: bare `claude`
- `test_raises_on_garbage_envelope()` — [`L90`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L90)
- `test_raises_on_nonzero_exit()` — [`L82`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L82)
- `test_raises_when_cli_missing()` — [`L76`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L76)
- `test_resolve_api_timeout_default(monkeypatch)` — [`L238`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L238)
- `test_resolve_api_timeout_env_override(monkeypatch)` — [`L243`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L243)
- `test_resolve_api_timeout_ignores_invalid(monkeypatch)` — [`L248`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L248)
- `test_resolve_api_timeout_ignores_nonpositive(monkeypatch)` — [`L253`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L253)
- `test_returns_parsed_nodes_and_edges(fake_claude)` — [`L52`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L52)
- `test_simple_completion_resolves_cmd_shim_on_windows(monkeypatch)` — [`L270`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L270) — The label/_simple_completion path must spawn the resolved claude.cmd on
- `test_token_accounting_includes_cache(fake_claude)` — [`L58`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L58)
- `test_user_turn_preserves_untrusted_source_guardrails(fake_claude)` — [`L149`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L149) — The <untrusted_source> guardrails from _extraction_system must survive
- `test_windows_falls_back_to_bare_claude_when_cmd_missing(monkeypatch)` — [`L188`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L188) — If `claude.cmd` is somehow unavailable but `claude` resolves
- `test_windows_prefers_claude_cmd_over_bare_claude(monkeypatch)` — [`L160`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L160) — On Windows, npm installs `claude.ps1` alongside `claude.cmd`. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `test_windows_raises_when_neither_cmd_nor_bare_claude_present()` — [`L211`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L211) — If neither `claude.cmd` nor `claude` are on PATH on Windows,

## Module values
- `_ENVELOPE` — [`L15`](../../../../../raw/code/graphify/tests/test_claude_cli_backend.py#L15)

