---
title: 'Module: generate_golden_masters.py'
type: catalog
provenance: extracted
module: generate_golden_masters.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 generate_golden_masters/
symbols:
  generate_golden_master: generate_golden_master().
  generate_all_formats: generate_all_formats().
  main: main().
  run_analyzer: run_analyzer().
---
# Module: [`generate_golden_masters.py`](../../../../raw/code/tree-sitter-analyzer/generate_golden_masters.py)

## Functions
- `generate_all_formats(file_path: str, base_name: str, formats: list[str] | None = None)` — [`L62`](../../../../raw/code/tree-sitter-analyzer/generate_golden_masters.py#L62) — Generate golden masters for all specified formats
- `generate_golden_master(file_path: str, format_type: str, output_name: str)` — [`L29`](../../../../raw/code/tree-sitter-analyzer/generate_golden_masters.py#L29) — Generate golden master for a specific format
- `main()` — [`L74`](../../../../raw/code/tree-sitter-analyzer/generate_golden_masters.py#L74) — Generate all golden master files
- `run_analyzer(input_file: str, table_format: str = "full")` — [`L18`](../../../../raw/code/tree-sitter-analyzer/generate_golden_masters.py#L18) — アナライザーを実行して出力を取得

