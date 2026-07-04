---
title: 'Module: evaluation/analyze_and_plot_mcp_efficiency.py'
type: catalog
provenance: extracted
module: evaluation/analyze_and_plot_mcp_efficiency.py
status: fresh
symbol_base: scip-python python claude-context 0.0.0 `evaluation.analyze_and_plot_mcp_efficiency`/
symbols:
  main: main().
  load_method_results: load_method_results().
  calculate_metrics: calculate_metrics().
  normalize_file_path: normalize_file_path().
  create_efficiency_chart: create_efficiency_chart().
---
# Module: [`evaluation/analyze_and_plot_mcp_efficiency.py`](../../../../../raw/code/claude-context/evaluation/analyze_and_plot_mcp_efficiency.py)

## Functions
- `calculate_metrics(hits: List[str], oracles: List[str])` — [`L23`](../../../../../raw/code/claude-context/evaluation/analyze_and_plot_mcp_efficiency.py#L23) — Calculate precision, recall, and F1-score.
- `create_efficiency_chart(both_results: Dict, grep_results: Dict)` — [`L136`](../../../../../raw/code/claude-context/evaluation/analyze_and_plot_mcp_efficiency.py#L136) — Create the efficiency comparison chart using Seaborn.
- `load_method_results(method_dirs: List[str], method_name: str)` — [`L54`](../../../../../raw/code/claude-context/evaluation/analyze_and_plot_mcp_efficiency.py#L54) — Load and aggregate results from multiple runs of the same method.
- `main()` — [`L344`](../../../../../raw/code/claude-context/evaluation/analyze_and_plot_mcp_efficiency.py#L344) — Main function to analyze and plot MCP efficiency.
- `normalize_file_path(file_path: str)` — [`L16`](../../../../../raw/code/claude-context/evaluation/analyze_and_plot_mcp_efficiency.py#L16) — Normalize file paths.

