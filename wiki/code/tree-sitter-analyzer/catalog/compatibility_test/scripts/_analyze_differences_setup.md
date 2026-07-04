---
title: 'Module: compatibility_test/scripts/_analyze_differences_setup.py'
type: catalog
provenance: extracted
module: compatibility_test/scripts/_analyze_differences_setup.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.scripts._analyze_differences_setup`/
symbols:
  run_analysis_cli: run_analysis_cli().
  configure_smart_comparison: configure_smart_comparison().
  initial_analysis_results: initial_analysis_results().
  build_argument_parser: build_argument_parser().
  write_optional_json_output: write_optional_json_output().
  print_completion_summary: print_completion_summary().
---
# Module: [`compatibility_test/scripts/_analyze_differences_setup.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_setup.py)

## Functions
- `build_argument_parser()` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_setup.py#L51) — Build the CLI argument parser.
- `configure_smart_comparison(analyzer: Any, config_path: str | None)` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_setup.py#L12) — Configure optional smart JSON comparison paths and comparator.
- `initial_analysis_results()` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_setup.py#L40) — Return the legacy analysis-results buckets.
- `print_completion_summary(summary: dict[str, int], report_file: str)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_setup.py#L116) — Print the CLI completion summary.
- `run_analysis_cli(args: argparse.Namespace, analyzer_factory: Any)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_setup.py#L76) — Run the CLI flow for parsed arguments.
- `write_optional_json_output(output_json: str | None, analysis_results: dict[str, Any])` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/scripts/_analyze_differences_setup.py#L101) — Write optional JSON output requested by the CLI.

