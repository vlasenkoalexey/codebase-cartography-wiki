---
title: 'Module: examples/html_analysis_demo.py'
type: catalog
provenance: extracted
module: examples/html_analysis_demo.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `examples.html_analysis_demo`/
symbols:
  HtmlAnalysisDemo.run_demo: HtmlAnalysisDemo#run_demo().
  HtmlAnalysisDemo.initialize: HtmlAnalysisDemo#initialize().
  HtmlAnalysisDemo.analyze_html_structure: HtmlAnalysisDemo#analyze_html_structure().
  main: main().
  HtmlAnalysisDemo.sample_file: HtmlAnalysisDemo#sample_file.
  HtmlAnalysisDemo.formatter: HtmlAnalysisDemo#formatter.
  HtmlAnalysisDemo.check_sample_file: HtmlAnalysisDemo#check_sample_file().
  HtmlAnalysisDemo.demonstrate_html_formatter: HtmlAnalysisDemo#demonstrate_html_formatter().
  e: e.
  HtmlAnalysisDemo.html_plugin: HtmlAnalysisDemo#html_plugin.
  HtmlAnalysisDemo.engine: HtmlAnalysisDemo#engine.
  HtmlAnalysisDemo: HtmlAnalysisDemo#
  HtmlAnalysisDemo.analyze_element_classification: HtmlAnalysisDemo#analyze_element_classification().
  HtmlAnalysisDemo.analyze_hierarchy: HtmlAnalysisDemo#analyze_hierarchy().
  HtmlAnalysisDemo.analyze_attributes: HtmlAnalysisDemo#analyze_attributes().
  HtmlAnalysisDemo.__init__: HtmlAnalysisDemo#__init__().
---
# Module: [`examples/html_analysis_demo.py`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py)

## Classes
### `HtmlAnalysisDemo`
- def: [`examples/html_analysis_demo.py:25`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L25)
- doc: HTML解析デモクラス
- signature: `class HtmlAnalysisDemo:`
- members:
  - `analyze_attributes(self, elements: list[dict[str, Any]])` — [`L154`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L154) — 属性の分析
  - `analyze_element_classification(self, elements: list[dict[str, Any]])` — [`L72`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L72) — 要素分類の分析
  - `analyze_hierarchy(self, elements: list[dict[str, Any]])` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L111) — 階層構造の分析
  - `analyze_html_structure(self)` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L48) — HTML構造の解析
  - `check_sample_file(self)` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L40) — サンプルファイルの存在確認
  - `demonstrate_html_formatter(self, analysis_result: dict[str, Any])` — [`L196`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L196) — HTMLフォーマッターのデモンストレーション
  - `initialize(self)` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L34) — 解析エンジンの初期化
  - `run_demo(self)` — [`L218`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L218) — デモの実行
  - `engine` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L29)
  - `formatter` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L31)
  - `html_plugin` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L30)
  - `sample_file` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L32)
- protocol/private: `__init__`[`L28`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L28)
- uses (calls/refs, reference-scoped): [`HtmlPlugin`](../tree_sitter_analyzer/languages/html_plugin.md#HtmlPlugin), [`get_analysis_engine`](../tree_sitter_analyzer/core/analysis_engine.md#get_analysis_engine), [`HtmlFormatter`](../tree_sitter_analyzer/formatters/html_formatter.md#HtmlFormatter)
- used by: (1 test-only callers)

## Functions
- `main()` — [`L251`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L251) — メイン関数

## Module values
- `e` — [`L18`](../../../../../raw/code/tree-sitter-analyzer/examples/html_analysis_demo.py#L18)

