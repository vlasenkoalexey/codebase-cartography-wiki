---
title: 'Module: tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools._refactoring_plan_builder`/
symbols:
  _build_plan_for_func: _build_plan_for_func().
  _build_extraction_target: _build_extraction_target().
  _find_extractable_blocks: _find_extractable_blocks().
  _infer_returns: _infer_returns().
  _assigned_names_from_statement_and_body: _assigned_names_from_statement_and_body().
  build_precise_plans: build_precise_plans().
  _assigned_names_from_statement: _assigned_names_from_statement().
  _next_extractable_block: _next_extractable_block().
  _suggest_helper_name: _suggest_helper_name().
  _infer_params_for_block: _infer_params_for_block().
  _build_extraction_targets: _build_extraction_targets().
  _is_block_continuation: _is_block_continuation().
  _scan_block_end: _scan_block_end().
  ExtractionTargetContext: ExtractionTargetContext#
  ExtractionTargetContext.func_name: ExtractionTargetContext#func_name.
  ExtractionTargetContext.lines: ExtractionTargetContext#lines.
  ExtractionTargetContext.func_assigned: ExtractionTargetContext#func_assigned.
  ExtractionTargetContext.ext: ExtractionTargetContext#ext.
  _collect_assigned_names: _collect_assigned_names().
  _assigned_names_from_target: _assigned_names_from_target().
  _nested_bodies_for_return_inference: _nested_bodies_for_return_inference().
  _make_skeleton: _make_skeleton().
  _helper_module_stem: _helper_module_stem().
  _body_indent: _body_indent().
  _unique_names: _unique_names().
  _assigned_names_from_statements: _assigned_names_from_statements().
  _assigned_names_from_targets: _assigned_names_from_targets().
  _helper_module_path: _helper_module_path().
  _helper_import_statement: _helper_import_statement().
  _classify_line: _classify_line().
  _BUILTINS: _BUILTINS.
---
# Module: [`tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py)

## Classes
### `ExtractionTargetContext`
- def: [`tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py:17`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L17)
- doc: Shared inputs for building extraction targets.
- signature: `class ExtractionTargetContext:`
- members:
  - `ext` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L23)
  - `func_assigned` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L22)
  - `func_name` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L21)
  - `lines` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L20)
- used by: [`_build_extraction_target`](_refactoring_plan_builder.md#_build_extraction_target), [`_build_extraction_targets`](_refactoring_plan_builder.md#_build_extraction_targets)  (4 test-only)

## Functions
- `_assigned_names_from_statement(node: ast.AST)` — [`L397`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L397) — Return direct assignment targets for one AST statement.
- `_assigned_names_from_statement_and_body(node: ast.AST)` — [`L381`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L381) — Return names assigned by a statement and selected direct child bodies.
- `_assigned_names_from_statements(statements: list[ast.stmt])` — [`L389`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L389) — Return names assigned by a list of direct statements.
- `_assigned_names_from_target(target: ast.expr)` — [`L416`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L416) — Return assigned names from one target expression.
- `_assigned_names_from_targets(targets: list[ast.expr])` — [`L408`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L408) — Return assigned names from assignment targets.
- `_body_indent(func_lines: list[str])` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L248)
- `_build_extraction_target(index: int, block: tuple[int, int, str], context: ExtractionTargetContext)` — [`L114`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L114) — Build one extraction target with inferred signature details.
- `_build_extraction_targets(blocks: list[tuple[int, int, str]], lines: list[str], func_name: str, func_assigned: set[str], ext: str)` — [`L99`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L99) — Build extraction target rows for the largest logical blocks.
- `_build_plan_for_func(file_path: str, lines: list[str], func: dict[str, Any], source: str)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L57) — Build a precise extraction plan for one long function.
- `_classify_line(stripped: str)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L257)
- `_collect_assigned_names(source: str)` — [`L295`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L295)
- `_find_extractable_blocks(func_lines: list[str], abs_start: int)` — [`L167`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L167) — Identify logical blocks within a function body that can be extracted.
- `_helper_import_statement(file_path: str, helper_stem: str, helper_names: str)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L154) — Return a copy-pasteable sibling helper import for a source file.
- `_helper_module_path(file_path: str, helper_stem: str)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L145) — Return the sibling helper module path shown in extraction plans.
- `_helper_module_stem(file_path: str)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L138) — Return a single-underscore helper module stem for a source file.
- `_infer_params_for_block(block_src: str, func_assigned: set[str])` — [`L345`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L345)
- `_infer_returns(block_src: str)` — [`L369`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L369)
- `_is_block_continuation(next_stripped: str, hint: str)` — [`L271`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L271)
- `_make_skeleton(name: str, params: list[str], returns: list[str], block_lines: list[str], ext: str)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L448)
- `_nested_bodies_for_return_inference(node: ast.AST)` — [`L425`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L425) — Return direct child bodies whose assignments should become returns.
- `_next_extractable_block(func_lines: list[str], index: int, total_lines: int, body_indent: int)` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L192) — Return the next extractable block and the following scan index.
- `_scan_block_end(func_lines: list[str], index: int, total_lines: int, body_indent: int, hint: str)` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L221) — Return the exclusive end index for one top-level logical block.
- `_suggest_helper_name(func_name: str, hint: str, index: int)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L279)
- `_unique_names(names: list[str])` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L436) — Return names without duplicates while preserving order.
- `build_precise_plans(file_path: str, source: str, analysis: Any, suggestions: list[dict[str, Any]])` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L27) — Attach precise extraction plans to long_function suggestions.

## Module values
- `_BUILTINS` — [`L310`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/_refactoring_plan_builder.py#L310)

