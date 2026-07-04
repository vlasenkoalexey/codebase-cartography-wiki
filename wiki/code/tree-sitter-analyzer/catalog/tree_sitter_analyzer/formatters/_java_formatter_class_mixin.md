---
title: 'Module: tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._java_formatter_class_mixin`/
symbols:
  JavaTableFormatterClassMixin._format_class_section: JavaTableFormatterClassMixin#_format_class_section().
  _append_method_group: _append_method_group().
  JavaTableFormatterClassMixin: JavaTableFormatterClassMixin#
  _append_visibility_groups: _append_visibility_groups().
  get_class_methods: get_class_methods().
  get_class_fields: get_class_fields().
  is_inner_class: is_inner_class().
  JavaTableFormatterClassMixin._format_method_row: JavaTableFormatterClassMixin#_format_method_row().
  get_inner_classes: get_inner_classes().
  is_in_range: is_in_range().
  _append_fields: _append_fields().
  _field_row: _field_row().
  _exclude_inner_members: _exclude_inner_members().
  MethodSection: MethodSection#
  MethodSection.methods: MethodSection#methods.
  _members_in_range: _members_in_range().
  _clean_doc_cell: _clean_doc_cell().
  MethodSection.title: MethodSection#title.
  MethodSection.header: MethodSection#header.
  MethodSection.separator: MethodSection#separator.
  _constructor_methods: _constructor_methods().
  _non_constructor_methods: _non_constructor_methods().
  _method_groups: _method_groups().
  _is_contained: _is_contained().
  _range_contains: _range_contains().
---
# Module: [`tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py)

## Classes
### `JavaTableFormatterClassMixin`
- def: [`tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py:15`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L15)
- doc: Class, member, and range helpers.
- signature: `class JavaTableFormatterClassMixin:`
- members:
  - `_format_class_section(self, class_info: dict[str, Any], data: dict[str, Any], all_classes: list[dict[str, Any]])` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L18) — Format a single class section with its fields and methods
  - `_format_method_row(self, method: dict[str, Any])` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L58) — Format a method table row for Java (golden master format)
- uses (calls/refs, reference-scoped): [`JavaTableFormatter`](java_formatter.md#JavaTableFormatter), [`_append_method_group`](_java_formatter_class_mixin.md#_append_method_group), [`_append_visibility_groups`](_java_formatter_class_mixin.md#_append_visibility_groups), [`get_class_fields`](_java_formatter_class_mixin.md#get_class_fields), [`get_class_methods`](_java_formatter_class_mixin.md#get_class_methods), [`get_inner_classes`](_java_formatter_class_mixin.md#get_inner_classes), [`_append_fields`](_java_formatter_class_mixin.md#_append_fields), [`_exclude_inner_members`](_java_formatter_class_mixin.md#_exclude_inner_members), [`MethodSection`](_java_formatter_class_mixin.md#MethodSection), [`_clean_doc_cell`](_java_formatter_class_mixin.md#_clean_doc_cell), [`_constructor_methods`](_java_formatter_class_mixin.md#_constructor_methods), [`_non_constructor_methods`](_java_formatter_class_mixin.md#_non_constructor_methods)
- used by: [`JavaTableFormatter`](java_formatter.md#JavaTableFormatter)  (2 test-only)

### `MethodSection`  ·  implements/extends NamedTuple
- def: [`tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py:6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L6)
- doc: Rendered method section metadata.
- signature: `class MethodSection(NamedTuple):`
- members:
  - `header` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L10)
  - `methods` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L12)
  - `separator` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L11)
  - `title` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L9)
- used by: [`_format_class_section`](_java_formatter_class_mixin.md#JavaTableFormatterClassMixin._format_class_section), [`_append_method_group`](_java_formatter_class_mixin.md#_append_method_group), [`_append_visibility_groups`](_java_formatter_class_mixin.md#_append_visibility_groups)

## Functions
- `_append_fields(lines: list[str], class_fields: list[dict[str, Any]], formatter: Any)` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L74)
- `_append_method_group(lines: list[str], section: MethodSection, row_formatter: Any)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L140)
- `_append_visibility_groups(lines: list[str], methods: list[dict[str, Any]], row_formatter: Any)` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L108)
- `_clean_doc_cell(doc: str)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L255)
- `_constructor_methods(methods: list[dict[str, Any]])` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L88)
- `_exclude_inner_members(_formatter: Any, inner_classes: list[dict[str, Any]], class_methods: list[dict[str, Any]], class_fields: list[dict[str, Any]])` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L156)
- `_field_row(field: dict[str, Any], formatter: Any)` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L96)
- `_is_contained(class_info: dict[str, Any], parent_start: int, parent_end: int)` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L238)
- `_members_in_range(members: list[dict[str, Any]], class_range: dict[str, Any])` — [`L177`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L177)
- `_method_groups()` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L131)
- `_non_constructor_methods(methods: list[dict[str, Any]])` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L92)
- `_range_contains(parent: dict[str, Any], class_start: int, class_end: int)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L248)
- `get_class_fields(fields: list[dict[str, Any]], class_range: dict[str, Any])` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L196) — Get fields that belong to a class based on line range.
- `get_class_methods(methods: list[dict[str, Any]], class_range: dict[str, Any])` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L189) — Get methods that belong to a class based on line range.
- `get_inner_classes(parent_class: dict[str, Any], all_classes: list[dict[str, Any]])` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L203) — Get inner classes of a parent class.
- `is_in_range(item_range: dict[str, Any], container_range: dict[str, Any])` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L230) — Check if an item's line range is within a container's range.
- `is_inner_class(class_info: dict[str, Any], all_classes: list[dict[str, Any]])` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_java_formatter_class_mixin.py#L217) — Check if a class is an inner class of another class.

