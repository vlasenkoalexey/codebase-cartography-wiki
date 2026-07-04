---
title: 'Module: tests/unit/test_b1_reader_edge_parity.py'
type: catalog
provenance: extracted
module: tests/unit/test_b1_reader_edge_parity.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_b1_reader_edge_parity`/
symbols:
  TestConstraintEvaluatorParity._run: TestConstraintEvaluatorParity#_run().
  _build_db: _build_db().
  TestB13PythonResolutionOnEdges.test_cross_file_resolution_lands_on_edges: TestB13PythonResolutionOnEdges#test_cross_file_resolution_lands_on_edges().
  TestSymbolResolverParity._run: TestSymbolResolverParity#_run().
  TestXrefParity._run: TestXrefParity#_run().
  _SPECS._SPECS: _SPECS._SPECS.
  TestGetCallEdgesParity._run: TestGetCallEdgesParity#_run().
  TestCallPathParity._run: TestCallPathParity#_run().
  TestCallPathParity.test_edges_only_matches_legacy: TestCallPathParity#test_edges_only_matches_legacy().
  TestAstCacheGraphParity.test_edges_only_matches_legacy: TestAstCacheGraphParity#test_edges_only_matches_legacy().
  TestXrefParity.test_edges_only_matches_legacy: TestXrefParity#test_edges_only_matches_legacy().
  TestSymbolResolverParity.test_edges_only_matches_legacy: TestSymbolResolverParity#test_edges_only_matches_legacy().
  TestGetCallEdgesParity.test_edges_only_matches_legacy: TestGetCallEdgesParity#test_edges_only_matches_legacy().
  TestGetCallEdgesParity.test_returns_all_columns_from_edges_alone: TestGetCallEdgesParity#test_returns_all_columns_from_edges_alone().
  TestConstraintEvaluatorParity.test_edges_only_matches_legacy: TestConstraintEvaluatorParity#test_edges_only_matches_legacy().
  TestAstCacheGraphParity._run: TestAstCacheGraphParity#_run().
  _mock_cache: _mock_cache().
  _AST_CALL_EDGES_DDL: _AST_CALL_EDGES_DDL.
  _EDGES_DDL: _EDGES_DDL.
  _normalise: _normalise().
  TestB13PythonResolutionOnEdges._write_project: TestB13PythonResolutionOnEdges#_write_project().
  TestCallPathParity: TestCallPathParity#
  TestAstCacheGraphParity: TestAstCacheGraphParity#
  TestXrefParity: TestXrefParity#
  TestSymbolResolverParity: TestSymbolResolverParity#
  TestGetCallEdgesParity: TestGetCallEdgesParity#
  TestConstraintEvaluatorParity: TestConstraintEvaluatorParity#
  TestB13PythonResolutionOnEdges: TestB13PythonResolutionOnEdges#
---
# Module: [`tests/unit/test_b1_reader_edge_parity.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py)

## Classes
### `TestAstCacheGraphParity`
- def: [`tests/unit/test_b1_reader_edge_parity.py:252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L252)
- signature: `class TestAstCacheGraphParity:`
- members:
  - `test_edges_only_matches_legacy(self, tmp_path: Path)` — [`L262`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L262)
- protocol/private: `_run`[`L253`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L253)
- uses (calls/refs, reference-scoped): [`bfs_callers`](../../tree_sitter_analyzer/_ast_cache_graph.md#bfs_callers), [`bfs_callees`](../../tree_sitter_analyzer/_ast_cache_graph.md#bfs_callees)  (2 test-only)

### `TestB13PythonResolutionOnEdges`
- def: [`tests/unit/test_b1_reader_edge_parity.py:442`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L442)
- signature: `class TestB13PythonResolutionOnEdges:`
- members:
  - `test_cross_file_resolution_lands_on_edges(self, tmp_path: Path)` — [`L464`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L464)
- protocol/private: `_write_project`[`L444`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L444)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`EdgeKind`](../../tree_sitter_analyzer/graph/edge_store.md#EdgeKind), [`get_conn`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_conn), [`symbol_node`](../../tree_sitter_analyzer/graph/edge_store.md#symbol_node), [`query_callees`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.query_callees), [`query_callers`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.query_callers), [`EXTENDS`](../../tree_sitter_analyzer/graph/edge_store.md#EdgeKind.EXTENDS)

### `TestCallPathParity`
- def: [`tests/unit/test_b1_reader_edge_parity.py:229`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L229)
- signature: `class TestCallPathParity:`
- members:
  - `test_edges_only_matches_legacy(self, tmp_path: Path)` — [`L239`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L239)
- protocol/private: `_run`[`L230`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L230)
- uses (calls/refs, reference-scoped): [`CallPathFinder`](../../tree_sitter_analyzer/call_path.md#CallPathFinder), [`_query_backward_edges`](../../tree_sitter_analyzer/call_path.md#CallPathFinder._query_backward_edges), [`_query_forward_edges`](../../tree_sitter_analyzer/call_path.md#CallPathFinder._query_forward_edges)  (2 test-only)

### `TestConstraintEvaluatorParity`
- def: [`tests/unit/test_b1_reader_edge_parity.py:395`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L395)
- signature: `class TestConstraintEvaluatorParity:`
- members:
  - `test_edges_only_matches_legacy(self, tmp_path: Path)` — [`L423`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L423)
- protocol/private: `_run`[`L396`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L396)
- uses (calls/refs, reference-scoped): [`evaluate`](../../tree_sitter_analyzer/constraints/evaluator.md#evaluate), [`Constraint`](../../tree_sitter_analyzer/constraints/schema.md#Constraint), [`id`](../../tree_sitter_analyzer/constraints/schema.md#Constraint.id), [`caller_file`](../../tree_sitter_analyzer/constraints/schema.md#Violation.caller_file), [`rule_id`](../../tree_sitter_analyzer/constraints/schema.md#Violation.rule_id), [`callee_file`](../../tree_sitter_analyzer/constraints/schema.md#Violation.callee_file), [`caller_line`](../../tree_sitter_analyzer/constraints/schema.md#Violation.caller_line), [`callee_name`](../../tree_sitter_analyzer/constraints/schema.md#Violation.callee_name), [`caller_name`](../../tree_sitter_analyzer/constraints/schema.md#Violation.caller_name), [`severity`](../../tree_sitter_analyzer/constraints/schema.md#Constraint.severity), [`from_glob`](../../tree_sitter_analyzer/constraints/schema.md#Constraint.from_glob), [`to_glob`](../../tree_sitter_analyzer/constraints/schema.md#Constraint.to_glob), [`reason`](../../tree_sitter_analyzer/constraints/schema.md#Constraint.reason), [`rule`](../../tree_sitter_analyzer/constraints/schema.md#Constraint.rule)  (2 test-only)

### `TestGetCallEdgesParity`
- def: [`tests/unit/test_b1_reader_edge_parity.py:326`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L326)
- doc: `ASTCache.get_call_edges` must return byte-for-byte identical rows
- signature: `class TestGetCallEdgesParity:`
- members:
  - `test_edges_only_matches_legacy(self, tmp_path: Path)` — [`L352`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L352)
  - `test_returns_all_columns_from_edges_alone(self, tmp_path: Path)` — [`L359`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L359) — The post-migration reader must surface every legacy column from the
- protocol/private: `_run`[`L331`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L331)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`get_call_edges`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.get_call_edges)  (3 test-only)

### `TestSymbolResolverParity`
- def: [`tests/unit/test_b1_reader_edge_parity.py:305`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L305)
- signature: `class TestSymbolResolverParity:`
- members:
  - `test_edges_only_matches_legacy(self, tmp_path: Path)` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L313)
- protocol/private: `_run`[`L306`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L306)
- uses (calls/refs, reference-scoped): [`_find_references`](../../tree_sitter_analyzer/symbol_resolver.md#SymbolResolver._find_references), [`SymbolResolver`](../../tree_sitter_analyzer/symbol_resolver.md#SymbolResolver), [`file`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.file), [`line`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.line), [`kind`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.kind), [`language`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.language), [`name`](../../tree_sitter_analyzer/symbol_resolver.md#ReferenceLocation.name)  (3 test-only)

### `TestXrefParity`
- def: [`tests/unit/test_b1_reader_edge_parity.py:276`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L276)
- signature: `class TestXrefParity:`
- members:
  - `test_edges_only_matches_legacy(self, tmp_path: Path)` — [`L292`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L292)
- protocol/private: `_run`[`L277`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L277)
- uses (calls/refs, reference-scoped): [`XRefEngine`](../../tree_sitter_analyzer/xref.md#XRefEngine), [`_find_file_dependents`](../../tree_sitter_analyzer/xref.md#XRefEngine._find_file_dependents), [`_file_callers`](../../tree_sitter_analyzer/xref.md#XRefEngine._file_callers), [`_find_callees`](../../tree_sitter_analyzer/xref.md#XRefEngine._find_callees), [`_find_callers`](../../tree_sitter_analyzer/xref.md#XRefEngine._find_callers), [`_file_callees`](../../tree_sitter_analyzer/xref.md#XRefEngine._file_callees)  (3 test-only)

## Functions
- `_build_db(tmp_path: Path, specs: list[dict[str, Any]], *, drop_ast_call_edges: bool = False)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L86) — Build a DB with both tables populated identically from ``specs``.
- `_mock_cache(tmp_path: Path, conn: sqlite3.Connection)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L176)
- `_normalise(spec: dict[str, Any])` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L70)

## Module values
- `_AST_CALL_EDGES_DDL` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L30)
- `_EDGES_DDL` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L46)
- `_SPECS` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_b1_reader_edge_parity.py#L187)

