---
title: 'Module: tests/unit/languages/test_c_cpp_fixes.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_c_cpp_fixes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_c_cpp_fixes`/
symbols:
  TestBug751CppNestedClass.test_template_nested_struct_has_parent_class: TestBug751CppNestedClass#test_template_nested_struct_has_parent_class().
  TestBug751CppNestedClass.test_nested_struct_has_parent_class: TestBug751CppNestedClass#test_nested_struct_has_parent_class().
  TestBug751CppNestedClass.test_outer_class_type_preserved: TestBug751CppNestedClass#test_outer_class_type_preserved().
  TestBug751CppNestedClass.test_field_type_reference_is_not_nested_class: TestBug751CppNestedClass#test_field_type_reference_is_not_nested_class().
  TestBug751CppNestedClass.test_union_nested_struct_has_parent_class: TestBug751CppNestedClass#test_union_nested_struct_has_parent_class().
  TestBug752CTypedefStructNoDuplicate.test_anonymous_typedef_struct_single_entry: TestBug752CTypedefStructNoDuplicate#test_anonymous_typedef_struct_single_entry().
  TestBug751CppNestedClass.test_nested_struct_inside_class: TestBug751CppNestedClass#test_nested_struct_inside_class().
  TestBug751CppNestedClass.test_nested_class_inside_class: TestBug751CppNestedClass#test_nested_class_inside_class().
  TestBug751CppNestedClass.test_multiple_nested_types: TestBug751CppNestedClass#test_multiple_nested_types().
  TestBug752CTypedefStructNoDuplicate.test_anonymous_typedef_struct_name_not_synthetic: TestBug752CTypedefStructNoDuplicate#test_anonymous_typedef_struct_name_not_synthetic().
  TestBug752CTypedefStructNoDuplicate.test_named_typedef_struct_single_entry: TestBug752CTypedefStructNoDuplicate#test_named_typedef_struct_single_entry().
  TestBug752CTypedefStructNoDuplicate.test_multiple_independent_typedefs: TestBug752CTypedefStructNoDuplicate#test_multiple_independent_typedefs().
  TestBug753CAnonymousNestedContainerSkipped.test_anonymous_nested_union_skipped: TestBug753CAnonymousNestedContainerSkipped#test_anonymous_nested_union_skipped().
  TestBug753CAnonymousNestedContainerSkipped.test_anonymous_nested_struct_skipped: TestBug753CAnonymousNestedContainerSkipped#test_anonymous_nested_struct_skipped().
  TestBug753CAnonymousNestedContainerSkipped.test_no_anonymous_synthetic_name_emitted: TestBug753CAnonymousNestedContainerSkipped#test_no_anonymous_synthetic_name_emitted().
  TestBug753CAnonymousNestedContainerSkipped.test_named_nested_struct_is_extracted: TestBug753CAnonymousNestedContainerSkipped#test_named_nested_struct_is_extracted().
  TestBitfields.test_c_unnamed_bitfield_is_skipped: TestBitfields#test_c_unnamed_bitfield_is_skipped().
  TestBitfields.test_cpp_unnamed_bitfield_is_skipped: TestBitfields#test_cpp_unnamed_bitfield_is_skipped().
  _parse_c: _parse_c().
  _parse_cpp: _parse_cpp().
  TestBug751CppNestedClass: TestBug751CppNestedClass#
  TestBug752CTypedefStructNoDuplicate: TestBug752CTypedefStructNoDuplicate#
  TestBug753CAnonymousNestedContainerSkipped: TestBug753CAnonymousNestedContainerSkipped#
  TestBitfields: TestBitfields#
---
# Module: [`tests/unit/languages/test_c_cpp_fixes.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py)

## Classes
### `TestBitfields`
- def: [`tests/unit/languages/test_c_cpp_fixes.py:286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L286)
- doc: Unnamed C/C++ bitfields are padding, not addressable field symbols.
- signature: `class TestBitfields:`
- members:
  - `test_c_unnamed_bitfield_is_skipped(self)` — [`L289`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L289)
  - `test_cpp_unnamed_bitfield_is_skipped(self)` — [`L297`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L297)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor), [`CppElementExtractor`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor), [`extract_variables`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_variables), [`extract_variables`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_variables)  (2 test-only)

### `TestBug751CppNestedClass`
- def: [`tests/unit/languages/test_c_cpp_fixes.py:38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L38)
- doc: C++ inner class/struct inside a class body must be extracted.
- signature: `class TestBug751CppNestedClass:`
- members:
  - `test_field_type_reference_is_not_nested_class(self)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L130) — struct Point field references inside Rect must not emit bogus nested Point.
  - `test_multiple_nested_types(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L96) — Multiple nested types all extracted.
  - `test_nested_class_inside_class(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L59) — class nested inside a class body.
  - `test_nested_struct_has_parent_class(self)` — [`L81`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L81) — Nested struct should have parent_class set to enclosing class name.
  - `test_nested_struct_inside_class(self)` — [`L41`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L41) — Simple struct nested inside a class body.
  - `test_outer_class_type_preserved(self)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L113) — Outer class class_type stays 'class'.
  - `test_template_nested_struct_has_parent_class(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L144)
  - `test_union_nested_struct_has_parent_class(self)` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L158)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`CppElementExtractor`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/cpp_plugin.md#CppElementExtractor.extract_classes), [`modifiers`](../../../tree_sitter_analyzer/models/base.md#Class.modifiers), [`parent_class`](../../../tree_sitter_analyzer/models/base.md#Class.parent_class)  (1 test-only)

### `TestBug752CTypedefStructNoDuplicate`
- def: [`tests/unit/languages/test_c_cpp_fixes.py:176`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L176)
- doc: typedef struct { ... } Name must produce exactly one entry.
- signature: `class TestBug752CTypedefStructNoDuplicate:`
- members:
  - `test_anonymous_typedef_struct_name_not_synthetic(self)` — [`L190`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L190) — typedef struct { ... } MyType must not also emit an anonymous_struct_ entry.
  - `test_anonymous_typedef_struct_single_entry(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L179) — Simplest case: typedef struct { ... } MyType produces exactly one entry.
  - `test_multiple_independent_typedefs(self)` — [`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L212) — Multiple typedef structs each produce exactly one entry.
  - `test_named_typedef_struct_single_entry(self)` — [`L201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L201) — typedef struct Foo { ... } Foo produces exactly one entry (no double Foo).
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_classes)  (1 test-only)

### `TestBug753CAnonymousNestedContainerSkipped`
- def: [`tests/unit/languages/test_c_cpp_fixes.py:230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L230)
- doc: Anonymous nested unions/structs inside a typedef struct must NOT be extracted
- signature: `class TestBug753CAnonymousNestedContainerSkipped:`
- members:
  - `test_anonymous_nested_struct_skipped(self)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L246) — Nested anonymous struct with a field name is skipped.
  - `test_anonymous_nested_union_skipped(self)` — [`L234`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L234) — typedef struct { union { int a; float b; } data; } Container — only
  - `test_named_nested_struct_is_extracted(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L274) — A NAMED nested struct (with type_identifier) inside a struct body IS extracted.
  - `test_no_anonymous_synthetic_name_emitted(self)` — [`L257`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L257) — No anonymous_union_N or anonymous_struct_N name should appear for
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`CElementExtractor`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/c_plugin.md#CElementExtractor.extract_classes)  (1 test-only)

## Functions
- `_parse_c(code: str)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L21)
- `_parse_cpp(code: str)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_c_cpp_fixes.py#L27)

