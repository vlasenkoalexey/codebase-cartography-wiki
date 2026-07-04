---
title: 'Module: graphify/extractors/elixir.py'
type: catalog
provenance: extracted
module: graphify/extractors/elixir.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.extractors.elixir`/extract_elixir().
symbols:
  extract_elixir: ''
  extract_elixir.walk: walk().
  extract_elixir.walk_calls: walk_calls().
  extract_elixir.add_edge: add_edge().
  extract_elixir._get_alias_modules._text: _get_alias_modules()._text().
  extract_elixir._get_alias_modules: _get_alias_modules().
  extract_elixir.add_node: add_node().
  extract_elixir._get_alias_text: _get_alias_text().
---
# Module: [`graphify/extractors/elixir.py`](../../../../../../raw/code/graphify/graphify/extractors/elixir.py)

## Functions
- `_get_alias_modules(node)` — [`L61`](../../../../../../raw/code/graphify/graphify/extractors/elixir.py#L61) — Every module named by an alias/import/require/use argument.
- `_get_alias_text(node)` — [`L55`](../../../../../../raw/code/graphify/graphify/extractors/elixir.py#L55)
- `_text(n)` — [`L69`](../../../../../../raw/code/graphify/graphify/extractors/elixir.py#L69)
- `add_edge(src: str, tgt: str, relation: str, line: int, confidence: str = "EXTRACTED", weight: float = 1, context: str | None = None)` — [`L40`](../../../../../../raw/code/graphify/graphify/extractors/elixir.py#L40)
- `add_node(nid: str, label: str, line: int)` — [`L34`](../../../../../../raw/code/graphify/graphify/extractors/elixir.py#L34)
- `extract_elixir(path: Path)` — [`L10`](../../../../../../raw/code/graphify/graphify/extractors/elixir.py#L10) — Extract modules, functions, imports, and calls from a .ex/.exs file. — documented in [graphify-extract](../../../concepts/graphify-extract.md)
- `walk(node, parent_module_nid: str | None = None)` — [`L90`](../../../../../../raw/code/graphify/graphify/extractors/elixir.py#L90) — documented in [graphify-extractors-base](../../../concepts/graphify-extractors-base.md)
- `walk_calls(node, caller_nid: str)` — [`L177`](../../../../../../raw/code/graphify/graphify/extractors/elixir.py#L177)

