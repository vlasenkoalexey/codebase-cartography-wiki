---
title: 'Module: tests/integration/mcp/test_resources/test_project_stats_resource.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_resources/test_project_stats_resource.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_resources.test_project_stats_resource`/TestProjectStatsResource
symbols:
  TestProjectStatsResourceFunctionality.resource: Functionality#resource.
  TestProjectStatsResourceFunctionality.project_path: Functionality#project_path.
  TestProjectStatsResourceFunctionality.test_overview_stats: Functionality#test_overview_stats().
  TestProjectStatsResourceFunctionality.test_languages_stats: Functionality#test_languages_stats().
  TestProjectStatsResourceFunctionality.test_complexity_stats: Functionality#test_complexity_stats().
  TestProjectStatsResourceFunctionality.test_files_stats: Functionality#test_files_stats().
  TestProjectStatsResourceFunctionality.test_invalid_stats_type: Functionality#test_invalid_stats_type().
  TestProjectStatsResourceFunctionality.test_nonexistent_project_path: Functionality#test_nonexistent_project_path().
  TestProjectStatsResourceIntegration.test_integration_with_universal_analyzer: Integration#test_integration_with_universal_analyzer().
  TestProjectStatsResourceIntegration.test_analyzer_integration_flow: Integration#test_analyzer_integration_flow().
  TestProjectStatsResourceErrorHandling.test_analyzer_error_handling: ErrorHandling#test_analyzer_error_handling().
  TestProjectStatsResourcePerformance.test_caching_behavior: Performance#test_caching_behavior().
  TestProjectStatsResourcePerformance.test_multiple_stats_types_access: Performance#test_multiple_stats_types_access().
  TestProjectStatsResourceSchema.resource: Schema#resource.
  TestProjectStatsResourceIntegration.resource: Integration#resource.
  TestProjectStatsResourceErrorHandling.resource: ErrorHandling#resource.
  TestProjectStatsResourceSchema.test_resource_info_structure: Schema#test_resource_info_structure().
  TestProjectStatsResourceSchema.test_uri_pattern_validation: Schema#test_uri_pattern_validation().
  TestProjectStatsResourceSchema.test_extract_stats_type: Schema#test_extract_stats_type().
  TestProjectStatsResourceFunctionality.test_no_project_path_set: Functionality#test_no_project_path_set().
  TestProjectStatsResourceErrorHandling.test_malformed_uri_handling: ErrorHandling#test_malformed_uri_handling().
  TestProjectStatsResourceErrorHandling.test_invalid_project_path_types: ErrorHandling#test_invalid_project_path_types().
  TestProjectStatsResourcePerformance.resource: Performance#resource.
  TestProjectStatsResourceFunctionality._create_sample_project: Functionality#_create_sample_project().
  TestProjectStatsResourceFunctionality.teardown_method: Functionality#teardown_method().
  TestProjectStatsResourceIntegration.test_integration_with_advanced_analyzer: Integration#test_integration_with_advanced_analyzer().
  TestProjectStatsResourcePerformance.setup_method: Performance#setup_method().
  TestProjectStatsResourceFunctionality.temp_dir: Functionality#temp_dir.
  TestProjectStatsResourceSchema: Schema#
  TestProjectStatsResourceSchema.setup_method: Schema#setup_method().
  TestProjectStatsResourceFunctionality: Functionality#
  TestProjectStatsResourceFunctionality.setup_method: Functionality#setup_method().
  TestProjectStatsResourceIntegration: Integration#
  TestProjectStatsResourceIntegration.setup_method: Integration#setup_method().
  TestProjectStatsResourceErrorHandling: ErrorHandling#
  TestProjectStatsResourceErrorHandling.setup_method: ErrorHandling#setup_method().
  TestProjectStatsResourcePerformance: Performance#
---
# Module: [`tests/integration/mcp/test_resources/test_project_stats_resource.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py)

## Classes
### `TestProjectStatsResourceErrorHandling`
- def: [`tests/integration/mcp/test_resources/test_project_stats_resource.py:359`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L359)
- doc: Test error handling in project statistics resource
- signature: `class TestProjectStatsResourceErrorHandling:`
- members:
  - `setup_method(self)` — [`L362`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L362) — Set up test fixtures
  - `test_analyzer_error_handling(self, mocker)` — [`L380`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L380) — Test handling of analyzer errors
  - `test_invalid_project_path_types(self)` — [`L408`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L408) — Test handling of invalid project path types
  - `test_malformed_uri_handling(self)` — [`L366`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L366) — Test handling of malformed URIs
  - `resource` — [`L364`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L364)
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.read_resource), [`set_project_path`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.set_project_path), [`matches_uri`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.matches_uri)

### `TestProjectStatsResourceFunctionality`
- def: [`tests/integration/mcp/test_resources/test_project_stats_resource.py:84`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L84)
- doc: Test project statistics resource core functionality
- signature: `class TestProjectStatsResourceFunctionality:`
- members:
  - `_create_sample_project(self)` — [`L104`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L104) — Create sample project structure for testing
  - `setup_method(self)` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L87) — Set up test fixtures
  - `teardown_method(self)` — [`L98`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L98) — Clean up test fixtures
  - `test_complexity_stats(self)` — [`L215`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L215) — Test complexity statistics
  - `test_files_stats(self)` — [`L236`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L236) — Test file-level statistics
  - `test_invalid_stats_type(self)` — [`L259`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L259) — Test error handling for invalid statistics type
  - `test_languages_stats(self)` — [`L193`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L193) — Test language-specific statistics
  - `test_no_project_path_set(self)` — [`L269`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L269) — Test error handling when no project path is set
  - `test_nonexistent_project_path(self)` — [`L277`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L277) — Test error handling for nonexistent project path
  - `test_overview_stats(self)` — [`L170`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L170) — Test overview statistics generation
  - `project_path` — [`L93`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L93)
  - `resource` — [`L89`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L89)
  - `temp_dir` — [`L92`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L92)
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.read_resource), [`set_project_path`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.set_project_path)

### `TestProjectStatsResourceIntegration`
- def: [`tests/integration/mcp/test_resources/test_project_stats_resource.py:290`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L290)
- doc: Test integration with existing analyzer components
- signature: `class TestProjectStatsResourceIntegration:`
- members:
  - `setup_method(self)` — [`L293`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L293) — Set up test fixtures
  - `test_analyzer_integration_flow(self, mocker)` — [`L318`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L318) — Test the complete analyzer integration flow
  - `test_integration_with_advanced_analyzer(self)` — [`L309`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L309) — Test integration with AdvancedAnalyzer
  - `test_integration_with_universal_analyzer(self)` — [`L297`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L297) — Test integration with UnifiedAnalysisEngine
  - `resource` — [`L295`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L295)
- uses (calls/refs, reference-scoped): [`get_analysis_engine`](../../../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.read_resource), [`set_project_path`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.set_project_path), [`analysis_engine`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.analysis_engine)

### `TestProjectStatsResourcePerformance`
- def: [`tests/integration/mcp/test_resources/test_project_stats_resource.py:422`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L422)
- doc: Test performance characteristics of project statistics resource
- signature: `class TestProjectStatsResourcePerformance:`
- members:
  - `setup_method(self)` — [`L425`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L425) — Set up test fixtures
  - `test_caching_behavior(self)` — [`L430`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L430) — Test that statistics are cached appropriately
  - `test_multiple_stats_types_access(self)` — [`L467`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L467) — Test accessing multiple statistics types efficiently
  - `resource` — [`L427`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L427)
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.read_resource), [`set_project_path`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.set_project_path)

### `TestProjectStatsResourceSchema`
- def: [`tests/integration/mcp/test_resources/test_project_stats_resource.py:21`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L21)
- doc: Test project statistics resource schema and validation
- signature: `class TestProjectStatsResourceSchema:`
- members:
  - `setup_method(self)` — [`L24`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L24) — Set up test fixtures
  - `test_extract_stats_type(self)` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L70) — Test statistics type extraction from URI
  - `test_resource_info_structure(self)` — [`L28`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L28) — Test that resource info has required structure
  - `test_uri_pattern_validation(self)` — [`L43`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L43) — Test URI pattern validation
  - `resource` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_project_stats_resource.py#L26)
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`matches_uri`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.matches_uri), [`get_resource_info`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.get_resource_info), [`_extract_stats_type`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource._extract_stats_type)

