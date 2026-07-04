---
title: 'Module: scripts/auto_review.py'
type: catalog
provenance: extracted
module: scripts/auto_review.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.auto_review`/
symbols:
  collect_backlog: collect_backlog().
  WorkItem.to_dict: WorkItem#to_dict().
  build_plan: build_plan().
  enrich_with_patterns: enrich_with_patterns().
  main: main().
  _run_tool: _run_tool().
  WorkItem: WorkItem#
  WorkItem.file_path: WorkItem#file_path.
  diff_impact: diff_impact().
  route_summary: route_summary().
  WorkItem.priority: WorkItem#priority.
  WorkItem.grade: WorkItem#grade.
  WorkItem.weakest_dimension: WorkItem#weakest_dimension.
  _shellify: _shellify().
  ROOT: ROOT.
  WorkItem.score: WorkItem#score.
  WorkItem.signal: WorkItem#signal.
  WorkItem.safety_command: WorkItem#safety_command.
  WorkItem.refactor_command: WorkItem#refactor_command.
  WorkItem.post_edit_commands: WorkItem#post_edit_commands.
  WorkItem.patterns: WorkItem#patterns.
  TOOL_BIN: TOOL_BIN.
  _looks_like_docstring_example: _looks_like_docstring_example().
  _utc_now: _utc_now().
---
# Module: [`scripts/auto_review.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py)

## Classes
### `WorkItem`
- def: [`scripts/auto_review.py:80`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L80)
- doc: One unit of work the autonomous loop can hand to a specialist agent.
- signature: `class WorkItem:`
- members:
  - `to_dict(self)` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L94)
  - `file_path` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L83)
  - `grade` — [`L85`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L85)
  - `patterns` — [`L92`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L92)
  - `post_edit_commands` — [`L91`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L91)
  - `priority` — [`L84`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L84)
  - `refactor_command` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L90)
  - `safety_command` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L89)
  - `score` — [`L86`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L86)
  - `signal` — [`L87`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L87)
  - `weakest_dimension` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L88)
- used by: [`collect_backlog`](auto_review.md#collect_backlog), [`build_plan`](auto_review.md#build_plan), [`enrich_with_patterns`](auto_review.md#enrich_with_patterns), [`main`](auto_review.md#main)

## Functions
- `_looks_like_docstring_example(file_path: str, pattern: dict[str, Any])` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L152) — Skip print-in-production hits whose line is inside a triple-quoted block.
- `_run_tool(args: list[str], *, timeout: int = 240)` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L46) — Run the analyzer with --output-format json and parse the result.
- `_shellify(cmd: str)` — [`L109`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L109) — Turn the project's recommended CLI string into a list[str] for subprocess.
- `_utc_now()` — [`L206`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L206)
- `build_plan(items: list[WorkItem])` — [`L183`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L183)
- `collect_backlog(max_items: int)` — [`L114`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L114)
- `diff_impact()` — [`L175`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L175)
- `enrich_with_patterns(items: list[WorkItem])` — [`L140`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L140) — Run --code-patterns on each work item to attach concrete smells.
- `main(argv: list[str] | None = None)` — [`L212`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L212)
- `route_summary()` — [`L179`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L179)

## Module values
- `ROOT` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L41)
- `TOOL_BIN` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/scripts/auto_review.py#L43)

