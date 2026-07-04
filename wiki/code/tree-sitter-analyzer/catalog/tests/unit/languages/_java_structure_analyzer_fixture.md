---
title: 'Module: tests/unit/languages/_java_structure_analyzer_fixture.py'
type: catalog
provenance: extracted
module: tests/unit/languages/_java_structure_analyzer_fixture.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages._java_structure_analyzer_fixture`/
symbols:
  StructureAnalyzerAdapter._analyze: StructureAnalyzerAdapter#_analyze().
  _build_legacy_structure_result: _build_legacy_structure_result().
  StructureAnalyzerAdapter.analyze_structure: StructureAnalyzerAdapter#analyze_structure().
  _elements_by_type: _elements_by_type().
  create_structure_analyzer_adapter: create_structure_analyzer_adapter().
  _run_async_analysis: _run_async_analysis().
  _class_info: _class_info().
  _method_info: _method_info().
  _field_info: _field_info().
  _annotation_infos: _annotation_infos().
  StructureAnalyzerAdapter.__init__: StructureAnalyzerAdapter#__init__().
  StructureAnalyzerAdapter.engine: StructureAnalyzerAdapter#engine.
  _run_async_analysis.run_in_thread: _run_async_analysis().run_in_thread().
  _package_info: _package_info().
  _import_info: _import_info().
  StructureAnalyzerAdapter: StructureAnalyzerAdapter#
---
# Module: [`tests/unit/languages/_java_structure_analyzer_fixture.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py)

## Classes
### `StructureAnalyzerAdapter`
- def: [`tests/unit/languages/_java_structure_analyzer_fixture.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L19)
- members:
  - `analyze_structure(self, file_path: str)` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L25) — Legacy analyze_structure method using unified analysis engine.
  - `engine` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L23)
- protocol/private: `__init__`[`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L22), `_analyze`[`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L28)
- uses (calls/refs, reference-scoped): [`AnalysisRequest`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest), [`file_path`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.file_path), [`language`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.language), [`get_analysis_engine`](../../../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`analyze`](../../../tree_sitter_analyzer/core/_analysis_engine_analysis_mixin.md#UnifiedAnalysisEngineAnalysisMixin.analyze), [`include_complexity`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_complexity), [`include_details`](../../../tree_sitter_analyzer/core/request.md#AnalysisRequest.include_details)  (2 test-only)
- used by: (1 test-only callers)

## Functions
- `_annotation_infos(annotations: list)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L244)
- `_build_legacy_structure_result(result)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L67)
- `_class_info(class_element)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L146)
- `_elements_by_type(elements, element_type: str)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L114)
- `_field_info(field_element)` — [`L210`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L210)
- `_import_info(import_element)` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L231)
- `_method_info(method_element)` — [`L176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L176)
- `_package_info(packages: list, source_code: str | None)` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L122)
- `_run_async_analysis(analyze_coroutine)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L50) — Run async analysis in an isolated thread to avoid event-loop collisions.
- `create_structure_analyzer_adapter()` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L14) — Create the legacy-compatible structure analyzer used by tests.
- `run_in_thread()` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_java_structure_analyzer_fixture.py#L53)

