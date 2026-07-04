---
title: 'Module: tests/unit/mcp/test_tools/test_analyze_scale_core.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_tools/test_analyze_scale_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_tools.test_analyze_scale_core`/
symbols:
  tool: tool().
  tool_with_project_root: tool_with_project_root().
  TestAnalyzeScaleToolExecute: TestAnalyzeScaleToolExecute#
  TestAnalyzeScaleToolExecuteMetricsBatch: TestAnalyzeScaleToolExecuteMetricsBatch#
  TestAnalyzeScaleToolCreateJsonFileAnalysis: TestAnalyzeScaleToolCreateJsonFileAnalysis#
  TestAnalyzeScaleToolCalculateFileMetrics: TestAnalyzeScaleToolCalculateFileMetrics#
  TestAnalyzeScaleToolCalculateFileMetrics.test_calculate_file_metrics_success: TestAnalyzeScaleToolCalculateFileMetrics#test_calculate_file_metrics_success().
  TestAnalyzeScaleToolCalculateFileMetrics.test_calculate_file_metrics_error_handling: TestAnalyzeScaleToolCalculateFileMetrics#test_calculate_file_metrics_error_handling().
  TestAnalyzeScaleToolExtractStructuralOverview: TestAnalyzeScaleToolExtractStructuralOverview#
  TestAnalyzeScaleToolExtractStructuralOverview.test_extract_structural_overview_empty: TestAnalyzeScaleToolExtractStructuralOverview#test_extract_structural_overview_empty().
  TestAnalyzeScaleToolExtractStructuralOverview.test_extract_structural_overview_with_classes: TestAnalyzeScaleToolExtractStructuralOverview#test_extract_structural_overview_with_classes().
  TestAnalyzeScaleToolExtractStructuralOverview.test_extract_structural_overview_with_methods: TestAnalyzeScaleToolExtractStructuralOverview#test_extract_structural_overview_with_methods().
  TestAnalyzeScaleToolExtractStructuralOverview.test_extract_structural_overview_with_high_complexity_method: TestAnalyzeScaleToolExtractStructuralOverview#test_extract_structural_overview_with_high_complexity_method().
  TestAnalyzeScaleToolExtractStructuralOverview.test_extract_structural_overview_with_fields: TestAnalyzeScaleToolExtractStructuralOverview#test_extract_structural_overview_with_fields().
  TestAnalyzeScaleToolExtractStructuralOverview.test_extract_structural_overview_with_imports: TestAnalyzeScaleToolExtractStructuralOverview#test_extract_structural_overview_with_imports().
  TestAnalyzeScaleToolGenerateLLMGuidance: TestAnalyzeScaleToolGenerateLLMGuidance#
  TestAnalyzeScaleToolGenerateLLMGuidance.test_generate_llm_guidance_small_file: TestAnalyzeScaleToolGenerateLLMGuidance#test_generate_llm_guidance_small_file().
  TestAnalyzeScaleToolGenerateLLMGuidance.test_generate_llm_guidance_medium_file: TestAnalyzeScaleToolGenerateLLMGuidance#test_generate_llm_guidance_medium_file().
  TestAnalyzeScaleToolGenerateLLMGuidance.test_generate_llm_guidance_large_file: TestAnalyzeScaleToolGenerateLLMGuidance#test_generate_llm_guidance_large_file().
  TestAnalyzeScaleToolGenerateLLMGuidance.test_generate_llm_guidance_very_large_file: TestAnalyzeScaleToolGenerateLLMGuidance#test_generate_llm_guidance_very_large_file().
  TestAnalyzeScaleToolGenerateLLMGuidance.test_generate_llm_guidance_with_complexity_hotspots: TestAnalyzeScaleToolGenerateLLMGuidance#test_generate_llm_guidance_with_complexity_hotspots().
  TestAnalyzeScaleToolGenerateLLMGuidance.test_generate_llm_guidance_without_complexity_hotspots: TestAnalyzeScaleToolGenerateLLMGuidance#test_generate_llm_guidance_without_complexity_hotspots().
  TestAnalyzeScaleToolGenerateLLMGuidance.test_generate_llm_guidance_multiple_classes: TestAnalyzeScaleToolGenerateLLMGuidance#test_generate_llm_guidance_multiple_classes().
  TestAnalyzeScaleToolGenerateLLMGuidance.test_generate_llm_guidance_many_methods: TestAnalyzeScaleToolGenerateLLMGuidance#test_generate_llm_guidance_many_methods().
  TestAnalyzeScaleToolGenerateLLMGuidance.test_generate_llm_guidance_many_imports: TestAnalyzeScaleToolGenerateLLMGuidance#test_generate_llm_guidance_many_imports().
  TestAnalyzeScaleToolExecute.__test__: TestAnalyzeScaleToolExecute#__test__.
  TestAnalyzeScaleToolExecuteMetricsBatch.__test__: TestAnalyzeScaleToolExecuteMetricsBatch#__test__.
  TestAnalyzeScaleToolCreateJsonFileAnalysis.__test__: TestAnalyzeScaleToolCreateJsonFileAnalysis#__test__.
  TestAnalyzeScaleToolExtractStructuralOverviewUniversal: TestAnalyzeScaleToolExtractStructuralOverviewUniversal#
  TestAnalyzeScaleToolExtractStructuralOverviewUniversal.test_extract_universal_none_result: TestAnalyzeScaleToolExtractStructuralOverviewUniversal#test_extract_universal_none_result().
  TestAnalyzeScaleToolExtractStructuralOverviewUniversal.test_extract_universal_no_elements_attr: TestAnalyzeScaleToolExtractStructuralOverviewUniversal#test_extract_universal_no_elements_attr().
  TestAnalyzeScaleToolExtractStructuralOverviewUniversal.test_extract_universal_with_class: TestAnalyzeScaleToolExtractStructuralOverviewUniversal#test_extract_universal_with_class().
  TestAnalyzeScaleToolExtractStructuralOverviewUniversal.test_extract_universal_with_function: TestAnalyzeScaleToolExtractStructuralOverviewUniversal#test_extract_universal_with_function().
  TestAnalyzeScaleToolExtractStructuralOverviewUniversal.test_extract_universal_with_method: TestAnalyzeScaleToolExtractStructuralOverviewUniversal#test_extract_universal_with_method().
  TestAnalyzeScaleToolExtractStructuralOverviewUniversal.test_extract_universal_high_complexity_hotspot: TestAnalyzeScaleToolExtractStructuralOverviewUniversal#test_extract_universal_high_complexity_hotspot().
  TestAnalyzeScaleToolExtractStructuralOverviewUniversal.test_extract_universal_with_variable: TestAnalyzeScaleToolExtractStructuralOverviewUniversal#test_extract_universal_with_variable().
  TestAnalyzeScaleToolExtractStructuralOverviewUniversal.test_extract_universal_with_import: TestAnalyzeScaleToolExtractStructuralOverviewUniversal#test_extract_universal_with_import().
  TestAnalyzeScaleToolExtractStructuralOverviewUniversal.test_extract_universal_unknown_type: TestAnalyzeScaleToolExtractStructuralOverviewUniversal#test_extract_universal_unknown_type().
---
# Module: [`tests/unit/mcp/test_tools/test_analyze_scale_core.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py)

## Classes
### `TestAnalyzeScaleToolCalculateFileMetrics`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_core.py:32`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L32)
- doc: Tests for _calculate_file_metrics method.
- signature: `class TestAnalyzeScaleToolCalculateFileMetrics:`
- members:
  - `test_calculate_file_metrics_error_handling(self, tool)` — [`L52`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L52) — Test error handling in file metrics calculation.
  - `test_calculate_file_metrics_success(self, tool)` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L35) — Test successful file metrics calculation.

### `TestAnalyzeScaleToolCreateJsonFileAnalysis`  ·  implements/extends AnalyzeScaleToolCreateJsonFileAnalysisMixin
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_core.py:349`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L349)
- doc: Tests for _create_json_file_analysis method.
- signature: `class TestAnalyzeScaleToolCreateJsonFileAnalysis(AnalyzeScaleToolCreateJsonFileAnalysisMixin):`
- protocol/private: `__test__`[`L354`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L354)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestAnalyzeScaleToolExecute`  ·  implements/extends AnalyzeScaleToolExecuteMixin
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_core.py:337`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L337)
- doc: Tests for execute method (single mode).
- signature: `class TestAnalyzeScaleToolExecute(AnalyzeScaleToolExecuteMixin):`
- protocol/private: `__test__`[`L340`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L340)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestAnalyzeScaleToolExecuteMetricsBatch`  ·  implements/extends AnalyzeScaleToolExecuteMetricsBatchMixin
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_core.py:343`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L343)
- doc: Tests for _execute_metrics_batch method.
- signature: `class TestAnalyzeScaleToolExecuteMetricsBatch(AnalyzeScaleToolExecuteMetricsBatchMixin):`
- protocol/private: `__test__`[`L346`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L346)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `TestAnalyzeScaleToolExtractStructuralOverview`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_core.py:65`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L65)
- doc: Tests for _extract_structural_overview method.
- signature: `class TestAnalyzeScaleToolExtractStructuralOverview:`
- members:
  - `test_extract_structural_overview_empty(self, tool)` — [`L68`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L68) — Test extraction with empty analysis result.
  - `test_extract_structural_overview_with_classes(self, tool)` — [`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L81) — Test extraction with class elements.
  - `test_extract_structural_overview_with_fields(self, tool)` — [`L163`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L163) — Test extraction with field elements.
  - `test_extract_structural_overview_with_high_complexity_method(self, tool)` — [`L137`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L137) — Test extraction tracks complexity hotspots.
  - `test_extract_structural_overview_with_imports(self, tool)` — [`L187`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L187) — Test extraction with import elements.
  - `test_extract_structural_overview_with_methods(self, tool)` — [`L110`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L110) — Test extraction with method elements.

### `TestAnalyzeScaleToolExtractStructuralOverviewUniversal`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_core.py:357`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L357)
- doc: Tests for _extract_structural_overview_universal method.
- signature: `class TestAnalyzeScaleToolExtractStructuralOverviewUniversal:`
- members:
  - `test_extract_universal_high_complexity_hotspot(self, tool)` — [`L414`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L414) — Test extraction tracks complexity hotspots for universal.
  - `test_extract_universal_no_elements_attr(self, tool)` — [`L366`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L366) — Test with result that has no elements attribute.
  - `test_extract_universal_none_result(self, tool)` — [`L360`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L360) — Test with None analysis result.
  - `test_extract_universal_unknown_type(self, tool)` — [`L454`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L454) — Test element with unknown type is ignored.
  - `test_extract_universal_with_class(self, tool)` — [`L371`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L371) — Test extraction of class element.
  - `test_extract_universal_with_function(self, tool)` — [`L385`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L385) — Test extraction of function element.
  - `test_extract_universal_with_import(self, tool)` — [`L441`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L441) — Test extraction of import element.
  - `test_extract_universal_with_method(self, tool)` — [`L400`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L400) — Test extraction of method element.
  - `test_extract_universal_with_variable(self, tool)` — [`L428`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L428) — Test extraction of variable element.

### `TestAnalyzeScaleToolGenerateLLMGuidance`
- def: [`tests/unit/mcp/test_tools/test_analyze_scale_core.py:209`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L209)
- doc: Tests for _generate_llm_guidance method.
- signature: `class TestAnalyzeScaleToolGenerateLLMGuidance:`
- members:
  - `test_generate_llm_guidance_large_file(self, tool)` — [`L240`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L240) — Test LLM guidance for large file.
  - `test_generate_llm_guidance_many_imports(self, tool)` — [`L323`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L323) — Test LLM guidance identifies many imports.
  - `test_generate_llm_guidance_many_methods(self, tool)` — [`L310`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L310) — Test LLM guidance identifies many methods.
  - `test_generate_llm_guidance_medium_file(self, tool)` — [`L226`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L226) — Test LLM guidance for medium file.
  - `test_generate_llm_guidance_multiple_classes(self, tool)` — [`L297`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L297) — Test LLM guidance identifies multiple classes.
  - `test_generate_llm_guidance_small_file(self, tool)` — [`L212`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L212) — Test LLM guidance for small file.
  - `test_generate_llm_guidance_very_large_file(self, tool)` — [`L254`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L254) — Test LLM guidance for very large file.
  - `test_generate_llm_guidance_with_complexity_hotspots(self, tool)` — [`L268`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L268) — Test LLM guidance includes complexity hotspots.
  - `test_generate_llm_guidance_without_complexity_hotspots(self, tool)` — [`L284`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L284) — Test LLM guidance without complexity hotspots.

## Functions
- `tool()` — [`L21`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L21) — Create an AnalyzeScaleTool instance for testing.
- `tool_with_project_root()` — [`L27`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_tools/test_analyze_scale_core.py#L27) — Create an AnalyzeScaleTool instance with a project root.

