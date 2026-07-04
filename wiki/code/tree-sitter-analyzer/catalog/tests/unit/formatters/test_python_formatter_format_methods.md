---
title: 'Module: tests/unit/formatters/test_python_formatter_format_methods.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_python_formatter_format_methods.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_python_formatter_format_methods`/TestPythonFormatter
symbols:
  TestPythonFormatterFormatSummary.formatter: FormatSummary#formatter().
  TestPythonFormatterFormatAdvanced.formatter: FormatAdvanced#formatter().
  TestPythonFormatterFullTable.formatter: FullTable#formatter().
  TestPythonFormatterCompactTable.formatter: CompactTable#formatter().
  TestPythonFormatterCreateCompactSignature.formatter: CreateCompactSignature#formatter().
  TestPythonFormatterFormatTableMethod.formatter: FormatTableMethod#formatter().
  TestPythonFormatterFormatJsonError.formatter: FormatJsonError#formatter().
  TestPythonFormatterFormatPythonSignature.formatter: FormatPythonSignature#formatter().
  TestPythonFormatterVisibilitySymbol.formatter: VisibilitySymbol#formatter().
  TestPythonFormatterDecoratorsEdge.formatter: DecoratorsEdge#formatter().
  TestPythonFormatterClassMethodRow.formatter: ClassMethodRow#formatter().
  TestPythonFormatterSignatureCompact.formatter: SignatureCompact#formatter().
  TestPythonFormatterFormatSummary: FormatSummary#
  TestPythonFormatterFormatSummary.test_format_summary: FormatSummary#test_format_summary().
  TestPythonFormatterFormatAdvanced: FormatAdvanced#
  TestPythonFormatterFormatAdvanced.test_format_advanced_json: FormatAdvanced#test_format_advanced_json().
  TestPythonFormatterFormatAdvanced.test_format_advanced_csv: FormatAdvanced#test_format_advanced_csv().
  TestPythonFormatterFormatAdvanced.test_format_advanced_fallback_to_full: FormatAdvanced#test_format_advanced_fallback_to_full().
  TestPythonFormatterFullTable: FullTable#
  TestPythonFormatterFullTable.test_full_table_none_data: FullTable#test_full_table_none_data().
  TestPythonFormatterFullTable.test_full_table_invalid_type: FullTable#test_full_table_invalid_type().
  TestPythonFormatterFullTable.test_full_table_none_file_path: FullTable#test_full_table_none_file_path().
  TestPythonFormatterFullTable.test_full_table_with_package: FullTable#test_full_table_with_package().
  TestPythonFormatterFullTable.test_full_table_with_imports: FullTable#test_full_table_with_imports().
  TestPythonFormatterFullTable.test_full_table_single_class_with_methods: FullTable#test_full_table_single_class_with_methods().
  TestPythonFormatterFullTable.test_full_table_multiple_classes: FullTable#test_full_table_multiple_classes().
  TestPythonFormatterFullTable.test_full_table_per_class_sections: FullTable#test_full_table_per_class_sections().
  TestPythonFormatterCompactTable: CompactTable#
  TestPythonFormatterCompactTable.test_compact_table_basic: CompactTable#test_compact_table_basic().
  TestPythonFormatterCompactTable.test_compact_table_with_methods: CompactTable#test_compact_table_with_methods().
  TestPythonFormatterCompactTable.test_compact_table_with_classes: CompactTable#test_compact_table_with_classes().
  TestPythonFormatterCompactTable.test_compact_table_with_none_class: CompactTable#test_compact_table_with_none_class().
  TestPythonFormatterCreateCompactSignature: CreateCompactSignature#
  TestPythonFormatterCreateCompactSignature.test_compact_signature_none_method: CreateCompactSignature#test_compact_signature_none_method().
  TestPythonFormatterCreateCompactSignature.test_compact_signature_invalid_type: CreateCompactSignature#test_compact_signature_invalid_type().
  TestPythonFormatterCreateCompactSignature.test_compact_signature_string_params: CreateCompactSignature#test_compact_signature_string_params().
  TestPythonFormatterCreateCompactSignature.test_compact_signature_none_type: CreateCompactSignature#test_compact_signature_none_type().
  TestPythonFormatterFormatTableMethod: FormatTableMethod#
  TestPythonFormatterFormatTableMethod.test_format_table_restores_format_type: FormatTableMethod#test_format_table_restores_format_type().
  TestPythonFormatterFormatJsonError: FormatJsonError#
  TestPythonFormatterFormatJsonError.test_format_json_with_set: FormatJsonError#test_format_json_with_set().
  TestPythonFormatterFormatPythonSignature: FormatPythonSignature#
  TestPythonFormatterFormatPythonSignature.test_python_signature_with_return_type: FormatPythonSignature#test_python_signature_with_return_type().
  TestPythonFormatterFormatPythonSignature.test_python_signature_no_return_type: FormatPythonSignature#test_python_signature_no_return_type().
  TestPythonFormatterFormatPythonSignature.test_python_signature_none_params: FormatPythonSignature#test_python_signature_none_params().
  TestPythonFormatterVisibilitySymbol: VisibilitySymbol#
  TestPythonFormatterVisibilitySymbol.test_visibility_public: VisibilitySymbol#test_visibility_public().
  TestPythonFormatterVisibilitySymbol.test_visibility_private: VisibilitySymbol#test_visibility_private().
  TestPythonFormatterVisibilitySymbol.test_visibility_protected: VisibilitySymbol#test_visibility_protected().
  TestPythonFormatterVisibilitySymbol.test_visibility_magic: VisibilitySymbol#test_visibility_magic().
  TestPythonFormatterVisibilitySymbol.test_visibility_unknown: VisibilitySymbol#test_visibility_unknown().
  TestPythonFormatterDecoratorsEdge: DecoratorsEdge#
  TestPythonFormatterDecoratorsEdge.test_decorators_important_classmethod: DecoratorsEdge#test_decorators_important_classmethod().
  TestPythonFormatterDecoratorsEdge.test_decorators_important_abstractmethod: DecoratorsEdge#test_decorators_important_abstractmethod().
  TestPythonFormatterDecoratorsEdge.test_decorators_important_dataclass: DecoratorsEdge#test_decorators_important_dataclass().
  TestPythonFormatterDecoratorsEdge.test_decorators_important_property: DecoratorsEdge#test_decorators_important_property().
  TestPythonFormatterDecoratorsEdge.test_decorators_multiple_with_plus: DecoratorsEdge#test_decorators_multiple_with_plus().
  TestPythonFormatterClassMethodRow: ClassMethodRow#
  TestPythonFormatterClassMethodRow.test_class_method_row_basic: ClassMethodRow#test_class_method_row_basic().
  TestPythonFormatterClassMethodRow.test_class_method_row_static: ClassMethodRow#test_class_method_row_static().
  TestPythonFormatterClassMethodRow.test_class_method_row_magic: ClassMethodRow#test_class_method_row_magic().
  TestPythonFormatterClassMethodRow.test_class_method_row_private: ClassMethodRow#test_class_method_row_private().
  TestPythonFormatterClassMethodRow.test_class_method_row_malformed_line_range: ClassMethodRow#test_class_method_row_malformed_line_range().
  TestPythonFormatterClassMethodRow.test_class_method_row_with_docstring: ClassMethodRow#test_class_method_row_with_docstring().
  TestPythonFormatterSignatureCompact: SignatureCompact#
  TestPythonFormatterSignatureCompact.test_python_signature_compact_with_return: SignatureCompact#test_python_signature_compact_with_return().
  TestPythonFormatterSignatureCompact.test_python_signature_compact_no_return: SignatureCompact#test_python_signature_compact_no_return().
  TestPythonFormatterSignatureCompact.test_python_signature_compact_none_params: SignatureCompact#test_python_signature_compact_none_params().
---
# Module: [`tests/unit/formatters/test_python_formatter_format_methods.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py)

## Classes
### `TestPythonFormatterClassMethodRow`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:483`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L483)
- doc: Test _format_class_method_row
- signature: `class TestPythonFormatterClassMethodRow:`
- members:
  - `formatter(self)` — [`L487`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L487)
  - `test_class_method_row_basic(self, formatter)` — [`L490`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L490)
  - `test_class_method_row_magic(self, formatter)` — [`L518`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L518)
  - `test_class_method_row_malformed_line_range(self, formatter)` — [`L544`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L544)
  - `test_class_method_row_private(self, formatter)` — [`L531`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L531)
  - `test_class_method_row_static(self, formatter)` — [`L504`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L504)
  - `test_class_method_row_with_docstring(self, formatter)` — [`L557`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L557)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterCompactTable`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L259)
- doc: Test _format_compact_table
- signature: `class TestPythonFormatterCompactTable:`
- members:
  - `formatter(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L263)
  - `test_compact_table_basic(self, formatter)` — [`L266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L266)
  - `test_compact_table_with_classes(self, formatter)` — [`L301`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L301)
  - `test_compact_table_with_methods(self, formatter)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L278)
  - `test_compact_table_with_none_class(self, formatter)` — [`L316`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L316)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterCreateCompactSignature`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L336)
- doc: Test _create_compact_signature edge cases
- signature: `class TestPythonFormatterCreateCompactSignature:`
- members:
  - `formatter(self)` — [`L340`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L340)
  - `test_compact_signature_invalid_type(self, formatter)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L347)
  - `test_compact_signature_none_method(self, formatter)` — [`L343`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L343)
  - `test_compact_signature_none_type(self, formatter)` — [`L360`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L360)
  - `test_compact_signature_string_params(self, formatter)` — [`L351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L351)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterDecoratorsEdge`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:455`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L455)
- doc: Test _format_decorators edge cases
- signature: `class TestPythonFormatterDecoratorsEdge:`
- members:
  - `formatter(self)` — [`L459`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L459)
  - `test_decorators_important_abstractmethod(self, formatter)` — [`L466`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L466)
  - `test_decorators_important_classmethod(self, formatter)` — [`L462`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L462)
  - `test_decorators_important_dataclass(self, formatter)` — [`L470`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L470)
  - `test_decorators_important_property(self, formatter)` — [`L474`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L474)
  - `test_decorators_multiple_with_plus(self, formatter)` — [`L478`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L478)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFormatAdvanced`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L31)
- doc: Test format_advanced with different output formats
- signature: `class TestPythonFormatterFormatAdvanced:`
- members:
  - `formatter(self)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L35)
  - `test_format_advanced_csv(self, formatter)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L43)
  - `test_format_advanced_fallback_to_full(self, formatter)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L48)
  - `test_format_advanced_json(self, formatter)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L38)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFormatJsonError`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:384`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L384)
- doc: Test _format_json error path
- signature: `class TestPythonFormatterFormatJsonError:`
- members:
  - `formatter(self)` — [`L388`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L388)
  - `test_format_json_with_set(self, formatter)` — [`L391`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L391)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFormatPythonSignature`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:397`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L397)
- doc: Test _format_python_signature
- signature: `class TestPythonFormatterFormatPythonSignature:`
- members:
  - `formatter(self)` — [`L401`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L401)
  - `test_python_signature_no_return_type(self, formatter)` — [`L413`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L413)
  - `test_python_signature_none_params(self, formatter)` — [`L422`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L422)
  - `test_python_signature_with_return_type(self, formatter)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L404)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFormatSummary`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:6`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L6)
- doc: Test format_summary delegates to compact table
- signature: `class TestPythonFormatterFormatSummary:`
- members:
  - `formatter(self)` — [`L10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L10)
  - `test_format_summary(self, formatter)` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L13)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFormatTableMethod`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:370`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L370)
- doc: Test format_table method
- signature: `class TestPythonFormatterFormatTableMethod:`
- members:
  - `formatter(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L374)
  - `test_format_table_restores_format_type(self, formatter)` — [`L377`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L377)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFullTable`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L61)
- doc: Test _format_full_table variants
- signature: `class TestPythonFormatterFullTable:`
- members:
  - `formatter(self)` — [`L65`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L65)
  - `test_full_table_invalid_type(self, formatter)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L72)
  - `test_full_table_multiple_classes(self, formatter)` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L181)
  - `test_full_table_none_data(self, formatter)` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L68)
  - `test_full_table_none_file_path(self, formatter)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L76)
  - `test_full_table_per_class_sections(self, formatter)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L209)
  - `test_full_table_single_class_with_methods(self, formatter)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L131)
  - `test_full_table_with_imports(self, formatter)` — [`L107`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L107)
  - `test_full_table_with_package(self, formatter)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L87)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterSignatureCompact`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:571`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L571)
- doc: Test _format_python_signature_compact
- signature: `class TestPythonFormatterSignatureCompact:`
- members:
  - `formatter(self)` — [`L575`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L575)
  - `test_python_signature_compact_no_return(self, formatter)` — [`L587`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L587)
  - `test_python_signature_compact_none_params(self, formatter)` — [`L596`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L596)
  - `test_python_signature_compact_with_return(self, formatter)` — [`L578`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L578)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterVisibilitySymbol`
- def: [`tests/unit/formatters/test_python_formatter_format_methods.py:432`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L432)
- doc: Test _get_python_visibility_symbol
- signature: `class TestPythonFormatterVisibilitySymbol:`
- members:
  - `formatter(self)` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L436)
  - `test_visibility_magic(self, formatter)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L448)
  - `test_visibility_private(self, formatter)` — [`L442`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L442)
  - `test_visibility_protected(self, formatter)` — [`L445`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L445)
  - `test_visibility_public(self, formatter)` — [`L439`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L439)
  - `test_visibility_unknown(self, formatter)` — [`L451`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_format_methods.py#L451)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

