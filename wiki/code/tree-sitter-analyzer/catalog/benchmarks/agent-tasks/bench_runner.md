---
title: 'Module: benchmarks/agent-tasks/bench_runner.py'
type: catalog
provenance: extracted
module: benchmarks/agent-tasks/bench_runner.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.agent-tasks.bench_runner`/
symbols:
  run_case: run_case().
  main: main().
  _THIS_DIR: _THIS_DIR.
  _build_arg_parser: _build_arg_parser().
  _assert_schema: _assert_schema().
  _error_row: _error_row().
  run_matrix: run_matrix().
  _extract_verdict: _extract_verdict().
  _build_input_blob: _build_input_blob().
  _build_output_blob: _build_output_blob().
  write_jsonl: write_jsonl().
  write_json_aggregate: write_json_aggregate().
  REQUIRED_FIELDS.REQUIRED_FIELDS: REQUIRED_FIELDS.REQUIRED_FIELDS.
---
# Module: [`benchmarks/agent-tasks/bench_runner.py`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py)

## Functions
- `_assert_schema(row: dict[str, Any])` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L209) — Verify a row carries every REQUIRED_FIELDS entry.
- `_build_arg_parser()` — [`L292`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L292)
- `_build_input_blob(task: str, repo: str, kwargs: dict[str, Any])` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L88) — Synthesize the prompt the agent would have to send.
- `_build_output_blob(result: dict[str, Any])` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L103) — Render the tool/baseline result for tokens_out estimation.
- `_error_row(*, repo: str, task: str, tool: str, wall_clock_s: float, tokens_in: int, error: str, traceback_str: str)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L175) — Build a schema-complete row for a failed case.
- `_extract_verdict(result: dict[str, Any])` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L70) — Pull the verdict from a tool result, mirroring base_tool's vocabulary.
- `main(argv: list[str] | None = None)` — [`L340`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L340) — Run the bench from the command line. Returns a process exit code.
- `run_case(repo: str, task: str, tool: str, **scenario_kwargs: Any)` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L117) — Run one (repo, task, tool) case and return a JSONL-ready row.
- `run_matrix(repos: list[str], tasks: list[str], tools: list[str], scenario_kwargs: dict[str, dict[str, Any]] | None = None)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L225) — Run the full (repos × tasks × tools) matrix and return all rows.
- `write_json_aggregate(rows: list[dict[str, Any]], out_path: Path)` — [`L269`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L269) — Write a single JSON object aggregating all rows for README rendering.
- `write_jsonl(rows: list[dict[str, Any]], out_path: Path)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L255) — Write rows as JSONL — one row per line, UTF-8, atomic via rename.

## Module values
- `REQUIRED_FIELDS` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L52)
- `_THIS_DIR` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/agent-tasks/bench_runner.py#L38)

