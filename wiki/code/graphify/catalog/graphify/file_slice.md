---
title: 'Module: graphify/file_slice.py'
type: catalog
provenance: extracted
module: graphify/file_slice.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.file_slice`/
symbols:
  FileSlice: FileSlice#
  expand_oversized_files: expand_oversized_files().
  bisect_slice: bisect_slice().
  FileSlice.end: FileSlice#end.
  unit_path: unit_path().
  read_slice_text: read_slice_text().
  FileSlice.start: FileSlice#start.
  slice_boundaries: slice_boundaries().
  FileSlice.path: FileSlice#path.
  is_splittable_text: is_splittable_text().
  FileSlice.total: FileSlice#total.
  FileSlice.index: FileSlice#index.
  _best_cut: _best_cut().
  _SPLITTABLE_TEXT_SUFFIXES: _SPLITTABLE_TEXT_SUFFIXES.
  _BOUNDARY_SEPARATORS: _BOUNDARY_SEPARATORS.
  Unit: Unit.
---
# Module: [`graphify/file_slice.py`](../../../../../raw/code/graphify/graphify/file_slice.py)

## Classes
### `FileSlice`
- def: [`graphify/file_slice.py:38`](../../../../../raw/code/graphify/graphify/file_slice.py#L38) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- doc: A contiguous `[start, end)` character range of a splittable text file.
- signature: `class FileSlice:`
- members:
  - `end` — [`L48`](../../../../../raw/code/graphify/graphify/file_slice.py#L48) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
  - `index` — [`L49`](../../../../../raw/code/graphify/graphify/file_slice.py#L49) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
  - `path` — [`L46`](../../../../../raw/code/graphify/graphify/file_slice.py#L46) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
  - `start` — [`L47`](../../../../../raw/code/graphify/graphify/file_slice.py#L47) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
  - `total` — [`L50`](../../../../../raw/code/graphify/graphify/file_slice.py#L50) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- used by: [`extract_files_direct`](llm.md#extract_files_direct), [`extract_corpus_parallel`](llm.md#extract_corpus_parallel), [`_estimate_file_tokens`](llm.md#_estimate_file_tokens), [`expand_oversized_files`](file_slice.md#expand_oversized_files), [`_pack_chunks_by_tokens`](llm.md#_pack_chunks_by_tokens), [`_read_files`](llm.md#_read_files), [`bisect_slice`](file_slice.md#bisect_slice), [`read_slice_text`](file_slice.md#read_slice_text), [`unit_path`](file_slice.md#unit_path), [`_partition_semantic_files`](llm.md#_partition_semantic_files), [`_split_lone_slice`](llm.md#_extract_with_adaptive_retry._split_lone_slice)  (7 test-only)

## Functions
- `_best_cut(text: str, start: int, end: int)` — [`L67`](../../../../../raw/code/graphify/graphify/file_slice.py#L67) — Return a cut index in ``(start, end]`` at the strongest nearby boundary. — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `bisect_slice(fs: FileSlice)` — [`L142`](../../../../../raw/code/graphify/graphify/file_slice.py#L142) — Split a slice into two halves at a newline near its midpoint, or None. — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `expand_oversized_files(files: list[Path], max_chars: int)` — [`L107`](../../../../../raw/code/graphify/graphify/file_slice.py#L107) — Replace each oversized splittable-text file with a list of ``FileSlice``s. — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `is_splittable_text(path: Path)` — [`L62`](../../../../../raw/code/graphify/graphify/file_slice.py#L62) — True for plain-text document types that may be sliced. — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `read_slice_text(fs: FileSlice)` — [`L136`](../../../../../raw/code/graphify/graphify/file_slice.py#L136) — Read just this slice's characters from its parent file. — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `slice_boundaries(text: str, max_chars: int)` — [`L86`](../../../../../raw/code/graphify/graphify/file_slice.py#L86) — Contiguous ``(start, end)`` ranges covering all of ``text``, each ≤ max_chars. — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `unit_path(unit: Path | FileSlice)` — [`L57`](../../../../../raw/code/graphify/graphify/file_slice.py#L57) — The on-disk path a unit belongs to (the parent file for a slice). — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)

## Module values
- `Unit` — [`L54`](../../../../../raw/code/graphify/graphify/file_slice.py#L54)
- `_BOUNDARY_SEPARATORS` — [`L34`](../../../../../raw/code/graphify/graphify/file_slice.py#L34) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `_SPLITTABLE_TEXT_SUFFIXES` — [`L29`](../../../../../raw/code/graphify/graphify/file_slice.py#L29) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)

