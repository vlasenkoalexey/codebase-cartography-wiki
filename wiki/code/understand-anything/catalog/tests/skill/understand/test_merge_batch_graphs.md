---
title: 'Module: tests/skill/understand/test_merge_batch_graphs.py'
type: catalog
provenance: extracted
module: tests/skill/understand/test_merge_batch_graphs.py
status: fresh
symbol_base: scip-python python understand-anything 0.0.0 `tests.skill.understand.test_merge_batch_graphs`/
symbols:
  mbg: mbg.
  _file_node: _file_node().
  TestMultiPart._write_batch: TestMultiPart#_write_batch().
  TestMultiPart._run_merge: TestMultiPart#_run_merge().
  TestUnrecognizedBatchFilename._write_batch: TestUnrecognizedBatchFilename#_write_batch().
  TestUnrecognizedBatchFilename._run_merge: TestUnrecognizedBatchFilename#_run_merge().
  TestMultiPart.test_malformed_part_is_skipped_with_warning: TestMultiPart#test_malformed_part_is_skipped_with_warning().
  TestMultiPart.intermediate: TestMultiPart#intermediate.
  TestUnrecognizedBatchFilename.intermediate: TestUnrecognizedBatchFilename#intermediate.
  TestMultiPart.test_two_parts_of_one_logical_batch_merge: TestMultiPart#test_two_parts_of_one_logical_batch_merge().
  TestMultiPart.test_three_parts_of_one_logical_batch_merge: TestMultiPart#test_three_parts_of_one_logical_batch_merge().
  TestMultiPart.test_mixed_single_and_multi_part: TestMultiPart#test_mixed_single_and_multi_part().
  TestMultiPart.test_missing_part_emits_warning: TestMultiPart#test_missing_part_emits_warning().
  TestMultiPart.test_stderr_report_format: TestMultiPart#test_stderr_report_format().
  TestUnrecognizedBatchFilename.test_fused_filename_emits_stderr_warning: TestUnrecognizedBatchFilename#test_fused_filename_emits_stderr_warning().
  TestUnrecognizedBatchFilename.test_fused_filename_surfaces_in_report: TestUnrecognizedBatchFilename#test_fused_filename_surfaces_in_report().
  TestUnrecognizedBatchFilename.test_recognized_batches_still_loaded: TestUnrecognizedBatchFilename#test_recognized_batches_still_loaded().
  TestUnrecognizedBatchFilename.test_range_filename_also_unrecognized: TestUnrecognizedBatchFilename#test_range_filename_also_unrecognized().
  _MODULE_PATH: _MODULE_PATH.
  LinkTestsTests.test_basic_pairing_emits_forward_edge: LinkTestsTests#test_basic_pairing_emits_forward_edge().
  LinkTestsTests.test_no_production_counterpart_no_edge: LinkTestsTests#test_no_production_counterpart_no_edge().
  LinkTestsTests.test_inverted_llm_edge_is_swapped_not_stripped: LinkTestsTests#test_inverted_llm_edge_is_swapped_not_stripped().
  LinkTestsTests.test_canonical_llm_edge_kept_unchanged: LinkTestsTests#test_canonical_llm_edge_kept_unchanged().
  LinkTestsTests.test_drops_test_to_test_edge: LinkTestsTests#test_drops_test_to_test_edge().
  LinkTestsTests.test_drops_orphan_endpoint_edge: LinkTestsTests#test_drops_orphan_endpoint_edge().
  LinkTestsTests.test_dup_keeps_higher_weight_canonical: LinkTestsTests#test_dup_keeps_higher_weight_canonical().
  LinkTestsTests.test_dup_lighter_inverted_dropped_no_swap_counted: LinkTestsTests#test_dup_lighter_inverted_dropped_no_swap_counted().
  LinkTestsTests.test_dup_replaces_with_heavier_inverted: LinkTestsTests#test_dup_replaces_with_heavier_inverted().
  LinkTestsTests.test_dup_swapped_then_canonical_heavier_clears_swapped_count: LinkTestsTests#test_dup_swapped_then_canonical_heavier_clears_swapped_count().
  LinkTestsTests.test_dup_two_inverted_keeps_heavier_swapped_once: LinkTestsTests#test_dup_two_inverted_keeps_heavier_swapped_once().
  LinkTestsTests.test_drops_duplicate_canonical_edges: LinkTestsTests#test_drops_duplicate_canonical_edges().
  LinkTestsTests.test_supplement_skips_pair_already_covered_by_llm: LinkTestsTests#test_supplement_skips_pair_already_covered_by_llm().
  LinkTestsTests.test_swap_recovers_real_world_one_test_many_production: LinkTestsTests#test_swap_recovers_real_world_one_test_many_production().
  LinkTestsTests.test_unrelated_edges_pass_through: LinkTestsTests#test_unrelated_edges_pass_through().
  LinkTestsTests.test_direction_always_forward_production_to_test: LinkTestsTests#test_direction_always_forward_production_to_test().
  LinkTestsTests.test_idempotent: LinkTestsTests#test_idempotent().
  LinkTestsTests.test_first_matching_candidate_wins: LinkTestsTests#test_first_matching_candidate_wins().
  LinkTestsTests.test_does_not_match_test_to_test: LinkTestsTests#test_does_not_match_test_to_test().
  LinkTestsTests.test_does_not_duplicate_existing_tag: LinkTestsTests#test_does_not_duplicate_existing_tag().
  LinkTestsTests.test_malformed_tags_is_replaced_not_crashed: LinkTestsTests#test_malformed_tags_is_replaced_not_crashed().
  MergeEdgeDirectionTests.test_missing_direction_is_persisted_as_forward: MergeEdgeDirectionTests#test_missing_direction_is_persisted_as_forward().
  MergeEdgeDirectionTests.test_alias_is_canonicalized_before_dedup: MergeEdgeDirectionTests#test_alias_is_canonicalized_before_dedup().
  _REPO_ROOT: _REPO_ROOT.
  _load_module: _load_module().
  MergeEdgeDirectionTests._two_node_batch: MergeEdgeDirectionTests#_two_node_batch().
  TestMultiPart.tmp: TestMultiPart#tmp.
  TestUnrecognizedBatchFilename.tmp: TestUnrecognizedBatchFilename#tmp.
  IsTestPathTests.test_js_ts_sibling_test_extensions: IsTestPathTests#test_js_ts_sibling_test_extensions().
  IsTestPathTests.test_underscore_test_dir_with_test_extension: IsTestPathTests#test_underscore_test_dir_with_test_extension().
  IsTestPathTests.test_tests_directory_with_test_extension: IsTestPathTests#test_tests_directory_with_test_extension().
  IsTestPathTests.test_go_test_files: IsTestPathTests#test_go_test_files().
  IsTestPathTests.test_python_test_files: IsTestPathTests#test_python_test_files().
  IsTestPathTests.test_java_test_files: IsTestPathTests#test_java_test_files().
  IsTestPathTests.test_kotlin_test_files: IsTestPathTests#test_kotlin_test_files().
  IsTestPathTests.test_csharp_test_files: IsTestPathTests#test_csharp_test_files().
  IsTestPathTests.test_c_cpp_test_files: IsTestPathTests#test_c_cpp_test_files().
  IsTestPathTests.test_production_files_rejected: IsTestPathTests#test_production_files_rejected().
  IsTestPathTests.test_helper_in_tests_dir_without_test_extension_is_not_test: IsTestPathTests#test_helper_in_tests_dir_without_test_extension_is_not_test().
  ProductionCandidatesTests.test_js_ts_sibling: ProductionCandidatesTests#test_js_ts_sibling().
  ProductionCandidatesTests.test_js_ts_spec_sibling: ProductionCandidatesTests#test_js_ts_spec_sibling().
  ProductionCandidatesTests.test_underscore_tests_dir: ProductionCandidatesTests#test_underscore_tests_dir().
  ProductionCandidatesTests.test_mirrored_tests_tree: ProductionCandidatesTests#test_mirrored_tests_tree().
  ProductionCandidatesTests.test_go_sibling: ProductionCandidatesTests#test_go_sibling().
  ProductionCandidatesTests.test_python_test_prefix: ProductionCandidatesTests#test_python_test_prefix().
  ProductionCandidatesTests.test_python_test_suffix: ProductionCandidatesTests#test_python_test_suffix().
  ProductionCandidatesTests.test_java_maven_layout: ProductionCandidatesTests#test_java_maven_layout().
  ProductionCandidatesTests.test_java_tests_suffix: ProductionCandidatesTests#test_java_tests_suffix().
  ProductionCandidatesTests.test_java_it_suffix: ProductionCandidatesTests#test_java_it_suffix().
  ProductionCandidatesTests.test_kotlin_maven_layout: ProductionCandidatesTests#test_kotlin_maven_layout().
  ProductionCandidatesTests.test_js_ts_test_subdir_walkout: ProductionCandidatesTests#test_js_ts_test_subdir_walkout().
  ProductionCandidatesTests.test_python_in_package_tests_walkout: ProductionCandidatesTests#test_python_in_package_tests_walkout().
  ProductionCandidatesTests.test_csharp_tests_subdir_mirror_to_src: ProductionCandidatesTests#test_csharp_tests_subdir_mirror_to_src().
  ProductionCandidatesTests.test_csharp_dotnet_sibling_project_mirror: ProductionCandidatesTests#test_csharp_dotnet_sibling_project_mirror().
  ProductionCandidatesTests.test_priority_underscore_tests_sibling_before_walkup: ProductionCandidatesTests#test_priority_underscore_tests_sibling_before_walkup().
  ProductionCandidatesTests.test_priority_mirrored_tree_sibling_before_mirror: ProductionCandidatesTests#test_priority_mirrored_tree_sibling_before_mirror().
  LinkTestsTests.test_empty_input: LinkTestsTests#test_empty_input().
  LinkTestsTests.test_node_without_filepath_falls_back_to_id: LinkTestsTests#test_node_without_filepath_falls_back_to_id().
  MergeIntegrationTests.test_linker_runs_during_merge: MergeIntegrationTests#test_linker_runs_during_merge().
  NormalizeDirectionTests.test_missing_defaults_to_forward: NormalizeDirectionTests#test_missing_defaults_to_forward().
  NormalizeDirectionTests.test_valid_values_pass_through: NormalizeDirectionTests#test_valid_values_pass_through().
  NormalizeDirectionTests.test_case_is_normalized: NormalizeDirectionTests#test_case_is_normalized().
  NormalizeDirectionTests.test_aliases_are_mapped: NormalizeDirectionTests#test_aliases_are_mapped().
  NormalizeDirectionTests.test_unknown_values_fall_back_to_forward: NormalizeDirectionTests#test_unknown_values_fall_back_to_forward().
  TestMultiPart.tearDown: TestMultiPart#tearDown().
  TestUnrecognizedBatchFilename.tearDown: TestUnrecognizedBatchFilename#tearDown().
  _HERE: _HERE.
  IsTestPathTests: IsTestPathTests#
  ProductionCandidatesTests: ProductionCandidatesTests#
  LinkTestsTests: LinkTestsTests#
  MergeIntegrationTests: MergeIntegrationTests#
  NormalizeDirectionTests: NormalizeDirectionTests#
  MergeEdgeDirectionTests: MergeEdgeDirectionTests#
  TestMultiPart: TestMultiPart#
  TestMultiPart.setUp: TestMultiPart#setUp().
  TestUnrecognizedBatchFilename: TestUnrecognizedBatchFilename#
  TestUnrecognizedBatchFilename.setUp: TestUnrecognizedBatchFilename#setUp().
---
# Module: [`tests/skill/understand/test_merge_batch_graphs.py`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py)

## Classes
### `IsTestPathTests`  ·  implements/extends TestCase
- def: [`tests/skill/understand/test_merge_batch_graphs.py:65`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L65)
- doc: Path classification: production vs. test.
- signature: `class IsTestPathTests(unittest.TestCase):`
- members:
  - `test_c_cpp_test_files(self)` — [`L116`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L116)
  - `test_csharp_test_files(self)` — [`L112`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L112)
  - `test_go_test_files(self)` — [`L94`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L94)
  - `test_helper_in_tests_dir_without_test_extension_is_not_test(self)` — [`L140`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L140)
  - `test_java_test_files(self)` — [`L103`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L103)
  - `test_js_ts_sibling_test_extensions(self)` — [`L68`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L68)
  - `test_kotlin_test_files(self)` — [`L108`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L108)
  - `test_production_files_rejected(self)` — [`L123`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L123)
  - `test_python_test_files(self)` — [`L98`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L98)
  - `test_tests_directory_with_test_extension(self)` — [`L89`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L89)
  - `test_underscore_test_dir_with_test_extension(self)` — [`L85`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L85)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `LinkTestsTests`  ·  implements/extends TestCase
- def: [`tests/skill/understand/test_merge_batch_graphs.py:275`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L275)
- doc: End-to-end behaviour of the linker against a node/edge set.
- signature: `class LinkTestsTests(unittest.TestCase):`
- members:
  - `test_basic_pairing_emits_forward_edge(self)` — [`L278`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L278)
  - `test_canonical_llm_edge_kept_unchanged(self)` — [`L350`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L350)
  - `test_direction_always_forward_production_to_test(self)` — [`L680`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L680)
  - `test_does_not_duplicate_existing_tag(self)` — [`L764`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L764)
  - `test_does_not_match_test_to_test(self)` — [`L750`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L750)
  - `test_drops_duplicate_canonical_edges(self)` — [`L539`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L539)
  - `test_drops_orphan_endpoint_edge(self)` — [`L402`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L402)
  - `test_drops_test_to_test_edge(self)` — [`L377`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L377)
  - `test_dup_keeps_higher_weight_canonical(self)` — [`L423`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L423)
  - `test_dup_lighter_inverted_dropped_no_swap_counted(self)` — [`L443`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L443)
  - `test_dup_replaces_with_heavier_inverted(self)` — [`L468`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L468)
  - `test_dup_swapped_then_canonical_heavier_clears_swapped_count(self)` — [`L493`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L493)
  - `test_dup_two_inverted_keeps_heavier_swapped_once(self)` — [`L515`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L515)
  - `test_empty_input(self)` — [`L779`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L779)
  - `test_first_matching_candidate_wins(self)` — [`L728`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L728)
  - `test_idempotent(self)` — [`L707`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L707)
  - `test_inverted_llm_edge_is_swapped_not_stripped(self)` — [`L315`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L315)
  - `test_malformed_tags_is_replaced_not_crashed(self)` — [`L805`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L805)
  - `test_no_production_counterpart_no_edge(self)` — [`L302`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L302)
  - `test_node_without_filepath_falls_back_to_id(self)` — [`L785`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L785)
  - `test_supplement_skips_pair_already_covered_by_llm(self)` — [`L573`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L573)
  - `test_swap_recovers_real_world_one_test_many_production(self)` — [`L607`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L607)
  - `test_unrelated_edges_pass_through(self)` — [`L650`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L650)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `MergeEdgeDirectionTests`  ·  implements/extends TestCase
- def: [`tests/skill/understand/test_merge_batch_graphs.py:905`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L905)
- doc: End-to-end: merge_and_normalize persists a canonical `direction`.
- signature: `class MergeEdgeDirectionTests(unittest.TestCase):`
- members:
  - `test_alias_is_canonicalized_before_dedup(self)` — [`L930`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L930)
  - `test_missing_direction_is_persisted_as_forward(self)` — [`L914`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L914)
- protocol/private: `_two_node_batch`[`L908`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L908)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `MergeIntegrationTests`  ·  implements/extends TestCase
- def: [`tests/skill/understand/test_merge_batch_graphs.py:830`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L830)
- doc: Verify the linker is wired into merge_and_normalize correctly.
- signature: `class MergeIntegrationTests(unittest.TestCase):`
- members:
  - `test_linker_runs_during_merge(self)` — [`L833`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L833)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `NormalizeDirectionTests`  ·  implements/extends TestCase
- def: [`tests/skill/understand/test_merge_batch_graphs.py:880`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L880)
- doc: `direction` canonicalization mirrors the dashboard schema validator.
- signature: `class NormalizeDirectionTests(unittest.TestCase):`
- members:
  - `test_aliases_are_mapped(self)` — [`L896`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L896)
  - `test_case_is_normalized(self)` — [`L892`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L892)
  - `test_missing_defaults_to_forward(self)` — [`L883`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L883)
  - `test_unknown_values_fall_back_to_forward(self)` — [`L900`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L900)
  - `test_valid_values_pass_through(self)` — [`L887`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L887)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `ProductionCandidatesTests`  ·  implements/extends TestCase
- def: [`tests/skill/understand/test_merge_batch_graphs.py:151`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L151)
- doc: For each test path, what production paths should we try?
- signature: `class ProductionCandidatesTests(unittest.TestCase):`
- members:
  - `test_csharp_dotnet_sibling_project_mirror(self)` — [`L242`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L242)
  - `test_csharp_tests_subdir_mirror_to_src(self)` — [`L226`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L226)
  - `test_go_sibling(self)` — [`L178`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L178)
  - `test_java_it_suffix(self)` — [`L201`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L201)
  - `test_java_maven_layout(self)` — [`L193`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L193)
  - `test_java_tests_suffix(self)` — [`L197`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L197)
  - `test_js_ts_sibling(self)` — [`L154`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L154)
  - `test_js_ts_spec_sibling(self)` — [`L162`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L162)
  - `test_js_ts_test_subdir_walkout(self)` — [`L209`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L209)
  - `test_kotlin_maven_layout(self)` — [`L205`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L205)
  - `test_mirrored_tests_tree(self)` — [`L172`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L172)
  - `test_priority_mirrored_tree_sibling_before_mirror(self)` — [`L263`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L263)
  - `test_priority_underscore_tests_sibling_before_walkup(self)` — [`L252`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L252)
  - `test_python_in_package_tests_walkout(self)` — [`L217`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L217)
  - `test_python_test_prefix(self)` — [`L182`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L182)
  - `test_python_test_suffix(self)` — [`L189`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L189)
  - `test_underscore_tests_dir(self)` — [`L167`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L167)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestMultiPart`  ·  implements/extends TestCase
- def: [`tests/skill/understand/test_merge_batch_graphs.py:954`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L954)
- doc: End-to-end tests for batch-&lt;i&gt;-part-&lt;k&gt;.json input handling.
- signature: `class TestMultiPart(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L961`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L961)
  - `tearDown(self)` — [`L967`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L967)
  - `test_malformed_part_is_skipped_with_warning(self)` — [`L1016`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1016)
  - `test_missing_part_emits_warning(self)` — [`L1046`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1046)
  - `test_mixed_single_and_multi_part(self)` — [`L1029`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1029)
  - `test_stderr_report_format(self)` — [`L1058`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1058)
  - `test_three_parts_of_one_logical_batch_merge(self)` — [`L1006`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1006)
  - `test_two_parts_of_one_logical_batch_merge(self)` — [`L989`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L989)
  - `intermediate` — [`L964`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L964)
  - `tmp` — [`L963`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L963)
- protocol/private: `_run_merge`[`L978`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L978), `_write_batch`[`L971`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L971)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestUnrecognizedBatchFilename`  ·  implements/extends TestCase
- def: [`tests/skill/understand/test_merge_batch_graphs.py:1072`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1072)
- doc: File-analyzer fuses multiple batches into one output (e.g.,
- signature: `class TestUnrecognizedBatchFilename(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L1080`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1080)
  - `tearDown(self)` — [`L1086`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1086)
  - `test_fused_filename_emits_stderr_warning(self)` — [`L1108`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1108)
  - `test_fused_filename_surfaces_in_report(self)` — [`L1127`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1127)
  - `test_range_filename_also_unrecognized(self)` — [`L1165`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1165)
  - `test_recognized_batches_still_loaded(self)` — [`L1145`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1145)
  - `intermediate` — [`L1083`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1083)
  - `tmp` — [`L1082`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1082)
- protocol/private: `_run_merge`[`L1097`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1097), `_write_batch`[`L1090`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L1090)
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `_file_node(path: str, **extra: Any)` — [`L48`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L48) — Build a minimal file node with the given relative path.
- `_load_module()` — [`L33`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L33)

## Module values
- `_HERE` — [`L22`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L22)
- `_MODULE_PATH` — [`L24`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L24)
- `_REPO_ROOT` — [`L23`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L23)
- `mbg` — [`L43`](../../../../../../../raw/code/understand-anything/tests/skill/understand/test_merge_batch_graphs.py#L43)

