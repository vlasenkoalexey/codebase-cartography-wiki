---
title: 'Module: scripts/check_ps_ascii.py'
type: catalog
provenance: extracted
module: scripts/check_ps_ascii.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.check_ps_ascii`/
symbols:
  find_powershell_run_blocks: find_powershell_run_blocks().
  scan_file: scan_file().
  main: main().
  indent: indent().
  SHELL_PS_RE: SHELL_PS_RE.
  SHELL_OTHER_RE: SHELL_OTHER_RE.
  ASCII_HI: ASCII_HI.
  RUN_BLOCK_RE: RUN_BLOCK_RE.
---
# Module: [`scripts/check_ps_ascii.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_ps_ascii.py)

## Functions
- `find_powershell_run_blocks(text: str)` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_ps_ascii.py#L43) — Return (start_line, end_line) inclusive 0-indexed ranges of every
- `indent(line: str)` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_ps_ascii.py#L39)
- `main()` — [`L144`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_ps_ascii.py#L144)
- `scan_file(path: str)` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_ps_ascii.py#L125) — Return [(line_no_1based, col_1based, line_text), ...] for every

## Module values
- `ASCII_HI` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_ps_ascii.py#L28)
- `RUN_BLOCK_RE` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_ps_ascii.py#L33)
- `SHELL_OTHER_RE` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_ps_ascii.py#L32)
- `SHELL_PS_RE` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/scripts/check_ps_ascii.py#L31)

