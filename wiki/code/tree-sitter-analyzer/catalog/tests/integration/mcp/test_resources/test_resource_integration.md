---
title: 'Module: tests/integration/mcp/test_resources/test_resource_integration.py'
type: catalog
provenance: extracted
module: tests/integration/mcp/test_resources/test_resource_integration.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.mcp.test_resources.test_resource_integration`/TestResource
symbols:
  TestResourceInteraction.stats_resource: Interaction#stats_resource.
  TestResourceConcurrency.stats_resource: Concurrency#stats_resource.
  TestResourcePerformance.stats_resource: Performance#stats_resource.
  TestResourceInteraction.test_file_and_stats_consistency: Interaction#test_file_and_stats_consistency().
  TestResourceInteraction.test_language_detection_consistency: Interaction#test_language_detection_consistency().
  TestResourcePerformance.test_multiple_file_access_performance: Performance#test_multiple_file_access_performance().
  TestResourceInteraction.project_path: Interaction#project_path.
  TestResourceRegistration.test_resource_uri_uniqueness: Registration#test_resource_uri_uniqueness().
  TestResourceErrorHandling.test_invalid_uri_handling: ErrorHandling#test_invalid_uri_handling().
  TestResourceErrorHandling.test_nonexistent_resource_handling: ErrorHandling#test_nonexistent_resource_handling().
  TestResourcePerformance.project_path: Performance#project_path.
  TestResourceConcurrency.project_path: Concurrency#project_path.
  TestResourceConcurrency.test_concurrent_file_access: Concurrency#test_concurrent_file_access().
  TestResourceErrorHandling.code_resource: ErrorHandling#code_resource.
  TestResourceInteraction.code_resource: Interaction#code_resource.
  TestResourceRegistration.test_code_file_resource_registration: Registration#test_code_file_resource_registration().
  TestResourceRegistration.test_project_stats_resource_registration: Registration#test_project_stats_resource_registration().
  TestResourceInteraction.test_file_count_accuracy: Interaction#test_file_count_accuracy().
  TestResourceErrorHandling.test_permission_error_handling: ErrorHandling#test_permission_error_handling().
  TestResourcePerformance.test_statistics_generation_performance: Performance#test_statistics_generation_performance().
  TestResourceConcurrency.test_concurrent_stats_access: Concurrency#test_concurrent_stats_access().
  TestResourceErrorHandling.stats_resource: ErrorHandling#stats_resource.
  TestResourceInteraction._create_sample_project: Interaction#_create_sample_project().
  TestResourcePerformance.code_resource: Performance#code_resource.
  TestResourcePerformance._create_large_project: Performance#_create_large_project().
  TestResourceConcurrency.code_resource: Concurrency#code_resource.
  TestResourceInteraction.teardown_method: Interaction#teardown_method().
  TestResourcePerformance.teardown_method: Performance#teardown_method().
  TestResourceConcurrency.teardown_method: Concurrency#teardown_method().
  TestResourceInteraction.temp_dir: Interaction#temp_dir.
  TestResourcePerformance.temp_dir: Performance#temp_dir.
  TestResourceConcurrency.temp_dir: Concurrency#temp_dir.
  TestResourceRegistration: Registration#
  TestResourceInteraction: Interaction#
  TestResourceInteraction.setup_method: Interaction#setup_method().
  TestResourceErrorHandling: ErrorHandling#
  TestResourceErrorHandling.setup_method: ErrorHandling#setup_method().
  TestResourcePerformance: Performance#
  TestResourcePerformance.setup_method: Performance#setup_method().
  TestResourceConcurrency: Concurrency#
  TestResourceConcurrency.setup_method: Concurrency#setup_method().
---
# Module: [`tests/integration/mcp/test_resources/test_resource_integration.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py)

## Classes
### `TestResourceConcurrency`
- def: [`tests/integration/mcp/test_resources/test_resource_integration.py:363`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L363)
- doc: Test concurrent access to resources
- signature: `class TestResourceConcurrency:`
- members:
  - `setup_method(self)` — [`L366`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L366) — Set up test fixtures
  - `teardown_method(self)` — [`L379`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L379) — Clean up test fixtures
  - `test_concurrent_file_access(self)` — [`L386`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L386) — Test concurrent access to the same file
  - `test_concurrent_stats_access(self)` — [`L403`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L403) — Test concurrent access to statistics
  - `code_resource` — [`L375`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L375)
  - `project_path` — [`L369`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L369)
  - `stats_resource` — [`L376`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L376)
  - `temp_dir` — [`L368`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L368)
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.read_resource), [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.read_resource), [`set_project_path`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.set_project_path)

### `TestResourceErrorHandling`
- def: [`tests/integration/mcp/test_resources/test_resource_integration.py:188`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L188)
- doc: Test error handling across resources
- signature: `class TestResourceErrorHandling:`
- members:
  - `setup_method(self)` — [`L191`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L191) — Set up test fixtures
  - `test_invalid_uri_handling(self)` — [`L196`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L196) — Test handling of invalid URIs across resources
  - `test_nonexistent_resource_handling(self)` — [`L211`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L211) — Test handling of nonexistent resources
  - `test_permission_error_handling(self, mocker)` — [`L224`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L224) — Test handling of permission errors
  - `code_resource` — [`L193`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L193)
  - `stats_resource` — [`L194`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L194)
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.read_resource), [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.read_resource), [`matches_uri`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.matches_uri), [`matches_uri`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.matches_uri)

### `TestResourceInteraction`
- def: [`tests/integration/mcp/test_resources/test_resource_integration.py:64`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L64)
- doc: Test interaction between different resources
- signature: `class TestResourceInteraction:`
- members:
  - `_create_sample_project(self)` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L87) — Create sample project for testing
  - `setup_method(self)` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L67) — Set up test fixtures
  - `teardown_method(self)` — [`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L81) — Clean up test fixtures
  - `test_file_and_stats_consistency(self)` — [`L122`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L122) — Test consistency between file content and project statistics
  - `test_file_count_accuracy(self)` — [`L171`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L171) — Test accuracy of file count in statistics
  - `test_language_detection_consistency(self)` — [`L148`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L148) — Test consistency of language detection across resources
  - `code_resource` — [`L77`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L77)
  - `project_path` — [`L71`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L71)
  - `stats_resource` — [`L78`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L78)
  - `temp_dir` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L70)
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.read_resource), [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.read_resource), [`set_project_path`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.set_project_path)

### `TestResourcePerformance`
- def: [`tests/integration/mcp/test_resources/test_resource_integration.py:238`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L238)
- doc: Test performance characteristics of resource operations
- signature: `class TestResourcePerformance:`
- members:
  - `_create_large_project(self)` — [`L258`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L258) — Create larger project for performance testing
  - `setup_method(self)` — [`L241`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L241) — Set up test fixtures
  - `teardown_method(self)` — [`L252`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L252) — Clean up test fixtures
  - `test_multiple_file_access_performance(self)` — [`L314`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L314) — Test performance of accessing multiple files
  - `test_statistics_generation_performance(self)` — [`L347`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L347) — Test performance of statistics generation
  - `code_resource` — [`L248`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L248)
  - `project_path` — [`L245`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L245)
  - `stats_resource` — [`L249`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L249)
  - `temp_dir` — [`L244`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L244)
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.read_resource), [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`read_resource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.read_resource), [`set_project_path`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.set_project_path)

### `TestResourceRegistration`
- def: [`tests/integration/mcp/test_resources/test_resource_integration.py:23`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L23)
- doc: Test resource registration and discovery
- signature: `class TestResourceRegistration:`
- members:
  - `test_code_file_resource_registration(self)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L26) — Test code file resource registration
  - `test_project_stats_resource_registration(self)` — [`L36`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L36) — Test project stats resource registration
  - `test_resource_uri_uniqueness(self)` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/mcp/test_resources/test_resource_integration.py#L46) — Test that resource URI patterns don't conflict
- uses (calls/refs, reference-scoped): [`ProjectStatsResource`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource), [`CodeFileResource`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource), [`matches_uri`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.matches_uri), [`matches_uri`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.matches_uri), [`get_resource_info`](../../../../tree_sitter_analyzer/mcp/resources/code_file_resource.md#CodeFileResource.get_resource_info), [`get_resource_info`](../../../../tree_sitter_analyzer/mcp/resources/project_stats_resource.md#ProjectStatsResource.get_resource_info)

