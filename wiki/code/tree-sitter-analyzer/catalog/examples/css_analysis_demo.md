---
title: 'Module: examples/css_analysis_demo.py'
type: catalog
provenance: extracted
module: examples/css_analysis_demo.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `examples.css_analysis_demo`/
symbols:
  CssAnalysisDemo.run_demo: CssAnalysisDemo#run_demo().
  CssAnalysisDemo.initialize: CssAnalysisDemo#initialize().
  CssAnalysisDemo.analyze_css_structure: CssAnalysisDemo#analyze_css_structure().
  main: main().
  CssAnalysisDemo.sample_file: CssAnalysisDemo#sample_file.
  CssAnalysisDemo.check_sample_file: CssAnalysisDemo#check_sample_file().
  e: e.
  CssAnalysisDemo.css_plugin: CssAnalysisDemo#css_plugin.
  CssAnalysisDemo.engine: CssAnalysisDemo#engine.
  CssAnalysisDemo: CssAnalysisDemo#
  CssAnalysisDemo.analyze_selectors: CssAnalysisDemo#analyze_selectors().
  CssAnalysisDemo.analyze_properties: CssAnalysisDemo#analyze_properties().
  CssAnalysisDemo.analyze_css_variables: CssAnalysisDemo#analyze_css_variables().
  CssAnalysisDemo.analyze_media_queries: CssAnalysisDemo#analyze_media_queries().
  CssAnalysisDemo.analyze_at_rules: CssAnalysisDemo#analyze_at_rules().
  CssAnalysisDemo.__init__: CssAnalysisDemo#__init__().
---
# Module: [`examples/css_analysis_demo.py`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py)

## Classes
### `CssAnalysisDemo`
- def: [`examples/css_analysis_demo.py:25`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L25)
- doc: CSS解析デモクラス
- signature: `class CssAnalysisDemo:`
- members:
  - `analyze_at_rules(self, elements: list[dict[str, Any]])` — [`L356`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L356) — @ルールの分析
  - `analyze_css_structure(self)` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L47) — CSS構造の解析
  - `analyze_css_variables(self, elements: list[dict[str, Any]])` — [`L224`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L224) — CSS変数（カスタムプロパティ）の分析
  - `analyze_media_queries(self, elements: list[dict[str, Any]])` — [`L290`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L290) — メディアクエリの分析
  - `analyze_properties(self, elements: list[dict[str, Any]])` — [`L144`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L144) — プロパティの分析
  - `analyze_selectors(self, elements: list[dict[str, Any]])` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L71) — セレクタの分析
  - `check_sample_file(self)` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L39) — サンプルファイルの存在確認
  - `initialize(self)` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L33) — 解析エンジンの初期化
  - `run_demo(self)` — [`L394`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L394) — デモの実行
  - `css_plugin` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L30)
  - `engine` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L29)
  - `sample_file` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L31)
- protocol/private: `__init__`[`L28`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L28)
- uses (calls/refs, reference-scoped): [`get_analysis_engine`](../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`CssPlugin`](../tree_sitter_analyzer/languages/css_plugin.md#CssPlugin)
- used by: (1 test-only callers)

## Functions
- `main()` — [`L428`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L428) — メイン関数

## Module values
- `e` — [`L18`](../../../../../raw/code/tree-sitter-analyzer/examples/css_analysis_demo.py#L18)

