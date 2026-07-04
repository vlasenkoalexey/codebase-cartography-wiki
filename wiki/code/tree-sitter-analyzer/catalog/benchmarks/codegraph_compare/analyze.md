---
title: 'Module: benchmarks/codegraph_compare/analyze.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/analyze.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.analyze`/
symbols:
  build_report: build_report().
  gate_violations: gate_violations().
  _f2: _f2().
  _med: _med().
  _agg: _agg().
  _s_per_arm: _s_per_arm().
  _s_per_repo_arm: _s_per_repo_arm().
  _s_cold_warm: _s_cold_warm().
  _s_failed: _s_failed().
  _is_dry: _is_dry().
  _s_savings._medians: _s_savings()._medians().
  _s_overview: _s_overview().
  _s_savings: _s_savings().
  _table: _table().
  _is_low_quality: _is_low_quality().
  estimate_cost: estimate_cost().
  _s_quality_efficiency: _s_quality_efficiency().
  _write_csv: _write_csv().
  main: main().
  _is_failed: _is_failed().
  _enrich: _enrich().
  _s_gate: _s_gate().
  _f: _f().
  _table._row: _table()._row().
  _GATE_MAX_FAILURE_RATE: _GATE_MAX_FAILURE_RATE.
  _GATE_MIN_QUALITY: _GATE_MIN_QUALITY.
  _load_jsonl: _load_jsonl().
  _pct: _pct().
  _INPUT_COST_PER_M: _INPUT_COST_PER_M.
  _OUTPUT_COST_PER_M: _OUTPUT_COST_PER_M.
  _is_timeout: _is_timeout().
  _s_notes: _s_notes().
  _RUN_FIELDS: _RUN_FIELDS.
  _EVAL_FIELDS: _EVAL_FIELDS.
  _parse_args: _parse_args().
---
# Module: [`benchmarks/codegraph_compare/analyze.py`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py)

## Functions
- `_agg(runs: list[dict[str, Any]])` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L138)
- `_enrich(run: dict[str, Any])` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L66) — Return a copy of *run* with derived fields: _cost, _total_tokens, _repo_name.
- `_f(v: float | None, d: int = 4)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L119)
- `_f2(v: float | None)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L123)
- `_is_dry(run: dict[str, Any])` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L92)
- `_is_failed(run: dict[str, Any])` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L96)
- `_is_low_quality(run: dict[str, Any])` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L104)
- `_is_timeout(run: dict[str, Any])` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L100)
- `_load_jsonl(path: Path)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L49)
- `_med(values: list)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L114)
- `_medians(repo: str, arm: str)` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L293)
- `_parse_args(argv: list[str] | None = None)` — [`L680`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L680)
- `_pct(native: float | None, arm: float | None)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L127)
- `_row(cells: list[str])` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L172)
- `_s_cold_warm(runs: list[dict[str, Any]])` — [`L382`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L382)
- `_s_failed(runs: list[dict[str, Any]])` — [`L443`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L443)
- `_s_gate(runs: list[dict[str, Any]], has_evals: bool)` — [`L505`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L505)
- `_s_notes(n_repeats: int)` — [`L462`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L462)
- `_s_overview(runs: list[dict[str, Any]], has_evals: bool)` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L191)
- `_s_per_arm(by_arm: dict[str, list[dict[str, Any]]], has_evals: bool)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L225)
- `_s_per_repo_arm(runs: list[dict[str, Any]], has_evals: bool)` — [`L259`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L259)
- `_s_quality_efficiency(runs: list[dict[str, Any]], has_evals: bool)` — [`L332`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L332)
- `_s_savings(runs: list[dict[str, Any]])` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L288)
- `_table(headers: list[str], rows: list[list[str]])` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L165)
- `_write_csv(runs: list[dict[str, Any]], evals_by_id: dict[str, dict[str, Any]], path: Path)` — [`L547`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L547)
- `build_report(runs_path: Path, evals_path: Path | None, output_path: Path)` — [`L602`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L602)
- `estimate_cost(input_tokens: int, output_tokens: int)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L38)
- `gate_violations(runs: list[dict[str, Any]], has_evals: bool)` — [`L474`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L474) — Return benchmark gate violations for already-enriched run records.
- `main(argv: list[str] | None = None)` — [`L710`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L710)

## Module values
- `_EVAL_FIELDS` — [`L544`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L544)
- `_GATE_MAX_FAILURE_RATE` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L34)
- `_GATE_MIN_QUALITY` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L35)
- `_INPUT_COST_PER_M` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L32)
- `_OUTPUT_COST_PER_M` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L33)
- `_RUN_FIELDS` — [`L518`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/analyze.py#L518)

