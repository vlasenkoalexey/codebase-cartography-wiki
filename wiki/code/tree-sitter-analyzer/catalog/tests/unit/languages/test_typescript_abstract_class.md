---
title: 'Module: tests/unit/languages/test_typescript_abstract_class.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_typescript_abstract_class.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_typescript_abstract_class`/
symbols:
  _extract_function_names: _extract_function_names().
  _extract_classes: _extract_classes().
  test_visibility_on_abstract_method_signature: test_visibility_on_abstract_method_signature().
  _abstract_sig_node: _abstract_sig_node().
  test_abstract_signature_parse_raising_yields_none: test_abstract_signature_parse_raising_yields_none().
  _parse: _parse().
  test_abstract_signature_parse_returning_none_yields_none: test_abstract_signature_parse_returning_none_yields_none().
  test_abstract_signature_nameless_parse_yields_none: test_abstract_signature_nameless_parse_yields_none().
  _abstract_sig_node.find: _abstract_sig_node().find().
  ABSTRACT_CLASS_SRC: ABSTRACT_CLASS_SRC.
  test_abstract_class_extracted_with_correct_type: test_abstract_class_extracted_with_correct_type().
  test_concrete_class_still_extracted: test_concrete_class_still_extracted().
  test_interface_still_extracted: test_interface_still_extracted().
  test_abstract_class_yields_four_methods: test_abstract_class_yields_four_methods().
  test_abstract_method_signature_extracted: test_abstract_method_signature_extracted().
  test_constructor_in_abstract_class_extracted: test_constructor_in_abstract_class_extracted().
  test_protected_method_in_abstract_class_extracted: test_protected_method_in_abstract_class_extracted().
  test_public_method_in_abstract_class_extracted: test_public_method_in_abstract_class_extracted().
  test_concrete_class_methods_still_extracted: test_concrete_class_methods_still_extracted().
  test_interface_method_still_extracted: test_interface_method_still_extracted().
  test_exact_method_count_for_base_entity_abstract_methods_only: test_exact_method_count_for_base_entity_abstract_methods_only().
  test_abstract_signature_parse_raising_yields_none.boom: test_abstract_signature_parse_raising_yields_none().boom().
---
# Module: [`tests/unit/languages/test_typescript_abstract_class.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py)

## Functions
- `_abstract_sig_node()` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L174) — Return the abstract_method_signature node from the fixture parse.
- `_extract_classes(src: str = ABSTRACT_CLASS_SRC)` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L45)
- `_extract_function_names(src: str = ABSTRACT_CLASS_SRC)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L50)
- `_parse(src: str = ABSTRACT_CLASS_SRC)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L39)
- `boom(node: tree_sitter.Node)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L228)
- `find(node: tree_sitter.Node)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L178)
- `test_abstract_class_extracted_with_correct_type()` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L58) — Abstract class itself must be extracted as class_type='abstract_class'.
- `test_abstract_class_yields_four_methods()` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L79) — BaseEntity has exactly 4 members: constructor, validate, updateTimestamp, getId.
- `test_abstract_method_signature_extracted()` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L98) — ``abstract validate()`` (abstract_method_signature node) must appear in functions.
- `test_abstract_signature_nameless_parse_yields_none()` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L207)
- `test_abstract_signature_parse_raising_yields_none()` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L223)
- `test_abstract_signature_parse_returning_none_yields_none()` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L192)
- `test_concrete_class_methods_still_extracted()` — [`L122`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L122) — Concrete subclass method must still be extracted.
- `test_concrete_class_still_extracted()` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L64) — Regular class inside same file must not be affected.
- `test_constructor_in_abstract_class_extracted()` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L104) — ``constructor`` (method_definition inside abstract class) must be extracted.
- `test_exact_method_count_for_base_entity_abstract_methods_only()` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L137) — Isolated snippet with only the two abstract members — exact count == 2.
- `test_interface_method_still_extracted()` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L128) — Interface method (method_signature) must still be extracted.
- `test_interface_still_extracted()` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L70) — Interface inside same file must not be affected.
- `test_protected_method_in_abstract_class_extracted()` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L110) — ``protected updateTimestamp()`` (method_definition) must be extracted.
- `test_public_method_in_abstract_class_extracted()` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L116) — ``public getId()`` (method_definition) must be extracted.
- `test_visibility_on_abstract_method_signature()` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L151) — abstract_method_signature carries visibility from the node text.

## Module values
- `ABSTRACT_CLASS_SRC` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_typescript_abstract_class.py#L21)

