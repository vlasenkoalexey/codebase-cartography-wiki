---
title: 'Module: tests/test_csharp_type_resolution.py'
type: catalog
provenance: extracted
module: tests/test_csharp_type_resolution.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_csharp_type_resolution`/
symbols:
  _write: _write().
  _targets: _targets().
  test_csharp_cross_namespace_enum_reference_resolves_to_real_def: test_csharp_cross_namespace_enum_reference_resolves_to_real_def().
  test_csharp_cross_namespace_struct_and_record_references_resolve: test_csharp_cross_namespace_struct_and_record_references_resolve().
  test_csharp_global_scope_id_unchanged: test_csharp_global_scope_id_unchanged().
  test_csharp_declaration_nodes_carry_enclosing_namespace: test_csharp_declaration_nodes_carry_enclosing_namespace().
  test_csharp_cross_file_inherits_resolves_to_real_def: test_csharp_cross_file_inherits_resolves_to_real_def().
  test_csharp_collision_disambiguated_by_using: test_csharp_collision_disambiguated_by_using().
  test_csharp_global_using_and_global_namespace: test_csharp_global_using_and_global_namespace().
  test_csharp_ambiguous_using_does_not_resolve: test_csharp_ambiguous_using_does_not_resolve().
  test_csharp_using_alias_resolves_to_aliased_type: test_csharp_using_alias_resolves_to_aliased_type().
  test_csharp_cross_namespace_ref_not_misbound: test_csharp_cross_namespace_ref_not_misbound().
  test_csharp_same_file_cross_namespace_ref_not_misbound: test_csharp_same_file_cross_namespace_ref_not_misbound().
  test_csharp_qualified_ref_unknown_qualifier_dangles: test_csharp_qualified_ref_unknown_qualifier_dangles().
  test_csharp_nested_type_not_importable_via_using: test_csharp_nested_type_not_importable_via_using().
  test_csharp_generic_alias_resolves_to_base_type: test_csharp_generic_alias_resolves_to_base_type().
  test_csharp_type_ref_never_targets_a_file_label: test_csharp_type_ref_never_targets_a_file_label().
  test_csharp_alias_matching_file_stem_resolves_via_token: test_csharp_alias_matching_file_stem_resolves_via_token().
  test_csharp_two_namespaces_each_resolve_own_type: test_csharp_two_namespaces_each_resolve_own_type().
  test_csharp_file_level_using_applies_across_blocks: test_csharp_file_level_using_applies_across_blocks().
  test_csharp_using_flows_into_nested_block: test_csharp_using_flows_into_nested_block().
  _defs: _defs().
  test_csharp_namespace_nodes_canonical_and_discriminated: test_csharp_namespace_nodes_canonical_and_discriminated().
  test_csharp_import_edges_carry_using_kind: test_csharp_import_edges_carry_using_kind().
  test_csharp_import_edges_resolve_internal_namespace_and_alias: test_csharp_import_edges_resolve_internal_namespace_and_alias().
  test_csharp_qualified_base_ref_is_flagged: test_csharp_qualified_base_ref_is_flagged().
  test_csharp_one_file_same_name_no_collision_flag: test_csharp_one_file_same_name_no_collision_flag().
  test_csharp_type_parameter_emits_no_reference: test_csharp_type_parameter_emits_no_reference().
  test_csharp_nested_type_carries_metadata: test_csharp_nested_type_carries_metadata().
  test_csharp_inherits_does_not_bind_namespace_node: test_csharp_inherits_does_not_bind_namespace_node().
  test_csharp_qualified_ref_known_namespace_resolves: test_csharp_qualified_ref_known_namespace_resolves().
  test_csharp_qualified_generic_resolves_to_real_def: test_csharp_qualified_generic_resolves_to_real_def().
  test_csharp_qualified_alias_namespace_resolves: test_csharp_qualified_alias_namespace_resolves().
  test_csharp_qualified_out_of_scope_alias_falls_through_to_namespace: test_csharp_qualified_out_of_scope_alias_falls_through_to_namespace().
  test_csharp_qualified_in_scope_alias_shadows_namespace: test_csharp_qualified_in_scope_alias_shadows_namespace().
  test_csharp_one_file_same_name_binds_own_namespace: test_csharp_one_file_same_name_binds_own_namespace().
  test_csharp_type_ref_edges_carry_ref_token: test_csharp_type_ref_edges_carry_ref_token().
  test_csharp_same_name_diff_namespace_have_distinct_ids: test_csharp_same_name_diff_namespace_have_distinct_ids().
  test_csharp_namespaced_id_carries_namespace_segment: test_csharp_namespaced_id_carries_namespace_segment().
  test_csharp_namespace_scoped_using_isolated_to_sibling_block: test_csharp_namespace_scoped_using_isolated_to_sibling_block().
  test_csharp_alias_using_scoped_to_its_block: test_csharp_alias_using_scoped_to_its_block().
  test_csharp_two_namespaces_each_resolve_own_type._n: test_csharp_two_namespaces_each_resolve_own_type()._n().
  _node_by_id: _node_by_id().
---
# Module: [`tests/test_csharp_type_resolution.py`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py)

## Functions
- `_defs(result: dict, label: str)` — [`L29`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L29)
- `_n(label, ns)` — [`L516`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L516)
- `_node_by_id(result: dict, nid: str)` — [`L14`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L14)
- `_targets(result: dict, relation: str, label: str)` — [`L18`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L18)
- `_write(path: Path, text: str)` — [`L8`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L8)
- `test_csharp_alias_matching_file_stem_resolves_via_token(tmp_path: Path)` — [`L471`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L471)
- `test_csharp_alias_using_scoped_to_its_block(tmp_path: Path)` — [`L557`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L557)
- `test_csharp_ambiguous_using_does_not_resolve(tmp_path: Path)` — [`L144`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L144)
- `test_csharp_collision_disambiguated_by_using(tmp_path: Path)` — [`L70`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L70)
- `test_csharp_cross_file_inherits_resolves_to_real_def(tmp_path: Path)` — [`L57`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L57)
- `test_csharp_cross_namespace_enum_reference_resolves_to_real_def(tmp_path: Path)` — [`L101`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L101)
- `test_csharp_cross_namespace_ref_not_misbound(tmp_path: Path)` — [`L314`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L314)
- `test_csharp_cross_namespace_struct_and_record_references_resolve(tmp_path: Path)` — [`L122`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L122)
- `test_csharp_declaration_nodes_carry_enclosing_namespace(tmp_path: Path)` — [`L36`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L36)
- `test_csharp_file_level_using_applies_across_blocks(tmp_path: Path)` — [`L526`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L526)
- `test_csharp_generic_alias_resolves_to_base_type(tmp_path: Path)` — [`L437`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L437)
- `test_csharp_global_scope_id_unchanged(tmp_path: Path)` — [`L489`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L489)
- `test_csharp_global_using_and_global_namespace(tmp_path: Path)` — [`L89`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L89)
- `test_csharp_import_edges_carry_using_kind(tmp_path: Path)` — [`L211`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L211)
- `test_csharp_import_edges_resolve_internal_namespace_and_alias(tmp_path: Path)` — [`L229`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L229)
- `test_csharp_inherits_does_not_bind_namespace_node(tmp_path: Path)` — [`L330`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L330)
- `test_csharp_namespace_nodes_canonical_and_discriminated(tmp_path: Path)` — [`L196`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L196)
- `test_csharp_namespace_scoped_using_isolated_to_sibling_block(tmp_path: Path)` — [`L534`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L534)
- `test_csharp_namespaced_id_carries_namespace_segment(tmp_path: Path)` — [`L502`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L502)
- `test_csharp_nested_type_carries_metadata(tmp_path: Path)` — [`L307`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L307)
- `test_csharp_nested_type_not_importable_via_using(tmp_path: Path)` — [`L428`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L428)
- `test_csharp_one_file_same_name_binds_own_namespace(tmp_path: Path)` — [`L411`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L411)
- `test_csharp_one_file_same_name_no_collision_flag(tmp_path: Path)` — [`L284`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L284)
- `test_csharp_qualified_alias_namespace_resolves(tmp_path: Path)` — [`L369`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L369)
- `test_csharp_qualified_base_ref_is_flagged(tmp_path: Path)` — [`L277`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L277)
- `test_csharp_qualified_generic_resolves_to_real_def(tmp_path: Path)` — [`L357`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L357)
- `test_csharp_qualified_in_scope_alias_shadows_namespace(tmp_path: Path)` — [`L393`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L393)
- `test_csharp_qualified_out_of_scope_alias_falls_through_to_namespace(tmp_path: Path)` — [`L380`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L380)
- `test_csharp_qualified_ref_known_namespace_resolves(tmp_path: Path)` — [`L347`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L347)
- `test_csharp_qualified_ref_unknown_qualifier_dangles(tmp_path: Path)` — [`L339`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L339)
- `test_csharp_same_file_cross_namespace_ref_not_misbound(tmp_path: Path)` — [`L322`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L322)
- `test_csharp_same_name_diff_namespace_have_distinct_ids(tmp_path: Path)` — [`L481`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L481)
- `test_csharp_two_namespaces_each_resolve_own_type(tmp_path: Path)` — [`L509`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L509)
- `test_csharp_type_parameter_emits_no_reference(tmp_path: Path)` — [`L294`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L294)
- `test_csharp_type_ref_edges_carry_ref_token(tmp_path: Path)` — [`L457`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L457)
- `test_csharp_type_ref_never_targets_a_file_label(tmp_path: Path)` — [`L445`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L445)
- `test_csharp_using_alias_resolves_to_aliased_type(tmp_path: Path)` — [`L174`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L174)
- `test_csharp_using_flows_into_nested_block(tmp_path: Path)` — [`L549`](../../../../../raw/code/graphify/tests/test_csharp_type_resolution.py#L549)

