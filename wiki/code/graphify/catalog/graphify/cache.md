---
title: 'Module: graphify/cache.py'
type: catalog
provenance: extracted
module: graphify/cache.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.cache`/
symbols:
  file_hash: file_hash().
  save_cached: save_cached().
  cache_dir: cache_dir().
  load_cached: load_cached().
  _ensure_stat_index: _ensure_stat_index().
  prune_semantic_cache: prune_semantic_cache().
  _body_content: _body_content().
  _flush_stat_index: _flush_stat_index().
  clear_cache: clear_cache().
  _stat_index._stat_index: _stat_index._stat_index.
  _stat_index_root._stat_index_root: _stat_index_root._stat_index_root.
  check_semantic_cache: check_semantic_cache().
  _stat_index_dirty._stat_index_dirty: _stat_index_dirty._stat_index_dirty.
  _EXTRACTOR_VERSION: _EXTRACTOR_VERSION.
  _stat_index_file: _stat_index_file().
  cached_files: cached_files().
  save_semantic_cache: save_semantic_cache().
  _cleanup_stale_ast_entries: _cleanup_stale_ast_entries().
  _FRONTMATTER_DELIM: _FRONTMATTER_DELIM.
  _normalize_path: _normalize_path().
  _cleaned_ast_dirs._cleaned_ast_dirs: _cleaned_ast_dirs._cleaned_ast_dirs.
  _relativize_source_files_in: _relativize_source_files_in().
  _absolutize_source_files_in: _absolutize_source_files_in().
---
# Module: [`graphify/cache.py`](../../../../../raw/code/graphify/graphify/cache.py)

## Functions
- `_absolutize_source_files_in(payload: dict, root: Path)` — [`L244`](../../../../../raw/code/graphify/graphify/cache.py#L244) — Inverse of :func:`_relativize_source_files_in`. — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_body_content(content: bytes)` — [`L71`](../../../../../raw/code/graphify/graphify/cache.py#L71) — Strip YAML frontmatter from Markdown content, returning only the body. — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_cleanup_stale_ast_entries(ast_base: Path, current_dir: Path)` — [`L37`](../../../../../raw/code/graphify/graphify/cache.py#L37) — Remove AST cache entries left behind by other graphify versions. — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_ensure_stat_index(root: Path)` — [`L103`](../../../../../raw/code/graphify/graphify/cache.py#L103) — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_flush_stat_index()` — [`L119`](../../../../../raw/code/graphify/graphify/cache.py#L119) — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_normalize_path(path: Path)` — [`L145`](../../../../../raw/code/graphify/graphify/cache.py#L145) — Normalize path for consistent cache keys across Windows path spellings. — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_relativize_source_files_in(payload: dict, root: Path)` — [`L208`](../../../../../raw/code/graphify/graphify/cache.py#L208) — Mutate ``payload`` to rewrite absolute ``source_file`` fields as — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_stat_index_file(root: Path)` — [`L97`](../../../../../raw/code/graphify/graphify/cache.py#L97) — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `cache_dir(root: Path = Path("."), kind: str = "ast")` — [`L272`](../../../../../raw/code/graphify/graphify/cache.py#L272) — Returns the cache directory for ``kind`` - creates it if needed. — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `cached_files(root: Path = Path("."))` — [`L380`](../../../../../raw/code/graphify/graphify/cache.py#L380) — Return set of file hashes that have a valid cache entry (any kind).
- `check_semantic_cache(files: list[str], root: Path = Path("."))` — [`L448`](../../../../../raw/code/graphify/graphify/cache.py#L448) — Check semantic extraction cache for a list of absolute file paths. — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `clear_cache(root: Path = Path("."))` — [`L395`](../../../../../raw/code/graphify/graphify/cache.py#L395) — Delete all cache entries (ast/, semantic/, and legacy flat entries).
- `file_hash(path: Path, root: Path = Path("."))` — [`L156`](../../../../../raw/code/graphify/graphify/cache.py#L156) — SHA256 of file contents + path relative to root. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `load_cached(path: Path, root: Path = Path("."), kind: str = "ast")` — [`L293`](../../../../../raw/code/graphify/graphify/cache.py#L293) — Return cached extraction for this file if hash matches, else None. — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `prune_semantic_cache(root: Path, live_hashes: set[str])` — [`L410`](../../../../../raw/code/graphify/graphify/cache.py#L410) — Remove orphaned semantic cache entries, returning the count pruned.
- `save_cached(path: Path, result: dict, root: Path = Path("."), kind: str = "ast")` — [`L325`](../../../../../raw/code/graphify/graphify/cache.py#L325) — Save extraction result for this file. — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `save_semantic_cache(nodes: list[dict], edges: list[dict], hyperedges: list[dict] | None = None, root: Path = Path("."))` — [`L477`](../../../../../raw/code/graphify/graphify/cache.py#L477) — Save semantic extraction results to cache, keyed by source_file. — documented in [graphify-cache](../../concepts/graphify-cache.md)

## Module values
- `_EXTRACTOR_VERSION` — [`L29`](../../../../../raw/code/graphify/graphify/cache.py#L29) — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_FRONTMATTER_DELIM` — [`L68`](../../../../../raw/code/graphify/graphify/cache.py#L68) — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_cleaned_ast_dirs` — [`L34`](../../../../../raw/code/graphify/graphify/cache.py#L34) — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_stat_index` — [`L92`](../../../../../raw/code/graphify/graphify/cache.py#L92) — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_stat_index_dirty` — [`L94`](../../../../../raw/code/graphify/graphify/cache.py#L94) — documented in [graphify-cache](../../concepts/graphify-cache.md)
- `_stat_index_root` — [`L93`](../../../../../raw/code/graphify/graphify/cache.py#L93) — documented in [graphify-cache](../../concepts/graphify-cache.md)

