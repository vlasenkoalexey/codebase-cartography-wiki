---
title: 'Module: tests/test_security.py'
type: catalog
provenance: extracted
module: tests/test_security.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_security`/
symbols:
  test_safe_fetch_returns_bytes: test_safe_fetch_returns_bytes().
  test_safe_fetch_raises_on_non_2xx: test_safe_fetch_raises_on_non_2xx().
  test_safe_fetch_text_decodes_utf8: test_safe_fetch_text_decodes_utf8().
  test_safe_fetch_text_replaces_bad_bytes: test_safe_fetch_text_replaces_bad_bytes().
  test_graph_size_cap_unreadable_directory_silently_returns: test_graph_size_cap_unreadable_directory_silently_returns().
  test_sanitize_metadata_string_caps_length: test_sanitize_metadata_string_caps_length().
  test_sanitize_metadata_string_coerces_non_string: test_sanitize_metadata_string_coerces_non_string().
  test_sanitize_metadata_value_caps_list_length: test_sanitize_metadata_value_caps_list_length().
  _make_mock_response: _make_mock_response().
  test_validate_url_accepts_http: test_validate_url_accepts_http().
  test_validate_url_accepts_https: test_validate_url_accepts_https().
  test_validate_url_rejects_file: test_validate_url_rejects_file().
  test_validate_url_rejects_ftp: test_validate_url_rejects_ftp().
  test_validate_url_rejects_data: test_validate_url_rejects_data().
  test_validate_url_rejects_empty_scheme: test_validate_url_rejects_empty_scheme().
  test_safe_fetch_rejects_file_url: test_safe_fetch_rejects_file_url().
  test_safe_fetch_rejects_ftp_url: test_safe_fetch_rejects_ftp_url().
  test_safe_fetch_raises_on_size_exceeded: test_safe_fetch_raises_on_size_exceeded().
  test_validate_graph_path_allows_inside_base: test_validate_graph_path_allows_inside_base().
  test_validate_graph_path_blocks_traversal: test_validate_graph_path_blocks_traversal().
  test_validate_graph_path_requires_base_exists: test_validate_graph_path_requires_base_exists().
  test_validate_graph_path_raises_if_file_missing: test_validate_graph_path_raises_if_file_missing().
  test_validate_graph_path_default_base_discovers_output_dir: test_validate_graph_path_default_base_discovers_output_dir().
  test_validate_graph_path_default_base_honours_graphify_out_override: test_validate_graph_path_default_base_honours_graphify_out_override().
  test_sanitize_label_passthrough_html_chars: test_sanitize_label_passthrough_html_chars().
  test_sanitize_label_strips_control_chars: test_sanitize_label_strips_control_chars().
  test_sanitize_label_caps_at_256: test_sanitize_label_caps_at_256().
  test_sanitize_label_safe_passthrough: test_sanitize_label_safe_passthrough().
  test_graph_size_cap_default_is_512_mib: test_graph_size_cap_default_is_512_mib().
  test_graph_size_cap_under_limit_returns_none: test_graph_size_cap_under_limit_returns_none().
  test_graph_size_cap_over_limit_raises: test_graph_size_cap_over_limit_raises().
  test_graph_size_cap_error_message_includes_size_and_cap: test_graph_size_cap_error_message_includes_size_and_cap().
  test_graph_size_cap_at_boundary_passes: test_graph_size_cap_at_boundary_passes().
  test_graph_size_cap_missing_file_silently_returns: test_graph_size_cap_missing_file_silently_returns().
  test_sanitize_metadata_string_strips_control_chars: test_sanitize_metadata_string_strips_control_chars().
  test_sanitize_metadata_string_escapes_html: test_sanitize_metadata_string_escapes_html().
  test_sanitize_metadata_string_escapes_quotes: test_sanitize_metadata_string_escapes_quotes().
  test_sanitize_metadata_value_preserves_simple_types: test_sanitize_metadata_value_preserves_simple_types().
  test_sanitize_metadata_value_recurses_into_dict: test_sanitize_metadata_value_recurses_into_dict().
  test_sanitize_metadata_value_recurses_into_list: test_sanitize_metadata_value_recurses_into_list().
  test_sanitize_metadata_value_converts_tuple_to_list: test_sanitize_metadata_value_converts_tuple_to_list().
  test_sanitize_metadata_none_returns_empty_dict: test_sanitize_metadata_none_returns_empty_dict().
  test_sanitize_metadata_drops_empty_key: test_sanitize_metadata_drops_empty_key().
  test_sanitize_metadata_sanitizes_keys: test_sanitize_metadata_sanitizes_keys().
  test_sanitize_metadata_recursive_nested: test_sanitize_metadata_recursive_nested().
  test_sanitize_metadata_bool_not_coerced_to_int: test_sanitize_metadata_bool_not_coerced_to_int().
  test_graph_size_cap_unreadable_directory_silently_returns._boom: test_graph_size_cap_unreadable_directory_silently_returns()._boom().
  test_sanitize_metadata_string_coerces_non_string._Custom: test_sanitize_metadata_string_coerces_non_string()._Custom#
  test_sanitize_metadata_string_coerces_non_string._Custom.__str__: test_sanitize_metadata_string_coerces_non_string()._Custom#__str__().
---
# Module: [`tests/test_security.py`](../../../../../raw/code/graphify/tests/test_security.py)

## Classes
### `_Custom`
- def: [`tests/test_security.py:320`](../../../../../raw/code/graphify/tests/test_security.py#L320)
- signature: `class _Custom:`
- protocol/private: `__str__`[`L321`](../../../../../raw/code/graphify/tests/test_security.py#L321)
- used by: (1 test-only callers)

## Functions
- `_boom(self)` — [`L280`](../../../../../raw/code/graphify/tests/test_security.py#L280)
- `_make_mock_response(content: bytes, status: int = 200)` — [`L61`](../../../../../raw/code/graphify/tests/test_security.py#L61)
- `test_graph_size_cap_at_boundary_passes(monkeypatch, tmp_path)` — [`L256`](../../../../../raw/code/graphify/tests/test_security.py#L256) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_graph_size_cap_default_is_512_mib()` — [`L226`](../../../../../raw/code/graphify/tests/test_security.py#L226)
- `test_graph_size_cap_error_message_includes_size_and_cap(monkeypatch, tmp_path)` — [`L244`](../../../../../raw/code/graphify/tests/test_security.py#L244) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_graph_size_cap_missing_file_silently_returns(tmp_path)` — [`L268`](../../../../../raw/code/graphify/tests/test_security.py#L268) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_graph_size_cap_over_limit_raises(monkeypatch, tmp_path)` — [`L236`](../../../../../raw/code/graphify/tests/test_security.py#L236) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_graph_size_cap_under_limit_returns_none(tmp_path)` — [`L230`](../../../../../raw/code/graphify/tests/test_security.py#L230)
- `test_graph_size_cap_unreadable_directory_silently_returns(monkeypatch, tmp_path)` — [`L275`](../../../../../raw/code/graphify/tests/test_security.py#L275) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_safe_fetch_raises_on_non_2xx()` — [`L89`](../../../../../raw/code/graphify/tests/test_security.py#L89)
- `test_safe_fetch_raises_on_size_exceeded()` — [`L98`](../../../../../raw/code/graphify/tests/test_security.py#L98)
- `test_safe_fetch_rejects_file_url()` — [`L72`](../../../../../raw/code/graphify/tests/test_security.py#L72)
- `test_safe_fetch_rejects_ftp_url()` — [`L76`](../../../../../raw/code/graphify/tests/test_security.py#L76)
- `test_safe_fetch_returns_bytes(tmp_path)` — [`L80`](../../../../../raw/code/graphify/tests/test_security.py#L80)
- `test_safe_fetch_text_decodes_utf8()` — [`L121`](../../../../../raw/code/graphify/tests/test_security.py#L121)
- `test_safe_fetch_text_replaces_bad_bytes()` — [`L131`](../../../../../raw/code/graphify/tests/test_security.py#L131)
- `test_sanitize_label_caps_at_256()` — [`L213`](../../../../../raw/code/graphify/tests/test_security.py#L213) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_sanitize_label_passthrough_html_chars()` — [`L201`](../../../../../raw/code/graphify/tests/test_security.py#L201) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_sanitize_label_safe_passthrough()` — [`L217`](../../../../../raw/code/graphify/tests/test_security.py#L217)
- `test_sanitize_label_strips_control_chars()` — [`L207`](../../../../../raw/code/graphify/tests/test_security.py#L207) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_sanitize_metadata_bool_not_coerced_to_int()` — [`L400`](../../../../../raw/code/graphify/tests/test_security.py#L400) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_sanitize_metadata_drops_empty_key()` — [`L363`](../../../../../raw/code/graphify/tests/test_security.py#L363) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_sanitize_metadata_none_returns_empty_dict()` — [`L359`](../../../../../raw/code/graphify/tests/test_security.py#L359) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_sanitize_metadata_recursive_nested()` — [`L377`](../../../../../raw/code/graphify/tests/test_security.py#L377) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_sanitize_metadata_sanitizes_keys()` — [`L371`](../../../../../raw/code/graphify/tests/test_security.py#L371)
- `test_sanitize_metadata_string_caps_length()` — [`L312`](../../../../../raw/code/graphify/tests/test_security.py#L312)
- `test_sanitize_metadata_string_coerces_non_string()` — [`L318`](../../../../../raw/code/graphify/tests/test_security.py#L318)
- `test_sanitize_metadata_string_escapes_html()` — [`L298`](../../../../../raw/code/graphify/tests/test_security.py#L298)
- `test_sanitize_metadata_string_escapes_quotes()` — [`L305`](../../../../../raw/code/graphify/tests/test_security.py#L305)
- `test_sanitize_metadata_string_strips_control_chars()` — [`L291`](../../../../../raw/code/graphify/tests/test_security.py#L291)
- `test_sanitize_metadata_value_caps_list_length()` — [`L346`](../../../../../raw/code/graphify/tests/test_security.py#L346) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_sanitize_metadata_value_converts_tuple_to_list()` — [`L353`](../../../../../raw/code/graphify/tests/test_security.py#L353) — documented in [graphify-security](../../concepts/graphify-security.md)
- `test_sanitize_metadata_value_preserves_simple_types()` — [`L326`](../../../../../raw/code/graphify/tests/test_security.py#L326)
- `test_sanitize_metadata_value_recurses_into_dict()` — [`L334`](../../../../../raw/code/graphify/tests/test_security.py#L334)
- `test_sanitize_metadata_value_recurses_into_list()` — [`L340`](../../../../../raw/code/graphify/tests/test_security.py#L340)
- `test_validate_graph_path_allows_inside_base(tmp_path)` — [`L148`](../../../../../raw/code/graphify/tests/test_security.py#L148)
- `test_validate_graph_path_blocks_traversal(tmp_path)` — [`L156`](../../../../../raw/code/graphify/tests/test_security.py#L156)
- `test_validate_graph_path_default_base_discovers_output_dir(tmp_path)` — [`L174`](../../../../../raw/code/graphify/tests/test_security.py#L174) — With base omitted, the output dir is discovered by walking the path's
- `test_validate_graph_path_default_base_honours_graphify_out_override(tmp_path, monkeypatch)` — [`L183`](../../../../../raw/code/graphify/tests/test_security.py#L183) — The base=None discovery must honour GRAPHIFY_OUT, not the hardcoded
- `test_validate_graph_path_raises_if_file_missing(tmp_path)` — [`L168`](../../../../../raw/code/graphify/tests/test_security.py#L168)
- `test_validate_graph_path_requires_base_exists(tmp_path)` — [`L163`](../../../../../raw/code/graphify/tests/test_security.py#L163)
- `test_validate_url_accepts_http()` — [`L34`](../../../../../raw/code/graphify/tests/test_security.py#L34)
- `test_validate_url_accepts_https()` — [`L37`](../../../../../raw/code/graphify/tests/test_security.py#L37)
- `test_validate_url_rejects_data()` — [`L48`](../../../../../raw/code/graphify/tests/test_security.py#L48)
- `test_validate_url_rejects_empty_scheme()` — [`L52`](../../../../../raw/code/graphify/tests/test_security.py#L52)
- `test_validate_url_rejects_file()` — [`L40`](../../../../../raw/code/graphify/tests/test_security.py#L40)
- `test_validate_url_rejects_ftp()` — [`L44`](../../../../../raw/code/graphify/tests/test_security.py#L44)

