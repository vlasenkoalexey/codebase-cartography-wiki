---
title: 'Module: graphify/symbol_resolution.py'
type: catalog
provenance: extracted
module: graphify/symbol_resolution.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.symbol_resolution`/
symbols:
  resolve_python_import_guided_calls: resolve_python_import_guided_calls().
  parse_python_import_aliases: parse_python_import_aliases().
  resolve_bash_source_edges: resolve_bash_source_edges().
  resolve_cross_file_raw_calls: resolve_cross_file_raw_calls().
  node_is_resolvable_symbol: node_is_resolvable_symbol().
  _bash_make_id: _bash_make_id().
  build_python_symbol_index: build_python_symbol_index().
  find_unique_python_symbol: find_unique_python_symbol().
  build_label_index: build_label_index().
  iter_raw_calls: iter_raw_calls().
  normalise_callable_label: normalise_callable_label().
  ImportedSymbol: ImportedSymbol#
  ImportedSymbol.module_stem: ImportedSymbol#module_stem.
  _file_node_id_for_path: _file_node_id_for_path().
  ImportedSymbol.imported_name: ImportedSymbol#imported_name.
  ImportedSymbol.source_location: ImportedSymbol#source_location.
  ImportedSymbol.local_name: ImportedSymbol#local_name.
  existing_edge_pairs: existing_edge_pairs().
  ImportedSymbol.source_file: ImportedSymbol#source_file.
  _module_stem: _module_stem().
  _node_source_stem: _node_source_stem().
---
# Module: [`graphify/symbol_resolution.py`](../../../../../raw/code/graphify/graphify/symbol_resolution.py)

## Classes
### `ImportedSymbol`
- def: [`graphify/symbol_resolution.py:20`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L20) — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- doc: A Python imported name that can be used as deterministic resolution evidence.
- signature: `class ImportedSymbol:`
- members:
  - `imported_name` — [`L24`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L24) — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
  - `local_name` — [`L23`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L23) — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
  - `module_stem` — [`L25`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L25) — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
  - `source_file` — [`L26`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L26)
  - `source_location` — [`L27`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L27) — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- used by: [`resolve_python_import_guided_calls`](symbol_resolution.md#resolve_python_import_guided_calls), [`parse_python_import_aliases`](symbol_resolution.md#parse_python_import_aliases), [`find_unique_python_symbol`](symbol_resolution.md#find_unique_python_symbol)  (4 test-only)

## Functions
- `_bash_make_id(*parts: str)` — [`L380`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L380) — Bash symbol node ID via the single shared recipe (#1378). — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `_file_node_id_for_path(path: Path, root: Path)` — [`L392`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L392) — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `_module_stem(module_name: str | None)` — [`L115`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L115) — Return the final module component used to match Graphify source stems.
- `_node_source_stem(node: dict[str, Any])` — [`L172`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L172) — Return the stem of a node's source file.
- `build_label_index(nodes: list[dict[str, Any]])` — [`L57`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L57) — Build label -> node id list for conservative cross-file resolution. — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `build_python_symbol_index(nodes: list[dict[str, Any]])` — [`L181`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L181) — Build ``(module_stem, normalized_symbol_name) -> node_ids``. — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `existing_edge_pairs(edges: list[dict[str, Any]])` — [`L74`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L74) — Return all existing source/target/relation edge triples. — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `find_unique_python_symbol(symbol_index: dict[tuple[str, str], list[str]], imported: ImportedSymbol)` — [`L206`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L206) — Resolve one imported symbol to exactly one Graphify node id. — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `iter_raw_calls(per_file: Sequence[object])` — [`L91`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L91) — Return raw calls from all per-file extraction fragments. — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `node_is_resolvable_symbol(node: dict[str, Any])` — [`L36`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L36) — Return True when a node is suitable for deterministic symbol lookup. — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `normalise_callable_label(label: str)` — [`L30`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L30) — Normalize a node label into the key used for call resolution. — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `parse_python_import_aliases(path: Path)` — [`L123`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L123) — Parse deterministic Python import aliases from one source file. — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `resolve_bash_source_edges(per_file: Sequence[dict | None], paths: Sequence[Path], root: Path, existing_edges: list[dict] | None = None)` — [`L404`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L404) — Resolve Bash source/import edges and source-backed function calls. — documented in [graphify-symbol_resolution](../../concepts/graphify-symbol_resolution.md)
- `resolve_cross_file_raw_calls(per_file: Sequence[dict[str, Any] | None], all_nodes: list[dict[str, Any]], all_edges: list[dict[str, Any]])` — [`L307`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L307) — Resolve unqualified raw calls conservatively after all files are known. — documented in [graphify-paths](../../concepts/graphify-paths.md)
- `resolve_python_import_guided_calls(per_file: Sequence[object], paths: Sequence[Path], all_nodes: list[dict[str, Any]], all_edges: list[dict[str, Any]])` — [`L218`](../../../../../raw/code/graphify/graphify/symbol_resolution.py#L218) — Resolve raw Python calls using explicit import evidence. — documented in [graphify-security](../../concepts/graphify-security.md)

