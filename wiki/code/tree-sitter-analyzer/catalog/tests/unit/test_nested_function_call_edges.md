---
title: 'Module: tests/unit/test_nested_function_call_edges.py'
type: catalog
provenance: extracted
module: tests/unit/test_nested_function_call_edges.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_nested_function_call_edges`/
symbols:
  TestSameLineSiblingCallAttribution._js_edges: TestSameLineSiblingCallAttribution#_js_edges().
  _parse: _parse().
  TestNestedFunctionCallEdgeAttribution._edges: TestNestedFunctionCallEdgeAttribution#_edges().
  TestDeeplyNestedCallEdgeAttribution.test_deep_is_caller: TestDeeplyNestedCallEdgeAttribution#test_deep_is_caller().
  TestMultipleCallsInNested.test_both_callees_attributed_to_inner: TestMultipleCallsInNested#test_both_callees_attributed_to_inner().
  nested_indexed_project: nested_indexed_project().
  TestNestedFunctionCalleesTool.test_inner_callees_returns_info_verdict: TestNestedFunctionCalleesTool#test_inner_callees_returns_info_verdict().
  TestNestedFunctionCalleesTool.test_inner_not_not_found: TestNestedFunctionCalleesTool#test_inner_not_not_found().
  TestNestedFunctionCallersTool.test_helper_callers_includes_inner: TestNestedFunctionCallersTool#test_helper_callers_includes_inner().
  TestNestedFunctionCallEdgeAttribution.test_inner_is_caller_for_helper: TestNestedFunctionCallEdgeAttribution#test_inner_is_caller_for_helper().
  TestNestedFunctionCallEdgeAttribution.test_outer_has_no_helper_edge: TestNestedFunctionCallEdgeAttribution#test_outer_has_no_helper_edge().
  TestSameLineSiblingCallAttribution.test_helper_attributed_to_outer_not_inner: TestSameLineSiblingCallAttribution#test_helper_attributed_to_outer_not_inner().
  TestSameLineSiblingCallAttribution.test_inner_has_no_helper_edge: TestSameLineSiblingCallAttribution#test_inner_has_no_helper_edge().
  TestNestedFunctionCallEdgeAttribution._SOURCE: TestNestedFunctionCallEdgeAttribution#_SOURCE.
  TestDeeplyNestedCallEdgeAttribution._SOURCE: TestDeeplyNestedCallEdgeAttribution#_SOURCE.
  TestMultipleCallsInNested._SOURCE: TestMultipleCallsInNested#_SOURCE.
  TestSameLineSiblingCallAttribution._JS_SOURCE: TestSameLineSiblingCallAttribution#_JS_SOURCE.
  TestNestedFunctionCallEdgeAttribution: TestNestedFunctionCallEdgeAttribution#
  TestDeeplyNestedCallEdgeAttribution: TestDeeplyNestedCallEdgeAttribution#
  TestMultipleCallsInNested: TestMultipleCallsInNested#
  TestSameLineSiblingCallAttribution: TestSameLineSiblingCallAttribution#
  TestNestedFunctionCalleesTool: TestNestedFunctionCalleesTool#
  TestNestedFunctionCallersTool: TestNestedFunctionCallersTool#
---
# Module: [`tests/unit/test_nested_function_call_edges.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py)

## Classes
### `TestDeeplyNestedCallEdgeAttribution`
- def: [`tests/unit/test_nested_function_call_edges.py:82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L82)
- doc: Three levels of nesting: calls in innermost must reach innermost.
- signature: `class TestDeeplyNestedCallEdgeAttribution:`
- members:
  - `test_deep_is_caller(self)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L95)
- protocol/private: `_SOURCE`[`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L85)
- uses (calls/refs, reference-scoped): [`_extract_call_edges`](../../tree_sitter_analyzer/_ast_extraction.md#_extract_call_edges)  (1 test-only)

### `TestMultipleCallsInNested`
- def: [`tests/unit/test_nested_function_call_edges.py:105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L105)
- doc: inner() calls two helpers; both edges should be attributed to inner.
- signature: `class TestMultipleCallsInNested:`
- members:
  - `test_both_callees_attributed_to_inner(self)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L121)
- protocol/private: `_SOURCE`[`L108`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L108)
- uses (calls/refs, reference-scoped): [`_extract_call_edges`](../../tree_sitter_analyzer/_ast_extraction.md#_extract_call_edges)  (1 test-only)

### `TestNestedFunctionCallEdgeAttribution`
- def: [`tests/unit/test_nested_function_call_edges.py:41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L41)
- doc: The call inside inner() must be attributed to inner, not outer.
- signature: `class TestNestedFunctionCallEdgeAttribution:`
- members:
  - `test_inner_is_caller_for_helper(self)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L57) — helper() call at line 6 lives inside inner() → caller must be inner.
  - `test_outer_has_no_helper_edge(self)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L69) — outer() itself never calls helper() — only inner() does.
- protocol/private: `_SOURCE`[`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L44), `_edges`[`L53`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L53)
- uses (calls/refs, reference-scoped): [`_extract_call_edges`](../../tree_sitter_analyzer/_ast_extraction.md#_extract_call_edges)  (1 test-only)

### `TestNestedFunctionCalleesTool`
- def: [`tests/unit/test_nested_function_call_edges.py:217`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L217)
- doc: nav action=callees on a nested function should return edges, not NOT_FOUND.
- signature: `class TestNestedFunctionCalleesTool:`
- members:
  - `test_inner_callees_returns_info_verdict(self, nested_indexed_project: str)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L221) — inner() calls helper() → verdict INFO, callee_count==1.
  - `test_inner_not_not_found(self, nested_indexed_project: str)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L243) — The NOT_FOUND-for-indexed-symbol contradiction must be gone.
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool.execute), [`CodeGraphCalleesTool`](../../tree_sitter_analyzer/mcp/tools/callees_tool.md#CodeGraphCalleesTool)

### `TestNestedFunctionCallersTool`
- def: [`tests/unit/test_nested_function_call_edges.py:257`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L257)
- doc: nav action=callers on helper should include inner as a caller.
- signature: `class TestNestedFunctionCallersTool:`
- members:
  - `test_helper_callers_includes_inner(self, nested_indexed_project: str)` — [`L261`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L261) — helper() is called by inner() → inner appears in callers of helper.
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool.execute), [`CodeGraphCallersTool`](../../tree_sitter_analyzer/mcp/tools/callers_tool.md#CodeGraphCallersTool)

### `TestSameLineSiblingCallAttribution`
- def: [`tests/unit/test_nested_function_call_edges.py:138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L138)
- doc: Compact brace-style code: a call that sits on the same line as a nested
- signature: `class TestSameLineSiblingCallAttribution:`
- members:
  - `test_helper_attributed_to_outer_not_inner(self)` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L165) — helper() is OUTSIDE inner's body column-wise → caller must be outer.
  - `test_inner_has_no_helper_edge(self)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L179) — inner() has an empty body — it must not appear as caller of helper.
- protocol/private: `_JS_SOURCE`[`L154`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L154), `_js_edges`[`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L156)
- uses (calls/refs, reference-scoped): [`Parser`](../../tree_sitter_analyzer/core/parser.md#Parser), [`tree`](../../tree_sitter_analyzer/core/parser.md#ParseResult.tree), [`parse_code`](../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`success`](../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`error_message`](../../tree_sitter_analyzer/core/parser.md#ParseResult.error_message), [`_extract_call_edges`](../../tree_sitter_analyzer/_ast_extraction.md#_extract_call_edges)

## Functions
- `_parse(source: str, language: str = "python")` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L28)
- `nested_indexed_project(tmp_path: Path)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_nested_function_call_edges.py#L198) — Index a file containing outer() { def inner(): calls helper() }.

