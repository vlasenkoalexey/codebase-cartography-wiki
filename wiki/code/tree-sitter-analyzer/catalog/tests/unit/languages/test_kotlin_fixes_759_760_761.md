---
title: 'Module: tests/unit/languages/test_kotlin_fixes_759_760_761.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_kotlin_fixes_759_760_761.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_kotlin_fixes_759_760_761`/
symbols:
  extractor: extractor().
  kotlin_parser: kotlin_parser().
  TestBug759LocalVarNotExtractedAsField: TestBug759LocalVarNotExtractedAsField#
  TestBug759LocalVarNotExtractedAsField.test_local_val_inside_method_excluded: TestBug759LocalVarNotExtractedAsField#test_local_val_inside_method_excluded().
  TestBug759LocalVarNotExtractedAsField.test_local_var_inside_method_excluded: TestBug759LocalVarNotExtractedAsField#test_local_var_inside_method_excluded().
  TestBug759LocalVarNotExtractedAsField.test_local_val_in_nested_block_excluded: TestBug759LocalVarNotExtractedAsField#test_local_val_in_nested_block_excluded().
  TestBug759LocalVarNotExtractedAsField.test_top_level_val_still_extracted: TestBug759LocalVarNotExtractedAsField#test_top_level_val_still_extracted().
  TestBug759LocalVarNotExtractedAsField.test_class_field_and_local_mixed: TestBug759LocalVarNotExtractedAsField#test_class_field_and_local_mixed().
  TestBug760PropertyModifiers: TestBug760PropertyModifiers#
  TestBug760PropertyModifiers.test_private_val_visibility: TestBug760PropertyModifiers#test_private_val_visibility().
  TestBug760PropertyModifiers.test_protected_var_visibility: TestBug760PropertyModifiers#test_protected_var_visibility().
  TestBug760PropertyModifiers.test_internal_visibility: TestBug760PropertyModifiers#test_internal_visibility().
  TestBug760PropertyModifiers.test_public_val_is_val: TestBug760PropertyModifiers#test_public_val_is_val().
  TestBug760PropertyModifiers.test_private_val_is_val: TestBug760PropertyModifiers#test_private_val_is_val().
  TestBug760PropertyModifiers.test_private_var_is_var: TestBug760PropertyModifiers#test_private_var_is_var().
  TestBug760PropertyModifiers.test_override_val_modifiers: TestBug760PropertyModifiers#test_override_val_modifiers().
  TestBug760PropertyModifiers.test_lateinit_var_modifiers: TestBug760PropertyModifiers#test_lateinit_var_modifiers().
  TestBug760PropertyModifiers.test_property_name_extracted_with_modifiers: TestBug760PropertyModifiers#test_property_name_extracted_with_modifiers().
  TestBug761ConstructorReturnType: TestBug761ConstructorReturnType#
  TestBug761ConstructorReturnType.test_primary_constructor_return_type_none: TestBug761ConstructorReturnType#test_primary_constructor_return_type_none().
  TestBug761ConstructorReturnType.test_primary_constructor_with_visibility_return_type_none: TestBug761ConstructorReturnType#test_primary_constructor_with_visibility_return_type_none().
  TestBug761ConstructorReturnType.test_primary_constructor_data_class_return_type_none: TestBug761ConstructorReturnType#test_primary_constructor_data_class_return_type_none().
  TestBug761ConstructorReturnType.test_primary_constructor_is_constructor_true: TestBug761ConstructorReturnType#test_primary_constructor_is_constructor_true().
  TestBug761ConstructorReturnType.test_regular_functions_not_affected: TestBug761ConstructorReturnType#test_regular_functions_not_affected().
---
# Module: [`tests/unit/languages/test_kotlin_fixes_759_760_761.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py)

## Classes
### `TestBug759LocalVarNotExtractedAsField`
- def: [`tests/unit/languages/test_kotlin_fixes_759_760_761.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L37)
- doc: Local val/var inside function bodies must not appear in extract_variables.
- signature: `class TestBug759LocalVarNotExtractedAsField:`
- members:
  - `test_class_field_and_local_mixed(self, extractor, kotlin_parser)` — [`L113`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L113) — Class field extracted, local variable skipped, in the same class.
  - `test_local_val_in_nested_block_excluded(self, extractor, kotlin_parser)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L77) — val inside an if-block or for-loop is also local.
  - `test_local_val_inside_method_excluded(self, extractor, kotlin_parser)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L40)
  - `test_local_var_inside_method_excluded(self, extractor, kotlin_parser)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L58)
  - `test_top_level_val_still_extracted(self, extractor, kotlin_parser)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L100) — Top-level (file-scope) val must still be extracted.

### `TestBug760PropertyModifiers`
- def: [`tests/unit/languages/test_kotlin_fixes_759_760_761.py:141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L141)
- doc: Modifier keywords must be captured and visibility must be set correctly.
- signature: `class TestBug760PropertyModifiers:`
- members:
  - `test_internal_visibility(self, extractor, kotlin_parser)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L168)
  - `test_lateinit_var_modifiers(self, extractor, kotlin_parser)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L242) — lateinit var: modifiers list contains 'lateinit'.
  - `test_override_val_modifiers(self, extractor, kotlin_parser)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L223) — override val: modifiers list contains 'override'.
  - `test_private_val_is_val(self, extractor, kotlin_parser)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L193) — private val: is_val=True despite modifier prefix.
  - `test_private_val_visibility(self, extractor, kotlin_parser)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L144)
  - `test_private_var_is_var(self, extractor, kotlin_parser)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L208) — private var: is_var=True despite modifier prefix.
  - `test_property_name_extracted_with_modifiers(self, extractor, kotlin_parser)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L256) — Name must be correct even when modifiers precede the val/var keyword.
  - `test_protected_var_visibility(self, extractor, kotlin_parser)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L157)
  - `test_public_val_is_val(self, extractor, kotlin_parser)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L179) — val without modifiers: is_val=True, is_var=False.

### `TestBug761ConstructorReturnType`
- def: [`tests/unit/languages/test_kotlin_fixes_759_760_761.py:276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L276)
- doc: Primary constructors must have return_type=None.
- signature: `class TestBug761ConstructorReturnType:`
- members:
  - `test_primary_constructor_data_class_return_type_none(self, extractor, kotlin_parser)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L304)
  - `test_primary_constructor_is_constructor_true(self, extractor, kotlin_parser)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L316) — is_constructor flag must be set.
  - `test_primary_constructor_return_type_none(self, extractor, kotlin_parser)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L279)
  - `test_primary_constructor_with_visibility_return_type_none(self, extractor, kotlin_parser)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L291) — Even with explicit `constructor` keyword and visibility, return_type=None.
  - `test_regular_functions_not_affected(self, extractor, kotlin_parser)` — [`L327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L327) — Regular functions should keep their return_type (not None).

## Functions
- `extractor()` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L28)
- `kotlin_parser()` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_kotlin_fixes_759_760_761.py#L22)

