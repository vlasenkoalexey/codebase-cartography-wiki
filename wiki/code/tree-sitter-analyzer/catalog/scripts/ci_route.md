---
title: 'Module: scripts/ci_route.py'
type: catalog
provenance: extracted
module: scripts/ci_route.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.ci_route`/
symbols:
  route_changed_files: route_changed_files().
  main: main().
  load_routing_config: load_routing_config().
  matches_any: matches_any().
  _parse_scalar: _parse_scalar().
  DEFAULT_OUTPUTS: DEFAULT_OUTPUTS.
  _next_meaningful_line_is_list: _next_meaningful_line_is_list().
  _read_changed_files: _read_changed_files().
  _write_github_outputs: _write_github_outputs().
---
# Module: [`scripts/ci_route.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/ci_route.py)

## Functions
- `_next_meaningful_line_is_list(path: Path, current_line: str)` — [`L84`](../../../../../raw/code/tree-sitter-analyzer/scripts/ci_route.py#L84)
- `_parse_scalar(value: str)` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/scripts/ci_route.py#L36)
- `_read_changed_files(args: argparse.Namespace)` — [`L171`](../../../../../raw/code/tree-sitter-analyzer/scripts/ci_route.py#L171)
- `_write_github_outputs(outputs: dict[str, Any], github_output: str)` — [`L181`](../../../../../raw/code/tree-sitter-analyzer/scripts/ci_route.py#L181)
- `load_routing_config(path: Path)` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/scripts/ci_route.py#L44)
- `main(argv: list[str] | None = None)` — [`L193`](../../../../../raw/code/tree-sitter-analyzer/scripts/ci_route.py#L193)
- `matches_any(path: str, patterns: list[str])` — [`L102`](../../../../../raw/code/tree-sitter-analyzer/scripts/ci_route.py#L102)
- `route_changed_files(changed_files: list[str], config: dict[str, Any])` — [`L109`](../../../../../raw/code/tree-sitter-analyzer/scripts/ci_route.py#L109)

## Module values
- `DEFAULT_OUTPUTS` — [`L18`](../../../../../raw/code/tree-sitter-analyzer/scripts/ci_route.py#L18)

