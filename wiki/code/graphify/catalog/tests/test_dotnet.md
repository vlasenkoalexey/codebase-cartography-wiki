---
title: 'Module: tests/test_dotnet.py'
type: catalog
provenance: extracted
module: tests/test_dotnet.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_dotnet`/
symbols:
  FIXTURES: FIXTURES.
  _view_model_edges: _view_model_edges().
  _labels: _labels().
  test_sln_extracts_projects: test_sln_extracts_projects().
  test_sln_project_dependency: test_sln_project_dependency().
  test_slnx_extracts_projects: test_slnx_extracts_projects().
  test_slnx_project_dependency: test_slnx_project_dependency().
  test_csproj_packages: test_csproj_packages().
  test_csproj_target_framework: test_csproj_target_framework().
  test_csproj_sdk: test_csproj_sdk().
  test_xaml_named_controls_and_bindings: test_xaml_named_controls_and_bindings().
  test_xaml_element_datacontext_links_real_viewmodel_class: test_xaml_element_datacontext_links_real_viewmodel_class().
  test_xaml_design_instance_datacontext_links_real_viewmodel_class: test_xaml_design_instance_datacontext_links_real_viewmodel_class().
  test_xaml_infers_viewmodel_by_name_only_without_datacontext: test_xaml_infers_viewmodel_by_name_only_without_datacontext().
  test_xaml_prism_autowire_infers_viewmodel_from_filename: test_xaml_prism_autowire_infers_viewmodel_from_filename().
  test_xaml_prism_autowire_false_does_not_infer_from_filename: test_xaml_prism_autowire_false_does_not_infer_from_filename().
  test_extract_preserves_xaml_viewmodel_edge_after_id_remap: test_extract_preserves_xaml_viewmodel_edge_after_id_remap().
  test_extract_xaml_viewmodel_resolution_stays_inside_cache_root: test_extract_xaml_viewmodel_resolution_stays_inside_cache_root().
  test_xaml_viewmodel_resolution_respects_graphifyignore: test_xaml_viewmodel_resolution_respects_graphifyignore().
  test_xaml_viewmodel_with_non_utf8_codebehind_does_not_crash: test_xaml_viewmodel_with_non_utf8_codebehind_does_not_crash().
  test_razor_page_route: test_razor_page_route().
  test_razor_inherits: test_razor_inherits().
  test_razor_code_methods: test_razor_code_methods().
  test_sln_contains_edges: test_sln_contains_edges().
  test_slnx_contains_edges: test_slnx_contains_edges().
  test_csproj_project_references: test_csproj_project_references().
  test_xaml_class_resolves_to_codebehind_partial_class: test_xaml_class_resolves_to_codebehind_partial_class().
  test_xaml_extracts_binding_paths_commands_and_converters: test_xaml_extracts_binding_paths_commands_and_converters().
  test_xaml_links_communitytoolkit_generated_members_and_event_to_command: test_xaml_links_communitytoolkit_generated_members_and_event_to_command().
  test_xaml_ambiguous_viewmodel_names_emit_no_edge: test_xaml_ambiguous_viewmodel_names_emit_no_edge().
  test_xaml_events_resolve_to_codebehind_methods: test_xaml_events_resolve_to_codebehind_methods().
  test_xaml_event_match_requires_handler_signature: test_xaml_event_match_requires_handler_signature().
  test_xaml_non_event_attribute_value_does_not_fabricate_event: test_xaml_non_event_attribute_value_does_not_fabricate_event().
  test_razor_using_and_inject: test_razor_using_and_inject().
  test_razor_components: test_razor_components().
  _relations: _relations().
  test_slnx_invalid_xml: test_slnx_invalid_xml().
  test_slnx_missing_file: test_slnx_missing_file().
  test_csproj_invalid_xml: test_csproj_invalid_xml().
  test_razor_missing_file: test_razor_missing_file().
  test_dispatch_table: test_dispatch_table().
  test_code_extensions: test_code_extensions().
  _event_targets: _event_targets().
---
# Module: [`tests/test_dotnet.py`](../../../../../raw/code/graphify/tests/test_dotnet.py)

## Functions
- `_event_targets(r)` — [`L350`](../../../../../raw/code/graphify/tests/test_dotnet.py#L350)
- `_labels(r)` — [`L11`](../../../../../raw/code/graphify/tests/test_dotnet.py#L11)
- `_relations(r)` — [`L15`](../../../../../raw/code/graphify/tests/test_dotnet.py#L15)
- `_view_model_edges(r)` — [`L19`](../../../../../raw/code/graphify/tests/test_dotnet.py#L19)
- `test_code_extensions()` — [`L477`](../../../../../raw/code/graphify/tests/test_dotnet.py#L477)
- `test_csproj_invalid_xml()` — [`L110`](../../../../../raw/code/graphify/tests/test_dotnet.py#L110)
- `test_csproj_packages()` — [`L85`](../../../../../raw/code/graphify/tests/test_dotnet.py#L85)
- `test_csproj_project_references()` — [`L94`](../../../../../raw/code/graphify/tests/test_dotnet.py#L94)
- `test_csproj_sdk()` — [`L105`](../../../../../raw/code/graphify/tests/test_dotnet.py#L105)
- `test_csproj_target_framework()` — [`L100`](../../../../../raw/code/graphify/tests/test_dotnet.py#L100)
- `test_dispatch_table()` — [`L471`](../../../../../raw/code/graphify/tests/test_dotnet.py#L471)
- `test_extract_preserves_xaml_viewmodel_edge_after_id_remap(tmp_path)` — [`L268`](../../../../../raw/code/graphify/tests/test_dotnet.py#L268)
- `test_extract_xaml_viewmodel_resolution_stays_inside_cache_root(tmp_path)` — [`L285`](../../../../../raw/code/graphify/tests/test_dotnet.py#L285)
- `test_razor_code_methods()` — [`L457`](../../../../../raw/code/graphify/tests/test_dotnet.py#L457)
- `test_razor_components()` — [`L440`](../../../../../raw/code/graphify/tests/test_dotnet.py#L440)
- `test_razor_inherits()` — [`L452`](../../../../../raw/code/graphify/tests/test_dotnet.py#L452)
- `test_razor_missing_file()` — [`L464`](../../../../../raw/code/graphify/tests/test_dotnet.py#L464)
- `test_razor_page_route()` — [`L447`](../../../../../raw/code/graphify/tests/test_dotnet.py#L447)
- `test_razor_using_and_inject()` — [`L432`](../../../../../raw/code/graphify/tests/test_dotnet.py#L432)
- `test_sln_contains_edges()` — [`L37`](../../../../../raw/code/graphify/tests/test_dotnet.py#L37)
- `test_sln_extracts_projects()` — [`L28`](../../../../../raw/code/graphify/tests/test_dotnet.py#L28)
- `test_sln_project_dependency()` — [`L43`](../../../../../raw/code/graphify/tests/test_dotnet.py#L43)
- `test_slnx_contains_edges()` — [`L59`](../../../../../raw/code/graphify/tests/test_dotnet.py#L59)
- `test_slnx_extracts_projects()` — [`L50`](../../../../../raw/code/graphify/tests/test_dotnet.py#L50)
- `test_slnx_invalid_xml()` — [`L70`](../../../../../raw/code/graphify/tests/test_dotnet.py#L70)
- `test_slnx_missing_file()` — [`L78`](../../../../../raw/code/graphify/tests/test_dotnet.py#L78)
- `test_slnx_project_dependency()` — [`L65`](../../../../../raw/code/graphify/tests/test_dotnet.py#L65)
- `test_xaml_ambiguous_viewmodel_names_emit_no_edge(tmp_path)` — [`L308`](../../../../../raw/code/graphify/tests/test_dotnet.py#L308)
- `test_xaml_class_resolves_to_codebehind_partial_class()` — [`L120`](../../../../../raw/code/graphify/tests/test_dotnet.py#L120)
- `test_xaml_design_instance_datacontext_links_real_viewmodel_class()` — [`L172`](../../../../../raw/code/graphify/tests/test_dotnet.py#L172)
- `test_xaml_element_datacontext_links_real_viewmodel_class()` — [`L161`](../../../../../raw/code/graphify/tests/test_dotnet.py#L161)
- `test_xaml_event_match_requires_handler_signature()` — [`L355`](../../../../../raw/code/graphify/tests/test_dotnet.py#L355) — A property value that matches an ordinary method's name must not become an
- `test_xaml_events_resolve_to_codebehind_methods()` — [`L333`](../../../../../raw/code/graphify/tests/test_dotnet.py#L333)
- `test_xaml_extracts_binding_paths_commands_and_converters()` — [`L143`](../../../../../raw/code/graphify/tests/test_dotnet.py#L143)
- `test_xaml_infers_viewmodel_by_name_only_without_datacontext()` — [`L182`](../../../../../raw/code/graphify/tests/test_dotnet.py#L182)
- `test_xaml_links_communitytoolkit_generated_members_and_event_to_command()` — [`L218`](../../../../../raw/code/graphify/tests/test_dotnet.py#L218)
- `test_xaml_named_controls_and_bindings()` — [`L136`](../../../../../raw/code/graphify/tests/test_dotnet.py#L136)
- `test_xaml_non_event_attribute_value_does_not_fabricate_event()` — [`L380`](../../../../../raw/code/graphify/tests/test_dotnet.py#L380) — Content=/Tag= holding a string that equals a real handler's name must not
- `test_xaml_prism_autowire_false_does_not_infer_from_filename(tmp_path)` — [`L202`](../../../../../raw/code/graphify/tests/test_dotnet.py#L202)
- `test_xaml_prism_autowire_infers_viewmodel_from_filename()` — [`L192`](../../../../../raw/code/graphify/tests/test_dotnet.py#L192)
- `test_xaml_viewmodel_resolution_respects_graphifyignore(tmp_path)` — [`L298`](../../../../../raw/code/graphify/tests/test_dotnet.py#L298)
- `test_xaml_viewmodel_with_non_utf8_codebehind_does_not_crash(tmp_path)` — [`L411`](../../../../../raw/code/graphify/tests/test_dotnet.py#L411) — A ViewModel .cs with invalid UTF-8 bytes must not abort extract_xaml: the

## Module values
- `FIXTURES` — [`L8`](../../../../../raw/code/graphify/tests/test_dotnet.py#L8)

