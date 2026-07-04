---
title: 'Module: src/codegraphcontext/tools/indexing/resolution/inheritance.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/indexing/resolution/inheritance.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.indexing.resolution.inheritance`/
symbols:
  build_inheritance_and_csharp_files: build_inheritance_and_csharp_files().
  build_decorated_by_links: build_decorated_by_links().
  build_go_implements_links: build_go_implements_links().
  build_metaclass_links: build_metaclass_links().
  build_haskell_implements_links: build_haskell_implements_links().
  build_partial_of_links: build_partial_of_links().
  build_part_of_links: build_part_of_links().
  _expand_go_interface_methods: _expand_go_interface_methods().
  build_companion_of_links: build_companion_of_links().
  build_embeds_links: build_embeds_links().
  build_elixir_implements_links: build_elixir_implements_links().
  _resolve_decorator_path: _resolve_decorator_path().
  resolve_inheritance_link: resolve_inheritance_link().
  _parse_decorator_name: _parse_decorator_name().
---
# Module: [`src/codegraphcontext/tools/indexing/resolution/inheritance.py`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py)

## Functions
- `_expand_go_interface_methods(iface_name: str, interface_methods: Dict[str, set], embedded_bases: Dict[str, List[str]], cache: Dict[str, set])` — [`L119`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L119)
- `_parse_decorator_name(dec_raw: str)` — [`L308`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L308)
- `_resolve_decorator_path(decorator_name: str, caller_file_path: str, local_names: set, local_imports: dict, imports_map: dict)` — [`L315`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L315)
- `build_companion_of_links(all_file_data: List[Dict[str, Any]])` — [`L444`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L444) — Link Kotlin companion objects to their enclosing class.
- `build_decorated_by_links(all_file_data: List[Dict[str, Any]], imports_map: dict)` — [`L339`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L339) — Build DECORATED_BY rows from parsed decorator metadata on functions/classes.
- `build_elixir_implements_links(all_file_data: List[Dict[str, Any]])` — [`L522`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L522) — Create defimpl -> defprotocol IMPLEMENTS edges for Elixir modules.
- `build_embeds_links(all_file_data: List[Dict[str, Any]])` — [`L484`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L484) — Create Go struct embedding EMBEDS edges.
- `build_go_implements_links(all_file_data: List[Dict[str, Any]])` — [`L136`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L136) — Infer Go struct->interface IMPLEMENTS edges from method sets.
- `build_haskell_implements_links(all_file_data: List[Dict[str, Any]])` — [`L191`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L191) — Create typeclass instance IMPLEMENTS edges (data type -> typeclass).
- `build_inheritance_and_csharp_files(all_file_data: List[Dict[str, Any]], imports_map: dict)` — [`L76`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L76) — Returns (inheritance_batch_rows, csharp_file_data_list).
- `build_metaclass_links(all_file_data: List[Dict[str, Any]], imports_map: dict)` — [`L398`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L398) — Build METACLASS rows from Python class metaclass= specifications.
- `build_part_of_links(all_file_data: List[Dict[str, Any]])` — [`L265`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L265) — Link Dart library part files to their library root file.
- `build_partial_of_links(all_file_data: List[Dict[str, Any]])` — [`L219`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L219) — Link C# partial class declarations across files.
- `resolve_inheritance_link(class_item: Dict[str, Any], base_class_str: str, caller_file_path: str, local_class_names: set, local_imports: dict, imports_map: dict)` — [`L9`](../../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/resolution/inheritance.py#L9) — Resolve a single inheritance link. Returns row dict or None.

