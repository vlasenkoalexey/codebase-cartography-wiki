---
title: 'Module: tree_sitter_analyzer/core/_analysis_engine_code_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/_analysis_engine_code_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core._analysis_engine_code_mixin`/
symbols:
  UnifiedAnalysisEngineCodeMixin.analyze_code: UnifiedAnalysisEngineCodeMixin#analyze_code().
  _clone_request_for_temp_path: _clone_request_for_temp_path().
  _prepare_code_request: _prepare_code_request().
  UnifiedAnalysisEngineCodeMixin.analyze_code_sync: UnifiedAnalysisEngineCodeMixin#analyze_code_sync().
  UnifiedAnalysisEngineCodeMixin: UnifiedAnalysisEngineCodeMixin#
  _write_temp_source: _write_temp_source().
---
# Module: [`tree_sitter_analyzer/core/_analysis_engine_code_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_code_mixin.py)

## Classes
### `UnifiedAnalysisEngineCodeMixin`
- def: [`tree_sitter_analyzer/core/_analysis_engine_code_mixin.py:11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_code_mixin.py#L11)
- doc: Compatibility code-analysis methods.
- signature: `class UnifiedAnalysisEngineCodeMixin:`
- members:
  - `analyze_code(self, code: str, language: str | None = None, filename: str = "string", request: AnalysisRequest | None = None)` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_code_mixin.py#L14) — Analyze source code string directly
  - `analyze_code_sync(self, code: str, language: str, filename: str = "string", request: AnalysisRequest | None = None)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_code_mixin.py#L36) — Sync version of analyze_code
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](request.md#AnalysisRequest), [`UnifiedAnalysisEngine`](analysis_engine.md#UnifiedAnalysisEngine), [`_clone_request_for_temp_path`](_analysis_engine_code_mixin.md#_clone_request_for_temp_path), [`_prepare_code_request`](_analysis_engine_code_mixin.md#_prepare_code_request), [`_write_temp_source`](_analysis_engine_code_mixin.md#_write_temp_source)
- used by: [`UnifiedAnalysisEngine`](analysis_engine.md#UnifiedAnalysisEngine), [`analyze_code`](../api.md#analyze_code)  (15 test-only)

## Functions
- `_clone_request_for_temp_path(request: AnalysisRequest, temp_path: str)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_code_mixin.py#L79)
- `_prepare_code_request(request: AnalysisRequest | None, filename: str, actual_language: str, explicit_language: str | None)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_code_mixin.py#L58)
- `_write_temp_source(code: str, language: str)` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/_analysis_engine_code_mixin.py#L71)

