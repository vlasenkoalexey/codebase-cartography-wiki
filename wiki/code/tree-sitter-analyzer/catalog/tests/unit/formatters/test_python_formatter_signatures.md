---
title: 'Module: tests/unit/formatters/test_python_formatter_signatures.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_python_formatter_signatures.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_python_formatter_signatures`/TestPythonFormatter
symbols:
  TestPythonFormatterFormatPythonSignature.formatter: FormatPythonSignature#formatter().
  TestPythonFormatterVisibilitySymbol.formatter: VisibilitySymbol#formatter().
  TestPythonFormatterDecoratorsEdge.formatter: DecoratorsEdge#formatter().
  TestPythonFormatterClassMethodRow.formatter: ClassMethodRow#formatter().
  TestPythonFormatterSignatureCompact.formatter: SignatureCompact#formatter().
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
# Module: [`tests/unit/formatters/test_python_formatter_signatures.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py)

## Classes
### `TestPythonFormatterClassMethodRow`
- def: [`tests/unit/formatters/test_python_formatter_signatures.py:96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L96)
- doc: Test _format_class_method_row
- signature: `class TestPythonFormatterClassMethodRow:`
- members:
  - `formatter(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L100)
  - `test_class_method_row_basic(self, formatter)` — [`L103`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L103)
  - `test_class_method_row_magic(self, formatter)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L131)
  - `test_class_method_row_malformed_line_range(self, formatter)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L157)
  - `test_class_method_row_private(self, formatter)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L144)
  - `test_class_method_row_static(self, formatter)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L117)
  - `test_class_method_row_with_docstring(self, formatter)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L170)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterDecoratorsEdge`
- def: [`tests/unit/formatters/test_python_formatter_signatures.py:68`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L68)
- doc: Test _format_decorators edge cases
- signature: `class TestPythonFormatterDecoratorsEdge:`
- members:
  - `formatter(self)` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L72)
  - `test_decorators_important_abstractmethod(self, formatter)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L79)
  - `test_decorators_important_classmethod(self, formatter)` — [`L75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L75)
  - `test_decorators_important_dataclass(self, formatter)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L83)
  - `test_decorators_important_property(self, formatter)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L87)
  - `test_decorators_multiple_with_plus(self, formatter)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L91)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterFormatPythonSignature`
- def: [`tests/unit/formatters/test_python_formatter_signatures.py:10`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L10)
- doc: Test _format_python_signature
- signature: `class TestPythonFormatterFormatPythonSignature:`
- members:
  - `formatter(self)` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L14)
  - `test_python_signature_no_return_type(self, formatter)` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L26)
  - `test_python_signature_none_params(self, formatter)` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L35)
  - `test_python_signature_with_return_type(self, formatter)` — [`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L17)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterSignatureCompact`
- def: [`tests/unit/formatters/test_python_formatter_signatures.py:184`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L184)
- doc: Test _format_python_signature_compact
- signature: `class TestPythonFormatterSignatureCompact:`
- members:
  - `formatter(self)` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L188)
  - `test_python_signature_compact_no_return(self, formatter)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L200)
  - `test_python_signature_compact_none_params(self, formatter)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L209)
  - `test_python_signature_compact_with_return(self, formatter)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L191)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

### `TestPythonFormatterVisibilitySymbol`
- def: [`tests/unit/formatters/test_python_formatter_signatures.py:45`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L45)
- doc: Test _get_python_visibility_symbol
- signature: `class TestPythonFormatterVisibilitySymbol:`
- members:
  - `formatter(self)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L49)
  - `test_visibility_magic(self, formatter)` — [`L61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L61)
  - `test_visibility_private(self, formatter)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L55)
  - `test_visibility_protected(self, formatter)` — [`L58`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L58)
  - `test_visibility_public(self, formatter)` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L52)
  - `test_visibility_unknown(self, formatter)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_python_formatter_signatures.py#L64)
- uses (calls/refs, reference-scoped): [`PythonTableFormatter`](../../../tree_sitter_analyzer/formatters/python_formatter.md#PythonTableFormatter)

