---
title: 'Module: tree_sitter_analyzer/xref.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/xref.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.xref`/
symbols:
  XRefEngine.xref: XRefEngine#xref().
  XRefEngine.file_xref: XRefEngine#file_xref().
  XRefResult.to_dict: XRefResult#to_dict().
  XRefEngine: XRefEngine#
  XRefResult.definitions: XRefResult#definitions.
  XRefResult.callers: XRefResult#callers.
  XRefResult.callees: XRefResult#callees.
  XRefEngine._find_file_dependents: XRefEngine#_find_file_dependents().
  XRefResult.import_dependents: XRefResult#import_dependents.
  XRefResult.file_dependents: XRefResult#file_dependents.
  XRefEngine._file_callers: XRefEngine#_file_callers().
  XRefResult: XRefResult#
  XRefEngine._find_definitions: XRefEngine#_find_definitions().
  XRefResult.symbol: XRefResult#symbol.
  XRefResult.file_path: XRefResult#file_path.
  XRefEngine._find_import_dependents: XRefEngine#_find_import_dependents().
  XRefEngine._file_defined_names: XRefEngine#_file_defined_names().
  XRefEngine._inbound_edge_rows: XRefEngine#_inbound_edge_rows().
  XRefResult.data_source: XRefResult#data_source.
  XRefEngine._backend: XRefEngine#_backend.
  XRefEngine._find_callers: XRefEngine#_find_callers().
  XRefEngine._find_callees: XRefEngine#_find_callees().
  _XREF_NAME_CHUNK: _XREF_NAME_CHUNK.
  XRefEngine._cache: XRefEngine#_cache.
  XRefEngine._file_symbols: XRefEngine#_file_symbols().
  XRefEngine._file_callees: XRefEngine#_file_callees().
  XRefEngine._get_signature: XRefEngine#_get_signature().
  XRefEngine._file_to_module: XRefEngine#_file_to_module().
  logger: logger.
  XRefEngine.__init__: XRefEngine#__init__().
---
# Module: [`tree_sitter_analyzer/xref.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py)

## Classes
### `XRefEngine`
- def: [`tree_sitter_analyzer/xref.py:73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L73)
- doc: AST-cache-backed cross-reference engine.
- signature: `class XRefEngine:`
- members:
  - `_file_defined_names(self, conn: sqlite3.Connection, file_path: str)` — [`L316`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L316) — Callable symbol names defined in ``file_path`` (function/method/class).
  - `_inbound_edge_rows(self, conn: sqlite3.Connection, names: list[str], file_path: str, prefix: str, suffix: str)` — [`L328`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L328) — Run a chunked inbound-edge query and concatenate the rows.
  - `file_xref(self, file_path: str)` — [`L133`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L133)
  - `xref(self, symbol: str, file_path: str | None = None, *, include_callers: bool = True, include_callees: bool = True, include_imports: bool = True, include_file_deps: bool = True)` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L89)
- protocol/private: `__init__`[`L81`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L81), `_backend`[`L87`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L87), `_cache`[`L86`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L86), `_file_callees`[`L452`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L452), `_file_callers`[`L413`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L413), `_file_symbols`[`L386`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L386), `_file_to_module`[`L476`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L476), `_find_callees`[`L240`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L240), `_find_callers`[`L201`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L201), `_find_definitions`[`L157`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L157), `_find_file_dependents`[`L356`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L356), `_find_import_dependents`[`L286`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L286), `_get_signature`[`L181`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L181)
- uses (calls/refs, reference-scoped): [`CodeGraphQueryBackend`](codegraph_query_backend.md#CodeGraphQueryBackend), [`definitions`](xref.md#XRefResult.definitions), [`callees`](xref.md#XRefResult.callees), [`callers`](xref.md#XRefResult.callers), [`file_dependents`](xref.md#XRefResult.file_dependents), [`import_dependents`](xref.md#XRefResult.import_dependents), [`XRefResult`](xref.md#XRefResult), [`file_path`](xref.md#XRefResult.file_path), [`symbol`](xref.md#XRefResult.symbol), [`data_source`](xref.md#XRefResult.data_source), [`_XREF_NAME_CHUNK`](xref.md#_XREF_NAME_CHUNK)
- used by: [`execute`](mcp/tools/codegraph_xref_tool.md#CodeGraphXRefTool.execute)  (19 test-only)

### `XRefResult`
- def: [`tree_sitter_analyzer/xref.py:38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L38)
- signature: `class XRefResult:`
- members:
  - `to_dict(self)` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L48)
  - `callees` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L43)
  - `callers` — [`L42`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L42)
  - `data_source` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L46)
  - `definitions` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L41)
  - `file_dependents` — [`L45`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L45)
  - `file_path` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L40)
  - `import_dependents` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L44)
  - `symbol` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L39)
- used by: [`xref`](xref.md#XRefEngine.xref), [`execute`](mcp/tools/codegraph_xref_tool.md#CodeGraphXRefTool.execute)  (12 test-only)

## Module values
- `_XREF_NAME_CHUNK` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L34)
- `logger` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/xref.py#L29)

