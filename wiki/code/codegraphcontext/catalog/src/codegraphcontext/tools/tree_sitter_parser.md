---
title: 'Module: src/codegraphcontext/tools/tree_sitter_parser.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/tree_sitter_parser.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.tree_sitter_parser`/TreeSitterParser#
symbols:
  TreeSitterParser.language_specific_parser: language_specific_parser.
  TreeSitterParser.language_name: language_name.
  TreeSitterParser.parse: parse().
  TreeSitterParser.language: language.
  TreeSitterParser.parser: parser.
  TreeSitterParser.ts_manager: ts_manager.
  TreeSitterParser: ''
  TreeSitterParser.__init__: __init__().
---
# Module: [`src/codegraphcontext/tools/tree_sitter_parser.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/tree_sitter_parser.py)

## Classes
### `TreeSitterParser`
- def: [`src/codegraphcontext/tools/tree_sitter_parser.py:13`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/tree_sitter_parser.py#L13)
- doc: A generic parser wrapper for a specific language using tree-sitter.
- signature: `class TreeSitterParser:`
- members:
  - `parse(self, path: Path, is_dependency: bool = False, **kwargs)` — [`L117`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/tree_sitter_parser.py#L117) — Dispatches parsing to the language-specific parser.
  - `language` — [`L20`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/tree_sitter_parser.py#L20)
  - `language_name` — [`L17`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/tree_sitter_parser.py#L17) — documented in [codegraphcontext-tools-graph_builder](../../../../concepts/codegraphcontext-tools-graph_builder.md)
  - `language_specific_parser` — [`L23`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/tree_sitter_parser.py#L23) — documented in [codegraphcontext-tools-graph_builder](../../../../concepts/codegraphcontext-tools-graph_builder.md)
  - `parser` — [`L21`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/tree_sitter_parser.py#L21)
  - `ts_manager` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/tree_sitter_parser.py#L18)
- protocol/private: `__init__`[`L16`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/tree_sitter_parser.py#L16)
- uses (calls/refs, reference-scoped): [`get_language_safe`](../utils/tree_sitter_manager.md#TreeSitterManager.get_language_safe), [`get_tree_sitter_manager`](../utils/tree_sitter_manager.md#get_tree_sitter_manager), [`create_parser`](../utils/tree_sitter_manager.md#TreeSitterManager.create_parser), [`TypescriptTreeSitterParser`](languages/typescript.md#TypescriptTreeSitterParser), [`TypescriptJSXTreeSitterParser`](languages/typescriptjsx.md#TypescriptJSXTreeSitterParser), [`DartTreeSitterParser`](languages/dart.md#DartTreeSitterParser), [`ElispTreeSitterParser`](languages/elisp.md#ElispTreeSitterParser), [`KotlinTreeSitterParser`](languages/kotlin.md#KotlinTreeSitterParser), [`LuaTreeSitterParser`](languages/lua.md#LuaTreeSitterParser), [`CSSTreeSitterParser`](languages/css.md#CSSTreeSitterParser), [`CSharpTreeSitterParser`](languages/csharp.md#CSharpTreeSitterParser), [`CTreeSitterParser`](languages/c.md#CTreeSitterParser), [`CppTreeSitterParser`](languages/cpp.md#CppTreeSitterParser), [`ElixirTreeSitterParser`](languages/elixir.md#ElixirTreeSitterParser), [`GoTreeSitterParser`](languages/go.md#GoTreeSitterParser), [`HTMLTreeSitterParser`](languages/html.md#HTMLTreeSitterParser), [`HaskellTreeSitterParser`](languages/haskell.md#HaskellTreeSitterParser), [`JavaTreeSitterParser`](languages/java.md#JavaTreeSitterParser), [`JavascriptTreeSitterParser`](languages/javascript.md#JavascriptTreeSitterParser), [`PerlTreeSitterParser`](languages/perl.md#PerlTreeSitterParser), [`PhpTreeSitterParser`](languages/php.md#PhpTreeSitterParser), [`PythonTreeSitterParser`](languages/python.md#PythonTreeSitterParser), [`RubyTreeSitterParser`](languages/ruby.md#RubyTreeSitterParser), [`RustTreeSitterParser`](languages/rust.md#RustTreeSitterParser), [`ScalaTreeSitterParser`](languages/scala.md#ScalaTreeSitterParser), [`SwiftTreeSitterParser`](languages/swift.md#SwiftTreeSitterParser), [`parse`](languages/python.md#PythonTreeSitterParser.parse)
- used by: [`parse_file`](graph_builder.md#GraphBuilder.parse_file), [`get_parser`](graph_builder.md#GraphBuilder.get_parser)

