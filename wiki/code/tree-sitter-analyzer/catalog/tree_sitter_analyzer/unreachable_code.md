---
title: 'Module: tree_sitter_analyzer/unreachable_code.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/unreachable_code.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.unreachable_code`/
symbols:
  analyze_file_unreachable: analyze_file_unreachable().
  _analyze_block_unreachable: _analyze_block_unreachable().
  UnreachableCodeResult.unreachable_blocks: UnreachableCodeResult#unreachable_blocks.
  analyze_project_unreachable: analyze_project_unreachable().
  UnreachableBlock: UnreachableBlock#
  _report_dead_branch: _report_dead_branch().
  _analyze_if_statement: _analyze_if_statement().
  UnreachableCodeResult.to_dict: UnreachableCodeResult#to_dict().
  _report_unreachable_after_terminal: _report_unreachable_after_terminal().
  UnreachableBlock.to_dict: UnreachableBlock#to_dict().
  UnreachableCodeResult: UnreachableCodeResult#
  _walk_functions_in_tree._visit: _walk_functions_in_tree()._visit().
  _check_constant_condition: _check_constant_condition().
  _analyze_alternative_clause: _analyze_alternative_clause().
  UnreachableCodeResult.errors: UnreachableCodeResult#errors.
  UnreachableBlock.reason: UnreachableBlock#reason.
  _analyze_child_nodes: _analyze_child_nodes().
  UnreachableCodeResult.language: UnreachableCodeResult#language.
  _analyze_try_statement: _analyze_try_statement().
  _parse_tree: _parse_tree().
  _is_false_literal: _is_false_literal().
  _is_true_literal: _is_true_literal().
  UnreachableCodeResult.file_path: UnreachableCodeResult#file_path.
  UnreachableCodeResult.functions_analyzed: UnreachableCodeResult#functions_analyzed.
  _is_terminal_call: _is_terminal_call().
  _s: _s.
  UnreachableBlock.severity: UnreachableBlock#severity.
  _analyze_handler_block: _analyze_handler_block().
  UnreachableBlock.function_name: UnreachableBlock#function_name.
  UnreachableBlock.start_line: UnreachableBlock#start_line.
  UnreachableBlock.end_line: UnreachableBlock#end_line.
  _node_text: _node_text().
  _is_terminal_statement: _is_terminal_statement().
  _walk_functions_in_tree: _walk_functions_in_tree().
  _analyze_function_body: _analyze_function_body().
  _get_function_name: _get_function_name().
  UnreachableBlock.file_path: UnreachableBlock#file_path.
  _BLOCK_TYPES._BLOCK_TYPES: _BLOCK_TYPES._BLOCK_TYPES.
  _CLASS_DEF_TYPES_SET._CLASS_DEF_TYPES_SET: _CLASS_DEF_TYPES_SET._CLASS_DEF_TYPES_SET.
  logger: logger.
  _read_file_bytes: _read_file_bytes().
  _infer_js_function_name: _infer_js_function_name().
  _LOOP_BREAK_TYPES._LOOP_BREAK_TYPES: _LOOP_BREAK_TYPES._LOOP_BREAK_TYPES.
  _IF_TYPES._IF_TYPES: _IF_TYPES._IF_TYPES.
  _EXCLUDE_DIRS: _EXCLUDE_DIRS.
  _TERMINAL_CALL_NAMES: _TERMINAL_CALL_NAMES.
  _find_call_func_node: _find_call_func_node().
  _get_if_condition: _get_if_condition().
  _get_consequence_and_alternative: _get_consequence_and_alternative().
  _find_block_in_clause: _find_block_in_clause().
  _TERMINAL_STATEMENT_TYPES._TERMINAL_STATEMENT_TYPES: _TERMINAL_STATEMENT_TYPES._TERMINAL_STATEMENT_TYPES.
  _TRY_TYPES._TRY_TYPES: _TRY_TYPES._TRY_TYPES.
  _find_children_by_type: _find_children_by_type().
---
# Module: [`tree_sitter_analyzer/unreachable_code.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py)

## Classes
### `UnreachableBlock`
- def: [`tree_sitter_analyzer/unreachable_code.py:116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L116)
- signature: `class UnreachableBlock:`
- members:
  - `to_dict(self)` — [`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L124)
  - `end_line` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L120)
  - `file_path` — [`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L117)
  - `function_name` — [`L118`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L118)
  - `reason` — [`L121`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L121)
  - `severity` — [`L122`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L122)
  - `start_line` — [`L119`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L119)
- used by: [`analyze_file_unreachable`](unreachable_code.md#analyze_file_unreachable), [`_analyze_block_unreachable`](unreachable_code.md#_analyze_block_unreachable), [`unreachable_blocks`](unreachable_code.md#UnreachableCodeResult.unreachable_blocks), [`_format_file_blocks_toon`](mcp/tools/unreachable_code_tool.md#UnreachableCodeTool._format_file_blocks_toon), [`_analyze_if_statement`](unreachable_code.md#_analyze_if_statement), [`_report_dead_branch`](unreachable_code.md#_report_dead_branch), [`to_dict`](unreachable_code.md#UnreachableCodeResult.to_dict), [`_report_unreachable_after_terminal`](unreachable_code.md#_report_unreachable_after_terminal), [`_analyze_alternative_clause`](unreachable_code.md#_analyze_alternative_clause), [`_check_constant_condition`](unreachable_code.md#_check_constant_condition), [`_analyze_child_nodes`](unreachable_code.md#_analyze_child_nodes), [`_analyze_try_statement`](unreachable_code.md#_analyze_try_statement), [`_analyze_handler_block`](unreachable_code.md#_analyze_handler_block), [`_analyze_function_body`](unreachable_code.md#_analyze_function_body), [`_walk_functions_in_tree`](unreachable_code.md#_walk_functions_in_tree)  (10 test-only)

### `UnreachableCodeResult`
- def: [`tree_sitter_analyzer/unreachable_code.py:136`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L136)
- signature: `class UnreachableCodeResult:`
- members:
  - `to_dict(self)` — [`L143`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L143)
  - `errors` — [`L141`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L141)
  - `file_path` — [`L137`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L137)
  - `functions_analyzed` — [`L140`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L140)
  - `language` — [`L138`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L138)
  - `unreachable_blocks` — [`L139`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L139)
- uses (calls/refs, reference-scoped): [`UnreachableBlock`](unreachable_code.md#UnreachableBlock), [`to_dict`](unreachable_code.md#UnreachableBlock.to_dict)
- used by: [`analyze_file_unreachable`](unreachable_code.md#analyze_file_unreachable), [`_build_file_response`](mcp/tools/unreachable_code_tool.md#UnreachableCodeTool._build_file_response), [`analyze_project_unreachable`](unreachable_code.md#analyze_project_unreachable), [`_format_file_blocks_toon`](mcp/tools/unreachable_code_tool.md#UnreachableCodeTool._format_file_blocks_toon), [`_build_project_response`](mcp/tools/unreachable_code_tool.md#UnreachableCodeTool._build_project_response)  (17 test-only)

## Functions
- `_analyze_alternative_clause(alternative: Any, source: str, language: str, func_name: str, file_path: str, results: list[UnreachableBlock])` — [`L463`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L463) — Recursively analyze the else or elif clause of an if statement.
- `_analyze_block_unreachable(block_node: Any, source: str, language: str, func_name: str, file_path: str, results: list[UnreachableBlock])` — [`L231`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L231) — Walk a block's children; detect unreachable statements after terminals.
- `_analyze_child_nodes(node: Any, source: str, language: str, func_name: str, file_path: str, results: list[UnreachableBlock])` — [`L313`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L313)
- `_analyze_function_body(func_node: Any, block_type: str, source: str, language: str, func_name: str, file_path: str, results: list[UnreachableBlock])` — [`L579`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L579) — Analyze the body of a single function node.
- `_analyze_handler_block(handler: Any, block_type: str, source: str, language: str, func_name: str, file_path: str, results: list[UnreachableBlock])` — [`L514`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L514) — Analyze all block children within an except/finally handler.
- `_analyze_if_statement(node: Any, source: str, language: str, func_name: str, file_path: str, results: list[UnreachableBlock])` — [`L388`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L388)
- `_analyze_try_statement(node: Any, source: str, language: str, func_name: str, file_path: str, results: list[UnreachableBlock])` — [`L490`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L490)
- `_check_constant_condition(condition: Any, consequence: Any, alternative: Any, block_type: str, source: str, func_name: str, file_path: str, results: list[UnreachableBlock])` — [`L422`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L422) — Flag consequence or alternative as unreachable for constant conditions.
- `_find_block_in_clause(clause: Any, block_type: str)` — [`L455`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L455) — Return the first block child of an else clause.
- `_find_call_func_node(node: Any, language: str)` — [`L185`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L185) — Extract the function-name node from a call node.
- `_find_children_by_type(node: Any, type_name: str)` — [`L218`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L218)
- `_get_consequence_and_alternative(node: Any, block_type: str)` — [`L352`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L352) — Return the (consequence_block, alternative_clause) for an if node.
- `_get_function_name(node: Any, source: str, language: str)` — [`L663`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L663)
- `_get_if_condition(node: Any, language: str)` — [`L336`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L336) — Return the condition node for an if statement.
- `_infer_js_function_name(node: Any, source: str)` — [`L672`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L672) — Try to infer name for anonymous JS/TS functions from their parent.
- `_is_false_literal(node: Any, source: str)` — [`L204`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L204)
- `_is_terminal_call(node: Any, source: str, language: str)` — [`L169`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L169)
- `_is_terminal_statement(node: Any, source: str, language: str)` — [`L197`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L197)
- `_is_true_literal(node: Any, source: str)` — [`L211`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L211)
- `_node_text(node: Any, source: str)` — [`L159`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L159)
- `_parse_tree(file_path: str, language: str, source_bytes: bytes)` — [`L619`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L619) — Parse source bytes with tree-sitter; return root node or None on failure.
- `_read_file_bytes(file_path: str)` — [`L609`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L609) — Read file bytes; return None on I/O error.
- `_report_dead_branch(branch_node: Any, condition: Any, reason_template: str, func_name: str, file_path: str, results: list[UnreachableBlock])` — [`L364`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L364) — Append an UnreachableBlock for a statically-dead if/else branch.
- `_report_unreachable_after_terminal(child: Any, terminal_node: Any, func_name: str, file_path: str, results: list[UnreachableBlock])` — [`L283`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L283) — Append an UnreachableBlock for code that follows a terminal statement.
- `_visit(node: Any)` — [`L555`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L555)
- `_walk_functions_in_tree(root: Any, func_def_types: set[str], block_type: str, source: str, language: str, file_path: str, results: list[UnreachableBlock])` — [`L536`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L536) — Walk the AST and analyze every function body for unreachable code.
- `analyze_file_unreachable(file_path: str, language: str | None = None)` — [`L628`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L628) — Analyze a single file for unreachable code paths.
- `analyze_project_unreachable(project_root: str, *, include_test_files: bool = False, max_files: int = 500)` — [`L691`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L691) — Scan a project for unreachable code paths.

## Module values
- `_BLOCK_TYPES` — [`L84`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L84)
- `_CLASS_DEF_TYPES_SET` — [`L735`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L735)
- `_EXCLUDE_DIRS` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L31)
- `_IF_TYPES` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L94)
- `_LOOP_BREAK_TYPES` — [`L61`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L61)
- `_TERMINAL_CALL_NAMES` — [`L71`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L71)
- `_TERMINAL_STATEMENT_TYPES` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L51)
- `_TRY_TYPES` — [`L104`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L104)
- `_s` — [`L739`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L739)
- `logger` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/unreachable_code.py#L29)

