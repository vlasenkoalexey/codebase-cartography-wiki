---
title: 'Module: tests/unit/_codegraph_query_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/_codegraph_query_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit._codegraph_query_helpers`/
symbols:
  _make_def: _make_def().
  _patch_resolver_with: _patch_resolver_with().
  _patch_resolver_with.FakeBackend.relation_entries: _patch_resolver_with().FakeBackend#relation_entries().
  _patch_resolver_with.FakeBackend.__init__: _patch_resolver_with().FakeBackend#__init__().
  _patch_resolver_with.FakeBackend.resolve_definitions: _patch_resolver_with().FakeBackend#resolve_definitions().
  _patch_resolver_with.FakeBackend.semantic_symbols: _patch_resolver_with().FakeBackend#semantic_symbols().
  _patch_resolver_with.FakeBackend: _patch_resolver_with().FakeBackend#
  FakeBackend._real_backend: FakeBackend#_real_backend.
---
# Module: [`tests/unit/_codegraph_query_helpers.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/_codegraph_query_helpers.py)

## Classes
### `FakeBackend`
- def: [`tests/unit/_codegraph_query_helpers.py:32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/_codegraph_query_helpers.py#L32)
- signature: `class FakeBackend:`
- members:
  - `relation_entries(self, **kwargs)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/_codegraph_query_helpers.py#L46)
  - `resolve_definitions(self, token: str)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/_codegraph_query_helpers.py#L36)
  - `semantic_symbols(self, token: str, *, limit: int)` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/_codegraph_query_helpers.py#L41)
- protocol/private: `__init__`[`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/_codegraph_query_helpers.py#L33), `_real_backend`[`L34`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/_codegraph_query_helpers.py#L34)
- uses (calls/refs, reference-scoped): [`CodeGraphQueryBackend`](../../tree_sitter_analyzer/codegraph_query_backend.md#CodeGraphQueryBackend), [`to_dict`](../../tree_sitter_analyzer/symbol_resolver.md#DefinitionLocation.to_dict), [`relation_entries`](../../tree_sitter_analyzer/codegraph_query_backend.md#CodeGraphQueryBackend.relation_entries)
- used by: (1 test-only callers)

## Functions
- `_make_def(file: str = "main.py", name: str = "run", kind: str = "function", line: int = 1, end_line: int = 2, language: str = "python")` — [`L13`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/_codegraph_query_helpers.py#L13)
- `_patch_resolver_with(defs_per_token: dict[str, list[DefinitionLocation]])` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/_codegraph_query_helpers.py#L31)

