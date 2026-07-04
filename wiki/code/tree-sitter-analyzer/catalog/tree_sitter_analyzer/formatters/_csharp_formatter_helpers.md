---
title: 'Module: tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.formatters._csharp_formatter_helpers`/
symbols:
  format_csharp_full_table: format_csharp_full_table().
  format_csharp_compact_table: format_csharp_compact_table().
  format_csharp_csv: format_csharp_csv().
  _append_class_sections: _append_class_sections().
  _append_class_methods: _append_class_methods().
  _append_method_group: _append_method_group().
  ClassMemberSelector: ClassMemberSelector.
  _append_compact_methods: _append_compact_methods().
  _append_class_fields: _append_class_fields().
  VisibilityConverter: VisibilityConverter.
  MethodRowFormatter: MethodRowFormatter.
  SignatureCreator: SignatureCreator.
  _append_compact_info: _append_compact_info().
  _append_csv_methods: _append_csv_methods().
  _append_classes_overview: _append_classes_overview().
  ModifierFormatter: ModifierFormatter.
  NamespaceExtractor: NamespaceExtractor.
  _append_file_header: _append_file_header().
  _append_imports: _append_imports().
  _append_csv_fields: _append_csv_fields().
  _append_class_heading: _append_class_heading().
  _group_methods_by_visibility: _group_methods_by_visibility().
---
# Module: [`tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py)

## Functions
- `_append_class_fields(lines: list[str], class_fields: list[dict[str, Any]], format_modifiers: ModifierFormatter, convert_visibility: VisibilityConverter)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L252)
- `_append_class_heading(lines: list[str], class_info: dict[str, Any], line_range: dict[str, int])` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L244)
- `_append_class_methods(lines: list[str], class_methods: list[dict[str, Any]], format_method_row: MethodRowFormatter)` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L281)
- `_append_class_sections(lines: list[str], classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]], get_class_methods: ClassMemberSelector, get_class_fields: ClassMemberSelector, format_modifiers: ModifierFormatter, convert_visibility: VisibilityConverter, format_method_row: MethodRowFormatter)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L223)
- `_append_classes_overview(lines: list[str], classes: list[dict[str, Any]], methods: list[dict[str, Any]], fields: list[dict[str, Any]], get_class_methods: ClassMemberSelector, get_class_fields: ClassMemberSelector)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L192)
- `_append_compact_info(lines: list[str], data: dict[str, Any], extract_namespace: NamespaceExtractor)` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L111)
- `_append_compact_methods(lines: list[str], methods: list[dict[str, Any]], create_compact_signature: SignatureCreator, convert_visibility: VisibilityConverter)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L127)
- `_append_csv_fields(lines: list[str], fields: list[dict[str, Any]])` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L153)
- `_append_csv_methods(lines: list[str], methods: list[dict[str, Any]], create_full_signature: SignatureCreator)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L168)
- `_append_file_header(lines: list[str], data: dict[str, Any])` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L90)
- `_append_imports(lines: list[str], imports: list[dict[str, Any]])` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L97)
- `_append_method_group(lines: list[str], title: str, first_column: str, methods: list[dict[str, Any]], format_method_row: MethodRowFormatter)` — [`L331`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L331)
- `_group_methods_by_visibility(class_methods: list[dict[str, Any]])` — [`L309`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L309)
- `format_csharp_compact_table(data: dict[str, Any], extract_namespace: NamespaceExtractor, create_compact_signature: SignatureCreator, convert_visibility: VisibilityConverter)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L55) — Format compact C# output.
- `format_csharp_csv(data: dict[str, Any], create_full_signature: SignatureCreator)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L76) — Format CSV C# output.
- `format_csharp_full_table(data: dict[str, Any], get_class_methods: ClassMemberSelector, get_class_fields: ClassMemberSelector, format_modifiers: ModifierFormatter, convert_visibility: VisibilityConverter, format_method_row: MethodRowFormatter)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L16) — Format full C# output while keeping section builders isolated.

## Module values
- `ClassMemberSelector` — [`L6`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L6)
- `MethodRowFormatter` — [`L11`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L11)
- `ModifierFormatter` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L9)
- `NamespaceExtractor` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L12)
- `SignatureCreator` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L13)
- `VisibilityConverter` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/formatters/_csharp_formatter_helpers.py#L10)

