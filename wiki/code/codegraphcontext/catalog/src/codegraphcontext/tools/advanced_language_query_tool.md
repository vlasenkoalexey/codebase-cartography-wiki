---
title: 'Module: src/codegraphcontext/tools/advanced_language_query_tool.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/advanced_language_query_tool.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.advanced_language_query_tool`/
symbols:
  Advanced_language_query.TOOLKITS: Advanced_language_query#TOOLKITS.
  Advanced_language_query.advanced_language_query: Advanced_language_query#advanced_language_query().
  Advanced_language_query.Supported_queries: Advanced_language_query#Supported_queries.
  Advanced_language_query.__init__: Advanced_language_query#__init__().
  Advanced_language_query.db_manager: Advanced_language_query#db_manager.
  Advanced_language_query.toolkit: Advanced_language_query#toolkit.
  logger: logger.
  Advanced_language_query: Advanced_language_query#
---
# Module: [`src/codegraphcontext/tools/advanced_language_query_tool.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/advanced_language_query_tool.py)

## Classes
### `Advanced_language_query`
- def: [`src/codegraphcontext/tools/advanced_language_query_tool.py:28`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/advanced_language_query_tool.py#L28)
- doc: Tool implementation for executing a read-only language specific Cypher query.
- signature: `class Advanced_language_query:`
- members:
  - `advanced_language_query(self, language: str, query: str)` — [`L68`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/advanced_language_query_tool.py#L68)
  - `Supported_queries` — [`L51`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/advanced_language_query_tool.py#L51)
  - `TOOLKITS` — [`L36`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/advanced_language_query_tool.py#L36)
  - `db_manager` — [`L66`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/advanced_language_query_tool.py#L66)
  - `toolkit` — [`L83`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/advanced_language_query_tool.py#L83)
- protocol/private: `__init__`[`L65`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/advanced_language_query_tool.py#L65)
- uses (calls/refs, reference-scoped): [`debug_log`](../utils/debug_log.md#debug_log), [`get_driver`](../core/database.md#DatabaseManager.get_driver), [`DatabaseManager`](../core/database.md#DatabaseManager), [`CSharpToolkit`](query_tool_languages/csharp_toolkit.md#CSharpToolkit), [`CToolkit`](query_tool_languages/c_toolkit.md#CToolkit), [`CppToolkit`](query_tool_languages/cpp_toolkit.md#CppToolkit), [`DartToolkit`](query_tool_languages/dart_toolkit.md#DartToolkit), [`ElispToolkit`](query_tool_languages/elisp_toolkit.md#ElispToolkit), [`GoToolkit`](query_tool_languages/go_toolkit.md#GoToolkit), [`JavaToolkit`](query_tool_languages/java_toolkit.md#JavaToolkit), [`JavascriptToolkit`](query_tool_languages/javascript_toolkit.md#JavascriptToolkit), [`PerlToolkit`](query_tool_languages/perl_toolkit.md#PerlToolkit), [`PythonToolkit`](query_tool_languages/python_toolkit.md#PythonToolkit), [`RubyToolkit`](query_tool_languages/ruby_toolkit.md#RubyToolkit), [`RustToolkit`](query_tool_languages/rust_toolkit.md#RustToolkit), [`TypescriptToolkit`](query_tool_languages/typescript_toolkit.md#TypescriptToolkit)

## Module values
- `logger` — [`L25`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/advanced_language_query_tool.py#L25)

