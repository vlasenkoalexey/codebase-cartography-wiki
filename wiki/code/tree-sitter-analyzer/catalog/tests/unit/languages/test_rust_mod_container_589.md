---
title: 'Module: tests/unit/languages/test_rust_mod_container_589.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_rust_mod_container_589.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_rust_mod_container_589`/
symbols:
  test_named_mod_extracted_as_package: test_named_mod_extracted_as_package().
  test_analyze_file_includes_package_element: test_analyze_file_includes_package_element().
  test_nested_items_still_extracted: test_nested_items_still_extracted().
  test_empty_mod_extracted: test_empty_mod_extracted().
  test_declaration_only_mod_emitted_with_declaration_span: test_declaration_only_mod_emitted_with_declaration_span().
  test_nested_mods_both_extracted: test_nested_mods_both_extracted().
  test_plugin_extract_elements_carries_packages_key: test_plugin_extract_elements_carries_packages_key().
  _parse: _parse().
  NAMED_MOD_SRC: NAMED_MOD_SRC.
  test_nameless_mod_node_yields_none: test_nameless_mod_node_yields_none().
  test_exploding_mod_node_yields_none: test_exploding_mod_node_yields_none().
  pytestmark: pytestmark.
  _rust_lang: _rust_lang().
  _NamelessModNode: _NamelessModNode#
  _ExplodingModNode: _ExplodingModNode#
  _NamelessModNode.type: _NamelessModNode#type.
  _NamelessModNode.parent: _NamelessModNode#parent.
  _NamelessModNode.children: _NamelessModNode#children.
  _NamelessModNode.child_by_field_name: _NamelessModNode#child_by_field_name().
  _ExplodingModNode.type: _ExplodingModNode#type.
  _ExplodingModNode.parent: _ExplodingModNode#parent.
  _ExplodingModNode.children: _ExplodingModNode#children.
  _ExplodingModNode.child_by_field_name: _ExplodingModNode#child_by_field_name().
---
# Module: [`tests/unit/languages/test_rust_mod_container_589.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py)

## Classes
### `_ExplodingModNode`
- def: [`tests/unit/languages/test_rust_mod_container_589.py:141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L141)
- doc: Stub mod_item whose name lookup raises (defensive except branch).
- signature: `class _ExplodingModNode:`
- members:
  - `child_by_field_name(self, _field: str)` — [`L148`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L148)
  - `children` — [`L146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L146)
  - `parent` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L145)
  - `type` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L144)
- used by: (1 test-only callers)

### `_NamelessModNode`
- def: [`tests/unit/languages/test_rust_mod_container_589.py:130`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L130)
- doc: Stub mod_item with no name field (grammar ERROR recovery shape).
- signature: `class _NamelessModNode:`
- members:
  - `child_by_field_name(self, _field: str)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L137)
  - `children` — [`L135`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L135)
  - `parent` — [`L134`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L134)
  - `type` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L133)
- used by: (1 test-only callers)

## Functions
- `_parse(src: str)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L39)
- `_rust_lang()` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L23)
- `test_analyze_file_includes_package_element(tmp_path)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L175) — analyze_file surfaces the mod container in the flat element list.
- `test_declaration_only_mod_emitted_with_declaration_span()` — [`L104`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L104) — ``mod tests;`` (body=None) is emitted; span == the declaration line.
- `test_empty_mod_extracted()` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L91) — ``mod empty {}`` still emits its container.
- `test_exploding_mod_node_yields_none()` — [`L158`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L158)
- `test_named_mod_extracted_as_package()` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L58) — A named mod block must yield exactly one Package-like container.
- `test_nameless_mod_node_yields_none()` — [`L152`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L152)
- `test_nested_items_still_extracted()` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L75) — Items inside the mod stay owned/extracted exactly as before.
- `test_nested_mods_both_extracted()` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L117) — Nested mod blocks each emit a container.
- `test_plugin_extract_elements_carries_packages_key()` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L164) — RustPlugin.extract_elements exposes the 'packages' group (go/kotlin parity).

## Module values
- `NAMED_MOD_SRC` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L45)
- `pytestmark` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_rust_mod_container_589.py#L33)

