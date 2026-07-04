---
title: 'Module: tree_sitter_analyzer/function_extraction.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/function_extraction.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.function_extraction`/
symbols:
  walk_tree: walk_tree().
  _extract_recursive: _extract_recursive().
  find_receiver_type_go: find_receiver_type_go().
  _node_text: _node_text().
  _CALL_DISPATCH._CALL_DISPATCH: _CALL_DISPATCH._CALL_DISPATCH.
  _normalize_go_receiver_type_for_graph: _normalize_go_receiver_type_for_graph().
  get_func_name: get_func_name().
  _FUNC_NAME_DISPATCH._FUNC_NAME_DISPATCH: _FUNC_NAME_DISPATCH._FUNC_NAME_DISPATCH.
  _FUNC_DEF_TYPES: _FUNC_DEF_TYPES.
  node_text: node_text().
  _collect_local_var_types._walk: _collect_local_var_types()._walk().
  _collect_fixture_types._walk: _collect_fixture_types()._walk().
  _node_text_value: _node_text_value().
  _call_info_field: _call_info_field().
  _func_name_c: _func_name_c().
  extract_call: extract_call().
  _func_name_field: _func_name_field().
  _CALL_NODE_TYPES: _CALL_NODE_TYPES.
  _func_name_js: _func_name_js().
  _call_info_c: _call_info_c().
  _call_info_kotlin: _call_info_kotlin().
  _infer_return_class._walk: _infer_return_class()._walk().
  _call_from_text: _call_from_text().
  find_parent_class_python: find_parent_class_python().
  find_parent_class_java: find_parent_class_java().
  _func_name_go: _func_name_go().
  _call_info_java: _call_info_java().
  _call_info_rust: _call_info_rust().
  _call_info_php: _call_info_php().
  _infer_return_class: _infer_return_class().
  _func_name_identifier: _func_name_identifier().
  _collect_local_var_types: _collect_local_var_types().
  _declarator_name: _declarator_name().
  _call_info_ruby: _call_info_ruby().
  _func_param_names: _func_param_names().
  _collect_fixture_types: _collect_fixture_types().
  _BUILTIN_LITERAL_NODE_TYPES._BUILTIN_LITERAL_NODE_TYPES: _BUILTIN_LITERAL_NODE_TYPES._BUILTIN_LITERAL_NODE_TYPES.
  _IDENT_TYPES_JS: _IDENT_TYPES_JS.
  _IDENT_TYPES_GO: _IDENT_TYPES_GO.
  _IDENT_TYPES_C: _IDENT_TYPES_C.
  _BUILTIN_CONSTRUCTOR_NAMES._BUILTIN_CONSTRUCTOR_NAMES: _BUILTIN_CONSTRUCTOR_NAMES._BUILTIN_CONSTRUCTOR_NAMES.
---
# Module: [`tree_sitter_analyzer/function_extraction.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py)

## Functions
- `_call_from_text(text: str, node: Any)` — [`L579`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L579)
- `_call_info_c(node: Any, source: str)` — [`L178`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L178) — C / C++: prefer function field, fall back to first identifier child.
- `_call_info_field(node: Any, source: str)` — [`L138`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L138) — Python / JS / TS / Go: extract call target from the ``function`` field.
- `_call_info_java(node: Any, source: str)` — [`L146`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L146) — Java method_invocation: method name from the ``name`` field, receiver
- `_call_info_kotlin(node: Any, source: str)` — [`L220`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L220) — Kotlin: ``call_expression`` / ``constructor_invocation`` carry the callee
- `_call_info_php(node: Any, source: str)` — [`L255`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L255) — PHP: ``member_call_expression`` / ``scoped_call_expression`` expose the
- `_call_info_ruby(node: Any, source: str)` — [`L236`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L236) — Ruby ``call``: method name in the ``method`` field, optional ``receiver``
- `_call_info_rust(node: Any, source: str)` — [`L196`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L196) — Rust: ``call_expression`` exposes the callee in the ``function`` field
- `_collect_fixture_types(module_node: Any, source: str, language: str)` — [`L436`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L436) — RFC-0002: map function name → returned class, for pytest-fixture typing.
- `_collect_local_var_types(func_node: Any, source: str, language: str)` — [`L339`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L339) — RFC-0002: infer local variable types from assignments.
- `_declarator_name(declarator_node: Any)` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L83) — Find the first identifier inside a ``function_declarator`` node.
- `_extract_recursive(node: Any, source: str, language: str, definitions: list[dict[str, Any]], calls: list[dict[str, Any]], enclosing_class: str | None, local_types: dict[str, tuple[str, int]] | None, fixture_types: dict[str, str] | None = None)` — [`L476`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L476)
- `_func_name_c(node: Any)` — [`L91`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L91) — C / C++: direct identifier types, or recurse into function_declarator.
- `_func_name_field(node: Any)` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L103) — Rust / Kotlin / Ruby / C# / PHP: name lives in the ``name`` field.
- `_func_name_go(node: Any)` — [`L72`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L72) — Go: prefer named field, fall back to identifier/field_identifier child.
- `_func_name_identifier(node: Any)` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L56) — Python / Java: first ``identifier`` child.
- `_func_name_js(node: Any)` — [`L64`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L64) — JavaScript / TypeScript: identifier or property_identifier child.
- `_func_param_names(func_node: Any, source: str)` — [`L388`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L388) — Parameter identifier names of a Python function def.
- `_infer_return_class(func_node: Any, source: str)` — [`L409`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L409) — Infer the class a Python function returns: ``return ClassName(...)`` or
- `_node_text(node: Any, source: str)` — [`L598`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L598)
- `_node_text_value(node: Any)` — [`L714`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L714)
- `_normalize_go_receiver_type_for_graph(receiver_type: str | None)` — [`L685`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L685) — Normalize Go receiver type for class matching in call graphs.
- `_walk(n: Any)` — [`L360`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L360)
- `_walk(n: Any)` — [`L415`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L415)
- `_walk(n: Any)` — [`L451`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L451)
- `extract_call(node: Any, source: str, language: str)` — [`L568`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L568) — Extract call target info from a call node.
- `find_parent_class_java(node: Any)` — [`L631`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L631) — Walk up from a Java method node to find an enclosing class.
- `find_parent_class_python(node: Any)` — [`L617`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L617) — Walk up from a Python function node to find an enclosing class.
- `find_receiver_type_go(node: Any)` — [`L645`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L645) — Extract the receiver type from a Go method_declaration node.
- `get_func_name(node: Any, language: str)` — [`L557`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L557) — Extract a function or method name from a definition node.
- `node_text(node: Any, source: str)` — [`L593`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L593) — Extract text from a node using UTF-8 byte offsets safely.
- `walk_tree(node: Any, source: str, language: str)` — [`L309`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L309) — Walk an AST and return function definitions plus call sites. — documented in [tree_sitter_analyzer-call_graph](../../concepts/tree_sitter_analyzer-call_graph.md)

## Module values
- `_BUILTIN_CONSTRUCTOR_NAMES` — [`L334`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L334)
- `_BUILTIN_LITERAL_NODE_TYPES` — [`L322`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L322)
- `_CALL_DISPATCH` — [`L284`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L284)
- `_CALL_NODE_TYPES` — [`L8`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L8)
- `_FUNC_DEF_TYPES` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L29)
- `_FUNC_NAME_DISPATCH` — [`L115`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L115)
- `_IDENT_TYPES_C` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L53)
- `_IDENT_TYPES_GO` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L52)
- `_IDENT_TYPES_JS` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/function_extraction.py#L51)

