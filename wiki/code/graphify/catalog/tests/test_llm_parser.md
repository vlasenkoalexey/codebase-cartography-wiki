---
title: 'Module: tests/test_llm_parser.py'
type: catalog
provenance: extracted
module: tests/test_llm_parser.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_llm_parser`/
symbols:
  test_instructions_ride_in_user_turn_not_system_prompt: test_instructions_ride_in_user_turn_not_system_prompt().
  test_model_env_var_adds_model_flag: test_model_env_var_adds_model_flag().
  test_no_model_flag_when_env_var_unset: test_no_model_flag_when_env_var_unset().
  _make_envelope: _make_envelope().
  test_preamble_then_fence_is_parsed: test_preamble_then_fence_is_parsed().
  test_prose_wrapped_json_without_fence_is_parsed: test_prose_wrapped_json_without_fence_is_parsed().
  test_raw_json_still_works: test_raw_json_still_works().
  test_total_refusal_returns_empty_fragment: test_total_refusal_returns_empty_fragment().
  test_fence_with_uppercase_language_tag: test_fence_with_uppercase_language_tag().
  test_fence_without_closing_backticks: test_fence_without_closing_backticks().
  test_empty_response_returns_empty_fragment: test_empty_response_returns_empty_fragment().
---
# Module: [`tests/test_llm_parser.py`](../../../../../raw/code/graphify/tests/test_llm_parser.py)

## Functions
- `_make_envelope(result_obj: dict)` — [`L89`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L89)
- `test_empty_response_returns_empty_fragment()` — [`L82`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L82)
- `test_fence_with_uppercase_language_tag()` — [`L68`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L68)
- `test_fence_without_closing_backticks()` — [`L74`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L74) — Truncated response: the model started the fence but ran out of
- `test_instructions_ride_in_user_turn_not_system_prompt(mock_run, _which)` — [`L104`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L104) — Extraction instructions must be delivered in the user turn, not via
- `test_model_env_var_adds_model_flag(mock_run, _which, monkeypatch)` — [`L132`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L132) — GRAPHIFY_CLAUDE_CLI_MODEL must be forwarded to claude -p --model.
- `test_no_model_flag_when_env_var_unset(mock_run, _which, monkeypatch)` — [`L146`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L146) — Default behaviour: when the env var is not set, --model is not
- `test_preamble_then_fence_is_parsed()` — [`L22`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L22) — Claude often prefixes the JSON with a short preamble before the
- `test_prose_wrapped_json_without_fence_is_parsed()` — [`L37`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L37) — Some models return prose around bare JSON with no markdown fence.
- `test_raw_json_still_works()` — [`L48`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L48) — Regression: clean JSON input (the original happy path) must keep
- `test_total_refusal_returns_empty_fragment()` — [`L56`](../../../../../raw/code/graphify/tests/test_llm_parser.py#L56) — When the model refuses or returns unrelated prose, the parser

