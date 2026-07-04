---
title: 'Module: examples/agent_workflow_comparison_demo.py'
type: catalog
provenance: extracted
module: examples/agent_workflow_comparison_demo.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `examples.agent_workflow_comparison_demo`/
symbols:
  build_comparison: build_comparison().
  Comparison.to_dict: Comparison#to_dict().
  main: main().
  format_asciicast: format_asciicast().
  format_markdown: format_markdown().
  Comparison: Comparison#
  Comparison.target_path: Comparison#target_path.
  Comparison.symbol_name: Comparison#symbol_name.
  Comparison.source_lines: Comparison#source_lines.
  Comparison.focused_lines: Comparison#focused_lines.
  Comparison.baseline_tokens: Comparison#baseline_tokens.
  Comparison.guided_tokens: Comparison#guided_tokens.
  Comparison.reduction_tokens: Comparison#reduction_tokens.
  Comparison.reduction_percent: Comparison#reduction_percent.
  Comparison.workflow_next_step: Comparison#workflow_next_step.
  Comparison.queue_boundary: Comparison#queue_boundary.
  Comparison.focused_range: Comparison#focused_range.
  Comparison.guided_context: Comparison#guided_context.
  estimate_tokens: estimate_tokens().
  run_tree_sitter_analyzer: run_tree_sitter_analyzer().
  build_guided_context: build_guided_context().
  _select_method: _select_method().
  parse_args: parse_args().
---
# Module: [`examples/agent_workflow_comparison_demo.py`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py)

## Classes
### `Comparison`
- def: [`examples/agent_workflow_comparison_demo.py:17`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L17)
- doc: Context comparison for a single target symbol.
- signature: `class Comparison:`
- members:
  - `to_dict(self)` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L33) — Return a JSON-serializable representation.
  - `baseline_tokens` — [`L24`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L24)
  - `focused_lines` — [`L23`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L23)
  - `focused_range` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L30)
  - `guided_context` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L31)
  - `guided_tokens` — [`L25`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L25)
  - `queue_boundary` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L29)
  - `reduction_percent` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L27)
  - `reduction_tokens` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L26)
  - `source_lines` — [`L22`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L22)
  - `symbol_name` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L21)
  - `target_path` — [`L20`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L20)
  - `workflow_next_step` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L28)
- used by: (4 test-only callers)

## Functions
- `_select_method(method_results: list[dict[str, Any]], symbol_name: str)` — [`L139`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L139) — Return the exact method match from query results.
- `build_comparison(*, project_root: Path, target_path: str, symbol_name: str)` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L88) — Build the comparison by calling the same CLI a human would demo.
- `build_guided_context(workflow_pack: dict[str, Any], method_result: dict[str, Any])` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L69) — Build the compact context an agent needs after SMART-guided retrieval.
- `estimate_tokens(text: str)` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L51) — Estimate LLM tokens with the common four-characters-per-token heuristic.
- `format_asciicast(comparison: Comparison)` — [`L178`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L178) — Render an asciinema v2 recording payload for repeatable demo evidence.
- `format_markdown(comparison: Comparison)` — [`L149`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L149) — Render a concise demo report suitable for terminal output or README snippets.
- `main(argv: list[str] | None = None)` — [`L236`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L236) — Run the demo.
- `parse_args(argv: list[str] | None = None)` — [`L212`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L212) — Parse CLI arguments for the demo.
- `run_tree_sitter_analyzer(args: list[str], project_root: Path)` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/examples/agent_workflow_comparison_demo.py#L56) — Run the local CLI and parse JSON output.

