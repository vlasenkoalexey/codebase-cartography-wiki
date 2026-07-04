---
title: 'Module: tests/unit/test_multilang_extraction_activation.py'
type: catalog
provenance: extracted
module: tests/unit/test_multilang_extraction_activation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_multilang_extraction_activation`/
symbols:
  test_extraction_produces_edges_and_moat_holds: test_extraction_produces_edges_and_moat_holds().
  test_csharp_extraction_and_moat: test_csharp_extraction_and_moat().
  test_language_wired_into_extraction: test_language_wired_into_extraction().
  test_php_scoped_call_keeps_scope: test_php_scoped_call_keeps_scope().
  _ADVANCED_LANGUAGE_FIXTURES: _ADVANCED_LANGUAGE_FIXTURES.
  test_advanced_elements_carry_analyzer_language_not_unknown: test_advanced_elements_carry_analyzer_language_not_unknown().
  test_advanced_backfill_preserves_markdown_embedded_languages: test_advanced_backfill_preserves_markdown_embedded_languages().
  _CORPUS: _CORPUS.
---
# Module: [`tests/unit/test_multilang_extraction_activation.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_multilang_extraction_activation.py)

## Functions
- `test_advanced_backfill_preserves_markdown_embedded_languages()` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_multilang_extraction_activation.py#L70) — #1019 guard: the backfill must NOT overwrite a Markdown fenced block's
- `test_advanced_elements_carry_analyzer_language_not_unknown(lang: str, path: str)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_multilang_extraction_activation.py#L47) — #1019: every real element reports the analyzer language, 0 "unknown".
- `test_csharp_extraction_and_moat()` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_multilang_extraction_activation.py#L141) — C# end-to-end moat (PR #360 review P2): index a .cs file + a Python shadow;
- `test_extraction_produces_edges_and_moat_holds(lang: str, ext: str)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_multilang_extraction_activation.py#L95) — A real index of a corpus file + a Python shadow: the language's call edges
- `test_language_wired_into_extraction(lang: str)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_multilang_extraction_activation.py#L87)
- `test_php_scoped_call_keeps_scope()` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_multilang_extraction_activation.py#L123) — P1 regression (PR #360 review): a PHP static call ``Class::method()`` must

## Module values
- `_ADVANCED_LANGUAGE_FIXTURES` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_multilang_extraction_activation.py#L38)
- `_CORPUS` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_multilang_extraction_activation.py#L22)

