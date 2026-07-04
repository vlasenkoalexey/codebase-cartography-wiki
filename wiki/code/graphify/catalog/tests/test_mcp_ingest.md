---
title: 'Module: tests/test_mcp_ingest.py'
type: catalog
provenance: extracted
module: tests/test_mcp_ingest.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_mcp_ingest`/
symbols:
  _write: _write().
  _label_by_kind: _label_by_kind().
  FIXTURES: FIXTURES.
  test_fixture_emits_every_server: test_fixture_emits_every_server().
  test_fixture_emits_commands_as_global_nodes: test_fixture_emits_commands_as_global_nodes().
  test_fixture_emits_npm_packages: test_fixture_emits_npm_packages().
  test_fixture_emits_python_packages: test_fixture_emits_python_packages().
  test_fixture_strips_version_from_npm_package: test_fixture_strips_version_from_npm_package().
  test_fixture_emits_env_var_names: test_fixture_emits_env_var_names().
  test_fixture_relations_include_contains_references_requires_env: test_fixture_relations_include_contains_references_requires_env().
  test_nested_mcp_servers_shape: test_nested_mcp_servers_shape().
  test_non_dict_server_entry_skipped: test_non_dict_server_entry_skipped().
  test_package_detection_skips_flags: test_package_detection_skips_flags().
  test_no_package_detected_for_unknown_arg_shape: test_no_package_detected_for_unknown_arg_shape().
  test_server_without_command_still_emits_server_node: test_server_without_command_still_emits_server_node().
  test_dispatch_routes_mcp_filename_to_mcp_extractor: test_dispatch_routes_mcp_filename_to_mcp_extractor().
  test_dispatch_does_not_reroute_generic_json: test_dispatch_does_not_reroute_generic_json().
  test_fixture_parses_without_error: test_fixture_parses_without_error().
  test_env_var_values_never_appear_anywhere: test_env_var_values_never_appear_anywhere().
  test_filesystem_path_not_persisted_as_node: test_filesystem_path_not_persisted_as_node().
  test_no_dangling_edges: test_no_dangling_edges().
  test_every_edge_has_confidence_score: test_every_edge_has_confidence_score().
  test_same_command_collapses_to_one_node_across_configs: test_same_command_collapses_to_one_node_across_configs().
  test_same_env_var_collapses_to_one_node_across_configs: test_same_env_var_collapses_to_one_node_across_configs().
  test_same_server_name_in_different_dirs_does_not_collide: test_same_server_name_in_different_dirs_does_not_collide().
  test_missing_mcp_servers_key: test_missing_mcp_servers_key().
  test_is_mcp_config_path_recognises_known_filenames: test_is_mcp_config_path_recognises_known_filenames().
  test_is_mcp_config_path_rejects_generic_json: test_is_mcp_config_path_rejects_generic_json().
  test_recognised_filenames_set_is_frozen: test_recognised_filenames_set_is_frozen().
  test_malformed_json_returns_error: test_malformed_json_returns_error().
  test_oversize_file_skipped: test_oversize_file_skipped().
  test_root_not_an_object: test_root_not_an_object().
  _relations: _relations().
  _labels: _labels().
  _node_kinds: _node_kinds().
---
# Module: [`tests/test_mcp_ingest.py`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py)

## Functions
- `_label_by_kind(result, kind)` — [`L31`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L31)
- `_labels(result)` — [`L19`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L19)
- `_node_kinds(result)` — [`L23`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L23)
- `_relations(result)` — [`L27`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L27)
- `_write(tmp_path: Path, name: str, payload)` — [`L39`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L39)
- `test_dispatch_does_not_reroute_generic_json(tmp_path)` — [`L326`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L326)
- `test_dispatch_routes_mcp_filename_to_mcp_extractor(tmp_path)` — [`L314`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L314)
- `test_env_var_values_never_appear_anywhere()` — [`L119`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L119)
- `test_every_edge_has_confidence_score()` — [`L157`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L157)
- `test_filesystem_path_not_persisted_as_node()` — [`L133`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L133)
- `test_fixture_emits_commands_as_global_nodes()` — [`L84`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L84)
- `test_fixture_emits_env_var_names()` — [`L112`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L112)
- `test_fixture_emits_every_server()` — [`L78`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L78)
- `test_fixture_emits_npm_packages()` — [`L90`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L90)
- `test_fixture_emits_python_packages()` — [`L97`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L97)
- `test_fixture_parses_without_error()` — [`L71`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L71)
- `test_fixture_relations_include_contains_references_requires_env()` — [`L141`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L141)
- `test_fixture_strips_version_from_npm_package()` — [`L104`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L104)
- `test_is_mcp_config_path_recognises_known_filenames()` — [`L51`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L51)
- `test_is_mcp_config_path_rejects_generic_json()` — [`L56`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L56)
- `test_malformed_json_returns_error(tmp_path)` — [`L244`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L244)
- `test_missing_mcp_servers_key(tmp_path)` — [`L225`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L225)
- `test_nested_mcp_servers_shape(tmp_path)` — [`L233`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L233)
- `test_no_dangling_edges()` — [`L149`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L149)
- `test_no_package_detected_for_unknown_arg_shape(tmp_path)` — [`L293`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L293)
- `test_non_dict_server_entry_skipped(tmp_path)` — [`L268`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L268)
- `test_oversize_file_skipped(tmp_path)` — [`L253`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L253)
- `test_package_detection_skips_flags(tmp_path)` — [`L284`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L284)
- `test_recognised_filenames_set_is_frozen()` — [`L62`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L62)
- `test_root_not_an_object(tmp_path)` — [`L261`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L261)
- `test_same_command_collapses_to_one_node_across_configs(tmp_path)` — [`L168`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L168)
- `test_same_env_var_collapses_to_one_node_across_configs(tmp_path)` — [`L184`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L184)
- `test_same_server_name_in_different_dirs_does_not_collide(tmp_path)` — [`L204`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L204)
- `test_server_without_command_still_emits_server_node(tmp_path)` — [`L302`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L302)

## Module values
- `FIXTURES` — [`L16`](../../../../../raw/code/graphify/tests/test_mcp_ingest.py#L16)

