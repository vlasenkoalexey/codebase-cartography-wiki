---
title: 'Module: scripts/grammar_structural_analysis.py'
type: catalog
provenance: extracted
module: scripts/grammar_structural_analysis.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.grammar_structural_analysis`/
symbols:
  main: main().
  analyze_node_structure.traverse: analyze_node_structure().traverse().
  analyze_node_structure: analyze_node_structure().
  identify_wrapper_nodes_structural: identify_wrapper_nodes_structural().
---
# Module: [`scripts/grammar_structural_analysis.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_structural_analysis.py)

## Functions
- `analyze_node_structure(lang: tree_sitter.Language, code_samples: list[str])` — [`L16`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_structural_analysis.py#L16) — 分析多个代码样本中的 node 结构特征
- `identify_wrapper_nodes_structural(node_stats: dict[str, dict[str, Any]])` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_structural_analysis.py#L89) — 基于结构特征识别 wrapper nodes
- `main()` — [`L161`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_structural_analysis.py#L161) — 运行结构化分析
- `traverse(node: tree_sitter.Node, parent_type: str | None = None)` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_structural_analysis.py#L42)

