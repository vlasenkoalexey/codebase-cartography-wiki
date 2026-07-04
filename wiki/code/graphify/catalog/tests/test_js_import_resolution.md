---
title: 'Module: tests/test_js_import_resolution.py'
type: catalog
provenance: extracted
module: tests/test_js_import_resolution.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_js_import_resolution`/
symbols:
  _write: _write().
  _extract_for: _extract_for().
  _has_edge: _has_edge().
  _has_symbol_edge: _has_symbol_edge().
  test_js_namespace_reexport_import_targets_real_binding: test_js_namespace_reexport_import_targets_real_binding().
  test_alias_import_edge_resolves_with_relative_input_paths: test_alias_import_edge_resolves_with_relative_input_paths().
  _has_symbol_to_symbol_edge: _has_symbol_to_symbol_edge().
  test_ts_named_reexport_alias_from_index_resolves_imported_symbol_to_origin: test_ts_named_reexport_alias_from_index_resolves_imported_symbol_to_origin().
  test_ts_export_star_from_index_resolves_imported_symbol_to_origin: test_ts_export_star_from_index_resolves_imported_symbol_to_origin().
  test_ts_import_alias_then_reexport_alias_resolves_imported_symbol_to_origin: test_ts_import_alias_then_reexport_alias_resolves_imported_symbol_to_origin().
  test_ts_import_from_index_then_exported_type_alias_resolves_to_origin_symbol: test_ts_import_from_index_then_exported_type_alias_resolves_to_origin_symbol().
  test_ts_reexported_interface_resolves_imported_symbol_to_origin: test_ts_reexported_interface_resolves_imported_symbol_to_origin().
  test_ts_reexported_type_alias_resolves_imported_symbol_to_origin: test_ts_reexported_type_alias_resolves_imported_symbol_to_origin().
  test_ts_reexported_abstract_class_resolves_imported_symbol_to_origin: test_ts_reexported_abstract_class_resolves_imported_symbol_to_origin().
  test_ts_const_alias_reexport_resolves_imported_symbol_to_origin: test_ts_const_alias_reexport_resolves_imported_symbol_to_origin().
  test_ts_local_const_alias_then_named_reexport_resolves_imported_symbol_to_origin: test_ts_local_const_alias_then_named_reexport_resolves_imported_symbol_to_origin().
  test_ts_type_relationships_and_contexts: test_ts_type_relationships_and_contexts().
  test_ts_bare_relative_import_resolves_existing_ts_file: test_ts_bare_relative_import_resolves_existing_ts_file().
  test_ts_directory_import_resolves_index_ts: test_ts_directory_import_resolves_index_ts().
  test_ts_reexport_cycle_resolves_symbol_from_non_cycle_branch: test_ts_reexport_cycle_resolves_symbol_from_non_cycle_branch().
  test_ts_reexport_chain_beyond_sixteen_hops_resolves_origin: test_ts_reexport_chain_beyond_sixteen_hops_resolves_origin().
  test_ts_arrow_function_call_through_barrel_targets_origin_symbol: test_ts_arrow_function_call_through_barrel_targets_origin_symbol().
  test_ts_import_alias_does_not_affect_same_named_local_symbol_when_unused: test_ts_import_alias_does_not_affect_same_named_local_symbol_when_unused().
  test_ts_import_alias_call_from_same_named_local_symbol_targets_origin: test_ts_import_alias_call_from_same_named_local_symbol_targets_origin().
  test_svelte_rune_import_resolves_svelte_ts_file: test_svelte_rune_import_resolves_svelte_ts_file().
  test_tsconfig_alias_import_resolves_existing_ts_file: test_tsconfig_alias_import_resolves_existing_ts_file().
  test_tsconfig_alias_with_subdirectory_baseurl_resolves_existing_ts_file: test_tsconfig_alias_with_subdirectory_baseurl_resolves_existing_ts_file().
  test_tsconfig_array_extends_alias_resolves_existing_ts_file: test_tsconfig_array_extends_alias_resolves_existing_ts_file().
  test_default_import_resolves_to_default_exported_class: test_default_import_resolves_to_default_exported_class().
  test_default_import_with_renamed_binding_resolves_to_origin: test_default_import_with_renamed_binding_resolves_to_origin().
  test_export_default_identifier_resolves_default_import: test_export_default_identifier_resolves_default_import().
  test_default_import_call_resolves_to_default_exported_function: test_default_import_call_resolves_to_default_exported_function().
  test_pnpm_workspace_package_import_resolves_package_entry: test_pnpm_workspace_package_import_resolves_package_entry().
  test_npm_workspace_package_import_resolves_package_entry: test_npm_workspace_package_import_resolves_package_entry().
  test_yarn_workspace_package_import_resolves_package_entry: test_yarn_workspace_package_import_resolves_package_entry().
  test_pnpm_workspace_takes_precedence_over_package_json_workspaces: test_pnpm_workspace_takes_precedence_over_package_json_workspaces().
  test_workspace_subpath_export_string_resolves: test_workspace_subpath_export_string_resolves().
  test_workspace_subpath_export_condition_object_resolves: test_workspace_subpath_export_condition_object_resolves().
  test_workspace_subpath_export_wildcard_resolves: test_workspace_subpath_export_wildcard_resolves().
  test_workspace_subpath_export_falls_back_to_filesystem: test_workspace_subpath_export_falls_back_to_filesystem().
  test_workspace_subpath_export_rejects_path_escape: test_workspace_subpath_export_rejects_path_escape().
  test_workspace_subpath_export_default_consulted_last: test_workspace_subpath_export_default_consulted_last().
  test_js_import_resolution_ignores_stale_importer_cache_when_target_appears: test_js_import_resolution_ignores_stale_importer_cache_when_target_appears().
  test_workspace_package_cache_refreshes_between_extract_calls: test_workspace_package_cache_refreshes_between_extract_calls().
  test_tsconfig_alias_resolves_second_target_when_first_missing: test_tsconfig_alias_resolves_second_target_when_first_missing().
  test_tsconfig_alias_first_target_wins_when_both_exist: test_tsconfig_alias_first_target_wins_when_both_exist().
  test_tsconfig_alias_none_exist_creates_no_false_edge: test_tsconfig_alias_none_exist_creates_no_false_edge().
  test_tsconfig_wildcard_alias_substitutes_captured_path: test_tsconfig_wildcard_alias_substitutes_captured_path().
  test_tsconfig_wildcard_alias_substitutes_before_suffix: test_tsconfig_wildcard_alias_substitutes_before_suffix().
  test_tsconfig_wildcard_alias_substitutes_before_normalizing_target: test_tsconfig_wildcard_alias_substitutes_before_normalizing_target().
  test_tsconfig_wildcard_alias_allows_empty_capture: test_tsconfig_wildcard_alias_allows_empty_capture().
  test_tsconfig_wildcard_alias_prefers_longest_matching_prefix: test_tsconfig_wildcard_alias_prefers_longest_matching_prefix().
  test_tsconfig_exact_alias_still_resolves: test_tsconfig_exact_alias_still_resolves().
  test_pnpm_workspace_dot_package_does_not_crash: test_pnpm_workspace_dot_package_does_not_crash().
  _has_no_symbol_to_symbol_edge: _has_no_symbol_to_symbol_edge().
  test_ts_type_relationships_and_contexts._norm: test_ts_type_relationships_and_contexts()._norm().
---
# Module: [`tests/test_js_import_resolution.py`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py)

## Functions
- `_extract_for(paths: list[Path], root: Path)` — [`L17`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L17)
- `_has_edge(result: dict, source: str, target: str, relation: str = "imports_from")` — [`L21`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L21)
- `_has_no_symbol_to_symbol_edge(result: dict, source_file: str, source_symbol: str, target_file: str, target_symbol: str, relation: str)` — [`L65`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L65)
- `_has_symbol_edge(result: dict, source: str, target_file: str, symbol: str, relation: str = "imports")` — [`L30`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L30)
- `_has_symbol_to_symbol_edge(result: dict, source_file: str, source_symbol: str, target_file: str, target_symbol: str, relation: str)` — [`L45`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L45)
- `_norm(label: str)` — [`L893`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L893)
- `_write(path: Path, text: str)` — [`L11`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L11)
- `test_alias_import_edge_resolves_with_relative_input_paths(tmp_path, monkeypatch)` — [`L1142`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L1142)
- `test_default_import_call_resolves_to_default_exported_function(tmp_path: Path)` — [`L508`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L508)
- `test_default_import_resolves_to_default_exported_class(tmp_path: Path)` — [`L470`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L470)
- `test_default_import_with_renamed_binding_resolves_to_origin(tmp_path: Path)` — [`L482`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L482)
- `test_export_default_identifier_resolves_default_import(tmp_path: Path)` — [`L496`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L496)
- `test_js_import_resolution_ignores_stale_importer_cache_when_target_appears(tmp_path: Path)` — [`L807`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L807)
- `test_js_namespace_reexport_import_targets_real_binding(tmp_path: Path, monkeypatch, suffix: str)` — [`L144`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L144)
- `test_npm_workspace_package_import_resolves_package_entry(tmp_path: Path)` — [`L548`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L548)
- `test_pnpm_workspace_dot_package_does_not_crash(tmp_path: Path)` — [`L849`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L849) — packages: - '.' in pnpm-workspace.yaml must not raise IndexError on any Python version.
- `test_pnpm_workspace_package_import_resolves_package_entry(tmp_path: Path)` — [`L525`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L525)
- `test_pnpm_workspace_takes_precedence_over_package_json_workspaces(tmp_path: Path)` — [`L594`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L594)
- `test_svelte_rune_import_resolves_svelte_ts_file(tmp_path: Path)` — [`L395`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L395)
- `test_ts_arrow_function_call_through_barrel_targets_origin_symbol(tmp_path: Path)` — [`L334`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L334)
- `test_ts_bare_relative_import_resolves_existing_ts_file(tmp_path: Path)` — [`L83`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L83)
- `test_ts_const_alias_reexport_resolves_imported_symbol_to_origin(tmp_path: Path)` — [`L300`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L300)
- `test_ts_directory_import_resolves_index_ts(tmp_path: Path)` — [`L95`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L95)
- `test_ts_export_star_from_index_resolves_imported_symbol_to_origin(tmp_path: Path)` — [`L129`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L129)
- `test_ts_import_alias_call_from_same_named_local_symbol_targets_origin(tmp_path: Path)` — [`L375`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L375)
- `test_ts_import_alias_does_not_affect_same_named_local_symbol_when_unused(tmp_path: Path)` — [`L355`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L355)
- `test_ts_import_alias_then_reexport_alias_resolves_imported_symbol_to_origin(tmp_path: Path)` — [`L227`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L227)
- `test_ts_import_from_index_then_exported_type_alias_resolves_to_origin_symbol(tmp_path: Path)` — [`L244`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L244)
- `test_ts_local_const_alias_then_named_reexport_resolves_imported_symbol_to_origin(tmp_path: Path)` — [`L317`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L317)
- `test_ts_named_reexport_alias_from_index_resolves_imported_symbol_to_origin(tmp_path: Path)` — [`L107`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L107)
- `test_ts_reexport_chain_beyond_sixteen_hops_resolves_origin(tmp_path: Path)` — [`L206`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L206)
- `test_ts_reexport_cycle_resolves_symbol_from_non_cycle_branch(tmp_path: Path)` — [`L189`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L189)
- `test_ts_reexported_abstract_class_resolves_imported_symbol_to_origin(tmp_path: Path)` — [`L286`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L286)
- `test_ts_reexported_interface_resolves_imported_symbol_to_origin(tmp_path: Path)` — [`L258`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L258)
- `test_ts_reexported_type_alias_resolves_imported_symbol_to_origin(tmp_path: Path)` — [`L272`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L272)
- `test_ts_type_relationships_and_contexts(tmp_path: Path)` — [`L873`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L873)
- `test_tsconfig_alias_first_target_wins_when_both_exist(tmp_path: Path)` — [`L935`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L935)
- `test_tsconfig_alias_import_resolves_existing_ts_file(tmp_path: Path)` — [`L407`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L407)
- `test_tsconfig_alias_none_exist_creates_no_false_edge(tmp_path: Path)` — [`L955`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L955)
- `test_tsconfig_alias_resolves_second_target_when_first_missing(tmp_path: Path)` — [`L916`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L916)
- `test_tsconfig_alias_with_subdirectory_baseurl_resolves_existing_ts_file(tmp_path: Path)` — [`L423`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L423)
- `test_tsconfig_array_extends_alias_resolves_existing_ts_file(tmp_path: Path)` — [`L444`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L444)
- `test_tsconfig_exact_alias_still_resolves(tmp_path: Path)` — [`L1118`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L1118)
- `test_tsconfig_wildcard_alias_allows_empty_capture(tmp_path: Path)` — [`L1068`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L1068)
- `test_tsconfig_wildcard_alias_prefers_longest_matching_prefix(tmp_path: Path)` — [`L1089`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L1089)
- `test_tsconfig_wildcard_alias_substitutes_before_normalizing_target(tmp_path: Path)` — [`L1040`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L1040)
- `test_tsconfig_wildcard_alias_substitutes_before_suffix(tmp_path: Path)` — [`L1012`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L1012)
- `test_tsconfig_wildcard_alias_substitutes_captured_path(tmp_path, monkeypatch)` — [`L977`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L977)
- `test_workspace_package_cache_refreshes_between_extract_calls(tmp_path: Path)` — [`L822`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L822)
- `test_workspace_subpath_export_condition_object_resolves(tmp_path: Path)` — [`L650`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L650)
- `test_workspace_subpath_export_default_consulted_last(tmp_path: Path)` — [`L768`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L768)
- `test_workspace_subpath_export_falls_back_to_filesystem(tmp_path: Path)` — [`L711`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L711)
- `test_workspace_subpath_export_rejects_path_escape(tmp_path: Path)` — [`L734`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L734)
- `test_workspace_subpath_export_string_resolves(tmp_path: Path)` — [`L621`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L621)
- `test_workspace_subpath_export_wildcard_resolves(tmp_path: Path)` — [`L683`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L683)
- `test_yarn_workspace_package_import_resolves_package_entry(tmp_path: Path)` — [`L571`](../../../../../raw/code/graphify/tests/test_js_import_resolution.py#L571)

