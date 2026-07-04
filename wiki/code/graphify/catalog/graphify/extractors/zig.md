---
title: 'Module: graphify/extractors/zig.py'
type: catalog
provenance: extracted
module: graphify/extractors/zig.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.extractors.zig`/extract_zig().
symbols:
  extract_zig.walk: walk().
  extract_zig: ''
  extract_zig._extract_import: _extract_import().
  extract_zig.walk_calls: walk_calls().
  extract_zig.add_edge: add_edge().
  extract_zig.add_node: add_node().
---
# Module: [`graphify/extractors/zig.py`](../../../../../../raw/code/graphify/graphify/extractors/zig.py)

## Functions
- `_extract_import(node)` — [`L53`](../../../../../../raw/code/graphify/graphify/extractors/zig.py#L53)
- `add_edge(src: str, tgt: str, relation: str, line: int, confidence: str = "EXTRACTED", weight: float = 1, context: str | None = None)` — [`L40`](../../../../../../raw/code/graphify/graphify/extractors/zig.py#L40)
- `add_node(nid: str, label: str, line: int)` — [`L34`](../../../../../../raw/code/graphify/graphify/extractors/zig.py#L34)
- `extract_zig(path: Path)` — [`L10`](../../../../../../raw/code/graphify/graphify/extractors/zig.py#L10) — Extract functions, structs, enums, unions, and imports from a .zig file.
- `walk(node, parent_struct_nid: str | None = None)` — [`L77`](../../../../../../raw/code/graphify/graphify/extractors/zig.py#L77)
- `walk_calls(node, caller_nid: str)` — [`L141`](../../../../../../raw/code/graphify/graphify/extractors/zig.py#L141)

