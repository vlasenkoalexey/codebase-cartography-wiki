---
title: 'Module: tree_sitter_analyzer/dead_code_analyzer.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/dead_code_analyzer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.dead_code_analyzer`/
symbols:
  analyze_dead_code: analyze_dead_code().
  find_unused_imports: find_unused_imports().
  find_unreferenced_variables: find_unreferenced_variables().
  find_transitive_dead_code: find_transitive_dead_code().
  DeadCodeResult.dead_functions: DeadCodeResult#dead_functions.
  _extract_top_level_variables: _extract_top_level_variables().
  DeadCodeResult: DeadCodeResult#
  DeadCodeResult.stats: DeadCodeResult#stats.
  DeadCodeResult.unused_imports: DeadCodeResult#unused_imports.
  DeadCodeResult.unreferenced_variables: DeadCodeResult#unreferenced_variables.
  _is_test_file: _is_test_file().
  UnusedImport: UnusedImport#
  DeadFunction: DeadFunction#
  _is_known_entry: _is_known_entry().
  UnusedImport.file: UnusedImport#file.
  UnreferencedVariable: UnreferencedVariable#
  _walk_identifiers: _walk_identifiers().
  _walk_func_body: _walk_func_body().
  UnreferencedVariable.file: UnreferencedVariable#file.
  _EXCLUDE_DIRS: _EXCLUDE_DIRS.
  UnusedImport.line: UnusedImport#line.
  UnusedImport.unused_names: UnusedImport#unused_names.
  _collect_function_body_identifiers: _collect_function_body_identifiers().
  DeadFunction.reason: DeadFunction#reason.
  DeadFunction.dead_callees: DeadFunction#dead_callees.
  UnreferencedVariable.name: UnreferencedVariable#name.
  UnreferencedVariable.line: UnreferencedVariable#line.
  _iter_candidate_files: _iter_candidate_files().
  UnusedImport.import_text: UnusedImport#import_text.
  _node_text: _node_text().
  _collect_identifiers: _collect_identifiers().
  _extract_python_top_level_vars: _extract_python_top_level_vars().
  _extract_js_top_level_vars: _extract_js_top_level_vars().
  _CLASS_DEF_TYPES: _CLASS_DEF_TYPES.
  UnreferencedVariable.language: UnreferencedVariable#language.
  logger: logger.
  _IDENTIFIER_NODE_TYPES: _IDENTIFIER_NODE_TYPES.
  _KNOWN_ENTRY_PATTERNS: _KNOWN_ENTRY_PATTERNS.
  _TEST_FILE_PATTERNS: _TEST_FILE_PATTERNS.
  _VARIABLE_ASSIGN_TYPES: _VARIABLE_ASSIGN_TYPES.
  _check_import_unused: _check_import_unused().
  _infer_import_line: _infer_import_line().
  DeadFunction.depth: DeadFunction#depth.
---
# Module: [`tree_sitter_analyzer/dead_code_analyzer.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py)

## Classes
### `DeadCodeResult`
- def: [`tree_sitter_analyzer/dead_code_analyzer.py:130`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L130)
- signature: `class DeadCodeResult:`
- members:
  - `dead_functions` — [`L131`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L131)
  - `stats` — [`L134`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L134)
  - `unreferenced_variables` — [`L133`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L133)
  - `unused_imports` — [`L132`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L132)
- uses (calls/refs, reference-scoped): [`UnusedImport`](dead_code_analyzer.md#UnusedImport), [`DeadFunction`](dead_code_analyzer.md#DeadFunction), [`UnreferencedVariable`](dead_code_analyzer.md#UnreferencedVariable)
- used by: [`execute`](mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.execute), [`analyze_dead_code`](dead_code_analyzer.md#analyze_dead_code)  (10 test-only)

### `DeadFunction`
- def: [`tree_sitter_analyzer/dead_code_analyzer.py:106`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L106)
- signature: `class DeadFunction:`
- members:
  - `dead_callees` — [`L110`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L110)
  - `depth` — [`L109`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L109)
  - `reason` — [`L108`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L108)
- uses (calls/refs, reference-scoped): [`FunctionRef`](call_graph.md#FunctionRef)
- used by: [`find_transitive_dead_code`](dead_code_analyzer.md#find_transitive_dead_code), [`dead_functions`](dead_code_analyzer.md#DeadCodeResult.dead_functions), [`_serialize_dead_function`](mcp/tools/dead_code_tool.md#_serialize_dead_function)  (3 test-only)

### `UnreferencedVariable`
- def: [`tree_sitter_analyzer/dead_code_analyzer.py:122`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L122)
- signature: `class UnreferencedVariable:`
- members:
  - `file` — [`L123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L123)
  - `language` — [`L126`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L126)
  - `line` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L125)
  - `name` — [`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L124)
- used by: [`execute`](mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.execute), [`analyze_dead_code`](dead_code_analyzer.md#analyze_dead_code), [`find_unreferenced_variables`](dead_code_analyzer.md#find_unreferenced_variables), [`_serialize_unref_var`](mcp/tools/dead_code_tool.md#_serialize_unref_var), [`unreferenced_variables`](dead_code_analyzer.md#DeadCodeResult.unreferenced_variables)  (3 test-only)

### `UnusedImport`
- def: [`tree_sitter_analyzer/dead_code_analyzer.py:114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L114)
- signature: `class UnusedImport:`
- members:
  - `file` — [`L115`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L115)
  - `import_text` — [`L117`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L117)
  - `line` — [`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L116)
  - `unused_names` — [`L118`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L118)
- used by: [`execute`](mcp/tools/dead_code_tool.md#CodeGraphDeadCodeTool.execute), [`analyze_dead_code`](dead_code_analyzer.md#analyze_dead_code), [`find_unused_imports`](dead_code_analyzer.md#find_unused_imports), [`_serialize_unused_import`](mcp/tools/dead_code_tool.md#_serialize_unused_import), [`unused_imports`](dead_code_analyzer.md#DeadCodeResult.unused_imports)  (5 test-only)

## Functions
- `_check_import_unused(imp: dict[str, Any], identifier_names: set[str])` — [`L307`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L307) — Return list of unused names for imp, or None if imp should be skipped.
- `_collect_function_body_identifiers(tree: Any, source: str, language: str)` — [`L463`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L463) — Collect identifiers that appear inside function bodies.
- `_collect_identifiers(node: Any, source: str, language: str, *, skip_import_subtrees: bool = False)` — [`L454`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L454) — Collect all identifier nodes from the AST.
- `_extract_js_top_level_vars(tree: Any, source: str, func_types: set[str], class_types: set[str], assign_types: set[str])` — [`L501`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L501) — Extract top-level variable declarations from JavaScript/TypeScript AST nodes.
- `_extract_python_top_level_vars(tree: Any, source: str, func_types: set[str], class_types: set[str])` — [`L475`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L475) — Extract top-level variable assignments from Python AST nodes.
- `_extract_top_level_variables(tree: Any, source: str, language: str)` — [`L527`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L527) — Extract variable names assigned at the top level (module scope).
- `_infer_import_line(source: str, imp: dict[str, Any])` — [`L322`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L322) — Best-effort line number fallback for extractors that omit line metadata.
- `_is_known_entry(name: str, language: str)` — [`L141`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L141)
- `_is_test_file(file_path: str)` — [`L137`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L137)
- `_iter_candidate_files(root: Path)` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L47) — Yield files under ``root``, PRUNING excluded and hidden (dot-prefixed)
- `_node_text(node: Any, source: str)` — [`L546`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L546) — Extract text from a tree-sitter node.
- `_walk_func_body(n: Any, source: str, func_types: set[str], inside_func: bool, result: set[str])` — [`L434`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L434) — Recursive helper for _collect_function_body_identifiers; avoids closure nesting.
- `_walk_identifiers(n: Any, source: str, skip_import_subtrees: bool, result: list[tuple[str, int]])` — [`L415`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L415) — Recursive helper for _collect_identifiers; avoids closure nesting.
- `analyze_dead_code(project_root: str, *, include_test_files: bool = False, include_unused_imports: bool = True, include_variables: bool = True, max_files: int = 500)` — [`L559`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L559) — Comprehensive dead code analysis. — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
- `find_transitive_dead_code(graph: CallGraph, *, include_test_files: bool = False, max_depth: int = 20)` — [`L148`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L148) — Find transitive dead code using flood-fill from entry points.
- `find_unreferenced_variables(project_root: str, *, include_test_files: bool = False, max_files: int = 500)` — [`L342`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L342) — Find file-level variable assignments that no function in the file references.
- `find_unused_imports(project_root: str, *, include_test_files: bool = False, max_files: int = 500)` — [`L221`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L221) — Find import statements whose imported names are never referenced in the same file.

## Module values
- `_CLASS_DEF_TYPES` — [`L96`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L96)
- `_EXCLUDE_DIRS` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L44)
- `_IDENTIFIER_NODE_TYPES` — [`L410`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L410)
- `_KNOWN_ENTRY_PATTERNS` — [`L68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L68)
- `_TEST_FILE_PATTERNS` — [`L81`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L81)
- `_VARIABLE_ASSIGN_TYPES` — [`L86`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L86)
- `logger` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/dead_code_analyzer.py#L35)

