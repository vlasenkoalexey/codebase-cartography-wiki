---
title: 'Module: tests/test_llm_backends.py'
type: catalog
provenance: extracted
module: tests/test_llm_backends.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_llm_backends`/
symbols:
  _clear_backend_env: _clear_backend_env().
  _install_capturing_openai: _install_capturing_openai().
  test_str_path_entry_points_handle_edge_cases: test_str_path_entry_points_handle_edge_cases().
  _fake_openai_response: _fake_openai_response().
  test_gemini_accepts_gemini_api_key: test_gemini_accepts_gemini_api_key().
  test_gemini_accepts_google_api_key: test_gemini_accepts_google_api_key().
  test_openai_backend_detected: test_openai_backend_detected().
  test_corpus_parallel_oversized_markdown_does_not_crash_on_fileslice: test_corpus_parallel_oversized_markdown_does_not_crash_on_fileslice().
  test_call_openai_compat_relabels_empty_content_as_length: test_call_openai_compat_relabels_empty_content_as_length().
  test_call_openai_compat_relabels_none_content_as_length: test_call_openai_compat_relabels_none_content_as_length().
  test_call_openai_compat_relabels_unparseable_json_as_length: test_call_openai_compat_relabels_unparseable_json_as_length().
  test_call_openai_compat_preserves_real_finish_reason: test_call_openai_compat_preserves_real_finish_reason().
  test_call_azure_uses_correct_client_params_and_max_completion_tokens: test_call_azure_uses_correct_client_params_and_max_completion_tokens().
  test_detect_backend_returns_azure_when_both_vars_set: test_detect_backend_returns_azure_when_both_vars_set().
  test_openai_compat_omits_temperature_for_o3_model: test_openai_compat_omits_temperature_for_o3_model().
  test_openai_compat_sends_temperature_for_normal_model: test_openai_compat_sends_temperature_for_normal_model().
  test_openai_compat_env_var_temperature_applied: test_openai_compat_env_var_temperature_applied().
  _install_fake_openai: _install_fake_openai().
  test_backend_detection_prefers_gemini: test_backend_detection_prefers_gemini().
  test_extract_files_direct_routes_gemini_through_openai_compat: test_extract_files_direct_routes_gemini_through_openai_compat().
  test_openai_compat_backends_resolve_full_output_cap: test_openai_compat_backends_resolve_full_output_cap().
  test_gemini_model_can_be_overridden_by_env: test_gemini_model_can_be_overridden_by_env().
  test_missing_gemini_key_names_both_supported_env_vars: test_missing_gemini_key_names_both_supported_env_vars().
  test_extract_files_direct_accepts_str_paths: test_extract_files_direct_accepts_str_paths().
  test_extract_corpus_parallel_accepts_str_and_mixed_paths: test_extract_corpus_parallel_accepts_str_and_mixed_paths().
  test_adaptive_retry_splits_on_context_exceeded: test_adaptive_retry_splits_on_context_exceeded().
  test_adaptive_retry_gives_up_on_single_file_overflow: test_adaptive_retry_gives_up_on_single_file_overflow().
  test_adaptive_retry_re_raises_unrelated_errors: test_adaptive_retry_re_raises_unrelated_errors().
  test_ollama_extra_body_sets_num_ctx_and_keep_alive: test_ollama_extra_body_sets_num_ctx_and_keep_alive().
  test_ollama_num_ctx_scales_with_small_token_budget: test_ollama_num_ctx_scales_with_small_token_budget().
  test_ollama_num_ctx_env_override: test_ollama_num_ctx_env_override().
  test_non_ollama_backend_gets_no_num_ctx_extra_body: test_non_ollama_backend_gets_no_num_ctx_extra_body().
  test_openai_compat_forces_non_streaming_response: test_openai_compat_forces_non_streaming_response().
  test_call_openai_compat_uses_explicit_extra_body: test_call_openai_compat_uses_explicit_extra_body().
  test_call_openai_compat_extra_body_wins_over_moonshot_default: test_call_openai_compat_extra_body_wins_over_moonshot_default().
  test_call_openai_compat_explicit_extra_body_skips_ollama_auto_derive: test_call_openai_compat_explicit_extra_body_skips_ollama_auto_derive().
  test_extract_corpus_parallel_ollama_runs_serially: test_extract_corpus_parallel_ollama_runs_serially().
  test_extract_corpus_parallel_ollama_parallel_env_restores_concurrency: test_extract_corpus_parallel_ollama_parallel_env_restores_concurrency().
  test_adaptive_retry_bisects_on_hollow_ollama_response: test_adaptive_retry_bisects_on_hollow_ollama_response().
  test_detect_backend_azure_requires_endpoint_not_just_key: test_detect_backend_azure_requires_endpoint_not_just_key().
  test_call_claude_cli_passes_errors_replace_to_subprocess: test_call_claude_cli_passes_errors_replace_to_subprocess().
  test_openai_compat_client_built_with_retries: test_openai_compat_client_built_with_retries().
  _FakeAnthropic.messages: _FakeAnthropic#messages.
  test_call_llm_openai_compat_client_built_with_timeout_and_retries: test_call_llm_openai_compat_client_built_with_timeout_and_retries().
  _ok: _ok().
  test_adaptive_retry_splits_on_context_exceeded.fake_extract: test_adaptive_retry_splits_on_context_exceeded().fake_extract().
  test_extract_corpus_parallel_ollama_runs_serially.fake_extract: test_extract_corpus_parallel_ollama_runs_serially().fake_extract().
  test_adaptive_retry_bisects_on_hollow_ollama_response.fake_extract: test_adaptive_retry_bisects_on_hollow_ollama_response().fake_extract().
  _install_fake_azure_openai: _install_fake_azure_openai().
  test_looks_like_context_exceeded_matches_common_messages: test_looks_like_context_exceeded_matches_common_messages().
  test_looks_like_context_exceeded_ignores_unrelated_errors: test_looks_like_context_exceeded_ignores_unrelated_errors().
  test_response_is_hollow_flags_empty_string: test_response_is_hollow_flags_empty_string().
  test_response_is_hollow_flags_none_content: test_response_is_hollow_flags_none_content().
  test_response_is_hollow_flags_whitespace_only: test_response_is_hollow_flags_whitespace_only().
  test_response_is_hollow_flags_parsed_but_no_nodes_or_edges: test_response_is_hollow_flags_parsed_but_no_nodes_or_edges().
  test_response_is_hollow_accepts_real_extraction: test_response_is_hollow_accepts_real_extraction().
  _Choice.message: _Choice#message.
  _fake_openai_response._Resp.__init__: _fake_openai_response()._Resp#__init__().
  _Resp.choices: _Resp#choices.
  _Resp.usage: _Resp#usage.
  _install_capturing_openai._FakeOpenAI.create: _install_capturing_openai()._FakeOpenAI#create().
  test_estimate_cost_azure_no_keyerror: test_estimate_cost_azure_no_keyerror().
  test_model_requires_default_temperature_true_for_reasoning_models: test_model_requires_default_temperature_true_for_reasoning_models().
  test_model_requires_default_temperature_false_for_normal_models: test_model_requires_default_temperature_false_for_normal_models().
  test_resolve_temperature_default_for_normal_model: test_resolve_temperature_default_for_normal_model().
  test_resolve_temperature_omitted_for_reasoning_model: test_resolve_temperature_omitted_for_reasoning_model().
  test_resolve_temperature_env_var_numeric_overrides: test_resolve_temperature_env_var_numeric_overrides().
  test_resolve_temperature_env_var_none_omits: test_resolve_temperature_env_var_none_omits().
  test_resolve_temperature_env_var_invalid_falls_back: test_resolve_temperature_env_var_invalid_falls_back().
  test_native_extraction_prompt_requests_hyperedges: test_native_extraction_prompt_requests_hyperedges().
  test_native_extraction_prompt_matches_skill_spec_on_hyperedges: test_native_extraction_prompt_matches_skill_spec_on_hyperedges().
  test_base_url_env_overrides: test_base_url_env_overrides().
  test_call_claude_cli_tolerates_non_utf8_in_stderr: test_call_claude_cli_tolerates_non_utf8_in_stderr().
  test_resolve_max_retries_default_and_env: test_resolve_max_retries_default_and_env().
  test_openai_compat_client_built_with_retries._FakeOpenAI.create: test_openai_compat_client_built_with_retries()._FakeOpenAI#create().
  test_call_llm_claude_client_built_with_timeout_and_retries._FakeAnthropic.__init__: test_call_llm_claude_client_built_with_timeout_and_retries()._FakeAnthropic#__init__().
  test_call_llm_openai_compat_client_built_with_timeout_and_retries._FakeOpenAI.create: test_call_llm_openai_compat_client_built_with_timeout_and_retries()._FakeOpenAI#create().
  test_str_path_entry_points_handle_edge_cases._SubPath: test_str_path_entry_points_handle_edge_cases()._SubPath#
  test_adaptive_retry_gives_up_on_single_file_overflow.fake_extract: test_adaptive_retry_gives_up_on_single_file_overflow().fake_extract().
  test_adaptive_retry_re_raises_unrelated_errors.fake_extract: test_adaptive_retry_re_raises_unrelated_errors().fake_extract().
  _fake_openai_response._Usage: _fake_openai_response()._Usage#
  _fake_openai_response._Message: _fake_openai_response()._Message#
  _fake_openai_response._Choice: _fake_openai_response()._Choice#
  _fake_openai_response._Resp: _fake_openai_response()._Resp#
  _install_fake_openai._FakeOpenAI: _install_fake_openai()._FakeOpenAI#
  _install_capturing_openai._FakeOpenAI: _install_capturing_openai()._FakeOpenAI#
  _install_fake_azure_openai._FakeAzureOpenAI: _install_fake_azure_openai()._FakeAzureOpenAI#
  _backend_base_url: _backend_base_url().
  _make_cli_envelope: _make_cli_envelope().
  test_openai_compat_client_built_with_retries._FakeOpenAI: test_openai_compat_client_built_with_retries()._FakeOpenAI#
  test_call_llm_claude_client_built_with_timeout_and_retries._FakeMessages: test_call_llm_claude_client_built_with_timeout_and_retries()._FakeMessages#
  test_call_llm_claude_client_built_with_timeout_and_retries._FakeAnthropic: test_call_llm_claude_client_built_with_timeout_and_retries()._FakeAnthropic#
  test_call_llm_openai_compat_client_built_with_timeout_and_retries._FakeOpenAI: test_call_llm_openai_compat_client_built_with_timeout_and_retries()._FakeOpenAI#
  _fake_openai_response._Usage.__init__: _fake_openai_response()._Usage#__init__().
  _Usage.prompt_tokens: _Usage#prompt_tokens.
  _Usage.completion_tokens: _Usage#completion_tokens.
  _fake_openai_response._Message.__init__: _fake_openai_response()._Message#__init__().
  _Message.content: _Message#content.
  _fake_openai_response._Choice.__init__: _fake_openai_response()._Choice#__init__().
  _Choice.finish_reason: _Choice#finish_reason.
  _install_fake_openai._FakeOpenAI.__init__: _install_fake_openai()._FakeOpenAI#__init__().
  _FakeOpenAI.chat: _FakeOpenAI#chat.
  _FakeOpenAI.completions: _FakeOpenAI#completions.
  _install_fake_openai._FakeOpenAI.create: _install_fake_openai()._FakeOpenAI#create().
  _install_capturing_openai._FakeOpenAI.__init__: _install_capturing_openai()._FakeOpenAI#__init__().
  _install_fake_azure_openai._FakeAzureOpenAI.__init__: _install_fake_azure_openai()._FakeAzureOpenAI#__init__().
  _FakeAzureOpenAI.chat: _FakeAzureOpenAI#chat.
  _FakeAzureOpenAI.completions: _FakeAzureOpenAI#completions.
  _install_fake_azure_openai._FakeAzureOpenAI.create: _install_fake_azure_openai()._FakeAzureOpenAI#create().
  test_base_url_defaults_without_env: test_base_url_defaults_without_env().
  test_openai_compat_client_built_with_retries._FakeOpenAI.__init__: test_openai_compat_client_built_with_retries()._FakeOpenAI#__init__().
  test_call_llm_claude_client_built_with_timeout_and_retries: test_call_llm_claude_client_built_with_timeout_and_retries().
  test_call_llm_claude_client_built_with_timeout_and_retries._FakeMessages.create: test_call_llm_claude_client_built_with_timeout_and_retries()._FakeMessages#create().
  test_call_llm_openai_compat_client_built_with_timeout_and_retries._FakeOpenAI.__init__: test_call_llm_openai_compat_client_built_with_timeout_and_retries()._FakeOpenAI#__init__().
---
# Module: [`tests/test_llm_backends.py`](../../../../../raw/code/graphify/tests/test_llm_backends.py)

## Classes
### `_Choice`
- def: [`tests/test_llm_backends.py:343`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L343)
- signature: `class _Choice:`
- members:
  - `finish_reason` — [`L346`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L346)
  - `message` — [`L345`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L345)
- protocol/private: `__init__`[`L344`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L344)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_FakeAnthropic`
- def: [`tests/test_llm_backends.py:1047`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1047)
- signature: `class _FakeAnthropic:`
- members:
  - `messages` — [`L1050`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1050)
- protocol/private: `__init__`[`L1048`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1048)
- uses (calls/refs, reference-scoped): [`_call_llm`](../graphify/llm.md#_call_llm)  (1 test-only)

### `_FakeAzureOpenAI`
- def: [`tests/test_llm_backends.py:701`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L701)
- signature: `class _FakeAzureOpenAI:`
- members:
  - `create(self, **kwargs)` — [`L707`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L707)
  - `chat` — [`L704`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L704)
  - `completions` — [`L705`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L705)
- protocol/private: `__init__`[`L702`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L702)
- used by: (1 test-only callers)

### `_FakeMessages`
- def: [`tests/test_llm_backends.py:1043`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1043)
- signature: `class _FakeMessages:`
- members:
  - `create(self, **_)` — [`L1044`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1044)
- used by: (1 test-only callers)

### `_FakeOpenAI`
- def: [`tests/test_llm_backends.py:1071`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1071)
- signature: `class _FakeOpenAI:`
- members:
  - `create(self, **__)` — [`L367`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L367)
  - `create(self, **kwargs)` — [`L453`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L453)
  - `create(self, **_)` — [`L1015`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1015)
  - `create(self, **_)` — [`L1077`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1077)
  - `chat` — [`L365`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L365)
  - `completions` — [`L366`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L366)
- protocol/private: `__init__`[`L364`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L364), `__init__`[`L449`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L449), `__init__`[`L1010`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1010), `__init__`[`L1072`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1072)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_Message`
- def: [`tests/test_llm_backends.py:339`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L339)
- signature: `class _Message:`
- members:
  - `content` — [`L341`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L341)
- protocol/private: `__init__`[`L340`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L340)
- used by: (1 test-only callers)

### `_Resp`
- def: [`tests/test_llm_backends.py:348`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L348)
- signature: `class _Resp:`
- members:
  - `choices` — [`L350`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L350)
  - `usage` — [`L351`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L351)
- protocol/private: `__init__`[`L349`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L349)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `_SubPath`  ·  implements/extends Path
- def: [`tests/test_llm_backends.py:200`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L200)
- signature: `class _SubPath(type(Path())):`
- used by: (1 test-only callers)

### `_Usage`
- def: [`tests/test_llm_backends.py:334`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L334)
- signature: `class _Usage:`
- members:
  - `completion_tokens` — [`L337`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L337)
  - `prompt_tokens` — [`L336`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L336)
- protocol/private: `__init__`[`L335`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L335)
- used by: (1 test-only callers)

## Functions
- `_backend_base_url(backend: str, env_extra: dict)` — [`L897`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L897)
- `_clear_backend_env(monkeypatch)` — [`L11`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L11)
- `_fake_openai_response(content, *, finish_reason="stop", prompt_tokens=100, completion_tokens=0)` — [`L332`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L332) — Build a minimal stand-in for an `openai` SDK ChatCompletion response.
- `_install_capturing_openai(monkeypatch)` — [`L441`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L441) — Like _install_fake_openai but records kwargs passed to create().
- `_install_fake_azure_openai(monkeypatch, fake_resp)` — [`L693`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L693) — Inject a stub openai module with AzureOpenAI so _call_azure and
- `_install_fake_openai(monkeypatch, fake_resp)` — [`L356`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L356) — Inject a stub `openai` module so `_call_openai_compat` can run without
- `_make_cli_envelope(result_text: str)` — [`L945`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L945) — Return a minimal claude -p --output-format json envelope.
- `_ok(nodes=None, edges=None, model="m")` — [`L212`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L212)
- `fake_extract(chunk, *_, **__)` — [`L248`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L248)
- `fake_extract(*_, **__)` — [`L270`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L270)
- `fake_extract(*_, **__)` — [`L289`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L289)
- `fake_extract(chunk, *_, **__)` — [`L609`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L609)
- `fake_extract(chunk, *_, **__)` — [`L663`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L663)
- `test_adaptive_retry_bisects_on_hollow_ollama_response(tmp_path)` — [`L651`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L651)
- `test_adaptive_retry_gives_up_on_single_file_overflow(tmp_path)` — [`L266`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L266)
- `test_adaptive_retry_re_raises_unrelated_errors(tmp_path)` — [`L285`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L285)
- `test_adaptive_retry_splits_on_context_exceeded(tmp_path)` — [`L241`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L241)
- `test_backend_detection_prefers_gemini(monkeypatch)` — [`L41`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L41)
- `test_base_url_defaults_without_env(backend, default)` — [`L923`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L923)
- `test_base_url_env_overrides(backend, env_var, override)` — [`L914`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L914)
- `test_call_azure_uses_correct_client_params_and_max_completion_tokens(monkeypatch)` — [`L717`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L717)
- `test_call_claude_cli_passes_errors_replace_to_subprocess()` — [`L950`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L950) — subprocess.run must be called with errors='replace' so non-UTF-8 output
- `test_call_claude_cli_tolerates_non_utf8_in_stderr()` — [`L971`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L971) — When errors='replace' is set, non-UTF-8 bytes in stderr produce replacement
- `test_call_llm_claude_client_built_with_timeout_and_retries(monkeypatch)` — [`L1033`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1033) — The secondary dispatch path (_call_llm, used by the dedup tiebreaker)
- `test_call_llm_openai_compat_client_built_with_timeout_and_retries(monkeypatch)` — [`L1064`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1064) — Same #1442 fix for the OpenAI-compatible branch of _call_llm.
- `test_call_openai_compat_explicit_extra_body_skips_ollama_auto_derive(monkeypatch)` — [`L581`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L581)
- `test_call_openai_compat_extra_body_wins_over_moonshot_default(monkeypatch)` — [`L567`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L567)
- `test_call_openai_compat_preserves_real_finish_reason(monkeypatch)` — [`L418`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L418)
- `test_call_openai_compat_relabels_empty_content_as_length(monkeypatch)` — [`L375`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L375)
- `test_call_openai_compat_relabels_none_content_as_length(monkeypatch)` — [`L393`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L393)
- `test_call_openai_compat_relabels_unparseable_json_as_length(monkeypatch)` — [`L404`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L404)
- `test_call_openai_compat_uses_explicit_extra_body(monkeypatch)` — [`L555`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L555)
- `test_corpus_parallel_oversized_markdown_does_not_crash_on_fileslice(tmp_path, monkeypatch)` — [`L170`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L170) — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `test_detect_backend_azure_requires_endpoint_not_just_key(monkeypatch)` — [`L752`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L752)
- `test_detect_backend_returns_azure_when_both_vars_set(monkeypatch)` — [`L743`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L743)
- `test_estimate_cost_azure_no_keyerror()` — [`L760`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L760)
- `test_extract_corpus_parallel_accepts_str_and_mixed_paths(tmp_path, monkeypatch)` — [`L152`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L152)
- `test_extract_corpus_parallel_ollama_parallel_env_restores_concurrency(tmp_path, monkeypatch)` — [`L626`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L626)
- `test_extract_corpus_parallel_ollama_runs_serially(tmp_path, monkeypatch)` — [`L599`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L599)
- `test_extract_files_direct_accepts_str_paths(tmp_path, monkeypatch)` — [`L140`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L140)
- `test_extract_files_direct_routes_gemini_through_openai_compat(tmp_path, monkeypatch)` — [`L59`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L59)
- `test_gemini_accepts_gemini_api_key(monkeypatch)` — [`L25`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L25)
- `test_gemini_accepts_google_api_key(monkeypatch)` — [`L33`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L33)
- `test_gemini_model_can_be_overridden_by_env(tmp_path, monkeypatch)` — [`L112`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L112)
- `test_looks_like_context_exceeded_ignores_unrelated_errors()` — [`L236`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L236)
- `test_looks_like_context_exceeded_matches_common_messages()` — [`L224`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L224)
- `test_missing_gemini_key_names_both_supported_env_vars(monkeypatch)` — [`L126`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L126)
- `test_model_requires_default_temperature_false_for_normal_models(model)` — [`L783`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L783)
- `test_model_requires_default_temperature_true_for_reasoning_models(model)` — [`L775`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L775)
- `test_native_extraction_prompt_matches_skill_spec_on_hyperedges()` — [`L876`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L876) — Both extraction paths share the same hyperedge contract (the '3 or more
- `test_native_extraction_prompt_requests_hyperedges()` — [`L861`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L861) — The native-backend prompt must request hyperedges, like the skill's
- `test_non_ollama_backend_gets_no_num_ctx_extra_body(monkeypatch)` — [`L524`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L524)
- `test_ollama_extra_body_sets_num_ctx_and_keep_alive(monkeypatch)` — [`L467`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L467)
- `test_ollama_num_ctx_env_override(monkeypatch)` — [`L511`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L511)
- `test_ollama_num_ctx_scales_with_small_token_budget(monkeypatch)` — [`L485`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L485)
- `test_openai_backend_detected(monkeypatch)` — [`L51`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L51)
- `test_openai_compat_backends_resolve_full_output_cap(tmp_path, monkeypatch, backend, env_key)` — [`L94`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L94)
- `test_openai_compat_client_built_with_retries(monkeypatch)` — [`L1000`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L1000) — The OpenAI-compatible client (kimi/openai/gemini/deepseek/ollama) is built with
- `test_openai_compat_env_var_temperature_applied(tmp_path, monkeypatch)` — [`L848`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L848)
- `test_openai_compat_forces_non_streaming_response(monkeypatch)` — [`L536`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L536)
- `test_openai_compat_omits_temperature_for_o3_model(tmp_path, monkeypatch)` — [`L817`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L817) — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `test_openai_compat_sends_temperature_for_normal_model(tmp_path, monkeypatch)` — [`L835`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L835)
- `test_resolve_max_retries_default_and_env(monkeypatch)` — [`L988`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L988) — Default retry count is generous (so 429s are absorbed, #1523); env overrides.
- `test_resolve_temperature_default_for_normal_model(monkeypatch)` — [`L787`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L787)
- `test_resolve_temperature_env_var_invalid_falls_back(monkeypatch)` — [`L810`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L810)
- `test_resolve_temperature_env_var_none_omits(monkeypatch)` — [`L805`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L805)
- `test_resolve_temperature_env_var_numeric_overrides(monkeypatch)` — [`L798`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L798)
- `test_resolve_temperature_omitted_for_reasoning_model(monkeypatch)` — [`L792`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L792)
- `test_response_is_hollow_accepts_real_extraction()` — [`L325`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L325)
- `test_response_is_hollow_flags_empty_string()` — [`L306`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L306)
- `test_response_is_hollow_flags_none_content()` — [`L310`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L310)
- `test_response_is_hollow_flags_parsed_but_no_nodes_or_edges()` — [`L318`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L318)
- `test_response_is_hollow_flags_whitespace_only()` — [`L314`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L314)
- `test_str_path_entry_points_handle_edge_cases(tmp_path, monkeypatch)` — [`L190`](../../../../../raw/code/graphify/tests/test_llm_backends.py#L190)

