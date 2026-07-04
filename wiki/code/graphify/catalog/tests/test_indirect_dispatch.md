---
title: 'Module: tests/test_indirect_dispatch.py'
type: catalog
provenance: extracted
module: tests/test_indirect_dispatch.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_indirect_dispatch`/
symbols:
  _rels: _rels().
  _extract: _extract().
  _extract_js_dir: _extract_js_dir().
  test_affected_includes_indirect_callers: test_affected_includes_indirect_callers().
  test_param_shadow_emits_no_indirect_call: test_param_shadow_emits_no_indirect_call().
  test_local_assignment_shadow_emits_no_indirect_call: test_local_assignment_shadow_emits_no_indirect_call().
  test_data_var_matching_function_name_emits_no_indirect_call: test_data_var_matching_function_name_emits_no_indirect_call().
  test_genuine_module_function_still_emits_indirect_call: test_genuine_module_function_still_emits_indirect_call().
  test_cross_file_affected_includes_importing_dispatcher: test_cross_file_affected_includes_importing_dispatcher().
  _build: _build().
  _extract_dir: _extract_dir().
  test_emits_indirect_call_edges_and_keeps_calls_precise: test_emits_indirect_call_edges_and_keeps_calls_precise().
  test_cross_file_indirect_survives_id_relativization: test_cross_file_indirect_survives_id_relativization().
  test_cross_file_imported_callback_emits_indirect_call: test_cross_file_imported_callback_emits_indirect_call().
  test_cross_file_param_shadow_emits_no_indirect_call: test_cross_file_param_shadow_emits_no_indirect_call().
  test_module_level_dict_registry_emits_indirect_call: test_module_level_dict_registry_emits_indirect_call().
  test_module_level_list_registry_emits_indirect_call: test_module_level_list_registry_emits_indirect_call().
  test_function_scoped_dispatch_table_attributes_to_function: test_function_scoped_dispatch_table_attributes_to_function().
  test_dict_keys_are_not_dispatch_targets: test_dict_keys_are_not_dispatch_targets().
  test_non_callable_collection_value_emits_no_indirect_call: test_non_callable_collection_value_emits_no_indirect_call().
  test_module_level_reassigned_name_shadows_dispatch_value: test_module_level_reassigned_name_shadows_dispatch_value().
  test_cross_file_dict_registry_emits_indirect_call: test_cross_file_dict_registry_emits_indirect_call().
  test_js_function_scoped_call_argument: test_js_function_scoped_call_argument().
  test_js_module_object_and_array_registry: test_js_module_object_and_array_registry().
  test_js_module_level_callback_registration: test_js_module_level_callback_registration().
  test_js_inline_arrow_argument_is_not_a_reference: test_js_inline_arrow_argument_is_not_a_reference().
  test_js_parameter_shadow_emits_no_indirect_call: test_js_parameter_shadow_emits_no_indirect_call().
  test_js_object_keys_and_data_values_excluded: test_js_object_keys_and_data_values_excluded().
  test_js_shorthand_property_reference: test_js_shorthand_property_reference().
  test_js_cross_file_imported_callback_in_object: test_js_cross_file_imported_callback_in_object().
  test_typescript_typed_params_and_arrow_consts: test_typescript_typed_params_and_arrow_consts().
  SRC: SRC.
  PARAM_SHADOW: PARAM_SHADOW.
  LOCAL_SHADOW: LOCAL_SHADOW.
  DATA_VAR: DATA_VAR.
  REAL_PASS: REAL_PASS.
---
# Module: [`tests/test_indirect_dispatch.py`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py)

## Functions
- `_build(tmp_path)` — [`L45`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L45)
- `_extract(tmp_path, src)` — [`L94`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L94)
- `_extract_dir(tmp_path, files: dict[str, str])` — [`L186`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L186)
- `_extract_js_dir(tmp_path, files: dict[str, str])` — [`L385`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L385)
- `_rels(r, relation)` — [`L52`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L52)
- `test_affected_includes_indirect_callers(tmp_path)` — [`L77`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L77)
- `test_cross_file_affected_includes_importing_dispatcher(tmp_path)` — [`L251`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L251)
- `test_cross_file_dict_registry_emits_indirect_call(tmp_path)` — [`L366`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L366)
- `test_cross_file_imported_callback_emits_indirect_call(tmp_path)` — [`L231`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L231)
- `test_cross_file_indirect_survives_id_relativization(tmp_path)` — [`L204`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L204) — Regression: when the scan root relativizes node ids (cache_root == project
- `test_cross_file_param_shadow_emits_no_indirect_call(tmp_path)` — [`L271`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L271) — Soundness carries across files: an imported name shadowed by a parameter
- `test_data_var_matching_function_name_emits_no_indirect_call(tmp_path)` — [`L156`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L156)
- `test_dict_keys_are_not_dispatch_targets(tmp_path)` — [`L326`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L326) — Only VALUES are references; a function used as a dict KEY is not invoked
- `test_emits_indirect_call_edges_and_keeps_calls_precise(tmp_path)` — [`L56`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L56)
- `test_function_scoped_dispatch_table_attributes_to_function(tmp_path)` — [`L318`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L318)
- `test_genuine_module_function_still_emits_indirect_call(tmp_path)` — [`L173`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L173) — No recall regression: a real module fn passed by name still emits an edge.
- `test_js_cross_file_imported_callback_in_object(tmp_path)` — [`L481`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L481)
- `test_js_function_scoped_call_argument(tmp_path)` — [`L403`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L403)
- `test_js_inline_arrow_argument_is_not_a_reference(tmp_path)` — [`L442`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L442) — An inline arrow / function expression is a direct definition, not a
- `test_js_module_level_callback_registration(tmp_path)` — [`L427`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L427) — Express routes / event wiring / timers live at module scope in JS.
- `test_js_module_object_and_array_registry(tmp_path)` — [`L413`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L413)
- `test_js_object_keys_and_data_values_excluded(tmp_path)` — [`L460`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L460)
- `test_js_parameter_shadow_emits_no_indirect_call(tmp_path)` — [`L451`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L451)
- `test_js_shorthand_property_reference(tmp_path)` — [`L472`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L472)
- `test_local_assignment_shadow_emits_no_indirect_call(tmp_path)` — [`L134`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L134)
- `test_module_level_dict_registry_emits_indirect_call(tmp_path)` — [`L291`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L291)
- `test_module_level_list_registry_emits_indirect_call(tmp_path)` — [`L306`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L306)
- `test_module_level_reassigned_name_shadows_dispatch_value(tmp_path)` — [`L354`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L354) — If the name is rebound to data at module scope, the table value is that
- `test_non_callable_collection_value_emits_no_indirect_call(tmp_path)` — [`L340`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L340) — A data value in the table (a number, a string) is not a callable and must
- `test_param_shadow_emits_no_indirect_call(tmp_path)` — [`L111`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L111)
- `test_typescript_typed_params_and_arrow_consts(tmp_path)` — [`L495`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L495)

## Module values
- `DATA_VAR` — [`L141`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L141)
- `LOCAL_SHADOW` — [`L119`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L119)
- `PARAM_SHADOW` — [`L101`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L101)
- `REAL_PASS` — [`L163`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L163)
- `SRC` — [`L20`](../../../../../raw/code/graphify/tests/test_indirect_dispatch.py#L20)

