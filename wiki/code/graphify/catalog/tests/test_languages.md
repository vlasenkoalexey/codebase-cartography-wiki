---
title: 'Module: tests/test_languages.py'
type: catalog
provenance: extracted
module: tests/test_languages.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_languages`/
symbols:
  FIXTURES: FIXTURES.
  _edge_labels: _edge_labels().
  _labels: _labels().
  _relations: _relations().
  _edges_with_relation: _edges_with_relation().
  _corpus: _corpus().
  _needs_dm: _needs_dm.
  _nodes_with_label: _nodes_with_label().
  test_dm_finds_global_proc: test_dm_finds_global_proc().
  test_dm_finds_type_definition: test_dm_finds_type_definition().
  test_dm_qualifies_proc_with_type_path: test_dm_qualifies_proc_with_type_path().
  test_dm_finds_path_form_proc_definition: test_dm_finds_path_form_proc_definition().
  test_dm_emits_include_edge: test_dm_emits_include_edge().
  test_dm_unresolved_include_flagged_external: test_dm_unresolved_include_flagged_external().
  test_dm_resolves_in_file_calls: test_dm_resolves_in_file_calls().
  test_dm_ambiguous_member_call_left_unresolved: test_dm_ambiguous_member_call_left_unresolved().
  test_dm_call_edges_have_call_context: test_dm_call_edges_have_call_context().
  test_dm_super_call_not_emitted: test_dm_super_call_not_emitted().
  test_apex_soql_uses_edge: test_apex_soql_uses_edge().
  test_apex_trigger_uses_sobject: test_apex_trigger_uses_sobject().
  test_systemverilog_preserves_existing_module_extraction: test_systemverilog_preserves_existing_module_extraction().
  test_java_finds_class: test_java_finds_class().
  test_java_finds_interface: test_java_finds_interface().
  test_java_finds_methods: test_java_finds_methods().
  test_java_finds_imports: test_java_finds_imports().
  test_java_import_edges_have_import_context: test_java_import_edges_have_import_context().
  test_c_finds_functions: test_c_finds_functions().
  test_c_finds_includes: test_c_finds_includes().
  test_c_import_edges_have_import_context: test_c_import_edges_have_import_context().
  test_c_parameter_and_return_type_contexts: test_c_parameter_and_return_type_contexts().
  test_c_call_edges_have_call_context: test_c_call_edges_have_call_context().
  test_cpp_finds_class: test_cpp_finds_class().
  test_cpp_finds_methods: test_cpp_finds_methods().
  test_cpp_finds_includes: test_cpp_finds_includes().
  test_cpp_import_edges_have_import_context: test_cpp_import_edges_have_import_context().
  test_cpp_method_parameter_and_return_type_contexts: test_cpp_method_parameter_and_return_type_contexts().
  test_cpp_field_and_template_argument_contexts: test_cpp_field_and_template_argument_contexts().
  test_cpp_generic_parents_include_type_argument_references: test_cpp_generic_parents_include_type_argument_references().
  test_cuda_finds_kernel_and_device_functions: test_cuda_finds_kernel_and_device_functions().
  test_cuda_finds_struct: test_cuda_finds_struct().
  test_cuda_finds_includes: test_cuda_finds_includes().
  test_cuda_host_call_edges: test_cuda_host_call_edges().
  test_metal_finds_kernel_function_and_struct: test_metal_finds_kernel_function_and_struct().
  test_ruby_finds_class: test_ruby_finds_class().
  test_ruby_finds_methods: test_ruby_finds_methods().
  test_ruby_finds_function: test_ruby_finds_function().
  test_csharp_finds_class: test_csharp_finds_class().
  test_csharp_finds_interface: test_csharp_finds_interface().
  test_csharp_finds_methods: test_csharp_finds_methods().
  test_csharp_finds_usings: test_csharp_finds_usings().
  test_csharp_splits_inherits_and_implements_edges: test_csharp_splits_inherits_and_implements_edges().
  test_csharp_parameter_return_and_generic_contexts: test_csharp_parameter_return_and_generic_contexts().
  test_java_normalizes_inherits_and_implements: test_java_normalizes_inherits_and_implements().
  test_java_type_parameters_do_not_emit_references: test_java_type_parameters_do_not_emit_references().
  test_java_parameter_return_generic_and_attribute_contexts: test_java_parameter_return_generic_and_attribute_contexts().
  test_csharp_field_type_references_have_field_context: test_csharp_field_type_references_have_field_context().
  test_csharp_property_type_references_have_field_context: test_csharp_property_type_references_have_field_context().
  test_kotlin_finds_class: test_kotlin_finds_class().
  test_kotlin_finds_data_class: test_kotlin_finds_data_class().
  test_kotlin_finds_methods: test_kotlin_finds_methods().
  test_kotlin_finds_function: test_kotlin_finds_function().
  test_kotlin_emits_in_file_calls: test_kotlin_emits_in_file_calls().
  test_kotlin_splits_inherits_and_implements: test_kotlin_splits_inherits_and_implements().
  test_kotlin_interface_delegation_emits_implements: test_kotlin_interface_delegation_emits_implements().
  test_kotlin_parameter_return_generic_and_field_contexts: test_kotlin_parameter_return_generic_and_field_contexts().
  test_scala_finds_class: test_scala_finds_class().
  test_scala_finds_object: test_scala_finds_object().
  test_scala_finds_methods: test_scala_finds_methods().
  test_scala_import_edges_have_import_context: test_scala_import_edges_have_import_context().
  test_scala_splits_inherits_and_mixes_in: test_scala_splits_inherits_and_mixes_in().
  test_scala_constructor_parameter_field_context: test_scala_constructor_parameter_field_context().
  test_scala_val_definition_field_context: test_scala_val_definition_field_context().
  test_scala_var_definition_field_context: test_scala_var_definition_field_context().
  test_scala_method_return_type_context: test_scala_method_return_type_context().
  test_scala_call_edges_have_call_context: test_scala_call_edges_have_call_context().
  test_php_finds_class: test_php_finds_class().
  test_php_finds_methods: test_php_finds_methods().
  test_php_finds_function: test_php_finds_function().
  test_php_finds_imports: test_php_finds_imports().
  test_php_import_edges_have_import_context: test_php_import_edges_have_import_context().
  test_php_call_edges_have_call_context: test_php_call_edges_have_call_context().
  test_php_finds_static_property_access: test_php_finds_static_property_access().
  test_php_finds_config_helper_call: test_php_finds_config_helper_call().
  test_php_finds_container_bind: test_php_finds_container_bind().
  test_php_finds_event_listeners: test_php_finds_event_listeners().
  test_php_splits_inherits_implements_mixes_in: test_php_splits_inherits_implements_mixes_in().
  test_php_property_parameter_and_return_contexts: test_php_property_parameter_and_return_contexts().
  test_php_constructor_property_promotion_contexts: test_php_constructor_property_promotion_contexts().
  test_swift_finds_class: test_swift_finds_class().
  test_swift_finds_protocol: test_swift_finds_protocol().
  test_swift_finds_struct: test_swift_finds_struct().
  test_swift_finds_methods: test_swift_finds_methods().
  test_swift_finds_function: test_swift_finds_function().
  test_swift_finds_imports: test_swift_finds_imports().
  test_swift_import_edges_have_import_context: test_swift_import_edges_have_import_context().
  test_swift_imports_survive_build: test_swift_imports_survive_build().
  test_swift_finds_actor: test_swift_finds_actor().
  test_swift_finds_enum: test_swift_finds_enum().
  test_swift_finds_enum_methods: test_swift_finds_enum_methods().
  test_swift_finds_enum_cases: test_swift_finds_enum_cases().
  test_swift_enum_associated_value_type_emits_references: test_swift_enum_associated_value_type_emits_references().
  test_swift_finds_deinit: test_swift_finds_deinit().
  test_swift_finds_subscript: test_swift_finds_subscript().
  test_swift_protocol_conformance_emits_implements: test_swift_protocol_conformance_emits_implements().
  test_swift_extension_conformance_emits_implements: test_swift_extension_conformance_emits_implements().
  test_swift_splits_inherits_and_implements: test_swift_splits_inherits_and_implements().
  test_swift_parameter_return_generic_and_field_contexts: test_swift_parameter_return_generic_and_field_contexts().
  test_swift_emits_calls: test_swift_emits_calls().
  test_swift_call_edges_have_call_context: test_swift_call_edges_have_call_context().
  test_elixir_import_edges_have_import_context: test_elixir_import_edges_have_import_context().
  test_elixir_call_edges_have_call_context: test_elixir_call_edges_have_call_context().
  test_objc_import_edges_have_import_context: test_objc_import_edges_have_import_context().
  test_objc_splits_inherits_and_implements: test_objc_splits_inherits_and_implements().
  test_objc_protocol_adopts_protocol: test_objc_protocol_adopts_protocol().
  test_objc_property_type_context: test_objc_property_type_context().
  test_objc_header_dispatch_routes_objc_not_c: test_objc_header_dispatch_routes_objc_not_c().
  test_julia_import_edges_have_import_context: test_julia_import_edges_have_import_context().
  test_julia_abstract_concrete_hierarchy_inherits: test_julia_abstract_concrete_hierarchy_inherits().
  test_julia_struct_field_type_context: test_julia_struct_field_type_context().
  test_julia_call_edges_have_call_context: test_julia_call_edges_have_call_context().
  test_fortran_parameter_and_return_type_contexts: test_fortran_parameter_and_return_type_contexts().
  test_powershell_class_base_type_emits_inherits_edge: test_powershell_class_base_type_emits_inherits_edge().
  test_powershell_property_field_type_context: test_powershell_property_field_type_context().
  test_powershell_method_parameter_and_return_type_contexts: test_powershell_method_parameter_and_return_type_contexts().
  test_js_module_level_arrow_produces_node_and_call_edges: test_js_module_level_arrow_produces_node_and_call_edges().
  test_markdown_finds_headings: test_markdown_finds_headings().
  test_markdown_finds_nested_heading: test_markdown_finds_nested_heading().
  test_markdown_skips_fenced_code_blocks: test_markdown_skips_fenced_code_blocks().
  test_markdown_contains_edges: test_markdown_contains_edges().
  test_groovy_finds_class: test_groovy_finds_class().
  test_groovy_finds_methods: test_groovy_finds_methods().
  test_groovy_finds_imports: test_groovy_finds_imports().
  test_groovy_import_edges_have_import_context: test_groovy_import_edges_have_import_context().
  test_groovy_spock_finds_class: test_groovy_spock_finds_class().
  test_groovy_spock_finds_feature_methods: test_groovy_spock_finds_feature_methods().
  test_groovy_spock_finds_method_with_apostrophe: test_groovy_spock_finds_method_with_apostrophe().
  test_groovy_spock_preserves_import_edges: test_groovy_spock_preserves_import_edges().
  test_dm_no_error: test_dm_no_error().
  test_dm_emits_new_as_instantiates: test_dm_emits_new_as_instantiates().
  test_dm_no_dangling_edges: test_dm_no_dangling_edges().
  test_dmi_emits_state_nodes: test_dmi_emits_state_nodes().
  test_dmf_extracts_windows: test_dmf_extracts_windows().
  test_dmf_elem_labels_carry_control_type: test_dmf_elem_labels_carry_control_type().
  test_sln_finds_projects: test_sln_finds_projects().
  test_sln_contains_edges: test_sln_contains_edges().
  test_sln_project_dependency_edges: test_sln_project_dependency_edges().
  test_csproj_finds_packages: test_csproj_finds_packages().
  test_csproj_finds_project_references: test_csproj_finds_project_references().
  test_csproj_finds_target_framework: test_csproj_finds_target_framework().
  test_csproj_finds_sdk: test_csproj_finds_sdk().
  test_xaml_finds_class_and_event_references: test_xaml_finds_class_and_event_references().
  test_razor_finds_using_directives: test_razor_finds_using_directives().
  test_razor_finds_component_references: test_razor_finds_component_references().
  test_razor_finds_inherits: test_razor_finds_inherits().
  test_razor_finds_code_block_methods: test_razor_finds_code_block_methods().
  test_apex_class_extraction: test_apex_class_extraction().
  test_apex_enum_extraction: test_apex_enum_extraction().
  test_apex_interface_extraction: test_apex_interface_extraction().
  test_apex_method_extraction: test_apex_method_extraction().
  test_apex_contains_and_method_relations: test_apex_contains_and_method_relations().
  test_apex_file_node_present: test_apex_file_node_present().
  test_apex_trigger_extraction: test_apex_trigger_extraction().
  test_systemverilog_splits_inherits_and_implements: test_systemverilog_splits_inherits_and_implements().
  test_systemverilog_field_parameter_return_and_generic_contexts: test_systemverilog_field_parameter_return_and_generic_contexts().
  test_systemverilog_qualified_field_references: test_systemverilog_qualified_field_references().
  test_systemverilog_does_not_emit_type_parameter_refs: test_systemverilog_does_not_emit_type_parameter_refs().
  test_cpp_header_routes_to_cpp_extractor: test_cpp_header_routes_to_cpp_extractor().
  test_plain_c_header_stays_on_c_extractor: test_plain_c_header_stays_on_c_extractor().
  test_objc_header_with_import_routes_to_objc: test_objc_header_with_import_routes_to_objc().
  test_swift_extension_folds_onto_objc_class: test_swift_extension_folds_onto_objc_class().
  _calls: _calls().
  test_java_no_error: test_java_no_error().
  test_java_no_dangling_edges: test_java_no_dangling_edges().
  test_c_no_error: test_c_no_error().
  test_c_emits_calls: test_c_emits_calls().
  test_c_calls_are_extracted: test_c_calls_are_extracted().
  test_cpp_no_error: test_cpp_no_error().
  test_cpp_class_inherits_edge: test_cpp_class_inherits_edge().
  test_cpp_struct_inherits_edge: test_cpp_struct_inherits_edge().
  test_cuda_no_error: test_cuda_no_error().
  test_metal_no_error: test_metal_no_error().
  test_ruby_no_error: test_ruby_no_error().
  test_ruby_inherits_edge: test_ruby_inherits_edge().
  test_csharp_no_error: test_csharp_no_error().
  test_csharp_inherits_edge: test_csharp_inherits_edge().
  test_csharp_implements_iprocessor: test_csharp_implements_iprocessor().
  test_java_generic_parents_include_type_argument_references: test_java_generic_parents_include_type_argument_references().
  test_java_field_type_references_have_field_context: test_java_field_type_references_have_field_context().
  test_java_record_component_type_references: test_java_record_component_type_references().
  test_java_record_components_skip_type_parameters: test_java_record_components_skip_type_parameters().
  test_java_type_annotations_have_attribute_context: test_java_type_annotations_have_attribute_context().
  test_java_enum_and_annotation_declarations_are_type_nodes: test_java_enum_and_annotation_declarations_are_type_nodes().
  test_csharp_call_edges_have_call_context: test_csharp_call_edges_have_call_context().
  test_csharp_import_edges_have_import_context: test_csharp_import_edges_have_import_context().
  test_kotlin_no_error: test_kotlin_no_error().
  test_scala_no_error: test_scala_no_error().
  test_php_no_error: test_php_no_error().
  test_php_static_prop_target_is_holding_class: test_php_static_prop_target_is_holding_class().
  test_php_config_helper_target_matches_first_segment: test_php_config_helper_target_matches_first_segment().
  test_php_container_bind_links_contract_to_implementation: test_php_container_bind_links_contract_to_implementation().
  test_php_event_listener_links_event_to_listener: test_php_event_listener_links_event_to_listener().
  test_swift_no_error: test_swift_no_error().
  test_swift_no_dangling_edges: test_swift_no_dangling_edges().
  test_swift_enum_cases_have_case_of_edge: test_swift_enum_cases_have_case_of_edge().
  test_swift_extension_methods_attach_to_type: test_swift_extension_methods_attach_to_type().
  test_swift_extension_does_not_duplicate_type_node: test_swift_extension_does_not_duplicate_type_node().
  test_swift_extension_across_files_merges_into_canonical_type: test_swift_extension_across_files_merges_into_canonical_type().
  test_elixir_finds_module: test_elixir_finds_module().
  test_elixir_finds_functions: test_elixir_finds_functions().
  test_elixir_finds_imports: test_elixir_finds_imports().
  test_elixir_multi_alias_expands: test_elixir_multi_alias_expands().
  test_elixir_finds_calls: test_elixir_finds_calls().
  test_elixir_method_edges: test_elixir_method_edges().
  test_objc_finds_interface: test_objc_finds_interface().
  test_objc_finds_subclass: test_objc_finds_subclass().
  test_objc_finds_methods: test_objc_finds_methods().
  test_objc_finds_imports: test_objc_finds_imports().
  test_objc_inherits_edge: test_objc_inherits_edge().
  test_objc_no_dangling_edges: test_objc_no_dangling_edges().
  test_objc_resolves_self_method_calls: test_objc_resolves_self_method_calls().
  test_objc_generic_property_type_extracted: test_objc_generic_property_type_extracted().
  test_objc_module_import_edge: test_objc_module_import_edge().
  test_objc_ns_assume_nonnull_macro_does_not_break_parsing: test_objc_ns_assume_nonnull_macro_does_not_break_parsing().
  test_objc_macro_free_header_unchanged: test_objc_macro_free_header_unchanged().
  test_objc_alloc_init_emits_type_reference: test_objc_alloc_init_emits_type_reference().
  test_go_receiver_methods_share_type_node: test_go_receiver_methods_share_type_node().
  test_go_receiver_uses_pkg_scope: test_go_receiver_uses_pkg_scope().
  test_julia_finds_module: test_julia_finds_module().
  test_julia_finds_structs: test_julia_finds_structs().
  test_julia_finds_abstract_type: test_julia_finds_abstract_type().
  test_julia_finds_functions: test_julia_finds_functions().
  test_julia_finds_short_function: test_julia_finds_short_function().
  test_julia_finds_imports: test_julia_finds_imports().
  test_julia_qualified_and_relative_imports: test_julia_qualified_and_relative_imports().
  test_julia_finds_inherits: test_julia_finds_inherits().
  test_julia_finds_calls: test_julia_finds_calls().
  test_julia_no_dangling_edges: test_julia_no_dangling_edges().
  test_fortran_finds_module: test_fortran_finds_module().
  test_fortran_finds_subroutines: test_fortran_finds_subroutines().
  test_fortran_finds_function: test_fortran_finds_function().
  test_fortran_finds_program: test_fortran_finds_program().
  test_fortran_finds_use_imports: test_fortran_finds_use_imports().
  test_fortran_use_edges_have_use_context: test_fortran_use_edges_have_use_context().
  test_fortran_finds_calls: test_fortran_finds_calls().
  test_fortran_finds_function_call: test_fortran_finds_function_call().
  test_fortran_case_insensitive_names: test_fortran_case_insensitive_names().
  test_fortran_finds_derived_type: test_fortran_finds_derived_type().
  test_fortran_no_dangling_edges: test_fortran_no_dangling_edges().
  test_fortran_capital_F_parses_preprocessed: test_fortran_capital_F_parses_preprocessed().
  test_powershell_no_error: test_powershell_no_error().
  test_powershell_psm1_dispatched_and_extracted: test_powershell_psm1_dispatched_and_extracted().
  test_powershell_finds_class_and_method: test_powershell_finds_class_and_method().
  test_powershell_import_module_emits_edge: test_powershell_import_module_emits_edge().
  test_powershell_import_module_with_name_param: test_powershell_import_module_with_name_param().
  test_powershell_dot_source_forward_slash_emits_edge: test_powershell_dot_source_forward_slash_emits_edge().
  test_powershell_dot_source_backslash_emits_edge: test_powershell_dot_source_backslash_emits_edge().
  test_powershell_import_module_inside_function_emits_edge: test_powershell_import_module_inside_function_emits_edge().
  test_powershell_import_module_not_a_raw_call: test_powershell_import_module_not_a_raw_call().
  test_powershell_dot_source_inside_function_emits_edge: test_powershell_dot_source_inside_function_emits_edge().
  test_powershell_psd1_dispatched: test_powershell_psd1_dispatched().
  test_powershell_psd1_no_error: test_powershell_psd1_no_error().
  test_powershell_psd1_has_file_node: test_powershell_psd1_has_file_node().
  test_powershell_psd1_root_module: test_powershell_psd1_root_module().
  test_powershell_psd1_nested_modules: test_powershell_psd1_nested_modules().
  test_powershell_psd1_required_modules_string: test_powershell_psd1_required_modules_string().
  test_powershell_psd1_required_modules_hashtable: test_powershell_psd1_required_modules_hashtable().
  test_powershell_psd1_no_moduleversion_as_edge: test_powershell_psd1_no_moduleversion_as_edge().
  test_powershell_psd1_no_dangling_edges: test_powershell_psd1_no_dangling_edges().
  test_ts_dynamic_import_no_error: test_ts_dynamic_import_no_error().
  test_ts_dynamic_import_extracts_edges: test_ts_dynamic_import_extracts_edges().
  test_ts_dynamic_import_confidence: test_ts_dynamic_import_confidence().
  test_ts_dynamic_import_source_is_function: test_ts_dynamic_import_source_is_function().
  test_ts_no_dynamic_import_in_sync_fn: test_ts_no_dynamic_import_in_sync_fn().
  test_ts_dynamic_template_literal_skipped: test_ts_dynamic_template_literal_skipped().
  test_ts_static_template_literal_resolved: test_ts_static_template_literal_resolved().
  test_js_local_const_does_not_emit_phantom_node: test_js_local_const_does_not_emit_phantom_node().
  test_ts_local_const_does_not_emit_phantom_node: test_ts_local_const_does_not_emit_phantom_node().
  test_ts_injected_field_ambiguous_type_emits_no_edge: test_ts_injected_field_ambiguous_type_emits_no_edge().
  test_markdown_no_error: test_markdown_no_error().
  test_markdown_fenced_heading_not_parsed: test_markdown_fenced_heading_not_parsed().
  test_markdown_no_dangling_edges: test_markdown_no_dangling_edges().
  test_markdown_link_edges_emitted: test_markdown_link_edges_emitted().
  test_markdown_link_skips_external_and_images: test_markdown_link_skips_external_and_images().
  test_markdown_link_edges_resolve_to_real_nodes: test_markdown_link_edges_resolve_to_real_nodes().
  test_groovy_no_error: test_groovy_no_error().
  test_groovy_no_dangling_edges: test_groovy_no_dangling_edges().
  test_groovy_extends_edge: test_groovy_extends_edge().
  test_groovy_implements_edge: test_groovy_implements_edge().
  test_groovy_spock_no_dangling_edges: test_groovy_spock_no_dangling_edges().
  test_dmi_no_error: test_dmi_no_error().
  test_dmi_state_contained_by_file: test_dmi_state_contained_by_file().
  test_dmm_no_error: test_dmm_no_error().
  test_dmm_extracts_type_paths_as_uses_edges: test_dmm_extracts_type_paths_as_uses_edges().
  test_dmm_strips_var_overrides: test_dmm_strips_var_overrides().
  test_dmm_handles_multiline_tile_definition: test_dmm_handles_multiline_tile_definition().
  test_dmm_skips_grid_section: test_dmm_skips_grid_section().
  test_dmf_no_error: test_dmf_no_error().
  test_dmf_elem_under_window: test_dmf_elem_under_window().
  test_dmf_no_dangling_edges: test_dmf_no_dangling_edges().
  test_sln_no_error: test_sln_no_error().
  test_csproj_no_error: test_csproj_no_error().
  test_razor_no_error: test_razor_no_error().
  test_razor_no_dangling_edges: test_razor_no_dangling_edges().
  test_apex_interface_extends: test_apex_interface_extends().
  test_apex_dml_uses_edge: test_apex_dml_uses_edge().
  test_apex_no_dangling_edges: test_apex_no_dangling_edges().
  test_systemverilog_no_error: test_systemverilog_no_error().
  test_systemverilog_no_dangling_edges: test_systemverilog_no_dangling_edges().
  test_cpp_paired_single_class_node: test_cpp_paired_single_class_node().
  test_cpp_paired_method_decl_and_def_are_one_node: test_cpp_paired_method_decl_and_def_are_one_node().
  test_cpp_paired_includes_resolve_to_real_header: test_cpp_paired_includes_resolve_to_real_header().
  test_cpp_paired_no_dangling_edges: test_cpp_paired_no_dangling_edges().
  test_objc_paired_single_class_methods_not_duplicated: test_objc_paired_single_class_methods_not_duplicated().
  test_objc_bridging_header_not_isolated: test_objc_bridging_header_not_isolated().
  test_objc_paired_no_dangling_edges: test_objc_paired_no_dangling_edges().
  test_decldef_merge_does_not_merge_across_directories: test_decldef_merge_does_not_merge_across_directories().
  test_decldef_merge_does_not_merge_same_name_same_dir_distinct_files: test_decldef_merge_does_not_merge_same_name_same_dir_distinct_files().
  _md_link_fixture: _md_link_fixture().
  _assert_no_dangling: _assert_no_dangling().
  _node_by_label: _node_by_label().
  test_metal_is_code_extension: test_metal_is_code_extension().
  test_objc_class_method_labeled_with_plus: test_objc_class_method_labeled_with_plus().
  test_objc_compound_selector_call_resolves: test_objc_compound_selector_call_resolves().
  test_objc_quoted_import_edges_resolve_to_real_nodes: test_objc_quoted_import_edges_resolve_to_real_nodes().
  test_objc_alloc_init_unknown_class_no_resolved_edge: test_objc_alloc_init_unknown_class_no_resolved_edge().
  test_objc_dot_syntax_property_accesses_edge: test_objc_dot_syntax_property_accesses_edge().
  test_objc_dot_syntax_no_fanout_two_same_named_properties: test_objc_dot_syntax_no_fanout_two_same_named_properties().
  test_objc_dot_syntax_unresolvable_property_zero_edges: test_objc_dot_syntax_unresolvable_property_zero_edges().
  test_objc_selector_expression_calls_edge: test_objc_selector_expression_calls_edge().
  test_objc_selector_no_fanout_two_same_named_methods: test_objc_selector_no_fanout_two_same_named_methods().
  test_objc_dot_syntax_substring_sibling_exact_match: test_objc_dot_syntax_substring_sibling_exact_match().
  test_objc_selector_substring_method_exact_match: test_objc_selector_substring_method_exact_match().
  test_ts_constructor_injection_calls_edge: test_ts_constructor_injection_calls_edge().
  test_ts_this_field_receiver_not_same_file_collision: test_ts_this_field_receiver_not_same_file_collision().
  test_ts_injected_field_resolves_to_typed_class_not_same_named_collision: test_ts_injected_field_resolves_to_typed_class_not_same_named_collision().
  test_apex_missing_file_returns_empty: test_apex_missing_file_returns_empty().
  test_systemverilog_missing_file_returns_empty: test_systemverilog_missing_file_returns_empty().
  _references: _references().
  _normalize_symbol_label: _normalize_symbol_label().
  _ts_label_calls: _ts_label_calls().
---
# Module: [`tests/test_languages.py`](../../../../../raw/code/graphify/tests/test_languages.py)

## Functions
- `_assert_no_dangling(r)` — [`L2788`](../../../../../raw/code/graphify/tests/test_languages.py#L2788)
- `_calls(r)` — [`L33`](../../../../../raw/code/graphify/tests/test_languages.py#L33)
- `_corpus(*relpaths)` — [`L2775`](../../../../../raw/code/graphify/tests/test_languages.py#L2775) — Run the full extract() pipeline on fixture files (absolute, resolved
- `_edge_labels(result: dict, relation: str, context: str | None = None)` — [`L68`](../../../../../raw/code/graphify/tests/test_languages.py#L68)
- `_edges_with_relation(r, *relations)` — [`L53`](../../../../../raw/code/graphify/tests/test_languages.py#L53)
- `_labels(r)` — [`L27`](../../../../../raw/code/graphify/tests/test_languages.py#L27)
- `_md_link_fixture(tmp_path)` — [`L2209`](../../../../../raw/code/graphify/tests/test_languages.py#L2209) — A hub doc linking to sibling docs, plus those docs (#1376).
- `_node_by_label(result: dict, label: str)` — [`L61`](../../../../../raw/code/graphify/tests/test_languages.py#L61)
- `_nodes_with_label(r, label)` — [`L2784`](../../../../../raw/code/graphify/tests/test_languages.py#L2784)
- `_normalize_symbol_label(label: str)` — [`L57`](../../../../../raw/code/graphify/tests/test_languages.py#L57)
- `_references(r)` — [`L41`](../../../../../raw/code/graphify/tests/test_languages.py#L41)
- `_relations(r)` — [`L30`](../../../../../raw/code/graphify/tests/test_languages.py#L30)
- `_ts_label_calls(r, src_sub)` — [`L2050`](../../../../../raw/code/graphify/tests/test_languages.py#L2050)
- `test_apex_class_extraction()` — [`L2622`](../../../../../raw/code/graphify/tests/test_languages.py#L2622)
- `test_apex_contains_and_method_relations()` — [`L2655`](../../../../../raw/code/graphify/tests/test_languages.py#L2655)
- `test_apex_dml_uses_edge()` — [`L2668`](../../../../../raw/code/graphify/tests/test_languages.py#L2668)
- `test_apex_enum_extraction()` — [`L2627`](../../../../../raw/code/graphify/tests/test_languages.py#L2627)
- `test_apex_file_node_present()` — [`L2673`](../../../../../raw/code/graphify/tests/test_languages.py#L2673)
- `test_apex_interface_extends(tmp_path)` — [`L2637`](../../../../../raw/code/graphify/tests/test_languages.py#L2637)
- `test_apex_interface_extraction()` — [`L2632`](../../../../../raw/code/graphify/tests/test_languages.py#L2632)
- `test_apex_method_extraction()` — [`L2647`](../../../../../raw/code/graphify/tests/test_languages.py#L2647)
- `test_apex_missing_file_returns_empty()` — [`L2691`](../../../../../raw/code/graphify/tests/test_languages.py#L2691)
- `test_apex_no_dangling_edges()` — [`L2696`](../../../../../raw/code/graphify/tests/test_languages.py#L2696)
- `test_apex_soql_uses_edge()` — [`L2661`](../../../../../raw/code/graphify/tests/test_languages.py#L2661)
- `test_apex_trigger_extraction()` — [`L2678`](../../../../../raw/code/graphify/tests/test_languages.py#L2678)
- `test_apex_trigger_uses_sobject()` — [`L2684`](../../../../../raw/code/graphify/tests/test_languages.py#L2684)
- `test_c_call_edges_have_call_context()` — [`L158`](../../../../../raw/code/graphify/tests/test_languages.py#L158)
- `test_c_calls_are_extracted()` — [`L138`](../../../../../raw/code/graphify/tests/test_languages.py#L138)
- `test_c_emits_calls()` — [`L134`](../../../../../raw/code/graphify/tests/test_languages.py#L134)
- `test_c_finds_functions()` — [`L124`](../../../../../raw/code/graphify/tests/test_languages.py#L124)
- `test_c_finds_includes()` — [`L130`](../../../../../raw/code/graphify/tests/test_languages.py#L130)
- `test_c_import_edges_have_import_context()` — [`L145`](../../../../../raw/code/graphify/tests/test_languages.py#L145)
- `test_c_no_error()` — [`L120`](../../../../../raw/code/graphify/tests/test_languages.py#L120)
- `test_c_parameter_and_return_type_contexts()` — [`L152`](../../../../../raw/code/graphify/tests/test_languages.py#L152)
- `test_cpp_class_inherits_edge()` — [`L206`](../../../../../raw/code/graphify/tests/test_languages.py#L206) — Regression for #915: `class Derived : public Base {}` should emit an inherits edge.
- `test_cpp_field_and_template_argument_contexts()` — [`L199`](../../../../../raw/code/graphify/tests/test_languages.py#L199)
- `test_cpp_finds_class()` — [`L171`](../../../../../raw/code/graphify/tests/test_languages.py#L171)
- `test_cpp_finds_includes()` — [`L181`](../../../../../raw/code/graphify/tests/test_languages.py#L181)
- `test_cpp_finds_methods()` — [`L175`](../../../../../raw/code/graphify/tests/test_languages.py#L175)
- `test_cpp_generic_parents_include_type_argument_references()` — [`L230`](../../../../../raw/code/graphify/tests/test_languages.py#L230) — `class PooledClient : public Connection<HttpClient>` must emit the inherits
- `test_cpp_header_routes_to_cpp_extractor()` — [`L2797`](../../../../../raw/code/graphify/tests/test_languages.py#L2797) — A `.h` with a C++ class must route to extract_cpp, not extract_c (which has
- `test_cpp_import_edges_have_import_context()` — [`L186`](../../../../../raw/code/graphify/tests/test_languages.py#L186)
- `test_cpp_method_parameter_and_return_type_contexts()` — [`L193`](../../../../../raw/code/graphify/tests/test_languages.py#L193)
- `test_cpp_no_error()` — [`L167`](../../../../../raw/code/graphify/tests/test_languages.py#L167)
- `test_cpp_paired_includes_resolve_to_real_header()` — [`L2838`](../../../../../raw/code/graphify/tests/test_languages.py#L2838) — Foo.cpp and Main.cpp `#include "Foo.h"` must resolve to the real Foo.h file
- `test_cpp_paired_method_decl_and_def_are_one_node()` — [`L2822`](../../../../../raw/code/graphify/tests/test_languages.py#L2822) — `void bar();` in Foo.h and `void Foo::bar() {}` in Foo.cpp must collapse to
- `test_cpp_paired_no_dangling_edges()` — [`L2851`](../../../../../raw/code/graphify/tests/test_languages.py#L2851)
- `test_cpp_paired_single_class_node()` — [`L2812`](../../../../../raw/code/graphify/tests/test_languages.py#L2812) — Foo.h (class) + Foo.cpp (Foo::bar def) + Main.cpp must yield exactly ONE
- `test_cpp_struct_inherits_edge()` — [`L218`](../../../../../raw/code/graphify/tests/test_languages.py#L218) — Structs use the same `: Base` syntax as classes and must also emit inherits.
- `test_csharp_call_edges_have_call_context()` — [`L565`](../../../../../raw/code/graphify/tests/test_languages.py#L565)
- `test_csharp_field_type_references_have_field_context()` — [`L545`](../../../../../raw/code/graphify/tests/test_languages.py#L545)
- `test_csharp_finds_class()` — [`L333`](../../../../../raw/code/graphify/tests/test_languages.py#L333)
- `test_csharp_finds_interface()` — [`L337`](../../../../../raw/code/graphify/tests/test_languages.py#L337)
- `test_csharp_finds_methods()` — [`L341`](../../../../../raw/code/graphify/tests/test_languages.py#L341)
- `test_csharp_finds_usings()` — [`L346`](../../../../../raw/code/graphify/tests/test_languages.py#L346)
- `test_csharp_implements_iprocessor()` — [`L355`](../../../../../raw/code/graphify/tests/test_languages.py#L355)
- `test_csharp_import_edges_have_import_context()` — [`L576`](../../../../../raw/code/graphify/tests/test_languages.py#L576)
- `test_csharp_inherits_edge()` — [`L350`](../../../../../raw/code/graphify/tests/test_languages.py#L350)
- `test_csharp_no_error()` — [`L329`](../../../../../raw/code/graphify/tests/test_languages.py#L329)
- `test_csharp_parameter_return_and_generic_contexts()` — [`L372`](../../../../../raw/code/graphify/tests/test_languages.py#L372)
- `test_csharp_property_type_references_have_field_context()` — [`L554`](../../../../../raw/code/graphify/tests/test_languages.py#L554)
- `test_csharp_splits_inherits_and_implements_edges()` — [`L366`](../../../../../raw/code/graphify/tests/test_languages.py#L366)
- `test_csproj_finds_packages()` — [`L2566`](../../../../../raw/code/graphify/tests/test_languages.py#L2566)
- `test_csproj_finds_project_references()` — [`L2572`](../../../../../raw/code/graphify/tests/test_languages.py#L2572)
- `test_csproj_finds_sdk()` — [`L2581`](../../../../../raw/code/graphify/tests/test_languages.py#L2581)
- `test_csproj_finds_target_framework()` — [`L2577`](../../../../../raw/code/graphify/tests/test_languages.py#L2577)
- `test_csproj_no_error()` — [`L2562`](../../../../../raw/code/graphify/tests/test_languages.py#L2562)
- `test_cuda_finds_includes()` — [`L258`](../../../../../raw/code/graphify/tests/test_languages.py#L258)
- `test_cuda_finds_kernel_and_device_functions()` — [`L248`](../../../../../raw/code/graphify/tests/test_languages.py#L248)
- `test_cuda_finds_struct()` — [`L254`](../../../../../raw/code/graphify/tests/test_languages.py#L254)
- `test_cuda_host_call_edges()` — [`L262`](../../../../../raw/code/graphify/tests/test_languages.py#L262)
- `test_cuda_no_error()` — [`L244`](../../../../../raw/code/graphify/tests/test_languages.py#L244)
- `test_decldef_merge_does_not_merge_across_directories()` — [`L2911`](../../../../../raw/code/graphify/tests/test_languages.py#L2911) — Two unrelated `class Logger` in DIFFERENT directories (each its own .h/.cpp)
- `test_decldef_merge_does_not_merge_same_name_same_dir_distinct_files()` — [`L2923`](../../../../../raw/code/graphify/tests/test_languages.py#L2923) — Two same-named `class Dup` in the SAME dir but different base stems
- `test_dm_ambiguous_member_call_left_unresolved()` — [`L2423`](../../../../../raw/code/graphify/tests/test_languages.py#L2423)
- `test_dm_call_edges_have_call_context()` — [`L2440`](../../../../../raw/code/graphify/tests/test_languages.py#L2440)
- `test_dm_emits_include_edge()` — [`L2401`](../../../../../raw/code/graphify/tests/test_languages.py#L2401)
- `test_dm_emits_new_as_instantiates()` — [`L2432`](../../../../../raw/code/graphify/tests/test_languages.py#L2432)
- `test_dm_finds_global_proc()` — [`L2375`](../../../../../raw/code/graphify/tests/test_languages.py#L2375)
- `test_dm_finds_path_form_proc_definition()` — [`L2396`](../../../../../raw/code/graphify/tests/test_languages.py#L2396)
- `test_dm_finds_type_definition()` — [`L2382`](../../../../../raw/code/graphify/tests/test_languages.py#L2382)
- `test_dm_no_dangling_edges()` — [`L2447`](../../../../../raw/code/graphify/tests/test_languages.py#L2447)
- `test_dm_no_error()` — [`L2370`](../../../../../raw/code/graphify/tests/test_languages.py#L2370)
- `test_dm_qualifies_proc_with_type_path()` — [`L2389`](../../../../../raw/code/graphify/tests/test_languages.py#L2389)
- `test_dm_resolves_in_file_calls()` — [`L2416`](../../../../../raw/code/graphify/tests/test_languages.py#L2416)
- `test_dm_super_call_not_emitted()` — [`L2454`](../../../../../raw/code/graphify/tests/test_languages.py#L2454)
- `test_dm_unresolved_include_flagged_external()` — [`L2408`](../../../../../raw/code/graphify/tests/test_languages.py#L2408)
- `test_dmf_elem_labels_carry_control_type()` — [`L2522`](../../../../../raw/code/graphify/tests/test_languages.py#L2522)
- `test_dmf_elem_under_window()` — [`L2527`](../../../../../raw/code/graphify/tests/test_languages.py#L2527)
- `test_dmf_extracts_windows()` — [`L2516`](../../../../../raw/code/graphify/tests/test_languages.py#L2516)
- `test_dmf_no_dangling_edges()` — [`L2534`](../../../../../raw/code/graphify/tests/test_languages.py#L2534)
- `test_dmf_no_error()` — [`L2512`](../../../../../raw/code/graphify/tests/test_languages.py#L2512)
- `test_dmi_emits_state_nodes()` — [`L2467`](../../../../../raw/code/graphify/tests/test_languages.py#L2467)
- `test_dmi_no_error()` — [`L2463`](../../../../../raw/code/graphify/tests/test_languages.py#L2463)
- `test_dmi_state_contained_by_file()` — [`L2472`](../../../../../raw/code/graphify/tests/test_languages.py#L2472)
- `test_dmm_extracts_type_paths_as_uses_edges()` — [`L2486`](../../../../../raw/code/graphify/tests/test_languages.py#L2486)
- `test_dmm_handles_multiline_tile_definition()` — [`L2499`](../../../../../raw/code/graphify/tests/test_languages.py#L2499)
- `test_dmm_no_error()` — [`L2482`](../../../../../raw/code/graphify/tests/test_languages.py#L2482)
- `test_dmm_skips_grid_section()` — [`L2504`](../../../../../raw/code/graphify/tests/test_languages.py#L2504)
- `test_dmm_strips_var_overrides()` — [`L2493`](../../../../../raw/code/graphify/tests/test_languages.py#L2493)
- `test_elixir_call_edges_have_call_context()` — [`L1048`](../../../../../raw/code/graphify/tests/test_languages.py#L1048)
- `test_elixir_finds_calls()` — [`L1041`](../../../../../raw/code/graphify/tests/test_languages.py#L1041)
- `test_elixir_finds_functions()` — [`L1005`](../../../../../raw/code/graphify/tests/test_languages.py#L1005)
- `test_elixir_finds_imports()` — [`L1012`](../../../../../raw/code/graphify/tests/test_languages.py#L1012)
- `test_elixir_finds_module()` — [`L999`](../../../../../raw/code/graphify/tests/test_languages.py#L999)
- `test_elixir_import_edges_have_import_context()` — [`L1018`](../../../../../raw/code/graphify/tests/test_languages.py#L1018)
- `test_elixir_method_edges()` — [`L1054`](../../../../../raw/code/graphify/tests/test_languages.py#L1054)
- `test_elixir_multi_alias_expands()` — [`L1025`](../../../../../raw/code/graphify/tests/test_languages.py#L1025) — `alias Foo.{Bar, Baz}` must emit one imports edge per expanded module.
- `test_fortran_capital_F_parses_preprocessed()` — [`L1649`](../../../../../raw/code/graphify/tests/test_languages.py#L1649)
- `test_fortran_case_insensitive_names()` — [`L1622`](../../../../../raw/code/graphify/tests/test_languages.py#L1622)
- `test_fortran_finds_calls()` — [`L1598`](../../../../../raw/code/graphify/tests/test_languages.py#L1598)
- `test_fortran_finds_derived_type()` — [`L1630`](../../../../../raw/code/graphify/tests/test_languages.py#L1630)
- `test_fortran_finds_function()` — [`L1574`](../../../../../raw/code/graphify/tests/test_languages.py#L1574)
- `test_fortran_finds_function_call()` — [`L1604`](../../../../../raw/code/graphify/tests/test_languages.py#L1604) — `y = f(x)` function invocations must emit a calls edge.
- `test_fortran_finds_module()` — [`L1560`](../../../../../raw/code/graphify/tests/test_languages.py#L1560)
- `test_fortran_finds_program()` — [`L1580`](../../../../../raw/code/graphify/tests/test_languages.py#L1580)
- `test_fortran_finds_subroutines()` — [`L1567`](../../../../../raw/code/graphify/tests/test_languages.py#L1567)
- `test_fortran_finds_use_imports()` — [`L1586`](../../../../../raw/code/graphify/tests/test_languages.py#L1586)
- `test_fortran_no_dangling_edges()` — [`L1642`](../../../../../raw/code/graphify/tests/test_languages.py#L1642)
- `test_fortran_parameter_and_return_type_contexts()` — [`L1636`](../../../../../raw/code/graphify/tests/test_languages.py#L1636)
- `test_fortran_use_edges_have_use_context()` — [`L1592`](../../../../../raw/code/graphify/tests/test_languages.py#L1592)
- `test_go_receiver_methods_share_type_node()` — [`L1440`](../../../../../raw/code/graphify/tests/test_languages.py#L1440) — Methods on the same receiver type must share one canonical type node.
- `test_go_receiver_uses_pkg_scope()` — [`L1447`](../../../../../raw/code/graphify/tests/test_languages.py#L1447) — Type node id should be scoped to directory, not file stem.
- `test_groovy_extends_edge()` — [`L2310`](../../../../../raw/code/graphify/tests/test_languages.py#L2310) — `class X extends Base` must emit an inherits edge.
- `test_groovy_finds_class()` — [`L2279`](../../../../../raw/code/graphify/tests/test_languages.py#L2279)
- `test_groovy_finds_imports()` — [`L2291`](../../../../../raw/code/graphify/tests/test_languages.py#L2291)
- `test_groovy_finds_methods()` — [`L2284`](../../../../../raw/code/graphify/tests/test_languages.py#L2284)
- `test_groovy_implements_edge()` — [`L2327`](../../../../../raw/code/graphify/tests/test_languages.py#L2327) — `class X implements Iface` must emit an implements edge.
- `test_groovy_import_edges_have_import_context()` — [`L2296`](../../../../../raw/code/graphify/tests/test_languages.py#L2296)
- `test_groovy_no_dangling_edges()` — [`L2303`](../../../../../raw/code/graphify/tests/test_languages.py#L2303)
- `test_groovy_no_error()` — [`L2274`](../../../../../raw/code/graphify/tests/test_languages.py#L2274)
- `test_groovy_spock_finds_class()` — [`L2339`](../../../../../raw/code/graphify/tests/test_languages.py#L2339)
- `test_groovy_spock_finds_feature_methods()` — [`L2344`](../../../../../raw/code/graphify/tests/test_languages.py#L2344)
- `test_groovy_spock_finds_method_with_apostrophe()` — [`L2350`](../../../../../raw/code/graphify/tests/test_languages.py#L2350)
- `test_groovy_spock_no_dangling_edges()` — [`L2360`](../../../../../raw/code/graphify/tests/test_languages.py#L2360)
- `test_groovy_spock_preserves_import_edges()` — [`L2355`](../../../../../raw/code/graphify/tests/test_languages.py#L2355)
- `test_java_enum_and_annotation_declarations_are_type_nodes(tmp_path)` — [`L515`](../../../../../raw/code/graphify/tests/test_languages.py#L515)
- `test_java_field_type_references_have_field_context(tmp_path)` — [`L443`](../../../../../raw/code/graphify/tests/test_languages.py#L443)
- `test_java_finds_class()` — [`L86`](../../../../../raw/code/graphify/tests/test_languages.py#L86)
- `test_java_finds_imports()` — [`L100`](../../../../../raw/code/graphify/tests/test_languages.py#L100)
- `test_java_finds_interface()` — [`L90`](../../../../../raw/code/graphify/tests/test_languages.py#L90)
- `test_java_finds_methods()` — [`L94`](../../../../../raw/code/graphify/tests/test_languages.py#L94)
- `test_java_generic_parents_include_type_argument_references(tmp_path)` — [`L385`](../../../../../raw/code/graphify/tests/test_languages.py#L385)
- `test_java_import_edges_have_import_context()` — [`L105`](../../../../../raw/code/graphify/tests/test_languages.py#L105)
- `test_java_no_dangling_edges()` — [`L111`](../../../../../raw/code/graphify/tests/test_languages.py#L111)
- `test_java_no_error()` — [`L82`](../../../../../raw/code/graphify/tests/test_languages.py#L82)
- `test_java_normalizes_inherits_and_implements()` — [`L379`](../../../../../raw/code/graphify/tests/test_languages.py#L379)
- `test_java_parameter_return_generic_and_attribute_contexts()` — [`L435`](../../../../../raw/code/graphify/tests/test_languages.py#L435)
- `test_java_record_component_type_references(tmp_path)` — [`L462`](../../../../../raw/code/graphify/tests/test_languages.py#L462)
- `test_java_record_components_skip_type_parameters(tmp_path)` — [`L480`](../../../../../raw/code/graphify/tests/test_languages.py#L480)
- `test_java_type_annotations_have_attribute_context(tmp_path)` — [`L500`](../../../../../raw/code/graphify/tests/test_languages.py#L500)
- `test_java_type_parameters_do_not_emit_references(tmp_path)` — [`L407`](../../../../../raw/code/graphify/tests/test_languages.py#L407)
- `test_js_local_const_does_not_emit_phantom_node(tmp_path)` — [`L1909`](../../../../../raw/code/graphify/tests/test_languages.py#L1909) — Local const/let/var inside an arrow callback must NOT emit a node (#1077).
- `test_js_module_level_arrow_produces_node_and_call_edges(tmp_path)` — [`L1939`](../../../../../raw/code/graphify/tests/test_languages.py#L1939) — Module-level arrow functions must still emit a node and capture their calls (#1077).
- `test_julia_abstract_concrete_hierarchy_inherits()` — [`L1525`](../../../../../raw/code/graphify/tests/test_languages.py#L1525)
- `test_julia_call_edges_have_call_context()` — [`L1544`](../../../../../raw/code/graphify/tests/test_languages.py#L1544)
- `test_julia_finds_abstract_type()` — [`L1473`](../../../../../raw/code/graphify/tests/test_languages.py#L1473)
- `test_julia_finds_calls()` — [`L1538`](../../../../../raw/code/graphify/tests/test_languages.py#L1538)
- `test_julia_finds_functions()` — [`L1479`](../../../../../raw/code/graphify/tests/test_languages.py#L1479)
- `test_julia_finds_imports()` — [`L1492`](../../../../../raw/code/graphify/tests/test_languages.py#L1492)
- `test_julia_finds_inherits()` — [`L1519`](../../../../../raw/code/graphify/tests/test_languages.py#L1519)
- `test_julia_finds_module()` — [`L1460`](../../../../../raw/code/graphify/tests/test_languages.py#L1460)
- `test_julia_finds_short_function()` — [`L1486`](../../../../../raw/code/graphify/tests/test_languages.py#L1486)
- `test_julia_finds_structs()` — [`L1466`](../../../../../raw/code/graphify/tests/test_languages.py#L1466)
- `test_julia_import_edges_have_import_context()` — [`L1498`](../../../../../raw/code/graphify/tests/test_languages.py#L1498)
- `test_julia_no_dangling_edges()` — [`L1551`](../../../../../raw/code/graphify/tests/test_languages.py#L1551)
- `test_julia_qualified_and_relative_imports()` — [`L1505`](../../../../../raw/code/graphify/tests/test_languages.py#L1505) — Qualified (`using Base.Threads`) and relative (`using ..Mod`) imports
- `test_julia_struct_field_type_context()` — [`L1531`](../../../../../raw/code/graphify/tests/test_languages.py#L1531)
- `test_kotlin_emits_in_file_calls()` — [`L607`](../../../../../raw/code/graphify/tests/test_languages.py#L607) — Regression test for the call-walker `simple_identifier` /
- `test_kotlin_finds_class()` — [`L589`](../../../../../raw/code/graphify/tests/test_languages.py#L589)
- `test_kotlin_finds_data_class()` — [`L593`](../../../../../raw/code/graphify/tests/test_languages.py#L593)
- `test_kotlin_finds_function()` — [`L603`](../../../../../raw/code/graphify/tests/test_languages.py#L603)
- `test_kotlin_finds_methods()` — [`L597`](../../../../../raw/code/graphify/tests/test_languages.py#L597)
- `test_kotlin_interface_delegation_emits_implements()` — [`L626`](../../../../../raw/code/graphify/tests/test_languages.py#L626) — `class Foo : Bar by baz` wraps the delegated interface in an
- `test_kotlin_no_error()` — [`L585`](../../../../../raw/code/graphify/tests/test_languages.py#L585)
- `test_kotlin_parameter_return_generic_and_field_contexts()` — [`L633`](../../../../../raw/code/graphify/tests/test_languages.py#L633)
- `test_kotlin_splits_inherits_and_implements()` — [`L620`](../../../../../raw/code/graphify/tests/test_languages.py#L620)
- `test_markdown_contains_edges()` — [`L2161`](../../../../../raw/code/graphify/tests/test_languages.py#L2161) — Headings should be connected via 'contains' edges (file->h, h->h).
- `test_markdown_fenced_heading_not_parsed()` — [`L2171`](../../../../../raw/code/graphify/tests/test_languages.py#L2171) — A '## heading' inside a fenced block must not produce a heading node (#1077).
- `test_markdown_finds_headings()` — [`L2134`](../../../../../raw/code/graphify/tests/test_languages.py#L2134)
- `test_markdown_finds_nested_heading()` — [`L2142`](../../../../../raw/code/graphify/tests/test_languages.py#L2142) — ### Database Migration is nested under ## Full Deploy.
- `test_markdown_link_edges_emitted(tmp_path)` — [`L2229`](../../../../../raw/code/graphify/tests/test_languages.py#L2229) — Inline/wikilink markdown links to sibling docs become references edges (#1376).
- `test_markdown_link_edges_resolve_to_real_nodes(tmp_path)` — [`L2253`](../../../../../raw/code/graphify/tests/test_languages.py#L2253) — End-to-end: after extract()'s ID remap, link targets are real doc nodes,
- `test_markdown_link_skips_external_and_images(tmp_path)` — [`L2243`](../../../../../raw/code/graphify/tests/test_languages.py#L2243) — External URLs, in-page anchors and images must not produce edges (#1376).
- `test_markdown_no_dangling_edges()` — [`L2202`](../../../../../raw/code/graphify/tests/test_languages.py#L2202)
- `test_markdown_no_error()` — [`L2130`](../../../../../raw/code/graphify/tests/test_languages.py#L2130)
- `test_markdown_skips_fenced_code_blocks()` — [`L2148`](../../../../../raw/code/graphify/tests/test_languages.py#L2148) — Fenced code blocks should NOT emit nodes (#1077).
- `test_metal_finds_kernel_function_and_struct()` — [`L282`](../../../../../raw/code/graphify/tests/test_languages.py#L282)
- `test_metal_is_code_extension()` — [`L272`](../../../../../raw/code/graphify/tests/test_languages.py#L272)
- `test_metal_no_error()` — [`L277`](../../../../../raw/code/graphify/tests/test_languages.py#L277)
- `test_objc_alloc_init_emits_type_reference(tmp_path)` — [`L1270`](../../../../../raw/code/graphify/tests/test_languages.py#L1270) — `[[Foo alloc] init]` must emit a `references` edge to the project class Foo (#1475).
- `test_objc_alloc_init_unknown_class_no_resolved_edge(tmp_path)` — [`L1286`](../../../../../raw/code/graphify/tests/test_languages.py#L1286) — `[[Unknown alloc] init]` with no such class must not produce a resolved
- `test_objc_bridging_header_not_isolated()` — [`L2878`](../../../../../raw/code/graphify/tests/test_languages.py#L2878) — A bridging header of only `#import "Widget.h"` must produce an imports edge
- `test_objc_class_method_labeled_with_plus(tmp_path)` — [`L1140`](../../../../../raw/code/graphify/tests/test_languages.py#L1140) — `+ (…)shared` is a class method and must be labeled +shared, not -shared (#1475).
- `test_objc_compound_selector_call_resolves(tmp_path)` — [`L1148`](../../../../../raw/code/graphify/tests/test_languages.py#L1148) — A compound message `[self a:x b:y]` resolves to the compound method def (#1475).
- `test_objc_dot_syntax_no_fanout_two_same_named_properties(tmp_path)` — [`L1323`](../../../../../raw/code/graphify/tests/test_languages.py#L1323) — Two classes each declaring -name: self.name in A must NOT fan out to B's -name.
- `test_objc_dot_syntax_property_accesses_edge(tmp_path)` — [`L1306`](../../../../../raw/code/graphify/tests/test_languages.py#L1306) — self.name dot-syntax resolves to an accesses edge within the same class.
- `test_objc_dot_syntax_substring_sibling_exact_match(tmp_path)` — [`L1396`](../../../../../raw/code/graphify/tests/test_languages.py#L1396) — A substring-colliding sibling must neither be falsely matched nor suppress
- `test_objc_dot_syntax_unresolvable_property_zero_edges(tmp_path)` — [`L1346`](../../../../../raw/code/graphify/tests/test_languages.py#L1346) — Accessing a property not defined in the current class produces zero accesses edges.
- `test_objc_finds_imports()` — [`L1082`](../../../../../raw/code/graphify/tests/test_languages.py#L1082)
- `test_objc_finds_interface()` — [`L1064`](../../../../../raw/code/graphify/tests/test_languages.py#L1064)
- `test_objc_finds_methods()` — [`L1076`](../../../../../raw/code/graphify/tests/test_languages.py#L1076)
- `test_objc_finds_subclass()` — [`L1070`](../../../../../raw/code/graphify/tests/test_languages.py#L1070)
- `test_objc_generic_property_type_extracted(tmp_path)` — [`L1163`](../../../../../raw/code/graphify/tests/test_languages.py#L1163) — `NSArray<Product *> *` must reference the element type Product (and the
- `test_objc_header_dispatch_routes_objc_not_c(tmp_path)` — [`L1182`](../../../../../raw/code/graphify/tests/test_languages.py#L1182) — An ObjC `.h` (has @interface) routes to extract_objc; a plain C `.h` stays
- `test_objc_header_with_import_routes_to_objc()` — [`L2858`](../../../../../raw/code/graphify/tests/test_languages.py#L2858) — A bridging header that is only `#import "X.h"` (no @interface) must route to
- `test_objc_import_edges_have_import_context()` — [`L1088`](../../../../../raw/code/graphify/tests/test_languages.py#L1088)
- `test_objc_inherits_edge()` — [`L1095`](../../../../../raw/code/graphify/tests/test_languages.py#L1095)
- `test_objc_macro_free_header_unchanged(tmp_path)` — [`L1216`](../../../../../raw/code/graphify/tests/test_languages.py#L1216) — A macro-free header still parses exactly as before (regression).
- `test_objc_module_import_edge(tmp_path)` — [`L1173`](../../../../../raw/code/graphify/tests/test_languages.py#L1173) — `@import Foundation;` / `@import UIKit.UIView;` produce imports edges (#1475).
- `test_objc_no_dangling_edges()` — [`L1123`](../../../../../raw/code/graphify/tests/test_languages.py#L1123)
- `test_objc_ns_assume_nonnull_macro_does_not_break_parsing(tmp_path)` — [`L1194`](../../../../../raw/code/graphify/tests/test_languages.py#L1194) — `NS_ASSUME_NONNULL_BEGIN` before `@interface` made tree-sitter-objc fail to
- `test_objc_paired_no_dangling_edges()` — [`L2889`](../../../../../raw/code/graphify/tests/test_languages.py#L2889)
- `test_objc_paired_single_class_methods_not_duplicated()` — [`L2866`](../../../../../raw/code/graphify/tests/test_languages.py#L2866) — Widget.h (@interface) + Widget.m (@implementation) -> ONE Widget class node
- `test_objc_property_type_context()` — [`L1118`](../../../../../raw/code/graphify/tests/test_languages.py#L1118)
- `test_objc_protocol_adopts_protocol()` — [`L1108`](../../../../../raw/code/graphify/tests/test_languages.py#L1108) — `@protocol Derived <Base>` must emit an implements edge Derived->Base.
- `test_objc_quoted_import_edges_resolve_to_real_nodes(tmp_path)` — [`L1230`](../../../../../raw/code/graphify/tests/test_languages.py#L1230) — Quoted `#import "X.h"` edges must target the real (disambiguated) file node id,
- `test_objc_resolves_self_method_calls()` — [`L1130`](../../../../../raw/code/graphify/tests/test_languages.py#L1130) — `[self speak]` inside Dog.fetch must produce a calls edge. The method-body
- `test_objc_selector_expression_calls_edge(tmp_path)` — [`L1359`](../../../../../raw/code/graphify/tests/test_languages.py#L1359) — @selector(uniqueMethod) with exactly one match produces a calls edge.
- `test_objc_selector_no_fanout_two_same_named_methods(tmp_path)` — [`L1376`](../../../../../raw/code/graphify/tests/test_languages.py#L1376) — @selector(doThing) with two doThing methods must emit zero calls edges.
- `test_objc_selector_substring_method_exact_match(tmp_path)` — [`L1416`](../../../../../raw/code/graphify/tests/test_languages.py#L1416) — @selector(doThing) must resolve to `-doThing` exactly, not be suppressed by
- `test_objc_splits_inherits_and_implements()` — [`L1101`](../../../../../raw/code/graphify/tests/test_languages.py#L1101)
- `test_php_call_edges_have_call_context()` — [`L734`](../../../../../raw/code/graphify/tests/test_languages.py#L734)
- `test_php_config_helper_target_matches_first_segment()` — [`L757`](../../../../../raw/code/graphify/tests/test_languages.py#L757)
- `test_php_constructor_property_promotion_contexts()` — [`L807`](../../../../../raw/code/graphify/tests/test_languages.py#L807)
- `test_php_container_bind_links_contract_to_implementation()` — [`L770`](../../../../../raw/code/graphify/tests/test_languages.py#L770)
- `test_php_event_listener_links_event_to_listener()` — [`L783`](../../../../../raw/code/graphify/tests/test_languages.py#L783)
- `test_php_finds_class()` — [`L708`](../../../../../raw/code/graphify/tests/test_languages.py#L708)
- `test_php_finds_config_helper_call()` — [`L753`](../../../../../raw/code/graphify/tests/test_languages.py#L753)
- `test_php_finds_container_bind()` — [`L766`](../../../../../raw/code/graphify/tests/test_languages.py#L766)
- `test_php_finds_event_listeners()` — [`L779`](../../../../../raw/code/graphify/tests/test_languages.py#L779)
- `test_php_finds_function()` — [`L718`](../../../../../raw/code/graphify/tests/test_languages.py#L718)
- `test_php_finds_imports()` — [`L722`](../../../../../raw/code/graphify/tests/test_languages.py#L722)
- `test_php_finds_methods()` — [`L712`](../../../../../raw/code/graphify/tests/test_languages.py#L712)
- `test_php_finds_static_property_access()` — [`L740`](../../../../../raw/code/graphify/tests/test_languages.py#L740)
- `test_php_import_edges_have_import_context()` — [`L727`](../../../../../raw/code/graphify/tests/test_languages.py#L727)
- `test_php_no_error()` — [`L704`](../../../../../raw/code/graphify/tests/test_languages.py#L704)
- `test_php_property_parameter_and_return_contexts()` — [`L800`](../../../../../raw/code/graphify/tests/test_languages.py#L800)
- `test_php_splits_inherits_implements_mixes_in()` — [`L793`](../../../../../raw/code/graphify/tests/test_languages.py#L793)
- `test_php_static_prop_target_is_holding_class()` — [`L744`](../../../../../raw/code/graphify/tests/test_languages.py#L744)
- `test_plain_c_header_stays_on_c_extractor()` — [`L2805`](../../../../../raw/code/graphify/tests/test_languages.py#L2805) — A plain C header (no C++ signal) must keep its extract_c routing.
- `test_powershell_class_base_type_emits_inherits_edge()` — [`L1685`](../../../../../raw/code/graphify/tests/test_languages.py#L1685)
- `test_powershell_dot_source_backslash_emits_edge()` — [`L1728`](../../../../../raw/code/graphify/tests/test_languages.py#L1728) — Dot-source `. .\Utils.ps1` (backslash path) emits an imports_from edge.
- `test_powershell_dot_source_forward_slash_emits_edge()` — [`L1721`](../../../../../raw/code/graphify/tests/test_languages.py#L1721) — Dot-source `. ./Shared.psm1` emits an imports_from edge.
- `test_powershell_dot_source_inside_function_emits_edge()` — [`L1756`](../../../../../raw/code/graphify/tests/test_languages.py#L1756) — Dot-source inside a function body still produces an imports_from edge.
- `test_powershell_finds_class_and_method()` — [`L1678`](../../../../../raw/code/graphify/tests/test_languages.py#L1678)
- `test_powershell_import_module_emits_edge()` — [`L1706`](../../../../../raw/code/graphify/tests/test_languages.py#L1706) — Import-Module Foo at top level emits an imports_from edge.
- `test_powershell_import_module_inside_function_emits_edge()` — [`L1735`](../../../../../raw/code/graphify/tests/test_languages.py#L1735) — Import-Module inside a function body still produces an imports_from edge.
- `test_powershell_import_module_not_a_raw_call()` — [`L1744`](../../../../../raw/code/graphify/tests/test_languages.py#L1744) — Import-Module must not appear in raw_calls (it is an import, not a function call).
- `test_powershell_import_module_with_name_param()` — [`L1714`](../../../../../raw/code/graphify/tests/test_languages.py#L1714) — Import-Module -Name Bar.psm1 resolves to module stem 'bar'.
- `test_powershell_method_parameter_and_return_type_contexts()` — [`L1697`](../../../../../raw/code/graphify/tests/test_languages.py#L1697)
- `test_powershell_no_error()` — [`L1659`](../../../../../raw/code/graphify/tests/test_languages.py#L1659)
- `test_powershell_property_field_type_context()` — [`L1692`](../../../../../raw/code/graphify/tests/test_languages.py#L1692)
- `test_powershell_psd1_dispatched()` — [`L1767`](../../../../../raw/code/graphify/tests/test_languages.py#L1767) — _get_extractor should route .psd1 to extract_powershell_manifest.
- `test_powershell_psd1_has_file_node()` — [`L1785`](../../../../../raw/code/graphify/tests/test_languages.py#L1785)
- `test_powershell_psd1_nested_modules()` — [`L1801`](../../../../../raw/code/graphify/tests/test_languages.py#L1801) — NestedModules = @('Helpers.psm1', 'Logger.psm1') produces edges for both.
- `test_powershell_psd1_no_dangling_edges()` — [`L1836`](../../../../../raw/code/graphify/tests/test_languages.py#L1836) — All imports_from edge sources must exist in the node set.
- `test_powershell_psd1_no_error()` — [`L1780`](../../../../../raw/code/graphify/tests/test_languages.py#L1780)
- `test_powershell_psd1_no_moduleversion_as_edge()` — [`L1827`](../../../../../raw/code/graphify/tests/test_languages.py#L1827) — ModuleVersion values ('5.0', '1.0.0') must NOT appear as import targets.
- `test_powershell_psd1_required_modules_hashtable()` — [`L1818`](../../../../../raw/code/graphify/tests/test_languages.py#L1818) — RequiredModules hashtable form @{{ ModuleName='Pester' }} produces an imports_from edge.
- `test_powershell_psd1_required_modules_string()` — [`L1809`](../../../../../raw/code/graphify/tests/test_languages.py#L1809) — RequiredModules string form 'PSReadLine' produces an imports_from edge.
- `test_powershell_psd1_root_module()` — [`L1792`](../../../../../raw/code/graphify/tests/test_languages.py#L1792) — RootModule = 'MyModule.psm1' produces an imports_from edge to 'mymodule'.
- `test_powershell_psm1_dispatched_and_extracted(tmp_path)` — [`L1664`](../../../../../raw/code/graphify/tests/test_languages.py#L1664)
- `test_razor_finds_code_block_methods()` — [`L2607`](../../../../../raw/code/graphify/tests/test_languages.py#L2607)
- `test_razor_finds_component_references()` — [`L2599`](../../../../../raw/code/graphify/tests/test_languages.py#L2599)
- `test_razor_finds_inherits()` — [`L2603`](../../../../../raw/code/graphify/tests/test_languages.py#L2603)
- `test_razor_finds_using_directives()` — [`L2595`](../../../../../raw/code/graphify/tests/test_languages.py#L2595)
- `test_razor_no_dangling_edges()` — [`L2613`](../../../../../raw/code/graphify/tests/test_languages.py#L2613)
- `test_razor_no_error()` — [`L2591`](../../../../../raw/code/graphify/tests/test_languages.py#L2591)
- `test_ruby_finds_class()` — [`L296`](../../../../../raw/code/graphify/tests/test_languages.py#L296)
- `test_ruby_finds_function()` — [`L306`](../../../../../raw/code/graphify/tests/test_languages.py#L306)
- `test_ruby_finds_methods()` — [`L300`](../../../../../raw/code/graphify/tests/test_languages.py#L300)
- `test_ruby_inherits_edge()` — [`L311`](../../../../../raw/code/graphify/tests/test_languages.py#L311) — `class Sub < Base` must emit an inherits edge.
- `test_ruby_no_error()` — [`L292`](../../../../../raw/code/graphify/tests/test_languages.py#L292)
- `test_scala_call_edges_have_call_context()` — [`L695`](../../../../../raw/code/graphify/tests/test_languages.py#L695)
- `test_scala_constructor_parameter_field_context()` — [`L675`](../../../../../raw/code/graphify/tests/test_languages.py#L675)
- `test_scala_finds_class()` — [`L647`](../../../../../raw/code/graphify/tests/test_languages.py#L647)
- `test_scala_finds_methods()` — [`L655`](../../../../../raw/code/graphify/tests/test_languages.py#L655)
- `test_scala_finds_object()` — [`L651`](../../../../../raw/code/graphify/tests/test_languages.py#L651)
- `test_scala_import_edges_have_import_context()` — [`L662`](../../../../../raw/code/graphify/tests/test_languages.py#L662)
- `test_scala_method_return_type_context()` — [`L690`](../../../../../raw/code/graphify/tests/test_languages.py#L690)
- `test_scala_no_error()` — [`L643`](../../../../../raw/code/graphify/tests/test_languages.py#L643)
- `test_scala_splits_inherits_and_mixes_in()` — [`L669`](../../../../../raw/code/graphify/tests/test_languages.py#L669)
- `test_scala_val_definition_field_context()` — [`L680`](../../../../../raw/code/graphify/tests/test_languages.py#L680)
- `test_scala_var_definition_field_context()` — [`L685`](../../../../../raw/code/graphify/tests/test_languages.py#L685)
- `test_sln_contains_edges()` — [`L2554`](../../../../../raw/code/graphify/tests/test_languages.py#L2554)
- `test_sln_finds_projects()` — [`L2548`](../../../../../raw/code/graphify/tests/test_languages.py#L2548)
- `test_sln_no_error()` — [`L2544`](../../../../../raw/code/graphify/tests/test_languages.py#L2544)
- `test_sln_project_dependency_edges()` — [`L2558`](../../../../../raw/code/graphify/tests/test_languages.py#L2558)
- `test_swift_call_edges_have_call_context()` — [`L968`](../../../../../raw/code/graphify/tests/test_languages.py#L968)
- `test_swift_emits_calls()` — [`L963`](../../../../../raw/code/graphify/tests/test_languages.py#L963)
- `test_swift_enum_associated_value_type_emits_references()` — [`L910`](../../../../../raw/code/graphify/tests/test_languages.py#L910)
- `test_swift_enum_cases_have_case_of_edge()` — [`L905`](../../../../../raw/code/graphify/tests/test_languages.py#L905)
- `test_swift_extension_across_files_merges_into_canonical_type()` — [`L975`](../../../../../raw/code/graphify/tests/test_languages.py#L975) — `extension Foo` in a separate file from `class Foo` must resolve to a
- `test_swift_extension_conformance_emits_implements()` — [`L945`](../../../../../raw/code/graphify/tests/test_languages.py#L945)
- `test_swift_extension_does_not_duplicate_type_node()` — [`L935`](../../../../../raw/code/graphify/tests/test_languages.py#L935)
- `test_swift_extension_folds_onto_objc_class()` — [`L2896`](../../../../../raw/code/graphify/tests/test_languages.py#L2896) — `extension Widget` in Swift over an ObjC `Widget` must fold onto the single
- `test_swift_extension_methods_attach_to_type()` — [`L922`](../../../../../raw/code/graphify/tests/test_languages.py#L922)
- `test_swift_finds_actor()` — [`L887`](../../../../../raw/code/graphify/tests/test_languages.py#L887)
- `test_swift_finds_class()` — [`L823`](../../../../../raw/code/graphify/tests/test_languages.py#L823)
- `test_swift_finds_deinit()` — [`L914`](../../../../../raw/code/graphify/tests/test_languages.py#L914)
- `test_swift_finds_enum()` — [`L891`](../../../../../raw/code/graphify/tests/test_languages.py#L891)
- `test_swift_finds_enum_cases()` — [`L899`](../../../../../raw/code/graphify/tests/test_languages.py#L899)
- `test_swift_finds_enum_methods()` — [`L895`](../../../../../raw/code/graphify/tests/test_languages.py#L895)
- `test_swift_finds_function()` — [`L841`](../../../../../raw/code/graphify/tests/test_languages.py#L841)
- `test_swift_finds_imports()` — [`L845`](../../../../../raw/code/graphify/tests/test_languages.py#L845)
- `test_swift_finds_methods()` — [`L835`](../../../../../raw/code/graphify/tests/test_languages.py#L835)
- `test_swift_finds_protocol()` — [`L827`](../../../../../raw/code/graphify/tests/test_languages.py#L827)
- `test_swift_finds_struct()` — [`L831`](../../../../../raw/code/graphify/tests/test_languages.py#L831)
- `test_swift_finds_subscript()` — [`L918`](../../../../../raw/code/graphify/tests/test_languages.py#L918)
- `test_swift_import_edges_have_import_context()` — [`L850`](../../../../../raw/code/graphify/tests/test_languages.py#L850)
- `test_swift_imports_survive_build()` — [`L865`](../../../../../raw/code/graphify/tests/test_languages.py#L865)
- `test_swift_no_dangling_edges()` — [`L856`](../../../../../raw/code/graphify/tests/test_languages.py#L856)
- `test_swift_no_error()` — [`L819`](../../../../../raw/code/graphify/tests/test_languages.py#L819)
- `test_swift_parameter_return_generic_and_field_contexts()` — [`L956`](../../../../../raw/code/graphify/tests/test_languages.py#L956)
- `test_swift_protocol_conformance_emits_implements()` — [`L940`](../../../../../raw/code/graphify/tests/test_languages.py#L940)
- `test_swift_splits_inherits_and_implements()` — [`L950`](../../../../../raw/code/graphify/tests/test_languages.py#L950)
- `test_systemverilog_does_not_emit_type_parameter_refs()` — [`L2739`](../../../../../raw/code/graphify/tests/test_languages.py#L2739)
- `test_systemverilog_field_parameter_return_and_generic_contexts()` — [`L2718`](../../../../../raw/code/graphify/tests/test_languages.py#L2718)
- `test_systemverilog_missing_file_returns_empty()` — [`L2752`](../../../../../raw/code/graphify/tests/test_languages.py#L2752)
- `test_systemverilog_no_dangling_edges()` — [`L2758`](../../../../../raw/code/graphify/tests/test_languages.py#L2758)
- `test_systemverilog_no_error()` — [`L2707`](../../../../../raw/code/graphify/tests/test_languages.py#L2707)
- `test_systemverilog_preserves_existing_module_extraction()` — [`L2744`](../../../../../raw/code/graphify/tests/test_languages.py#L2744)
- `test_systemverilog_qualified_field_references()` — [`L2727`](../../../../../raw/code/graphify/tests/test_languages.py#L2727) — Class properties with leading qualifiers (rand/local/protected/etc.) must
- `test_systemverilog_splits_inherits_and_implements()` — [`L2712`](../../../../../raw/code/graphify/tests/test_languages.py#L2712)
- `test_ts_constructor_injection_calls_edge(tmp_path)` — [`L1978`](../../../../../raw/code/graphify/tests/test_languages.py#L1978) — this.repo.findById() in a class with constructor(private repo: IUserRepository)
- `test_ts_dynamic_import_confidence()` — [`L1860`](../../../../../raw/code/graphify/tests/test_languages.py#L1860) — Dynamic imports should have EXTRACTED confidence (they are deterministic string literals).
- `test_ts_dynamic_import_extracts_edges()` — [`L1850`](../../../../../raw/code/graphify/tests/test_languages.py#L1850) — Dynamic import() calls inside functions should produce imports_from edges.
- `test_ts_dynamic_import_no_error()` — [`L1846`](../../../../../raw/code/graphify/tests/test_languages.py#L1846)
- `test_ts_dynamic_import_source_is_function()` — [`L1869`](../../../../../raw/code/graphify/tests/test_languages.py#L1869) — Dynamic import edge source should be the enclosing function, not the file.
- `test_ts_dynamic_template_literal_skipped()` — [`L1890`](../../../../../raw/code/graphify/tests/test_languages.py#L1890) — Dynamic template literals (with ${}) must not produce an imports_from edge.
- `test_ts_injected_field_ambiguous_type_emits_no_edge(tmp_path)` — [`L2101`](../../../../../raw/code/graphify/tests/test_languages.py#L2101) — If the injected field's type name is ambiguous (two classes named Database),
- `test_ts_injected_field_resolves_to_typed_class_not_same_named_collision(tmp_path)` — [`L2059`](../../../../../raw/code/graphify/tests/test_languages.py#L2059) — The decisive #1316 guardrail: two classes each define `query`, but the
- `test_ts_local_const_does_not_emit_phantom_node(tmp_path)` — [`L1960`](../../../../../raw/code/graphify/tests/test_languages.py#L1960) — Scope guard applies to TypeScript files too (shared _js_extra_walk path).
- `test_ts_no_dynamic_import_in_sync_fn()` — [`L1880`](../../../../../raw/code/graphify/tests/test_languages.py#L1880) — Functions without dynamic imports should not get spurious imports_from edges.
- `test_ts_static_template_literal_resolved()` — [`L1901`](../../../../../raw/code/graphify/tests/test_languages.py#L1901) — Static template literals (no ${}) should resolve the same as a plain string.
- `test_ts_this_field_receiver_not_same_file_collision(tmp_path)` — [`L2020`](../../../../../raw/code/graphify/tests/test_languages.py#L2020) — this.db.query() should NOT match an unrelated query() in the same file (#1316).
- `test_xaml_finds_class_and_event_references()` — [`L2585`](../../../../../raw/code/graphify/tests/test_languages.py#L2585)

## Module values
- `FIXTURES` — [`L15`](../../../../../raw/code/graphify/tests/test_languages.py#L15)
- `_needs_dm` — [`L21`](../../../../../raw/code/graphify/tests/test_languages.py#L21)

