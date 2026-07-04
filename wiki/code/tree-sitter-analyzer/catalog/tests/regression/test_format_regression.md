---
title: 'Module: tests/regression/test_format_regression.py'
type: catalog
provenance: extracted
module: tests/regression/test_format_regression.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.regression.test_format_regression`/Test
symbols:
  TestFormatRegressionPython.test_python_format_stability: FormatRegressionPython#test_python_format_stability().
  TestFormatRegressionPython.test_python_format_detailed_analysis: FormatRegressionPython#test_python_format_detailed_analysis().
  TestFormatRegressionJava.test_java_format_stability: FormatRegressionJava#test_java_format_stability().
  TestFormatRegressionJava.test_java_format_with_imports: FormatRegressionJava#test_java_format_with_imports().
  TestFormatRegressionJavaScript.test_javascript_format_stability: FormatRegressionJavaScript#test_javascript_format_stability().
  TestFormatRegressionJavaScript.test_javascript_es6_format: FormatRegressionJavaScript#test_javascript_es6_format().
  TestFormatRegressionTypeScript.test_typescript_format_stability: FormatRegressionTypeScript#test_typescript_format_stability().
  TestFormatRegressionCSharp.test_csharp_format_stability: FormatRegressionCSharp#test_csharp_format_stability().
  TestFormatRegressionGo.test_go_format_stability: FormatRegressionGo#test_go_format_stability().
  TestFormatRegressionRust.test_rust_format_stability: FormatRegressionRust#test_rust_format_stability().
  TestFormatRegressionToon.test_toon_format_stability: FormatRegressionToon#test_toon_format_stability().
  TestFormatRegressionToon.test_toon_format_with_details: FormatRegressionToon#test_toon_format_with_details().
  TestFormatRegressionMarkdown.test_markdown_format_stability: FormatRegressionMarkdown#test_markdown_format_stability().
  TestGoldenMasterUpdate.test_create_new_golden_master: GoldenMasterUpdate#test_create_new_golden_master().
  TestGoldenMasterUpdate.test_golden_master_consistency: GoldenMasterUpdate#test_golden_master_consistency().
  TestFormatRegressionPython._get_golden_master: FormatRegressionPython#_get_golden_master().
  TestFormatRegressionPython._compare_with_golden_master: FormatRegressionPython#_compare_with_golden_master().
  TestFormatRegressionPython: FormatRegressionPython#
  TestFormatRegressionJava: FormatRegressionJava#
  TestFormatRegressionJavaScript: FormatRegressionJavaScript#
  TestFormatRegressionTypeScript: FormatRegressionTypeScript#
  TestFormatRegressionCSharp: FormatRegressionCSharp#
  TestFormatRegressionGo: FormatRegressionGo#
  TestFormatRegressionRust: FormatRegressionRust#
  TestFormatRegressionToon: FormatRegressionToon#
  TestFormatRegressionMarkdown: FormatRegressionMarkdown#
  TestGoldenMasterUpdate: GoldenMasterUpdate#
  TestGoldenMasterUpdate.test_update_golden_master_python: GoldenMasterUpdate#test_update_golden_master_python().
---
# Module: [`tests/regression/test_format_regression.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py)

## Classes
### `TestFormatRegressionCSharp`
- def: [`tests/regression/test_format_regression.py:295`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L295)
- doc: C#格式稳定性测试
- signature: `class TestFormatRegressionCSharp:`
- members:
  - `test_csharp_format_stability(self, tmp_path)` — [`L299`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L299) — 测试C#格式稳定性
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)

### `TestFormatRegressionGo`
- def: [`tests/regression/test_format_regression.py:339`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L339)
- doc: Go格式稳定性测试
- signature: `class TestFormatRegressionGo:`
- members:
  - `test_go_format_stability(self, tmp_path)` — [`L343`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L343) — 测试Go格式稳定性
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)

### `TestFormatRegressionJava`
- def: [`tests/regression/test_format_regression.py:107`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L107)
- doc: Java格式稳定性测试
- signature: `class TestFormatRegressionJava:`
- members:
  - `test_java_format_stability(self, tmp_path)` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L111) — 测试Java格式稳定性
  - `test_java_format_with_imports(self, tmp_path)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L146) — 测试带导入的Java格式
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)

### `TestFormatRegressionJavaScript`
- def: [`tests/regression/test_format_regression.py:179`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L179)
- doc: JavaScript格式稳定性测试
- signature: `class TestFormatRegressionJavaScript:`
- members:
  - `test_javascript_es6_format(self, tmp_path)` — [`L220`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L220) — 测试ES6格式
  - `test_javascript_format_stability(self, tmp_path)` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L183) — 测试JavaScript格式稳定性
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)

### `TestFormatRegressionMarkdown`
- def: [`tests/regression/test_format_regression.py:486`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L486)
- doc: Markdown格式稳定性测试
- signature: `class TestFormatRegressionMarkdown:`
- members:
  - `test_markdown_format_stability(self, tmp_path)` — [`L490`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L490) — 测试Markdown格式稳定性
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)

### `TestFormatRegressionPython`
- def: [`tests/regression/test_format_regression.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L15)
- doc: Python格式稳定性测试
- signature: `class TestFormatRegressionPython:`
- members:
  - `_compare_with_golden_master(self, result: dict[str, Any], golden: dict[str, Any])` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L66) — 与Golden Master比较
  - `_get_golden_master(self, language: str, filename: str)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L56) — 获取Golden Master数据
  - `test_python_format_detailed_analysis(self, tmp_path)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L75) — 测试Python详细分析格式
  - `test_python_format_stability(self, tmp_path)` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L19) — 测试Python格式稳定性
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)

### `TestFormatRegressionRust`
- def: [`tests/regression/test_format_regression.py:382`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L382)
- doc: Rust格式稳定性测试
- signature: `class TestFormatRegressionRust:`
- members:
  - `test_rust_format_stability(self, tmp_path)` — [`L386`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L386) — 测试Rust格式稳定性
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)

### `TestFormatRegressionToon`
- def: [`tests/regression/test_format_regression.py:428`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L428)
- doc: Toon格式稳定性测试
- signature: `class TestFormatRegressionToon:`
- members:
  - `test_toon_format_stability(self, tmp_path)` — [`L432`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L432) — 测试Toon格式稳定性
  - `test_toon_format_with_details(self, tmp_path)` — [`L459`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L459) — 测试Toon格式带详细信息
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)

### `TestFormatRegressionTypeScript`
- def: [`tests/regression/test_format_regression.py:253`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L253)
- doc: TypeScript格式稳定性测试
- signature: `class TestFormatRegressionTypeScript:`
- members:
  - `test_typescript_format_stability(self, tmp_path)` — [`L257`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L257) — 测试TypeScript格式稳定性
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)

### `TestGoldenMasterUpdate`
- def: [`tests/regression/test_format_regression.py:535`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L535)
- doc: Golden Master自动更新机制测试
- signature: `class TestGoldenMasterUpdate:`
- members:
  - `test_create_new_golden_master(self, tmp_path)` — [`L560`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L560) — 测试创建新的Golden Master
  - `test_golden_master_consistency(self, tmp_path)` — [`L590`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L590) — 测试Golden Master一致性
  - `test_update_golden_master_python(self, tmp_path, monkeypatch)` — [`L539`](../../../../../../raw/code/tree-sitter-analyzer/tests/regression/test_format_regression.py#L539) — 测试Python Golden Master更新
- uses (calls/refs, reference-scoped): [`UnifiedAnalysisEngine`](../../tree_sitter_analyzer/core/analysis_engine.md#UnifiedAnalysisEngine), [`analyze_file`](../../tree_sitter_analyzer/core/_analysis_engine_file_mixin.md#UnifiedAnalysisEngineFileMixin.analyze_file)

