---
title: 'Module: tree_sitter_analyzer/_ast_extraction.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_ast_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._ast_extraction`/_
symbols:
  _walk_for_symbols: walk_for_symbols().
  _worker_index_file: worker_index_file().
  _node_text: node_text().
  _extract_symbols: extract_symbols().
  _c_declarator_name: c_declarator_name().
  _content_hash: content_hash().
  _extract_call_edges: extract_call_edges().
  _scala_symbol_from_node: scala_symbol_from_node().
  _scala_symbol_name: scala_symbol_name().
  _annotate_canonical_complexity: annotate_canonical_complexity().
  _python_module_constant: python_module_constant().
  _worker_parser._worker_parser: worker_parser._worker_parser.
  _has_fts5: has_fts5().
  _bash_subscript_base: bash_subscript_base().
  _init_worker_parser: init_worker_parser().
  _count_decision_points: count_decision_points().
  _scala_given_type_text: scala_given_type_text().
  _python_docstring: python_docstring().
  _extract_parent_classes: extract_parent_classes().
  _go_package_constants: go_package_constants().
  _count_nodes: count_nodes().
  _find_parent_class: find_parent_class().
  _php_constants: php_constants().
  _EXCLUDE_DIRS: EXCLUDE_DIRS.
  _CLASS_LIKE: CLASS_LIKE.
  _c_function_def_name: c_function_def_name().
  _PY_SCOPE_BODY_NODES: PY_SCOPE_BODY_NODES.
  _DOCSTRING_MAX_CHARS: DOCSTRING_MAX_CHARS.
  _extract_imports: extract_imports().
  _extract_structure: extract_structure().
  _ENUM_LIKE: ENUM_LIKE.
  _SCALA_CLASS_LIKE: SCALA_CLASS_LIKE.
  _C_DECLARATOR_WRAPPERS: C_DECLARATOR_WRAPPERS.
  _FUNCTION_LIKE: FUNCTION_LIKE.
  _IMPORT_LIKE: IMPORT_LIKE.
  _VAR_DECL_LIKE: VAR_DECL_LIKE.
  _CONST_STYLE_NAME: CONST_STYLE_NAME.
  _PY_CONST_STYLE_NAME: PY_CONST_STYLE_NAME.
  _PY_DUNDER_NAME: PY_DUNDER_NAME.
  _GO_CONST_LIKE: GO_CONST_LIKE.
  _GO_SCOPE_BODY_NODES: GO_SCOPE_BODY_NODES.
  _RUST_CONST_LIKE: RUST_CONST_LIKE.
  _RUST_SCOPE_BODY_NODES: RUST_SCOPE_BODY_NODES.
  _PHP_SCOPE_BODY_NODES: PHP_SCOPE_BODY_NODES.
  _JSTS_SCOPE_BODY_NODES: JSTS_SCOPE_BODY_NODES.
  _JAVA_SCOPE_BODY_NODES: JAVA_SCOPE_BODY_NODES.
  _CSHARP_SCOPE_BODY_NODES: CSHARP_SCOPE_BODY_NODES.
  _SCALA_SCOPE_BODY_NODES: SCALA_SCOPE_BODY_NODES.
  _WALK_MAX_DEPTH: WALK_MAX_DEPTH.
  _COMPLEXITY_NODE_TYPES._COMPLEXITY_NODE_TYPES: COMPLEXITY_NODE_TYPES._COMPLEXITY_NODE_TYPES.
---
# Module: [`tree_sitter_analyzer/_ast_extraction.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py)

## Functions
- `_annotate_canonical_complexity(symbols: list[dict[str, Any]], tree: Any, source_code: str, language: str)` — [`L1135`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L1135) — Stamp each function/method symbol with the extractor's ``complexity``.
- `_bash_subscript_base(subscript: Any)` — [`L859`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L859) — Return the base ``variable_name`` node of a Bash ``subscript`` target.
- `_c_declarator_name(declarator: Any, source: str, depth: int)` — [`L830`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L830) — Descend a C declarator chain to its innermost identifier.
- `_c_function_def_name(node: Any, source: str)` — [`L799`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L799) — Recover the name of a C ``function_definition`` node.
- `_content_hash(source: str | bytes)` — [`L129`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L129)
- `_count_decision_points(node: Any, language: str)` — [`L704`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L704)
- `_count_nodes(node: Any)` — [`L692`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L692) — Count AST nodes iteratively to avoid RecursionError on deeply-nested trees.
- `_extract_call_edges(tree: Any, source_code: str, language: str, symbols: dict[str, Any])` — [`L1183`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L1183) — Extract call edges from the AST using shared function-call helpers.
- `_extract_imports(symbols: dict[str, Any])` — [`L1168`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L1168)
- `_extract_parent_classes(node: Any, source: str, language: str)` — [`L749`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L749) — Extract base class names from a class definition node.
- `_extract_structure(symbols: dict[str, Any])` — [`L1172`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L1172)
- `_extract_symbols(tree: Any, source_code: str, language: str)` — [`L1118`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L1118)
- `_find_parent_class(node: Any, source: str)` — [`L722`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L722) — Walk up the parent chain to find the innermost enclosing class-like
- `_go_package_constants(node: Any, source: str)` — [`L254`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L254) — Return kind="constant" symbols for a package-scope Go const/var
- `_has_fts5(conn: sqlite3.Connection)` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L26)
- `_init_worker_parser()` — [`L58`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L58)
- `_node_text(node: Any, source: str)` — [`L662`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L662) — Extract the source text of a tree-sitter node.
- `_php_constants(node: Any, source: str)` — [`L463`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L463) — Return kind="constant" symbols for a PHP const_declaration, one row
- `_python_docstring(node: Any, source: str)` — [`L523`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L523) — Return the PEP 257 docstring of a Python function/class node, or None.
- `_python_module_constant(node: Any, source: str)` — [`L489`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L489) — Return a kind="constant" symbol for a module-scope Python assignment,
- `_scala_given_type_text(node: Any, source: str)` — [`L906`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L906)
- `_scala_symbol_from_node(node: Any, source: str)` — [`L875`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L875)
- `_scala_symbol_name(node: Any, source: str)` — [`L891`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L891)
- `_walk_for_symbols(node: Any, source: str, symbols: list[dict[str, Any]], language: str, depth: int = 0, enclosed: bool = False, _truncated_flag: list[bool] | None = None)` — [`L924`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L924) — Walk the AST collecting symbol dicts.
- `_worker_index_file(args: tuple[str, str, str])` — [`L63`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L63) — Worker used by ``ASTCache._index_parallel`` via a process pool. — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)

## Module values
- `_CLASS_LIKE` — [`L171`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L171)
- `_COMPLEXITY_NODE_TYPES` — [`L560`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L560)
- `_CONST_STYLE_NAME` — [`L229`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L229)
- `_CSHARP_SCOPE_BODY_NODES` — [`L434`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L434)
- `_C_DECLARATOR_WRAPPERS` — [`L823`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L823)
- `_DOCSTRING_MAX_CHARS` — [`L520`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L520)
- `_ENUM_LIKE` — [`L164`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L164)
- `_EXCLUDE_DIRS` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L48)
- `_FUNCTION_LIKE` — [`L139`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L139)
- `_GO_CONST_LIKE` — [`L244`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L244)
- `_GO_SCOPE_BODY_NODES` — [`L249`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L249)
- `_IMPORT_LIKE` — [`L196`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L196)
- `_JAVA_SCOPE_BODY_NODES` — [`L399`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L399)
- `_JSTS_SCOPE_BODY_NODES` — [`L365`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L365)
- `_PHP_SCOPE_BODY_NODES` — [`L337`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L337)
- `_PY_CONST_STYLE_NAME` — [`L233`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L233)
- `_PY_DUNDER_NAME` — [`L234`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L234)
- `_PY_SCOPE_BODY_NODES` — [`L238`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L238)
- `_RUST_CONST_LIKE` — [`L307`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L307)
- `_RUST_SCOPE_BODY_NODES` — [`L314`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L314)
- `_SCALA_CLASS_LIKE` — [`L186`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L186)
- `_SCALA_SCOPE_BODY_NODES` — [`L455`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L455)
- `_VAR_DECL_LIKE` — [`L209`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L209)
- `_WALK_MAX_DEPTH` — [`L919`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L919)
- `_worker_parser` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_ast_extraction.py#L55)

