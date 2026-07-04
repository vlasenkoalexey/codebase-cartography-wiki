---
title: 'Module: tests/test_provider_registry.py'
type: catalog
provenance: extracted
module: tests/test_provider_registry.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_provider_registry`/test_
symbols:
  test_custom_provider_add_list_show_remove: custom_provider_add_list_show_remove().
  test_project_local_providers_loaded_with_optin: project_local_providers_loaded_with_optin().
  test_non_http_provider_base_url_rejected: non_http_provider_base_url_rejected().
  test_detect_backend_custom_provider_after_builtins: detect_backend_custom_provider_after_builtins().
  test_custom_provider_pricing_defaults_to_zero: custom_provider_pricing_defaults_to_zero().
  test_custom_provider_cannot_shadow_builtin: custom_provider_cannot_shadow_builtin().
  test_project_local_providers_ignored_without_optin: project_local_providers_ignored_without_optin().
  test_provider_base_url_ok_scheme_and_warnings: provider_base_url_ok_scheme_and_warnings().
---
# Module: [`tests/test_provider_registry.py`](../../../../../raw/code/graphify/tests/test_provider_registry.py)

## Functions
- `test_custom_provider_add_list_show_remove(tmp_path, monkeypatch)` — [`L6`](../../../../../raw/code/graphify/tests/test_provider_registry.py#L6) — Full round-trip: add → list → show → remove via providers.json.
- `test_custom_provider_cannot_shadow_builtin(tmp_path)` — [`L52`](../../../../../raw/code/graphify/tests/test_provider_registry.py#L52) — Built-in provider names are protected from being overridden.
- `test_custom_provider_pricing_defaults_to_zero(tmp_path)` — [`L30`](../../../../../raw/code/graphify/tests/test_provider_registry.py#L30) — Missing pricing field defaults to zero so estimate_cost doesn't blow up.
- `test_detect_backend_custom_provider_after_builtins(monkeypatch)` — [`L141`](../../../../../raw/code/graphify/tests/test_provider_registry.py#L141) — Custom providers appear after all built-ins in detect_backend() priority.
- `test_non_http_provider_base_url_rejected(tmp_path, monkeypatch)` — [`L112`](../../../../../raw/code/graphify/tests/test_provider_registry.py#L112) — A provider whose base_url uses a non-http(s) scheme is skipped on load (F1).
- `test_project_local_providers_ignored_without_optin(tmp_path, monkeypatch, capsys)` — [`L72`](../../../../../raw/code/graphify/tests/test_provider_registry.py#L72) — A project-local ./.graphify/providers.json is NOT loaded by default (F1).
- `test_project_local_providers_loaded_with_optin(tmp_path, monkeypatch)` — [`L94`](../../../../../raw/code/graphify/tests/test_provider_registry.py#L94) — With explicit opt-in the project-local file is honoured (F1).
- `test_provider_base_url_ok_scheme_and_warnings(capsys)` — [`L128`](../../../../../raw/code/graphify/tests/test_provider_registry.py#L128) — provider_base_url_ok rejects bad schemes and warns on plaintext-http egress (F1).

