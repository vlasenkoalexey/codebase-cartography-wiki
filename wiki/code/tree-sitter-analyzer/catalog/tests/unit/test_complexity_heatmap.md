---
title: 'Module: tests/unit/test_complexity_heatmap.py'
type: catalog
provenance: extracted
module: tests/unit/test_complexity_heatmap.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_complexity_heatmap`/
symbols:
  TestComplexityHeatmapTool._make_tool: TestComplexityHeatmapTool#_make_tool().
  TestCacheBackedComplexity.test_cache_backed_analyze: TestCacheBackedComplexity#test_cache_backed_analyze().
  TestComplexityEngine.test_class_method_detection: TestComplexityEngine#test_class_method_detection().
  indexed_complex_project: indexed_complex_project().
  TestComplexityEngine.test_analyze_complex_file: TestComplexityEngine#test_analyze_complex_file().
  TestComplexityEngine.test_javascript_complexity: TestComplexityEngine#test_javascript_complexity().
  TestComplexityEngine.test_decision_points_populated: TestComplexityEngine#test_decision_points_populated().
  TestCacheBackedComplexity.test_project_heatmap_with_cache: TestCacheBackedComplexity#test_project_heatmap_with_cache().
  TestPluginFallbackLanguages.test_csharp_file_complexity: TestPluginFallbackLanguages#test_csharp_file_complexity().
  TestComplexityEngine.test_analyze_simple_file: TestComplexityEngine#test_analyze_simple_file().
  TestCacheBackedComplexity.test_cache_backed_fallback: TestCacheBackedComplexity#test_cache_backed_fallback().
  TestComplexityHeatmapTool.test_project_mode: TestComplexityHeatmapTool#test_project_mode().
  TestComplexityHeatmapTool.test_project_mode_string_max_files: TestComplexityHeatmapTool#test_project_mode_string_max_files().
  TestComplexityHeatmapTool.test_file_mode: TestComplexityHeatmapTool#test_file_mode().
  TestComplexityHeatmapTool.test_function_mode: TestComplexityHeatmapTool#test_function_mode().
  TestComplexityHeatmapTool.test_function_not_found: TestComplexityHeatmapTool#test_function_not_found().
  TestComplexityHeatmapTool.test_file_not_found: TestComplexityHeatmapTool#test_file_not_found().
  TestComplexityHeatmapTool.test_project_with_cache: TestComplexityHeatmapTool#test_project_with_cache().
  TestComplexityHeatmapTool.test_language_filter: TestComplexityHeatmapTool#test_language_filter().
  TestComplexityHeatmapTool.test_validate_bad_mode: TestComplexityHeatmapTool#test_validate_bad_mode().
  TestComplexityHeatmapTool.test_validate_file_mode_no_path: TestComplexityHeatmapTool#test_validate_file_mode_no_path().
  TestComplexityHeatmapTool.test_tool_definition: TestComplexityHeatmapTool#test_tool_definition().
  TestPluginFallbackLanguages.test_ruby_file_complexity: TestPluginFallbackLanguages#test_ruby_file_complexity().
  TestComplexityEngine.test_empty_file: TestComplexityEngine#test_empty_file().
  TestComplexityEngine.test_risk_bands: TestComplexityEngine#test_risk_bands().
  TestComplexityEngine.test_project_heatmap: TestComplexityEngine#test_project_heatmap().
  TestComplexityEngine.test_project_heatmap_language_filter: TestComplexityEngine#test_project_heatmap_language_filter().
  TestComplexityEngine.test_project_heatmap_directory_filter: TestComplexityEngine#test_project_heatmap_directory_filter().
  TestComplexityCLI.test_cli_project_mode: TestComplexityCLI#test_cli_project_mode().
  TestComplexityCLI.test_cli_file_mode: TestComplexityCLI#test_cli_file_mode().
  TestComplexityCLI.test_cli_function_mode: TestComplexityCLI#test_cli_function_mode().
  csharp_project: csharp_project().
  ruby_project: ruby_project().
  TestPluginFallbackLanguages.test_csharp_project_heatmap: TestPluginFallbackLanguages#test_csharp_project_heatmap().
  TestPluginFallbackLanguages.test_ruby_project_heatmap: TestPluginFallbackLanguages#test_ruby_project_heatmap().
  TestPluginFallbackLanguages.test_empty_project_warns: TestPluginFallbackLanguages#test_empty_project_warns().
  TestCacheBackedComplexity.test_cache_backed_fallback.FakeCache: TestCacheBackedComplexity#test_cache_backed_fallback().FakeCache#
  _CSHARP_FIXTURE: _CSHARP_FIXTURE.
  _RUBY_FIXTURE: _RUBY_FIXTURE.
  complex_project: complex_project().
  TestComplexityEngine: TestComplexityEngine#
  TestCacheBackedComplexity: TestCacheBackedComplexity#
  TestCacheBackedComplexity.test_cache_backed_fallback.FakeCache.lookup: TestCacheBackedComplexity#test_cache_backed_fallback().FakeCache#lookup().
  TestComplexityHeatmapTool: TestComplexityHeatmapTool#
  TestComplexityCLI: TestComplexityCLI#
  TestPluginFallbackLanguages: TestPluginFallbackLanguages#
---
# Module: [`tests/unit/test_complexity_heatmap.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py)

## Classes
### `FakeCache`
- def: [`tests/unit/test_complexity_heatmap.py:189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L189)
- signature: `class FakeCache:`
- members:
  - `lookup(self, fp)` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L190)
- used by: (1 test-only callers)

### `TestCacheBackedComplexity`
- def: [`tests/unit/test_complexity_heatmap.py:167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L167)
- signature: `class TestCacheBackedComplexity:`
- members:
  - `test_cache_backed_analyze(self, indexed_complex_project)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L168)
  - `test_cache_backed_fallback(self, complex_project)` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L184)
  - `test_project_heatmap_with_cache(self, indexed_complex_project)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L198)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`analyze_project_heatmap`](../../tree_sitter_analyzer/complexity_heatmap.md#analyze_project_heatmap), [`analyze_file_complexity_from_cache`](../../tree_sitter_analyzer/complexity_heatmap.md#analyze_file_complexity_from_cache), [`complexity`](../../tree_sitter_analyzer/complexity_heatmap.md#FunctionComplexity.complexity), [`name`](../../tree_sitter_analyzer/complexity_heatmap.md#FunctionComplexity.name)  (1 test-only)

### `TestComplexityCLI`
- def: [`tests/unit/test_complexity_heatmap.py:345`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L345)
- signature: `class TestComplexityCLI:`
- members:
  - `test_cli_file_mode(self, complex_project, monkeypatch)` — [`L380`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L380)
  - `test_cli_function_mode(self, complex_project, monkeypatch)` — [`L415`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L415)
  - `test_cli_project_mode(self, indexed_complex_project, monkeypatch)` — [`L346`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L346)
- uses (calls/refs, reference-scoped): [`main`](../../tree_sitter_analyzer/cli_main.md#main)

### `TestComplexityEngine`
- def: [`tests/unit/test_complexity_heatmap.py:76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L76)
- signature: `class TestComplexityEngine:`
- members:
  - `test_analyze_complex_file(self, complex_project)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L84)
  - `test_analyze_simple_file(self, complex_project)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L77)
  - `test_class_method_detection(self, complex_project)` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L93)
  - `test_decision_points_populated(self, complex_project)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L158)
  - `test_empty_file(self, complex_project)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L102)
  - `test_javascript_complexity(self, complex_project)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L108)
  - `test_project_heatmap(self, complex_project)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L129)
  - `test_project_heatmap_directory_filter(self, complex_project)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L152)
  - `test_project_heatmap_language_filter(self, complex_project)` — [`L143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L143)
  - `test_risk_bands(self)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L117)
- uses (calls/refs, reference-scoped): [`analyze_project_heatmap`](../../tree_sitter_analyzer/complexity_heatmap.md#analyze_project_heatmap), [`analyze_file_complexity`](../../tree_sitter_analyzer/complexity_heatmap.md#analyze_file_complexity), [`complexity`](../../tree_sitter_analyzer/complexity_heatmap.md#FunctionComplexity.complexity), [`_risk_band`](../../tree_sitter_analyzer/complexity_heatmap.md#_risk_band), [`name`](../../tree_sitter_analyzer/complexity_heatmap.md#FunctionComplexity.name), [`decision_points`](../../tree_sitter_analyzer/complexity_heatmap.md#FunctionComplexity.decision_points), [`class_name`](../../tree_sitter_analyzer/complexity_heatmap.md#FunctionComplexity.class_name)

### `TestComplexityHeatmapTool`
- def: [`tests/unit/test_complexity_heatmap.py:209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L209)
- signature: `class TestComplexityHeatmapTool:`
- members:
  - `test_file_mode(self, complex_project)` — [`L247`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L247)
  - `test_file_not_found(self, complex_project)` — [`L296`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L296)
  - `test_function_mode(self, complex_project)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L265)
  - `test_function_not_found(self, complex_project)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L282)
  - `test_language_filter(self, complex_project)` — [`L317`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L317)
  - `test_project_mode(self, complex_project)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L218)
  - `test_project_mode_string_max_files(self, complex_project)` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L229) — Project mode must coerce a string ``max_files`` to int.
  - `test_project_with_cache(self, indexed_complex_project)` — [`L309`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L309)
  - `test_tool_definition(self, complex_project)` — [`L338`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L338)
  - `test_validate_bad_mode(self, complex_project)` — [`L328`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L328)
  - `test_validate_file_mode_no_path(self, complex_project)` — [`L333`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L333)
- protocol/private: `_make_tool`[`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L210)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.md#CodeGraphComplexityHeatmapTool.execute), [`CodeGraphComplexityHeatmapTool`](../../tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.md#CodeGraphComplexityHeatmapTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.md#CodeGraphComplexityHeatmapTool.validate_arguments), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/complexity_heatmap_tool.md#CodeGraphComplexityHeatmapTool.get_tool_definition)

### `TestPluginFallbackLanguages`
- def: [`tests/unit/test_complexity_heatmap.py:496`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L496)
- doc: Verify that languages absent from _METHOD_NODES get correct results
- signature: `class TestPluginFallbackLanguages:`
- members:
  - `test_csharp_file_complexity(self, csharp_project)` — [`L500`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L500)
  - `test_csharp_project_heatmap(self, csharp_project)` — [`L520`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L520)
  - `test_empty_project_warns(self, tmp_path)` — [`L536`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L536) — When a project yields 0 functions, result must carry a note/warning.
  - `test_ruby_file_complexity(self, ruby_project)` — [`L511`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L511)
  - `test_ruby_project_heatmap(self, ruby_project)` — [`L528`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L528)
- uses (calls/refs, reference-scoped): [`analyze_project_heatmap`](../../tree_sitter_analyzer/complexity_heatmap.md#analyze_project_heatmap), [`analyze_file_complexity`](../../tree_sitter_analyzer/complexity_heatmap.md#analyze_file_complexity), [`complexity`](../../tree_sitter_analyzer/complexity_heatmap.md#FunctionComplexity.complexity), [`name`](../../tree_sitter_analyzer/complexity_heatmap.md#FunctionComplexity.name)

## Functions
- `complex_project(tmp_path)` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L12)
- `csharp_project(tmp_path)` — [`L481`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L481)
- `indexed_complex_project(complex_project)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L66)
- `ruby_project(tmp_path)` — [`L489`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L489)

## Module values
- `_CSHARP_FIXTURE` — [`L453`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L453)
- `_RUBY_FIXTURE` — [`L465`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_complexity_heatmap.py#L465)

