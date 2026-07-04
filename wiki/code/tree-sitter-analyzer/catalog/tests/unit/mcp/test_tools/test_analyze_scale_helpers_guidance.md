---
title: 'Module: tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools.test_analyze_scale_helpers_guidance`/Test
symbols:
  TestGenerateLlmGuidance._base_metrics: GenerateLlmGuidance#_base_metrics().
  TestGenerateLlmGuidance._base_overview: GenerateLlmGuidance#_base_overview().
  TestGenerateLlmGuidance.test_small_file_size_category: GenerateLlmGuidance#test_small_file_size_category().
  TestGenerateLlmGuidance.test_medium_file_size_category: GenerateLlmGuidance#test_medium_file_size_category().
  TestGenerateLlmGuidance.test_large_file_size_category: GenerateLlmGuidance#test_large_file_size_category().
  TestGenerateLlmGuidance.test_very_large_file_size_category: GenerateLlmGuidance#test_very_large_file_size_category().
  TestGenerateLlmGuidance.test_large_file_recommends_targeted_tools: GenerateLlmGuidance#test_large_file_recommends_targeted_tools().
  TestGenerateLlmGuidance.test_small_file_no_targeted_tools: GenerateLlmGuidance#test_small_file_no_targeted_tools().
  TestGenerateLlmGuidance.test_complexity_hotspots_recommends_structure_analysis: GenerateLlmGuidance#test_complexity_hotspots_recommends_structure_analysis().
  TestGenerateLlmGuidance.test_no_hotspots_assessment: GenerateLlmGuidance#test_no_hotspots_assessment().
  TestGenerateLlmGuidance.test_multiple_classes_key_area: GenerateLlmGuidance#test_multiple_classes_key_area().
  TestGenerateLlmGuidance.test_many_methods_key_area: GenerateLlmGuidance#test_many_methods_key_area().
  TestGenerateLlmGuidance.test_many_imports_key_area: GenerateLlmGuidance#test_many_imports_key_area().
  TestGenerateLlmGuidance.test_python_language_suggested_queries: GenerateLlmGuidance#test_python_language_suggested_queries().
  TestGenerateLlmGuidance.test_unknown_language_no_suggested_queries: GenerateLlmGuidance#test_unknown_language_no_suggested_queries().
  TestGenerateLlmGuidance.test_workflow_steps_always_start_with_check_scale: GenerateLlmGuidance#test_workflow_steps_always_start_with_check_scale().
  TestGenerateLlmGuidance.test_large_file_workflow_includes_targeted_steps: GenerateLlmGuidance#test_large_file_workflow_includes_targeted_steps().
  TestGenerateLlmGuidance.test_small_file_workflow_includes_full_analysis: GenerateLlmGuidance#test_small_file_workflow_includes_full_analysis().
  TestGenerateLlmGuidance.test_many_imports_suggests_dependency_analysis: GenerateLlmGuidance#test_many_imports_suggests_dependency_analysis().
  TestGenerateLlmGuidance.test_hotspot_in_large_file_workflow: GenerateLlmGuidance#test_hotspot_in_large_file_workflow().
  TestGenerateLlmGuidance.test_available_queries_populated_from_loader: GenerateLlmGuidance#test_available_queries_populated_from_loader().
  TestGenerateLlmGuidance.test_missing_structural_fields_populated: GenerateLlmGuidance#test_missing_structural_fields_populated().
  TestValidateScaleArguments.test_single_file_valid: ValidateScaleArguments#test_single_file_valid().
  TestValidateScaleArguments.test_single_file_with_options: ValidateScaleArguments#test_single_file_with_options().
  TestValidateScaleArguments.test_batch_mode_valid: ValidateScaleArguments#test_batch_mode_valid().
  TestValidateScaleArguments.test_missing_file_path_raises: ValidateScaleArguments#test_missing_file_path_raises().
  TestValidateScaleArguments.test_empty_file_path_raises: ValidateScaleArguments#test_empty_file_path_raises().
  TestValidateScaleArguments.test_non_string_file_path_raises: ValidateScaleArguments#test_non_string_file_path_raises().
  TestValidateScaleArguments.test_file_paths_mutually_exclusive: ValidateScaleArguments#test_file_paths_mutually_exclusive().
  TestValidateScaleArguments.test_file_paths_non_list_raises: ValidateScaleArguments#test_file_paths_non_list_raises().
  TestValidateScaleArguments.test_file_paths_empty_list_raises: ValidateScaleArguments#test_file_paths_empty_list_raises().
  TestValidateScaleArguments.test_file_paths_metrics_only_false_raises: ValidateScaleArguments#test_file_paths_metrics_only_false_raises().
  TestValidateScaleArguments.test_metrics_only_non_bool_raises: ValidateScaleArguments#test_metrics_only_non_bool_raises().
  TestValidateScaleArguments.test_language_non_string_raises: ValidateScaleArguments#test_language_non_string_raises().
  TestValidateScaleArguments.test_include_complexity_non_bool_raises: ValidateScaleArguments#test_include_complexity_non_bool_raises().
  TestValidateScaleArguments.test_include_details_non_bool_raises: ValidateScaleArguments#test_include_details_non_bool_raises().
  TestValidateScaleArguments.test_include_guidance_non_bool_raises: ValidateScaleArguments#test_include_guidance_non_bool_raises().
  TestGenerateLlmGuidance: GenerateLlmGuidance#
  TestValidateScaleArguments: ValidateScaleArguments#
---
# Module: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py)

## Classes
### `TestGenerateLlmGuidance`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py:13`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L13)
- signature: `class TestGenerateLlmGuidance:`
- members:
  - `test_available_queries_populated_from_loader(self, mock_loader)` — [`L170`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L170)
  - `test_complexity_hotspots_recommends_structure_analysis(self)` — [`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L64)
  - `test_hotspot_in_large_file_workflow(self)` — [`L144`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L144)
  - `test_large_file_recommends_targeted_tools(self)` — [`L51`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L51)
  - `test_large_file_size_category(self)` — [`L39`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L39)
  - `test_large_file_workflow_includes_targeted_steps(self)` — [`L123`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L123)
  - `test_many_imports_key_area(self)` — [`L91`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L91)
  - `test_many_imports_suggests_dependency_analysis(self)` — [`L137`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L137)
  - `test_many_methods_key_area(self)` — [`L85`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L85)
  - `test_medium_file_size_category(self)` — [`L33`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L33)
  - `test_missing_structural_fields_populated(self)` — [`L160`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L160)
  - `test_multiple_classes_key_area(self)` — [`L79`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L79)
  - `test_no_hotspots_assessment(self)` — [`L73`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L73)
  - `test_python_language_suggested_queries(self, mock_loader)` — [`L98`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L98)
  - `test_small_file_no_targeted_tools(self)` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L58)
  - `test_small_file_size_category(self)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L26)
  - `test_small_file_workflow_includes_full_analysis(self)` — [`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L130)
  - `test_unknown_language_no_suggested_queries(self, mock_loader)` — [`L110`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L110)
  - `test_very_large_file_size_category(self)` — [`L45`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L45)
  - `test_workflow_steps_always_start_with_check_scale(self)` — [`L117`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L117)
- protocol/private: `_base_metrics`[`L14`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L14), `_base_overview`[`L17`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L17)
- uses (calls/refs, reference-scoped): [`generate_llm_guidance`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#generate_llm_guidance)

### `TestValidateScaleArguments`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py:184`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L184)
- signature: `class TestValidateScaleArguments:`
- members:
  - `test_batch_mode_valid(self)` — [`L199`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L199)
  - `test_empty_file_path_raises(self)` — [`L212`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L212)
  - `test_file_paths_empty_list_raises(self)` — [`L238`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L238)
  - `test_file_paths_metrics_only_false_raises(self)` — [`L244`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L244)
  - `test_file_paths_mutually_exclusive(self)` — [`L224`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L224)
  - `test_file_paths_non_list_raises(self)` — [`L232`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L232)
  - `test_include_complexity_non_bool_raises(self)` — [`L266`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L266)
  - `test_include_details_non_bool_raises(self)` — [`L274`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L274)
  - `test_include_guidance_non_bool_raises(self)` — [`L282`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L282)
  - `test_language_non_string_raises(self)` — [`L260`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L260)
  - `test_metrics_only_non_bool_raises(self)` — [`L252`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L252)
  - `test_missing_file_path_raises(self)` — [`L206`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L206)
  - `test_non_string_file_path_raises(self)` — [`L218`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L218)
  - `test_single_file_valid(self)` — [`L185`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L185)
  - `test_single_file_with_options(self)` — [`L189`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_helpers_guidance.py#L189)
- uses (calls/refs, reference-scoped): [`validate_scale_arguments`](../../../../tree_sitter_analyzer/mcp/tools/analyze_scale_helpers.md#validate_scale_arguments)

