---
title: 'Module: tests/unit/languages/test_js_prototype_methods_791.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_js_prototype_methods_791.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_js_prototype_methods_791`/
symbols:
  extracted: extracted().
  js_parser: js_parser().
  prototype_fixture: prototype_fixture().
  test_method_count: test_method_count().
  test_class_count: test_class_count().
  test_class_name: test_class_name().
  test_speak_present: test_speak_present().
  test_walk_present: test_walk_present().
  test_speak_is_method: test_speak_is_method().
  test_walk_is_method: test_walk_is_method().
  test_speak_parent_class: test_speak_parent_class().
  test_walk_parent_class: test_walk_parent_class().
  test_constructor_not_lost: test_constructor_not_lost().
  test_no_duplicate_names: test_no_duplicate_names().
---
# Module: [`tests/unit/languages/test_js_prototype_methods_791.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py)

## Functions
- `extracted(js_parser: Parser, prototype_fixture: str)` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L37)
- `js_parser()` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L22)
- `prototype_fixture()` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L27)
- `test_class_count(extracted)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L57) — Animal is synthesised as a class via prototype aggregation.
- `test_class_name(extracted)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L62)
- `test_constructor_not_lost(extracted)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L96) — The Animal constructor function must still be extracted.
- `test_method_count(extracted)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L52) — Exactly 3 functions: Animal constructor + speak + walk.
- `test_no_duplicate_names(extracted)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L102) — No function name should appear more than once.
- `test_speak_is_method(extracted)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L76)
- `test_speak_parent_class(extracted)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L86)
- `test_speak_present(extracted)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L66)
- `test_walk_is_method(extracted)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L81)
- `test_walk_parent_class(extracted)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L91)
- `test_walk_present(extracted)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_js_prototype_methods_791.py#L71)

