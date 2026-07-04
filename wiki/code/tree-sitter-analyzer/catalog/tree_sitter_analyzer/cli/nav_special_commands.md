---
title: 'Module: tree_sitter_analyzer/cli/nav_special_commands.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/nav_special_commands.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.nav_special_commands`/
symbols:
  handle_nav_actions: handle_nav_actions().
  _execute_nav_facade: _execute_nav_facade().
  _dispatch_test_map: _dispatch_test_map().
  _dispatch_co_change: _dispatch_co_change().
---
# Module: [`tree_sitter_analyzer/cli/nav_special_commands.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/nav_special_commands.py)

## Functions
- `_dispatch_co_change(args: Any, context: SpecialCommandContext, facade: Any, output_format: str)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/nav_special_commands.py#L30) — Dispatch --co-change action.
- `_dispatch_test_map(args: Any, context: SpecialCommandContext, facade: Any, output_format: str)` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/nav_special_commands.py#L12) — Dispatch --test-map action.
- `_execute_nav_facade(facade: Any, tool_args: dict[str, Any], output_format: str, label: str, context: SpecialCommandContext)` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/nav_special_commands.py#L54) — Execute nav facade tool and handle output.
- `handle_nav_actions(args: Any, context: SpecialCommandContext)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/nav_special_commands.py#L78) — Dispatch RFC-0014 nav facade actions: --test-map and --co-change.

