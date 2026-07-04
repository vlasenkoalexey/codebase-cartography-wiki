---
title: 'Module: benchmarks/agent-tasks/scenarios.py'
type: catalog
provenance: extracted
module: benchmarks/agent-tasks/scenarios.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.agent-tasks.scenarios`/
symbols:
  SCENARIOS.SCENARIOS: SCENARIOS.SCENARIOS.
  _run_subprocess: _run_subprocess().
  refactor_suggest_tsa: refactor_suggest_tsa().
  cold_start_tsa: cold_start_tsa().
  find_callers_tsa: find_callers_tsa().
  change_impact_tsa: change_impact_tsa().
  list_scenarios: list_scenarios().
  refactor_suggest_baseline: refactor_suggest_baseline().
  estimate_tokens: estimate_tokens().
  _is_decidable: _is_decidable().
  cold_start_baseline: cold_start_baseline().
  find_callers_baseline: find_callers_baseline().
  change_impact_baseline: change_impact_baseline().
  _pick_default_file: _pick_default_file().
  _CHARS_PER_TOKEN: _CHARS_PER_TOKEN.
  _serialize_for_tokens: _serialize_for_tokens().
---
# Module: [`benchmarks/agent-tasks/scenarios.py`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py)

## Functions
- `_is_decidable(result: dict[str, Any])` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L76) — A result is agent-decidable when it has a verdict that isn't ERROR.
- `_pick_default_file(repo: str)` — [`L393`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L393) — Choose a non-trivial Python file for refactor-suggest.
- `_run_subprocess(cmd: list[str], cwd: str | Path, timeout: float = 30)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L56) — Run a shell command and return stdout (stderr swallowed).
- `_serialize_for_tokens(obj: Any)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L44) — Render ``obj`` to a string for token estimation.
- `change_impact_baseline(repo: str, **_: Any)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L264) — Baseline change-impact: agent runs git diff + greps for test files.
- `change_impact_tsa(repo: str, **_: Any)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L248) — TSA change-impact: 1 call to analyze_change_impact mode=diff.
- `cold_start_baseline(repo: str, **_: Any)` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L115) — Baseline cold-start: agent reads README + lists files + tails git log.
- `cold_start_tsa(repo: str, **_: Any)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L100) — TSA cold-start: 1 call to get_project_summary.
- `estimate_tokens(text: str)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L37) — Estimate token count from a text blob using the 4-chars-per-token heuristic.
- `find_callers_baseline(repo: str, symbol: str = "execute", **_: Any)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L193) — Baseline find-callers: agent greps for the symbol with rg/grep.
- `find_callers_tsa(repo: str, symbol: str = "execute", **_: Any)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L172) — TSA find-callers: 1 call to codegraph_call_graph mode=callers.
- `list_scenarios()` — [`L453`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L453) — Return the scenario ids the harness knows about.
- `refactor_suggest_baseline(repo: str, file: str = "", **_: Any)` — [`L345`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L345) — Baseline refactor-suggest: agent reads file + greps for long methods.
- `refactor_suggest_tsa(repo: str, file: str = "", **_: Any)` — [`L320`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L320) — TSA refactor-suggest: 1 call to refactoring_suggestions.

## Module values
- `SCENARIOS` — [`L429`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L429)
- `_CHARS_PER_TOKEN` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/scenarios.py#L34)

