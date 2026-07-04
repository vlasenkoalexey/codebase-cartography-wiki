---
title: 'Module: tests/unit/hyphae/test_evaluator.py'
type: catalog
provenance: extracted
module: tests/unit/hyphae/test_evaluator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.hyphae.test_evaluator`/
symbols:
  _fixture: _fixture().
  _names: _names().
  test_implements_queries_implements_edge_kind: test_implements_queries_implements_edge_kind().
  test_name_lookup: test_name_lookup().
  test_kind_method_requires_class_field: test_kind_method_requires_class_field().
  test_kind_class_enumerates_class_symbols: test_kind_class_enumerates_class_symbols().
  test_kind_interface_aliases_class: test_kind_interface_aliases_class().
  test_calls_edge_driven: test_calls_edge_driven().
  test_callees_edge_driven: test_callees_edge_driven().
  test_extends_edge: test_extends_edge().
  test_implements_aliases_extends: test_implements_aliases_extends().
  test_has_via_contains_edge: test_has_via_contains_edge().
  test_first_child_per_class: test_first_child_per_class().
  test_nth_child_second: test_nth_child_second().
  test_only_child: test_only_child().
  test_imports_file_level: test_imports_file_level().
  test_not_excludes: test_not_excludes().
  test_in_path_filter: test_in_path_filter().
  test_attribute_file_filter: test_attribute_file_filter().
  test_child_combinator: test_child_combinator().
  test_selector_list_union: test_selector_list_union().
  test_unknown_pseudo_raises: test_unknown_pseudo_raises().
  test_nth_child_requires_number: test_nth_child_requires_number().
  test_subclasses_returns_children: test_subclasses_returns_children().
  test_calls_distinguishes_same_name_across_files: test_calls_distinguishes_same_name_across_files().
  FakeCache.search_symbols_cascade: FakeCache#search_symbols_cascade().
  FakeCache: FakeCache#
  FakeCache.get_functions: FakeCache#get_functions().
  FakeCache.get_symbols_by_kind: FakeCache#get_symbols_by_kind().
  FakeCache.query_edges: FakeCache#query_edges().
  FakeCache._functions: FakeCache#_functions.
  FakeCache._classes: FakeCache#_classes.
  FakeCache._edges: FakeCache#_edges.
  FakeCache.__init__: FakeCache#__init__().
---
# Module: [`tests/unit/hyphae/test_evaluator.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py)

## Classes
### `FakeCache`
- def: [`tests/unit/hyphae/test_evaluator.py:11`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L11)
- doc: ASTCache stand-in backed by in-memory symbols + edges fixtures.
- signature: `class FakeCache:`
- members:
  - `get_functions(self)` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L19)
  - `get_symbols_by_kind(self, kind, limit=50000)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L22)
  - `query_edges(self, kind, caller_name=None, callee_name=None, limit=10000)` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L31)
  - `search_symbols_cascade(self, query, limit=100)` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L27)
- protocol/private: `__init__`[`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L14), `_classes`[`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L16), `_edges`[`L17`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L17), `_functions`[`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L15)
- used by: (3 test-only callers)

## Functions
- `_fixture()` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L48)
- `_names(rows)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L44)
- `test_attribute_file_filter()` — [`L231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L231)
- `test_callees_edge_driven()` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L175)
- `test_calls_distinguishes_same_name_across_files()` — [`L265`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L265)
- `test_calls_edge_driven()` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L170)
- `test_child_combinator()` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L237)
- `test_extends_edge()` — [`L181`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L181)
- `test_first_child_per_class()` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L197)
- `test_has_via_contains_edge()` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L192)
- `test_implements_aliases_extends()` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L186)
- `test_implements_queries_implements_edge_kind()` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L287)
- `test_imports_file_level()` — [`L213`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L213)
- `test_in_path_filter()` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L226)
- `test_kind_class_enumerates_class_symbols()` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L159)
- `test_kind_interface_aliases_class()` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L164)
- `test_kind_method_requires_class_field()` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L154)
- `test_name_lookup()` — [`L150`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L150)
- `test_not_excludes()` — [`L221`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L221)
- `test_nth_child_requires_number()` — [`L252`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L252)
- `test_nth_child_second()` — [`L203`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L203)
- `test_only_child()` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L208)
- `test_selector_list_union()` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L242)
- `test_subclasses_returns_children()` — [`L258`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L258)
- `test_unknown_pseudo_raises()` — [`L247`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/hyphae/test_evaluator.py#L247)

