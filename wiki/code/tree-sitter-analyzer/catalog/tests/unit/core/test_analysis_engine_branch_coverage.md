---
title: 'Module: tests/unit/core/test_analysis_engine_branch_coverage.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_analysis_engine_branch_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_analysis_engine_branch_coverage`/
symbols:
  TestAnalyzeFileCoverage.test_analyze_file_with_request_and_params: TestAnalyzeFileCoverage#test_analyze_file_with_request_and_params().
  TestAnalyzeCodeCoverage.test_analyze_code_with_request_and_explicit_language: TestAnalyzeCodeCoverage#test_analyze_code_with_request_and_explicit_language().
  TestCacheKeyCoverage.test_cache_key_os_error_handled: TestCacheKeyCoverage#test_cache_key_os_error_handled().
  TestDetectLanguageCoverage.test_detect_language_exception_returns_unknown: TestDetectLanguageCoverage#test_detect_language_exception_returns_unknown().
  TestCleanupCoverage.test_cleanup_with_initialized_components: TestCleanupCoverage#test_cleanup_with_initialized_components().
  reset_engine_instances: reset_engine_instances().
  TestCleanupCoverage: TestCleanupCoverage#
  TestCacheKeyCoverage: TestCacheKeyCoverage#
  TestDetectLanguageCoverage: TestDetectLanguageCoverage#
  TestAnalyzeCodeCoverage: TestAnalyzeCodeCoverage#
  TestAnalyzeFileCoverage: TestAnalyzeFileCoverage#
---
# Module: [`tests/unit/core/test_analysis_engine_branch_coverage.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py)

## Classes
### `TestAnalyzeCodeCoverage`
- def: [`tests/unit/core/test_analysis_engine_branch_coverage.py:65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L65)
- doc: Hit alternate language path in analyze_code (lines 271-272)
- signature: `class TestAnalyzeCodeCoverage:`
- members:
  - `test_analyze_code_with_request_and_explicit_language(self)` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L69) — analyze_code with request + explicit language sets language on request (lines 271-272)
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`analyze_code`](../../../tree_sitter_analyzer/core/_analysis_engine_code_mixin.md#UnifiedAnalysisEngineCodeMixin.analyze_code)

### `TestAnalyzeFileCoverage`
- def: [`tests/unit/core/test_analysis_engine_branch_coverage.py:81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L81)
- doc: Hit update-request path in analyze_file (lines 229-242)
- signature: `class TestAnalyzeFileCoverage:`
- members:
  - `test_analyze_file_with_request_and_params(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L85) — analyze_file with existing request + params should update request fields (lines 229-242)
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`include_complexity`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details), [`analyze_file`](../../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file), [`format_type`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.format_type)

### `TestCacheKeyCoverage`
- def: [`tests/unit/core/test_analysis_engine_branch_coverage.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L33)
- doc: Hit exception paths in _generate_cache_key (lines 372-373)
- signature: `class TestCacheKeyCoverage:`
- members:
  - `test_cache_key_os_error_handled(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L36) — _generate_cache_key should handle OSError from stat (lines 372-373)
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`get_analysis_engine`](../../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`_generate_cache_key`](../../../tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin._generate_cache_key)

### `TestCleanupCoverage`
- def: [`tests/unit/core/test_analysis_engine_branch_coverage.py:23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L23)
- doc: Hit cleanup paths that require _ensure_initialized first (lines 402-404)
- signature: `class TestCleanupCoverage:`
- members:
  - `test_cleanup_with_initialized_components(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L26) — cleanup should clear cache and performance monitor when initialized
- uses (calls/refs, reference-scoped): [`get_analysis_engine`](../../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`_ensure_initialized`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine._ensure_initialized), [`cleanup`](../../../tree_sitter_analyzer/core/_analysis_engine_runtime_mixin.md#UnifiedAnalysisEngineRuntimeMixin.cleanup)

### `TestDetectLanguageCoverage`
- def: [`tests/unit/core/test_analysis_engine_branch_coverage.py:51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L51)
- doc: Hit exception path in _detect_language (lines 381-382)
- signature: `class TestDetectLanguageCoverage:`
- members:
  - `test_detect_language_exception_returns_unknown(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L54) — _detect_language returns 'unknown' on exception (lines 381-382)
- uses (calls/refs, reference-scoped): [`get_analysis_engine`](../../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`_ensure_initialized`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine._ensure_initialized), [`_detect_language`](../../../tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin._detect_language), [`_language_detector`](../../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine._language_detector)

## Functions
- `reset_engine_instances()` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_engine_branch_coverage.py#L16) — Reset singleton state before each test.

