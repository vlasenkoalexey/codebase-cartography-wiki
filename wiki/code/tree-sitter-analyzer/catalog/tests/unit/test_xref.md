---
title: 'Module: tests/unit/test_xref.py'
type: catalog
provenance: extracted
module: tests/unit/test_xref.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_xref`/
symbols:
  TestXRefResult.test_to_dict_full: TestXRefResult#test_to_dict_full().
  TestXRefEngineSymbol.test_xref_alpha: TestXRefEngineSymbol#test_xref_alpha().
  TestXRefEngineSymbol.test_xref_exclude_dimensions: TestXRefEngineSymbol#test_xref_exclude_dimensions().
  TestXRefEngineSymbol.test_xref_definitions_use_shared_backend_and_file_filter: TestXRefEngineSymbol#test_xref_definitions_use_shared_backend_and_file_filter().
  TestXRefEngineSymbol.test_xref_unknown_symbol: TestXRefEngineSymbol#test_xref_unknown_symbol().
  TestXRefEngineNoCache.test_empty_cache: TestXRefEngineNoCache#test_empty_cache().
  TestXRefEngineFile.test_file_xref_excludes_same_name_resolved_to_other_file: TestXRefEngineFile#test_file_xref_excludes_same_name_resolved_to_other_file().
  TestXRefEngineFile.test_file_xref_chunks_large_symbol_list: TestXRefEngineFile#test_file_xref_chunks_large_symbol_list().
  TestXRefEngineFile.test_file_xref_excludes_unresolved_stdlib_name_collision: TestXRefEngineFile#test_file_xref_excludes_unresolved_stdlib_name_collision().
  TestXRefEngineFile.test_file_xref_includes_methods: TestXRefEngineFile#test_file_xref_includes_methods().
  TestXRefResult.test_to_dict_minimal: TestXRefResult#test_to_dict_minimal().
  TestXRefEngineSymbol.test_xref_callers: TestXRefEngineSymbol#test_xref_callers().
  TestXRefEngineSymbol.test_xref_callees: TestXRefEngineSymbol#test_xref_callees().
  TestXRefEngineSymbol.test_xref_import_dependents: TestXRefEngineSymbol#test_xref_import_dependents().
  TestXRefEngineSymbol.test_xref_file_path_filter: TestXRefEngineSymbol#test_xref_file_path_filter().
  TestXRefEngineFile.test_symbol_xref_file_dependents_resolved: TestXRefEngineFile#test_symbol_xref_file_dependents_resolved().
  indexed_project: indexed_project().
  TestXRefEngineFile.test_file_xref: TestXRefEngineFile#test_file_xref().
  TestXRefEngineFile.test_file_xref_symbols: TestXRefEngineFile#test_file_xref_symbols().
  TestXRefEngineFile.test_file_xref_unknown: TestXRefEngineFile#test_file_xref_unknown().
  TestXRefEngineFile.test_file_xref_inbound_callers_resolved: TestXRefEngineFile#test_file_xref_inbound_callers_resolved().
  TestXRefEngineSymbol.test_xref_definitions_use_shared_backend_and_file_filter.MockCache.get_conn: TestXRefEngineSymbol#test_xref_definitions_use_shared_backend_and_file_filter().MockCache#get_conn().
  TestXRefEngineSymbol.test_xref_definitions_use_shared_backend_and_file_filter.MockConn.execute: TestXRefEngineSymbol#test_xref_definitions_use_shared_backend_and_file_filter().MockConn#execute().
  TestXRefEngineSymbol.test_xref_definitions_use_shared_backend_and_file_filter.MockCache._get_conn: TestXRefEngineSymbol#test_xref_definitions_use_shared_backend_and_file_filter().MockCache#_get_conn().
  TestXRefEngineSymbol.test_xref_definitions_use_shared_backend_and_file_filter.MockCursor: TestXRefEngineSymbol#test_xref_definitions_use_shared_backend_and_file_filter().MockCursor#
  TestXRefEngineSymbol.test_xref_definitions_use_shared_backend_and_file_filter.MockConn: TestXRefEngineSymbol#test_xref_definitions_use_shared_backend_and_file_filter().MockConn#
  TestXRefEngineSymbol.test_xref_definitions_use_shared_backend_and_file_filter.MockCache: TestXRefEngineSymbol#test_xref_definitions_use_shared_backend_and_file_filter().MockCache#
  TestXRefEngineSymbol.test_xref_definitions_use_shared_backend_and_file_filter.FakeBackend: TestXRefEngineSymbol#test_xref_definitions_use_shared_backend_and_file_filter().FakeBackend#
  TestXRefEngineSymbol: TestXRefEngineSymbol#
  TestXRefEngineSymbol.test_xref_definitions_use_shared_backend_and_file_filter.MockCursor.fetchone: TestXRefEngineSymbol#test_xref_definitions_use_shared_backend_and_file_filter().MockCursor#fetchone().
  TestXRefEngineSymbol.test_xref_definitions_use_shared_backend_and_file_filter.FakeBackend.resolve_definitions: TestXRefEngineSymbol#test_xref_definitions_use_shared_backend_and_file_filter().FakeBackend#resolve_definitions().
  TestXRefEngineFile: TestXRefEngineFile#
  TestXRefResult: TestXRefResult#
  TestXRefEngineNoCache: TestXRefEngineNoCache#
---
# Module: [`tests/unit/test_xref.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py)

## Classes
### `FakeBackend`
- def: [`tests/unit/test_xref.py:46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L46)
- signature: `class FakeBackend:`
- members:
  - `resolve_definitions(self, symbol)` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L47)
- used by: (1 test-only callers)

### `MockCache`
- def: [`tests/unit/test_xref.py:37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L37)
- signature: `class MockCache:`
- members:
  - `get_conn(self)` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L38)
- protocol/private: `_get_conn`[`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L41)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `MockConn`
- def: [`tests/unit/test_xref.py:33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L33)
- signature: `class MockConn:`
- members:
  - `execute(self, *args, **kwargs)` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L34)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `MockCursor`
- def: [`tests/unit/test_xref.py:29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L29)
- signature: `class MockCursor:`
- members:
  - `fetchone(self)` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L30)
- used by: (1 test-only callers)

### `TestXRefEngineFile`
- def: [`tests/unit/test_xref.py:157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L157)
- signature: `class TestXRefEngineFile:`
- members:
  - `test_file_xref(self, indexed_project)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L158)
  - `test_file_xref_chunks_large_symbol_list(self, tmp_path, monkeypatch)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L225)
  - `test_file_xref_excludes_same_name_resolved_to_other_file(self, tmp_path)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L203)
  - `test_file_xref_excludes_unresolved_stdlib_name_collision(self, tmp_path)` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L250)
  - `test_file_xref_inbound_callers_resolved(self, indexed_project)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L180)
  - `test_file_xref_includes_methods(self, tmp_path)` — [`L268`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L268) — Codex P2 on #314: class methods (kind='method') must appear in file
  - `test_file_xref_symbols(self, indexed_project)` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L166)
  - `test_file_xref_unknown(self, indexed_project)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L174)
  - `test_symbol_xref_file_dependents_resolved(self, indexed_project)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L195)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`xref`](../../tree_sitter_analyzer/xref.md#XRefEngine.xref), [`file_xref`](../../tree_sitter_analyzer/xref.md#XRefEngine.file_xref), [`XRefEngine`](../../tree_sitter_analyzer/xref.md#XRefEngine), [`file_dependents`](../../tree_sitter_analyzer/xref.md#XRefResult.file_dependents)

### `TestXRefEngineNoCache`
- def: [`tests/unit/test_xref.py:325`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L325)
- signature: `class TestXRefEngineNoCache:`
- members:
  - `test_empty_cache(self, tmp_path)` — [`L326`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L326)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`xref`](../../tree_sitter_analyzer/xref.md#XRefEngine.xref), [`XRefEngine`](../../tree_sitter_analyzer/xref.md#XRefEngine), [`definitions`](../../tree_sitter_analyzer/xref.md#XRefResult.definitions), [`data_source`](../../tree_sitter_analyzer/xref.md#XRefResult.data_source)

### `TestXRefEngineSymbol`
- def: [`tests/unit/test_xref.py:27`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L27)
- signature: `class TestXRefEngineSymbol:`
- members:
  - `test_xref_alpha(self, indexed_project)` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L79)
  - `test_xref_callees(self, indexed_project)` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L102)
  - `test_xref_callers(self, indexed_project)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L90)
  - `test_xref_definitions_use_shared_backend_and_file_filter(self)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L28)
  - `test_xref_exclude_dimensions(self, indexed_project)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L141)
  - `test_xref_file_path_filter(self, indexed_project)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L126)
  - `test_xref_import_dependents(self, indexed_project)` — [`L114`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L114)
  - `test_xref_unknown_symbol(self, indexed_project)` — [`L133`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L133)
- uses (calls/refs, reference-scoped): [`xref`](../../tree_sitter_analyzer/xref.md#XRefEngine.xref), [`XRefEngine`](../../tree_sitter_analyzer/xref.md#XRefEngine), [`definitions`](../../tree_sitter_analyzer/xref.md#XRefResult.definitions), [`callees`](../../tree_sitter_analyzer/xref.md#XRefResult.callees), [`callers`](../../tree_sitter_analyzer/xref.md#XRefResult.callers), [`file_dependents`](../../tree_sitter_analyzer/xref.md#XRefResult.file_dependents), [`import_dependents`](../../tree_sitter_analyzer/xref.md#XRefResult.import_dependents), [`XRefResult`](../../tree_sitter_analyzer/xref.md#XRefResult), [`symbol`](../../tree_sitter_analyzer/xref.md#XRefResult.symbol), [`data_source`](../../tree_sitter_analyzer/xref.md#XRefResult.data_source)  (2 test-only)

### `TestXRefResult`
- def: [`tests/unit/test_xref.py:294`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L294)
- signature: `class TestXRefResult:`
- members:
  - `test_to_dict_full(self)` — [`L303`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L303)
  - `test_to_dict_minimal(self)` — [`L295`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L295)
- uses (calls/refs, reference-scoped): [`to_dict`](../../tree_sitter_analyzer/xref.md#XRefResult.to_dict), [`definitions`](../../tree_sitter_analyzer/xref.md#XRefResult.definitions), [`callees`](../../tree_sitter_analyzer/xref.md#XRefResult.callees), [`callers`](../../tree_sitter_analyzer/xref.md#XRefResult.callers), [`file_dependents`](../../tree_sitter_analyzer/xref.md#XRefResult.file_dependents), [`import_dependents`](../../tree_sitter_analyzer/xref.md#XRefResult.import_dependents), [`XRefResult`](../../tree_sitter_analyzer/xref.md#XRefResult), [`file_path`](../../tree_sitter_analyzer/xref.md#XRefResult.file_path), [`symbol`](../../tree_sitter_analyzer/xref.md#XRefResult.symbol)

## Functions
- `indexed_project(tmp_path)` — [`L10`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_xref.py#L10)

