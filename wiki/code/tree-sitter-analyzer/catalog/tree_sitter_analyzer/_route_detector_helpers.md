---
title: 'Module: tree_sitter_analyzer/_route_detector_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_route_detector_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._route_detector_helpers`/
symbols:
  walk: walk().
  unquote: unquote().
  extract_annotation_value: extract_annotation_value().
  unquote_java_string: unquote_java_string().
  parse_methods_list: parse_methods_list().
  function_name_after_decorator: function_name_after_decorator().
  extract_django_handler: extract_django_handler().
  extract_js_handler: extract_js_handler().
  method_after_annotation: method_after_annotation().
  find_keyword: find_keyword().
  extract_template_string: extract_template_string().
---
# Module: [`tree_sitter_analyzer/_route_detector_helpers.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py)

## Functions
- `extract_annotation_value(node)` — [`L150`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L150) — Extract the literal `value=` of a Spring annotation, returning None if absent.
- `extract_django_handler(text: str)` — [`L100`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L100) — Extract the handler name from a Django `path()` view argument expression.
- `extract_js_handler(args_node)` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L111) — Extract the handler reference from an Express call's `arguments` node.
- `extract_template_string(node)` — [`L135`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L135) — Extract the inner text of a JS template-literal route pattern.
- `find_keyword(args_node, keyword: str)` — [`L90`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L90) — Find a Python keyword argument by name inside an `arguments` node.
- `function_name_after_decorator(decorator_node)` — [`L62`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L62) — Return the name of the function/identifier sibling that follows a decorator.
- `method_after_annotation(annotation_node)` — [`L77`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L77) — Return the name of the Java method declared after an annotation.
- `parse_methods_list(methods_str: str)` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L56) — Extract quoted HTTP method names from a `methods=['GET', 'POST']` fragment.
- `unquote(s: str)` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L40) — Strip a single matched pair of leading/trailing quotes.
- `unquote_java_string(s: str)` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L48) — Strip a Java double-quoted string's surrounding quotes.
- `walk(node)` — [`L18`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_route_detector_helpers.py#L18) — Yield every descendant of `node` in pre-order, using a tree-cursor.

