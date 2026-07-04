---
title: 'Module: tree_sitter_analyzer/import_extractors/_other_langs.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/import_extractors/_other_langs.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.import_extractors._other_langs`/_
symbols:
  _extract_ruby_imports: extract_ruby_imports().
  _extract_csharp_imports: extract_csharp_imports().
  _extract_kotlin_imports: extract_kotlin_imports().
  _extract_swift_imports: extract_swift_imports().
  _extract_php_imports: extract_php_imports().
  _csharp_qualified_name_parts: csharp_qualified_name_parts().
  _ruby_call_function_name: ruby_call_function_name().
  _ruby_call_string_arg: ruby_call_string_arg().
  _CSHARP_STD_NAMESPACES: CSHARP_STD_NAMESPACES.
  _KOTLIN_STD_ROOTS: KOTLIN_STD_ROOTS.
  _SWIFT_STD_MODULES: SWIFT_STD_MODULES.
  _RUBY_STDLIB: RUBY_STDLIB.
---
# Module: [`tree_sitter_analyzer/import_extractors/_other_langs.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py)

## Functions
- `_csharp_qualified_name_parts(node: Any, source: str)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L132) — Collect identifier parts from a C# qualified_name node.
- `_extract_csharp_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L141) — Extract C# using directives.
- `_extract_kotlin_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L182) — Extract Kotlin import declarations.
- `_extract_php_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L314`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L314) — Extract PHP use declarations (namespace imports).
- `_extract_ruby_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L280) — Extract Ruby require/require_relative calls.
- `_extract_swift_imports(node: Any, source: str, imports: list[dict[str, Any]])` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L223) — Extract Swift import declarations.
- `_ruby_call_function_name(node: Any, source: str)` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L254) — Return the function-name text from a Ruby ``call`` node, or ``None``.
- `_ruby_call_string_arg(node: Any, source: str)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L264) — Return the first ``string``/``string_content`` arg text (quotes stripped).

## Module values
- `_CSHARP_STD_NAMESPACES` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L7)
- `_KOTLIN_STD_ROOTS` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L42)
- `_RUBY_STDLIB` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L81)
- `_SWIFT_STD_MODULES` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_extractors/_other_langs.py#L49)

