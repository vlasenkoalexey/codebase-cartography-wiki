---
title: 'Module: tests/test_extract.py'
type: catalog
provenance: extracted
module: tests/test_extract.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_extract`/
symbols:
  FIXTURES: FIXTURES.
  test_extract_generic_surfaces_tree_sitter_version_mismatch_hint: test_extract_generic_surfaces_tree_sitter_version_mismatch_hint().
  test_extract_falls_back_to_sequential_when_parallel_returns_false: test_extract_falls_back_to_sequential_when_parallel_returns_false().
  _legacy_collect_files: _legacy_collect_files().
  test_extract_js_destructured_require_named_symbols: test_extract_js_destructured_require_named_symbols().
  test_extract_js_member_require_emits_property_symbol: test_extract_js_member_require_emits_property_symbol().
  test_extract_bash_skip_builtins_in_calls: test_extract_bash_skip_builtins_in_calls().
  test_collect_files_from_dir: test_collect_files_from_dir().
  test_collect_files_parity_with_legacy_on_fixtures: test_collect_files_parity_with_legacy_on_fixtures().
  test_extract_tsx_uses_tsx_grammar: test_extract_tsx_uses_tsx_grammar().
  test_extract_parallel_returns_false_on_broken_pool: test_extract_parallel_returns_false_on_broken_pool().
  test_extract_bash_missing_grammar_returns_error: test_extract_bash_missing_grammar_returns_error().
  test_dart_child_node_ids_are_stem_based: test_dart_child_node_ids_are_stem_based().
  test_non_colliding_path_id_is_not_salted: test_non_colliding_path_id_is_not_salted().
  test_extract_python_finds_class: test_extract_python_finds_class().
  test_extract_python_finds_methods: test_extract_python_finds_methods().
  test_extract_python_no_dangling_edges: test_extract_python_no_dangling_edges().
  test_structural_edges_are_extracted: test_structural_edges_are_extracted().
  test_extract_merges_multiple_files: test_extract_merges_multiple_files().
  test_collect_files_skips_hidden: test_collect_files_skips_hidden().
  test_collect_files_parity_with_legacy_synthetic: test_collect_files_parity_with_legacy_synthetic().
  test_collect_files_walks_each_directory_once: test_collect_files_walks_each_directory_once().
  test_no_dangling_edges_on_extract: test_no_dangling_edges_on_extract().
  test_calls_edges_emitted: test_calls_edges_emitted().
  test_calls_edges_are_extracted: test_calls_edges_are_extracted().
  test_python_call_edges_have_call_context: test_python_call_edges_have_call_context().
  test_calls_no_self_loops: test_calls_no_self_loops().
  test_run_analysis_calls_compute_score: test_run_analysis_calls_compute_score().
  test_run_analysis_calls_normalize: test_run_analysis_calls_normalize().
  test_method_calls_module_function: test_method_calls_module_function().
  test_calls_deduplication: test_calls_deduplication().
  test_extract_js_destructured_require_imports_from: test_extract_js_destructured_require_imports_from().
  test_extract_js_arrow_function_still_extracted: test_extract_js_arrow_function_still_extracted().
  test_extract_js_this_assigned_methods: test_extract_js_this_assigned_methods().
  test_extract_tsx_finds_helpers_and_component: test_extract_tsx_finds_helpers_and_component().
  test_extract_tsx_jsx_expression_calls_resolve: test_extract_tsx_jsx_expression_calls_resolve().
  test_extract_bash_finds_functions: test_extract_bash_finds_functions().
  test_extract_bash_emits_defines_edges: test_extract_bash_emits_defines_edges().
  test_extract_bash_emits_calls_edges: test_extract_bash_emits_calls_edges().
  test_extract_bash_calls_have_extracted_confidence: test_extract_bash_calls_have_extracted_confidence().
  test_extract_bash_no_self_loops: test_extract_bash_no_self_loops().
  test_extract_bash_no_dangling_edges: test_extract_bash_no_dangling_edges().
  test_extract_json_top_level_keys: test_extract_json_top_level_keys().
  test_extract_json_nested_contains: test_extract_json_nested_contains().
  test_extract_json_dependencies_become_imports: test_extract_json_dependencies_become_imports().
  test_extract_json_extends_resolved: test_extract_json_extends_resolved().
  test_extract_json_no_self_loops: test_extract_json_no_self_loops().
  test_extract_bash_via_dispatch: test_extract_bash_via_dispatch().
  test_extract_json_via_dispatch: test_extract_json_via_dispatch().
  test_extract_bash_node_metadata_is_sanitized: test_extract_bash_node_metadata_is_sanitized().
  test_barrel_reexport_emits_re_exports_edges: test_barrel_reexport_emits_re_exports_edges().
  test_barrel_reexport_emits_imports_from: test_barrel_reexport_emits_imports_from().
  test_barrel_reexport_context_tagged: test_barrel_reexport_context_tagged().
  test_barrel_local_exports_still_extracted: test_barrel_local_exports_still_extracted().
  test_barrel_reexport_confidence_extracted: test_barrel_reexport_confidence_extracted().
  test_make_id_strips_dots_and_underscores: test_make_id_strips_dots_and_underscores().
  test_make_id_consistent: test_make_id_consistent().
  test_make_id_no_leading_trailing_underscores: test_make_id_no_leading_trailing_underscores().
  test_extract_disambiguates_duplicate_symbol_ids_by_source_path: test_extract_disambiguates_duplicate_symbol_ids_by_source_path().
  test_cross_file_type_annotation_refs_resolve_to_single_node: test_cross_file_type_annotation_refs_resolve_to_single_node().
  test_go_cross_file_type_refs_resolve_to_single_node: test_go_cross_file_type_refs_resolve_to_single_node().
  test_imported_type_stubs_do_not_collide_across_source_files: test_imported_type_stubs_do_not_collide_across_source_files().
  test_origin_file_is_not_serialized_into_extract_output: test_origin_file_is_not_serialized_into_extract_output().
  test_go_imported_type_stubs_do_not_collide_across_source_files: test_go_imported_type_stubs_do_not_collide_across_source_files().
  test_extract_updates_raw_call_callers_after_duplicate_id_disambiguation: test_extract_updates_raw_call_callers_after_duplicate_id_disambiguation().
  test_extract_rewires_unique_inheritance_stub_to_real_definition: test_extract_rewires_unique_inheritance_stub_to_real_definition().
  test_extract_keeps_stub_when_multiple_real_definitions_match: test_extract_keeps_stub_when_multiple_real_definitions_match().
  test_extract_does_not_rewire_inheritance_stub_to_same_named_function: test_extract_does_not_rewire_inheritance_stub_to_same_named_function().
  test_extract_does_not_rewire_constructor_method_to_same_named_class: test_extract_does_not_rewire_constructor_method_to_same_named_class().
  test_collect_files_follows_symlinked_directory: test_collect_files_follows_symlinked_directory().
  test_collect_files_skips_out_of_root_symlinked_directory: test_collect_files_skips_out_of_root_symlinked_directory().
  test_collect_files_skips_out_of_root_symlinked_file_by_default: test_collect_files_skips_out_of_root_symlinked_file_by_default().
  test_collect_files_handles_circular_symlinks: test_collect_files_handles_circular_symlinks().
  test_cross_file_calls_skip_ambiguous_duplicate_labels: test_cross_file_calls_skip_ambiguous_duplicate_labels().
  test_cross_file_call_survives_same_named_test_mock: test_cross_file_call_survives_same_named_test_mock().
  test_cross_file_call_god_node_guard_two_real_defs: test_cross_file_call_god_node_guard_two_real_defs().
  test_cross_file_call_survives_many_test_mocks: test_cross_file_call_survives_many_test_mocks().
  test_extract_js_commonjs_exports_assignment: test_extract_js_commonjs_exports_assignment().
  test_extract_js_prototype_method_assignment: test_extract_js_prototype_method_assignment().
  test_extract_js_const_function_expression: test_extract_js_const_function_expression().
  test_extract_ts_class_arrow_field: test_extract_ts_class_arrow_field().
  test_extract_js_arbitrary_member_assignment_not_captured: test_extract_js_arbitrary_member_assignment_not_captured().
  test_cross_file_call_promoted_to_extracted_with_import_evidence: test_cross_file_call_promoted_to_extracted_with_import_evidence().
  test_cross_file_call_remains_inferred_without_import_evidence: test_cross_file_call_remains_inferred_without_import_evidence().
  test_python_qualified_class_method_call_resolves_extracted: test_python_qualified_class_method_call_resolves_extracted().
  test_python_qualified_call_resolves_when_method_name_collides_with_caller: test_python_qualified_call_resolves_when_method_name_collides_with_caller().
  test_python_instance_member_call_not_overconnected: test_python_instance_member_call_not_overconnected().
  test_python_qualified_call_ambiguous_class_bails: test_python_qualified_call_ambiguous_class_bails().
  test_dispatch_includes_sh_and_json: test_dispatch_includes_sh_and_json().
  test_extract_bash_emits_source_imports_from: test_extract_bash_emits_source_imports_from().
  test_extract_bash_rejects_command_substitution_as_call: test_extract_bash_rejects_command_substitution_as_call().
  test_extract_bash_process_substitution_not_recorded: test_extract_bash_process_substitution_not_recorded().
  test_extract_bash_shadowing_function_is_recorded: test_extract_bash_shadowing_function_is_recorded().
  test_extract_bash_creates_entrypoint_node: test_extract_bash_creates_entrypoint_node().
  test_extract_bash_top_level_call_attributes_to_entrypoint: test_extract_bash_top_level_call_attributes_to_entrypoint().
  test_extract_bash_entrypoint_no_collision_with_function_named_script: test_extract_bash_entrypoint_no_collision_with_function_named_script().
  test_extract_bash_nested_function_calls_recorded: test_extract_bash_nested_function_calls_recorded().
  test_extract_bash_source_user_defined_emits_calls_not_imports_from: test_extract_bash_source_user_defined_emits_calls_not_imports_from().
  test_extract_json_large_file_skipped: test_extract_json_large_file_skipped().
  test_extract_json_handles_invalid_json: test_extract_json_handles_invalid_json().
  test_extract_json_data_file_skipped: test_extract_json_data_file_skipped().
  test_extract_json_top_level_array_skipped: test_extract_json_top_level_array_skipped().
  test_extract_json_config_by_filename_still_extracted: test_extract_json_config_by_filename_still_extracted().
  test_extract_json_config_by_key_probe: test_extract_json_config_by_key_probe().
  test_semantic_reference_edges_carry_context_and_source: test_semantic_reference_edges_carry_context_and_source().
  test_pure_export_no_from_not_treated_as_reexport: test_pure_export_no_from_not_treated_as_reexport().
  test_separator_collision_paths_get_distinct_ids: test_separator_collision_paths_get_distinct_ids().
  test_collect_files_walks_each_directory_once.counting_scandir: test_collect_files_walks_each_directory_once().counting_scandir().
  test_extract_generic_surfaces_tree_sitter_version_mismatch_hint._raise: test_extract_generic_surfaces_tree_sitter_version_mismatch_hint()._raise().
  by_label_by_id: by_label_by_id().
  test_extract_falls_back_to_sequential_when_parallel_returns_false.fake_parallel: test_extract_falls_back_to_sequential_when_parallel_returns_false().fake_parallel().
  test_extract_falls_back_to_sequential_when_parallel_returns_false.wrapped_sequential: test_extract_falls_back_to_sequential_when_parallel_returns_false().wrapped_sequential().
  test_extract_parallel_returns_false_on_broken_pool.FakePool: test_extract_parallel_returns_false_on_broken_pool().FakePool#
  test_extract_bash_missing_grammar_returns_error.patched: test_extract_bash_missing_grammar_returns_error().patched().
  test_extract_parallel_returns_false_on_broken_pool.FakePool.__init__: test_extract_parallel_returns_false_on_broken_pool().FakePool#__init__().
  test_extract_parallel_returns_false_on_broken_pool.FakePool.__enter__: test_extract_parallel_returns_false_on_broken_pool().FakePool#__enter__().
  test_extract_parallel_returns_false_on_broken_pool.FakePool.__exit__: test_extract_parallel_returns_false_on_broken_pool().FakePool#__exit__().
  test_extract_parallel_returns_false_on_broken_pool.FakePool.submit: test_extract_parallel_returns_false_on_broken_pool().FakePool#submit().
---
# Module: [`tests/test_extract.py`](../../../../../raw/code/graphify/tests/test_extract.py)

## Classes
### `FakePool`
- def: [`tests/test_extract.py:1102`](../../../../../raw/code/graphify/tests/test_extract.py#L1102)
- signature: `class FakePool:`
- members:
  - `submit(self, *a, **kw)` — [`L1106`](../../../../../raw/code/graphify/tests/test_extract.py#L1106)
- protocol/private: `__enter__`[`L1104`](../../../../../raw/code/graphify/tests/test_extract.py#L1104), `__exit__`[`L1105`](../../../../../raw/code/graphify/tests/test_extract.py#L1105), `__init__`[`L1103`](../../../../../raw/code/graphify/tests/test_extract.py#L1103)
- used by: (1 test-only callers)

## Functions
- `_legacy_collect_files(target, *, root=None)` — [`L401`](../../../../../raw/code/graphify/tests/test_extract.py#L401) — The pre-#1261 rglob-per-extension implementation, kept as a parity oracle.
- `_raise(*args, **kwargs)` — [`L685`](../../../../../raw/code/graphify/tests/test_extract.py#L685)
- `by_label_by_id(result, node_id)` — [`L849`](../../../../../raw/code/graphify/tests/test_extract.py#L849)
- `counting_scandir(path=".", *args, **kwargs)` — [`L466`](../../../../../raw/code/graphify/tests/test_extract.py#L466)
- `fake_parallel(uncached_work, per_file, effective_root, max_workers, total_files)` — [`L1079`](../../../../../raw/code/graphify/tests/test_extract.py#L1079)
- `patched(name, *args, **kwargs)` — [`L1216`](../../../../../raw/code/graphify/tests/test_extract.py#L1216)
- `test_barrel_local_exports_still_extracted()` — [`L1568`](../../../../../raw/code/graphify/tests/test_extract.py#L1568) — export function/const in a barrel file must still create nodes.
- `test_barrel_reexport_confidence_extracted()` — [`L1578`](../../../../../raw/code/graphify/tests/test_extract.py#L1578) — All re_exports edges should have confidence=EXTRACTED.
- `test_barrel_reexport_context_tagged()` — [`L1559`](../../../../../raw/code/graphify/tests/test_extract.py#L1559) — re_exports edges should have context='re-export'.
- `test_barrel_reexport_emits_imports_from()` — [`L1548`](../../../../../raw/code/graphify/tests/test_extract.py#L1548) — Barrel file must emit file-level imports_from edges to source modules.
- `test_barrel_reexport_emits_re_exports_edges()` — [`L1534`](../../../../../raw/code/graphify/tests/test_extract.py#L1534) — export { X } from './mod' must emit re_exports edges for each named specifier.
- `test_calls_deduplication()` — [`L558`](../../../../../raw/code/graphify/tests/test_extract.py#L558) — Same caller→callee pair must appear only once even if called multiple times.
- `test_calls_edges_are_extracted()` — [`L503`](../../../../../raw/code/graphify/tests/test_extract.py#L503) — AST-resolved call edges are deterministic and should be EXTRACTED/1.0.
- `test_calls_edges_emitted()` — [`L496`](../../../../../raw/code/graphify/tests/test_extract.py#L496) — Call-graph pass must produce INFERRED calls edges.
- `test_calls_no_self_loops()` — [`L519`](../../../../../raw/code/graphify/tests/test_extract.py#L519)
- `test_collect_files_follows_symlinked_directory(tmp_path)` — [`L352`](../../../../../raw/code/graphify/tests/test_extract.py#L352)
- `test_collect_files_from_dir()` — [`L338`](../../../../../raw/code/graphify/tests/test_extract.py#L338)
- `test_collect_files_handles_circular_symlinks(tmp_path)` — [`L391`](../../../../../raw/code/graphify/tests/test_extract.py#L391)
- `test_collect_files_parity_with_legacy_on_fixtures()` — [`L417`](../../../../../raw/code/graphify/tests/test_extract.py#L417)
- `test_collect_files_parity_with_legacy_synthetic(tmp_path)` — [`L421`](../../../../../raw/code/graphify/tests/test_extract.py#L421)
- `test_collect_files_skips_hidden()` — [`L346`](../../../../../raw/code/graphify/tests/test_extract.py#L346)
- `test_collect_files_skips_out_of_root_symlinked_directory(tmp_path)` — [`L365`](../../../../../raw/code/graphify/tests/test_extract.py#L365)
- `test_collect_files_skips_out_of_root_symlinked_file_by_default(tmp_path)` — [`L378`](../../../../../raw/code/graphify/tests/test_extract.py#L378)
- `test_collect_files_walks_each_directory_once(tmp_path, monkeypatch)` — [`L452`](../../../../../raw/code/graphify/tests/test_extract.py#L452) — collect_files must scan every directory at most once and never descend
- `test_cross_file_call_god_node_guard_two_real_defs(tmp_path)` — [`L619`](../../../../../raw/code/graphify/tests/test_extract.py#L619) — Two genuine NON-test defs of the same name + one caller => ZERO edges.
- `test_cross_file_call_promoted_to_extracted_with_import_evidence(tmp_path)` — [`L856`](../../../../../raw/code/graphify/tests/test_extract.py#L856) — A cross-file `calls` edge must be EXTRACTED when the caller's file has
- `test_cross_file_call_remains_inferred_without_import_evidence(tmp_path)` — [`L882`](../../../../../raw/code/graphify/tests/test_extract.py#L882) — A cross-file `calls` edge must stay INFERRED when there is no import
- `test_cross_file_call_survives_many_test_mocks(tmp_path)` — [`L648`](../../../../../raw/code/graphify/tests/test_extract.py#L648) — One src def + many same-named test stubs + caller => exactly one src edge.
- `test_cross_file_call_survives_same_named_test_mock(tmp_path)` — [`L587`](../../../../../raw/code/graphify/tests/test_extract.py#L587) — A real cross-file call must NOT be erased by a same-named test mock.
- `test_cross_file_calls_skip_ambiguous_duplicate_labels(tmp_path)` — [`L565`](../../../../../raw/code/graphify/tests/test_extract.py#L565) — Unqualified cross-file calls must not guess between duplicate helper names.
- `test_cross_file_type_annotation_refs_resolve_to_single_node(tmp_path)` — [`L103`](../../../../../raw/code/graphify/tests/test_extract.py#L103) — #1402: a class defined once but referenced via type annotations in N other
- `test_dart_child_node_ids_are_stem_based(tmp_path)` — [`L1623`](../../../../../raw/code/graphify/tests/test_extract.py#L1623) — Dart child node IDs must be built from _file_stem rather than absolute path.
- `test_dispatch_includes_sh_and_json()` — [`L1126`](../../../../../raw/code/graphify/tests/test_extract.py#L1126)
- `test_extract_bash_calls_have_extracted_confidence()` — [`L1156`](../../../../../raw/code/graphify/tests/test_extract.py#L1156)
- `test_extract_bash_creates_entrypoint_node(tmp_path)` — [`L1283`](../../../../../raw/code/graphify/tests/test_extract.py#L1283) — Every bash file produces a `bash_entrypoint` node distinct from the file node, joined by a `contains` edge.
- `test_extract_bash_emits_calls_edges()` — [`L1147`](../../../../../raw/code/graphify/tests/test_extract.py#L1147)
- `test_extract_bash_emits_defines_edges()` — [`L1141`](../../../../../raw/code/graphify/tests/test_extract.py#L1141)
- `test_extract_bash_emits_source_imports_from(tmp_path)` — [`L1164`](../../../../../raw/code/graphify/tests/test_extract.py#L1164)
- `test_extract_bash_entrypoint_no_collision_with_function_named_script(tmp_path)` — [`L1331`](../../../../../raw/code/graphify/tests/test_extract.py#L1331) — Entrypoint node must have a distinct ID from a function also named 'script'.
- `test_extract_bash_finds_functions()` — [`L1132`](../../../../../raw/code/graphify/tests/test_extract.py#L1132)
- `test_extract_bash_missing_grammar_returns_error()` — [`L1210`](../../../../../raw/code/graphify/tests/test_extract.py#L1210) — extract_bash returns error dict when tree-sitter-bash not installed (mocked).
- `test_extract_bash_nested_function_calls_recorded(tmp_path)` — [`L1352`](../../../../../raw/code/graphify/tests/test_extract.py#L1352) — Calls made inside a nested (inner) function body must be collected.
- `test_extract_bash_no_dangling_edges()` — [`L1181`](../../../../../raw/code/graphify/tests/test_extract.py#L1181)
- `test_extract_bash_no_self_loops()` — [`L1175`](../../../../../raw/code/graphify/tests/test_extract.py#L1175)
- `test_extract_bash_node_metadata_is_sanitized()` — [`L1515`](../../../../../raw/code/graphify/tests/test_extract.py#L1515) — Bash extractor must route node metadata through sanitize_metadata so
- `test_extract_bash_process_substitution_not_recorded(tmp_path)` — [`L1245`](../../../../../raw/code/graphify/tests/test_extract.py#L1245) — `<(helper)` (process substitution) must not be recorded as a call edge.
- `test_extract_bash_rejects_command_substitution_as_call(tmp_path)` — [`L1227`](../../../../../raw/code/graphify/tests/test_extract.py#L1227) — `$(build)` must not be recorded as a call edge to build().
- `test_extract_bash_shadowing_function_is_recorded(tmp_path)` — [`L1263`](../../../../../raw/code/graphify/tests/test_extract.py#L1263) — User-defined function shadowing an external command (install/find/etc.) must still produce a call edge.
- `test_extract_bash_skip_builtins_in_calls()` — [`L1191`](../../../../../raw/code/graphify/tests/test_extract.py#L1191)
- `test_extract_bash_source_user_defined_emits_calls_not_imports_from(tmp_path)` — [`L1377`](../../../../../raw/code/graphify/tests/test_extract.py#L1377) — When 'source' is a user-defined function, 'source ./file.sh' must emit a
- `test_extract_bash_top_level_call_attributes_to_entrypoint(tmp_path)` — [`L1300`](../../../../../raw/code/graphify/tests/test_extract.py#L1300) — Top-level function call attaches to the entrypoint node, not orphaned.
- `test_extract_bash_via_dispatch()` — [`L1504`](../../../../../raw/code/graphify/tests/test_extract.py#L1504)
- `test_extract_disambiguates_duplicate_symbol_ids_by_source_path(tmp_path)` — [`L62`](../../../../../raw/code/graphify/tests/test_extract.py#L62)
- `test_extract_does_not_rewire_constructor_method_to_same_named_class(tmp_path)` — [`L316`](../../../../../raw/code/graphify/tests/test_extract.py#L316)
- `test_extract_does_not_rewire_inheritance_stub_to_same_named_function(tmp_path)` — [`L294`](../../../../../raw/code/graphify/tests/test_extract.py#L294)
- `test_extract_falls_back_to_sequential_when_parallel_returns_false(tmp_path, monkeypatch)` — [`L1068`](../../../../../raw/code/graphify/tests/test_extract.py#L1068) — extract() must run sequential when _extract_parallel signals failure (returns False).
- `test_extract_generic_surfaces_tree_sitter_version_mismatch_hint(monkeypatch)` — [`L672`](../../../../../raw/code/graphify/tests/test_extract.py#L672) — When Language() raises TypeError (e.g. old tree-sitter binding meets a
- `test_extract_js_arbitrary_member_assignment_not_captured(tmp_path)` — [`L834`](../../../../../raw/code/graphify/tests/test_extract.py#L834) — Guard against the phantom-god-node class (#1077): an arbitrary
- `test_extract_js_arrow_function_still_extracted()` — [`L737`](../../../../../raw/code/graphify/tests/test_extract.py#L737) — Regression: arrow functions in lexical_declaration must still produce nodes.
- `test_extract_js_commonjs_exports_assignment(tmp_path)` — [`L782`](../../../../../raw/code/graphify/tests/test_extract.py#L782) — `exports.X = fn` and `module.exports.X = fn` must produce function nodes.
- `test_extract_js_const_function_expression(tmp_path)` — [`L808`](../../../../../raw/code/graphify/tests/test_extract.py#L808) — `const f = function(){}` (function expression, not arrow) must be captured.
- `test_extract_js_destructured_require_imports_from()` — [`L704`](../../../../../raw/code/graphify/tests/test_extract.py#L704) — `const { foo } = require('./mod')` must emit imports_from to the resolved module path.
- `test_extract_js_destructured_require_named_symbols()` — [`L718`](../../../../../raw/code/graphify/tests/test_extract.py#L718) — Destructured CJS requires must emit symbol-level `imports` edges per binder.
- `test_extract_js_member_require_emits_property_symbol()` — [`L728`](../../../../../raw/code/graphify/tests/test_extract.py#L728) — `const x = require('./m').y` must emit symbol edge for `y`.
- `test_extract_js_prototype_method_assignment(tmp_path)` — [`L795`](../../../../../raw/code/graphify/tests/test_extract.py#L795) — `Foo.prototype.bar = fn` must be captured as a method owned by Foo.
- `test_extract_js_this_assigned_methods(tmp_path)` — [`L750`](../../../../../raw/code/graphify/tests/test_extract.py#L750) — `this.X = () => {}` / `this.X = function(){}` in a constructor-style
- `test_extract_json_config_by_filename_still_extracted(tmp_path)` — [`L1485`](../../../../../raw/code/graphify/tests/test_extract.py#L1485) — tsconfig.json must still be AST-extracted even without telltale keys.
- `test_extract_json_config_by_key_probe(tmp_path)` — [`L1494`](../../../../../raw/code/graphify/tests/test_extract.py#L1494) — An arbitrarily-named JSON with config keys (dependencies) is still extracted.
- `test_extract_json_data_file_skipped(tmp_path)` — [`L1462`](../../../../../raw/code/graphify/tests/test_extract.py#L1462) — A data-shaped .json (eval fixture / dataset) must NOT emit per-key nodes.
- `test_extract_json_dependencies_become_imports()` — [`L1418`](../../../../../raw/code/graphify/tests/test_extract.py#L1418)
- `test_extract_json_extends_resolved()` — [`L1427`](../../../../../raw/code/graphify/tests/test_extract.py#L1427)
- `test_extract_json_handles_invalid_json(tmp_path)` — [`L1443`](../../../../../raw/code/graphify/tests/test_extract.py#L1443)
- `test_extract_json_large_file_skipped(tmp_path)` — [`L1434`](../../../../../raw/code/graphify/tests/test_extract.py#L1434)
- `test_extract_json_nested_contains()` — [`L1410`](../../../../../raw/code/graphify/tests/test_extract.py#L1410)
- `test_extract_json_no_self_loops()` — [`L1452`](../../../../../raw/code/graphify/tests/test_extract.py#L1452)
- `test_extract_json_top_level_array_skipped(tmp_path)` — [`L1476`](../../../../../raw/code/graphify/tests/test_extract.py#L1476) — A JSON file whose root is an array is data, never a config/manifest.
- `test_extract_json_top_level_keys()` — [`L1400`](../../../../../raw/code/graphify/tests/test_extract.py#L1400)
- `test_extract_json_via_dispatch()` — [`L1510`](../../../../../raw/code/graphify/tests/test_extract.py#L1510)
- `test_extract_keeps_stub_when_multiple_real_definitions_match(tmp_path)` — [`L274`](../../../../../raw/code/graphify/tests/test_extract.py#L274)
- `test_extract_merges_multiple_files()` — [`L55`](../../../../../raw/code/graphify/tests/test_extract.py#L55)
- `test_extract_parallel_returns_false_on_broken_pool(tmp_path, monkeypatch, capsys)` — [`L1096`](../../../../../raw/code/graphify/tests/test_extract.py#L1096) — _extract_parallel must catch BrokenProcessPool internally and return False.
- `test_extract_python_finds_class()` — [`L26`](../../../../../raw/code/graphify/tests/test_extract.py#L26)
- `test_extract_python_finds_methods()` — [`L32`](../../../../../raw/code/graphify/tests/test_extract.py#L32)
- `test_extract_python_no_dangling_edges()` — [`L38`](../../../../../raw/code/graphify/tests/test_extract.py#L38) — All edge sources must reference a known node (targets may be external imports).
- `test_extract_rewires_unique_inheritance_stub_to_real_definition(tmp_path)` — [`L246`](../../../../../raw/code/graphify/tests/test_extract.py#L246)
- `test_extract_ts_class_arrow_field(tmp_path)` — [`L817`](../../../../../raw/code/graphify/tests/test_extract.py#L817) — A class field initialised with an arrow function (`x = () => {}`) must be
- `test_extract_tsx_finds_helpers_and_component()` — [`L1023`](../../../../../raw/code/graphify/tests/test_extract.py#L1023) — Functions defined alongside a JSX-returning component must be captured.
- `test_extract_tsx_jsx_expression_calls_resolve()` — [`L1033`](../../../../../raw/code/graphify/tests/test_extract.py#L1033) — Calls inside JSX expressions like `{fmtDate(now)}` must yield call edges.
- `test_extract_tsx_uses_tsx_grammar()` — [`L1055`](../../../../../raw/code/graphify/tests/test_extract.py#L1055) — Wiring check: the .tsx config must use tree-sitter's `language_tsx`.
- `test_extract_updates_raw_call_callers_after_duplicate_id_disambiguation(tmp_path)` — [`L226`](../../../../../raw/code/graphify/tests/test_extract.py#L226)
- `test_go_cross_file_type_refs_resolve_to_single_node(tmp_path)` — [`L126`](../../../../../raw/code/graphify/tests/test_extract.py#L126) — #1402 (Go): the sourceless-stub fix landed in six extractors but the Go copy
- `test_go_imported_type_stubs_do_not_collide_across_source_files(tmp_path)` — [`L204`](../../../../../raw/code/graphify/tests/test_extract.py#L204) — #1462 (dedicated extractors): the imported-type-stub disambiguation (the
- `test_imported_type_stubs_do_not_collide_across_source_files(tmp_path)` — [`L155`](../../../../../raw/code/graphify/tests/test_extract.py#L155) — #1462: imported stdlib/type stubs with the same label are distinct uses
- `test_make_id_consistent()` — [`L15`](../../../../../raw/code/graphify/tests/test_extract.py#L15) — Same input always produces same output.
- `test_make_id_no_leading_trailing_underscores()` — [`L20`](../../../../../raw/code/graphify/tests/test_extract.py#L20)
- `test_make_id_strips_dots_and_underscores()` — [`L10`](../../../../../raw/code/graphify/tests/test_extract.py#L10)
- `test_method_calls_module_function()` — [`L547`](../../../../../raw/code/graphify/tests/test_extract.py#L547) — Analyzer.process() calls run_analysis() - cross class→function calls edge.
- `test_no_dangling_edges_on_extract()` — [`L484`](../../../../../raw/code/graphify/tests/test_extract.py#L484) — After merging multiple files, no internal edges should be dangling.
- `test_non_colliding_path_id_is_not_salted(tmp_path)` — [`L1684`](../../../../../raw/code/graphify/tests/test_extract.py#L1684) — The collision hash must touch only actual colliders — a path with no collision
- `test_origin_file_is_not_serialized_into_extract_output(tmp_path)` — [`L174`](../../../../../raw/code/graphify/tests/test_extract.py#L174) — origin_file is an internal disambiguation hint (#1462) consumed only by the
- `test_pure_export_no_from_not_treated_as_reexport()` — [`L1610`](../../../../../raw/code/graphify/tests/test_extract.py#L1610) — export { localVar } without 'from' should NOT create re_exports edges.
- `test_python_call_edges_have_call_context()` — [`L512`](../../../../../raw/code/graphify/tests/test_extract.py#L512)
- `test_python_instance_member_call_not_overconnected(tmp_path)` — [`L967`](../../../../../raw/code/graphify/tests/test_extract.py#L967) — A lowercase-receiver member call (`obj.run()`, `self.run()`) must NOT be
- `test_python_qualified_call_ambiguous_class_bails(tmp_path)` — [`L993`](../../../../../raw/code/graphify/tests/test_extract.py#L993) — When the class name is defined in 2+ files, the qualified call must not
- `test_python_qualified_call_resolves_when_method_name_collides_with_caller(tmp_path)` — [`L935`](../../../../../raw/code/graphify/tests/test_extract.py#L935) — The real #1446 shape: a viewset action `approve()` delegates to a SERVICE
- `test_python_qualified_class_method_call_resolves_extracted(tmp_path)` — [`L905`](../../../../../raw/code/graphify/tests/test_extract.py#L905) — `ClassName.method()` across files resolves to the class-qualified method
- `test_run_analysis_calls_compute_score()` — [`L526`](../../../../../raw/code/graphify/tests/test_extract.py#L526) — run_analysis() calls compute_score() - must appear as a calls edge.
- `test_run_analysis_calls_normalize()` — [`L537`](../../../../../raw/code/graphify/tests/test_extract.py#L537)
- `test_semantic_reference_edges_carry_context_and_source()` — [`L1587`](../../../../../raw/code/graphify/tests/test_extract.py#L1587)
- `test_separator_collision_paths_get_distinct_ids(tmp_path)` — [`L1664`](../../../../../raw/code/graphify/tests/test_extract.py#L1664) — #1522: two distinct paths whose only difference is a separator-vs-punctuation
- `test_structural_edges_are_extracted()` — [`L46`](../../../../../raw/code/graphify/tests/test_extract.py#L46) — contains / method / inherits / imports edges must always be EXTRACTED.
- `wrapped_sequential(*args, **kwargs)` — [`L1083`](../../../../../raw/code/graphify/tests/test_extract.py#L1083)

## Module values
- `FIXTURES` — [`L7`](../../../../../raw/code/graphify/tests/test_extract.py#L7)

