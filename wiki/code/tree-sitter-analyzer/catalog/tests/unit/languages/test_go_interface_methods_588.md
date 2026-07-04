---
title: 'Module: tests/unit/languages/test_go_interface_methods_588.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_go_interface_methods_588.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_go_interface_methods_588`/
symbols:
  TestReaderInterfaceMethod.test_read_signature_extracted_and_owned: TestReaderInterfaceMethod#test_read_signature_extracted_and_owned().
  _extract: _extract().
  TestAliasToInterface.test_alias_interface_method_owned: TestAliasToInterface#test_alias_interface_method_owned().
  TestGuardBranches._node: TestGuardBranches#_node().
  TestReaderInterfaceMethod.test_interface_class_still_extracted: TestReaderInterfaceMethod#test_interface_class_still_extracted().
  TestReadWriterEmbeddingNoPhantoms.test_no_phantom_methods: TestReadWriterEmbeddingNoPhantoms#test_no_phantom_methods().
  TestReadWriterEmbeddingNoPhantoms.test_embedding_still_reflected: TestReadWriterEmbeddingNoPhantoms#test_embedding_still_reflected().
  TestAnonymousInterfaceParamIgnored.test_only_the_real_function_extracted: TestAnonymousInterfaceParamIgnored#test_only_the_real_function_extracted().
  TestReaderInterfaceMethod._parsed: TestReaderInterfaceMethod#_parsed().
  TestGuardBranches._extract: TestGuardBranches#_extract().
  TestEmptyInterface.test_no_methods: TestEmptyInterface#test_no_methods().
  TestGuardBranches.test_missing_name_or_type_field_returns_empty: TestGuardBranches#test_missing_name_or_type_field_returns_empty().
  TestGuardBranches.test_non_interface_type_spec_returns_empty: TestGuardBranches#test_non_interface_type_spec_returns_empty().
  TestGuardBranches.test_empty_interface_name_text_returns_empty: TestGuardBranches#test_empty_interface_name_text_returns_empty().
  TestGuardBranches.test_nameless_method_elem_skipped: TestGuardBranches#test_nameless_method_elem_skipped().
  TestGuardBranches.test_exception_returns_empty: TestGuardBranches#test_exception_returns_empty().
  TestReadWriterEmbeddingNoPhantoms.SRC: TestReadWriterEmbeddingNoPhantoms#SRC.
  TestReaderInterfaceMethod.SRC: TestReaderInterfaceMethod#SRC.
  TestAnonymousInterfaceParamIgnored.SRC: TestAnonymousInterfaceParamIgnored#SRC.
  TestAliasToInterface.SRC: TestAliasToInterface#SRC.
  TestReaderInterfaceMethod: TestReaderInterfaceMethod#
  TestReadWriterEmbeddingNoPhantoms: TestReadWriterEmbeddingNoPhantoms#
  TestEmptyInterface: TestEmptyInterface#
  TestAnonymousInterfaceParamIgnored: TestAnonymousInterfaceParamIgnored#
  TestGuardBranches: TestGuardBranches#
  TestAliasToInterface: TestAliasToInterface#
---
# Module: [`tests/unit/languages/test_go_interface_methods_588.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py)

## Classes
### `TestAliasToInterface`
- def: [`tests/unit/languages/test_go_interface_methods_588.py:188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L188)
- doc: `type R = interface{ M() }` (type_alias) also owns its signatures.
- signature: `class TestAliasToInterface:`
- members:
  - `test_alias_interface_method_owned(self)` — [`L193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L193)
  - `SRC` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L191)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method)  (1 test-only)

### `TestAnonymousInterfaceParamIgnored`
- def: [`tests/unit/languages/test_go_interface_methods_588.py:100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L100)
- doc: An anonymous `interface{ ... }` in a parameter is NOT a named owner.
- signature: `class TestAnonymousInterfaceParamIgnored:`
- members:
  - `test_only_the_real_function_extracted(self)` — [`L110`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L110)
  - `SRC` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L103)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name)  (1 test-only)

### `TestEmptyInterface`
- def: [`tests/unit/languages/test_go_interface_methods_588.py:90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L90)
- doc: `type Empty interface {}` emits no functions.
- signature: `class TestEmptyInterface:`
- members:
  - `test_no_methods(self)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L93)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name)  (1 test-only)

### `TestGuardBranches`
- def: [`tests/unit/languages/test_go_interface_methods_588.py:115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L115)
- doc: Defensive guards in extract_go_interface_methods (direct unit calls).
- signature: `class TestGuardBranches:`
- members:
  - `test_empty_interface_name_text_returns_empty(self)` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L150)
  - `test_exception_returns_empty(self)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L175)
  - `test_missing_name_or_type_field_returns_empty(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L136)
  - `test_nameless_method_elem_skipped(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L161)
  - `test_non_interface_type_spec_returns_empty(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L140)
- protocol/private: `_extract`[`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L129), `_node`[`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L119)
- uses (calls/refs, reference-scoped): [`extract_go_interface_methods`](../../../tree_sitter_analyzer/languages/_go_function_helpers.md#extract_go_interface_methods)

### `TestReadWriterEmbeddingNoPhantoms`
- def: [`tests/unit/languages/test_go_interface_methods_588.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L75)
- doc: Embedding-only interface: embeds preserved, zero phantom methods.
- signature: `class TestReadWriterEmbeddingNoPhantoms:`
- members:
  - `test_embedding_still_reflected(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L84)
  - `test_no_phantom_methods(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L80)
  - `SRC` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L78)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`interfaces`](../../../tree_sitter_analyzer/models/base.md#Class.interfaces)  (1 test-only)

### `TestReaderInterfaceMethod`
- def: [`tests/unit/languages/test_go_interface_methods_588.py:37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L37)
- doc: Single-method interface: signature fully extracted and owned.
- signature: `class TestReaderInterfaceMethod:`
- members:
  - `test_interface_class_still_extracted(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L65)
  - `test_read_signature_extracted_and_owned(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L50)
  - `SRC` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L40)
- protocol/private: `_parsed`[`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L71)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Function.parameters), [`return_type`](../../../tree_sitter_analyzer/models/base.md#Function.return_type), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`visibility`](../../../tree_sitter_analyzer/models/base.md#Function.visibility), [`receiver_type`](../../../tree_sitter_analyzer/models/base.md#Function.receiver_type), [`is_method`](../../../tree_sitter_analyzer/models/base.md#Function.is_method), [`receiver`](../../../tree_sitter_analyzer/models/base.md#Function.receiver)  (1 test-only)

## Functions
- `_extract(src: str)` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_go_interface_methods_588.py#L20) — Run the Go plugin's function + class extraction over ``src``.

