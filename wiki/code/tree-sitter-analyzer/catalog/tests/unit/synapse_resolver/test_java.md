---
title: 'Module: tests/unit/synapse_resolver/test_java.py'
type: catalog
provenance: extracted
module: tests/unit/synapse_resolver/test_java.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.synapse_resolver.test_java`/
symbols:
  TestParseJavaImports.test_single_type_import: TestParseJavaImports#test_single_type_import().
  _build_two_file_ctx: _build_two_file_ctx().
  TestParseJavaImports.test_wildcard_import: TestParseJavaImports#test_wildcard_import().
  TestParseJavaImports.test_package_declaration: TestParseJavaImports#test_package_declaration().
  TestParseJavaImports.test_static_member_import: TestParseJavaImports#test_static_member_import().
  TestParseJavaImports.test_static_wildcard_import: TestParseJavaImports#test_static_wildcard_import().
  TestResolveJavaCallee.test_same_package_resolution: TestResolveJavaCallee#test_same_package_resolution().
  TestResolveJavaCallee.test_local_implicit_this: TestResolveJavaCallee#test_local_implicit_this().
  TestResolveJavaCallee.test_this_qualified: TestResolveJavaCallee#test_this_qualified().
  TestResolveJavaCallee.test_type_import_cross_file: TestResolveJavaCallee#test_type_import_cross_file().
  TestResolveJavaCallee.test_jdk_receiver_is_external: TestResolveJavaCallee#test_jdk_receiver_is_external().
  TestResolveJavaCallee.test_java_lang_simple_type_external: TestResolveJavaCallee#test_java_lang_simple_type_external().
  TestResolveJavaCallee.test_single_global_unqualified: TestResolveJavaCallee#test_single_global_unqualified().
  TestResolveJavaCallee.test_unknown_instance_receiver: TestResolveJavaCallee#test_unknown_instance_receiver().
  TestParseJavaImports.test_non_import_returns_empty: TestParseJavaImports#test_non_import_returns_empty().
  TestParseJavaImports: TestParseJavaImports#
  TestResolveJavaCallee: TestResolveJavaCallee#
---
# Module: [`tests/unit/synapse_resolver/test_java.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py)

## Classes
### `TestParseJavaImports`
- def: [`tests/unit/synapse_resolver/test_java.py:25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L25)
- signature: `class TestParseJavaImports:`
- members:
  - `test_non_import_returns_empty(self, text: str)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L67)
  - `test_package_declaration(self)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L26)
  - `test_single_type_import(self)` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L32)
  - `test_static_member_import(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L54)
  - `test_static_wildcard_import(self)` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L60)
  - `test_wildcard_import(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L47)
- uses (calls/refs, reference-scoped): [`parse_java_imports`](../../../tree_sitter_analyzer/synapse_resolver/_java.md#parse_java_imports), [`local_name`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.local_name), [`ImportEntry`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry), [`module_path`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.module_path), [`is_relative`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.is_relative), [`is_star`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.is_star), [`alias_of`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.alias_of), [`file_path`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.file_path), [`language`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.language), [`line`](../../../tree_sitter_analyzer/synapse_resolver/_imports.md#ImportEntry.line)

### `TestResolveJavaCallee`
- def: [`tests/unit/synapse_resolver/test_java.py:115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L115)
- signature: `class TestResolveJavaCallee:`
- members:
  - `test_java_lang_simple_type_external(self)` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L146)
  - `test_jdk_receiver_is_external(self)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L138)
  - `test_local_implicit_this(self)` — [`L116`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L116)
  - `test_same_package_resolution(self)` — [`L169`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L169)
  - `test_single_global_unqualified(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L153)
  - `test_this_qualified(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L124)
  - `test_type_import_cross_file(self)` — [`L132`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L132)
  - `test_unknown_instance_receiver(self)` — [`L161`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L161)
- uses (calls/refs, reference-scoped): [`resolve_java_callee`](../../../tree_sitter_analyzer/synapse_resolver/_java.md#resolve_java_callee), [`build_java_context`](../../../tree_sitter_analyzer/synapse_resolver/_java.md#build_java_context), [`parse_java_imports`](../../../tree_sitter_analyzer/synapse_resolver/_java.md#parse_java_imports)  (1 test-only)

## Functions
- `_build_two_file_ctx()` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/synapse_resolver/test_java.py#L76) — Service.java (pkg com.acme.svc) imports Helper from com.acme.util.

