---
title: Incremental extraction cache
type: concept
provenance: mixed
concept: graphify-cache
concepts: [incremental-reconcile]
updated: 2026-07-04
status: fresh
---
# Incremental extraction cache

<!-- connect:up:begin -->
> **Cross-repo concept:** part of [incremental-reconcile](../../../concepts/incremental-reconcile.md) across this wiki's repos.
<!-- connect:up:end -->
## Overview
Extraction is the expensive half of graphify — AST parsing for code, and LLM calls for
semantic/prose extraction. The cache exists so that re-ingesting a corpus only pays for
the files that actually changed. It is a **content-addressed** store: the cache key is a
SHA256 of a file's *contents plus its path relative to the root*
([`file_hash`](../catalog/graphify/cache.md#file_hash)), and each entry is a JSON blob at
`graphify-out/cache/{kind}/{hash}.json` ([`save_cached`](../catalog/graphify/cache.md#save_cached),
[`load_cached`](../catalog/graphify/cache.md#load_cached)). Two things make it more than a
naive hashmap: a **stat-based fastpath** that skips re-reading unchanged files, and a
deliberate split between an AST cache (versioned by extractor code) and a semantic cache
(unversioned, because re-extraction burns money).

## Diagram
```mermaid
flowchart TD
    L[load_cached path] --> FH[file_hash]
    FH --> SI[_ensure_stat_index]
    SI -->|size+mtime match| FAST[return cached hash]
    SI -->|stat changed| READ[read_bytes → _body_content for .md → SHA256]
    FH --> CD[cache_dir kind]
    CD -->|ast| VER[v{_EXTRACTOR_VERSION} + _cleanup_stale_ast_entries]
    CD -->|semantic| UNV[unversioned dir]
    L --> HIT{hash.json exists?}
    HIT -->|yes| ABS[_absolutize_source_files_in → return dict]
    HIT -->|no| MISS[return None → re-extract → save_cached]
```

## Design rationale (why it's built this way)
**Content hashing, not mtime, is the cache identity.** Because the key is the file's
content plus its *relative* path, a cache written in one checkout works in another —
`file_hash`'s docstring states it plainly: "Using a relative path (not absolute) makes
cache entries portable across machines and checkout directories, so shared caches and CI
work correctly." `test_cache_portable_across_roots` proves a corpus + cache copied to a
different absolute prefix still hits, and that the returned `source_file` is re-anchored to
the new root.

**AST is versioned; semantic is not.** [`cache_dir`](../catalog/graphify/cache.md#cache_dir)
puts AST entries under `cache/ast/v{version}/` but semantic entries under a flat
`cache/semantic/`. The docstring gives the reason: AST results "depend on extractor code,
not just file contents," so a graphify upgrade must invalidate them
(`test_ast_cache_invalidated_on_version_bump`), whereas "re-extraction costs LLM calls" for
semantic entries, so they deliberately survive a version bump
(`test_semantic_cache_survives_version_bump`). The two kinds also live in separate
subdirectories so a semantic entry can't clobber the AST entry for the same file (#582).

**The stat-index is a speed hack, not correctness.** `file_hash` keeps a per-root index of
`{size, mtime_ns → hash}` so an unchanged file returns its stored digest without a full
read — the fastpath. It's populated lazily by
[`_ensure_stat_index`](../catalog/graphify/cache.md#_ensure_stat_index) and flushed once at
process exit via [`_flush_stat_index`](../catalog/graphify/cache.md#_flush_stat_index)
(registered with `atexit`). The content hash is still the source of truth; the stat check
only decides whether to recompute it.

**Markdown metadata must not churn the cache.** For `.md` files, `file_hash` hashes only the
body below the YAML frontmatter, stripped by
[`_body_content`](../catalog/graphify/cache.md#_body_content) using
[`_FRONTMATTER_DELIM`](../catalog/graphify/cache.md#_FRONTMATTER_DELIM). So editing
`status:` or `tags:` doesn't invalidate an expensive semantic extraction
(`test_md_frontmatter_only_change_same_hash`), but editing prose above a mid-document rule
still does (`test_md_edit_above_hr_changes_hash`).

## Entry points
- [`file_hash`](../catalog/graphify/cache.md#file_hash) — computes the content-address for a
  file; the primitive every other cache op is keyed on. Hit whenever a file is considered
  for extraction.
- [`load_cached`](../catalog/graphify/cache.md#load_cached) — the read side; returns the
  cached extraction dict if the hash matches, else `None`. Called by
  [`_extract_single_file`](../catalog/graphify/extract.md#_extract_single_file) (parallel) and
  [`_extract_sequential`](../catalog/graphify/extract.md#_extract_sequential) before doing any
  work.
- [`save_cached`](../catalog/graphify/cache.md#save_cached) — the write side; persists a
  result under its content hash after extraction.
- [`check_semantic_cache`](../catalog/graphify/cache.md#check_semantic_cache) /
  [`save_semantic_cache`](../catalog/graphify/cache.md#save_semantic_cache) — the semantic-kind
  entry points reached from [`main`](../catalog/graphify/__main__.md#main)'s corpus extraction.

## Mechanism (step-by-step)
1. **Hash the file.** [`file_hash`](../catalog/graphify/cache.md#file_hash) normalizes the path
   with [`_normalize_path`](../catalog/graphify/cache.md#_normalize_path) (stable keys across
   Windows spellings), consults the stat index via
   [`_ensure_stat_index`](../catalog/graphify/cache.md#_ensure_stat_index), and if `size` +
   `mtime_ns` match a stored [`_stat_index`](../catalog/graphify/cache.md#_stat_index._stat_index)
   entry, returns the cached digest immediately.
2. **Full hash on miss.** When stat disagrees (or on first sight),
   [`file_hash`](../catalog/graphify/cache.md#file_hash) reads the bytes — running
   [`_body_content`](../catalog/graphify/cache.md#_body_content) first for `.md` — SHA256s the
   content plus the posix relative path, and records the new digest, marking
   [`_stat_index_dirty`](../catalog/graphify/cache.md#_stat_index_dirty._stat_index_dirty) so it
   gets flushed at exit.
3. **Resolve the cache directory.** [`cache_dir`](../catalog/graphify/cache.md#cache_dir) roots
   at [`GRAPHIFY_OUT`](../catalog/graphify/paths.md#GRAPHIFY_OUT), then appends `cache/{kind}`;
   for `ast` it adds `v{_EXTRACTOR_VERSION}`
   ([`_EXTRACTOR_VERSION`](../catalog/graphify/cache.md#_EXTRACTOR_VERSION)) and prunes entries
   left by other versions through
   [`_cleanup_stale_ast_entries`](../catalog/graphify/cache.md#_cleanup_stale_ast_entries)
   (guarded by [`_cleaned_ast_dirs`](../catalog/graphify/cache.md#_cleaned_ast_dirs._cleaned_ast_dirs)
   so it runs once).
4. **Read.** [`load_cached`](../catalog/graphify/cache.md#load_cached) hashes the file, looks for
   `{hash}.json` in the resolved dir, and on a hit re-anchors stored relative `source_file`
   fields back to absolute with
   [`_absolutize_source_files_in`](../catalog/graphify/cache.md#_absolutize_source_files_in) so
   callers see the same shape a fresh extraction produces.
5. **Write.** [`save_cached`](../catalog/graphify/cache.md#save_cached) deep-copies the result,
   rewrites its `source_file` fields to root-relative with
   [`_relativize_source_files_in`](../catalog/graphify/cache.md#_relativize_source_files_in) (so
   the on-disk blob stays portable, #777), and writes atomically via a temp file + `os.replace`
   into the directory from [`cache_dir`](../catalog/graphify/cache.md#cache_dir).
6. **Semantic layer.** [`save_semantic_cache`](../catalog/graphify/cache.md#save_semantic_cache)
   fans nodes/edges out to per-file [`save_cached`](../catalog/graphify/cache.md#save_cached)
   calls under `kind="semantic"`, and
   [`check_semantic_cache`](../catalog/graphify/cache.md#check_semantic_cache) uses
   [`load_cached`](../catalog/graphify/cache.md#load_cached) to report which files already have
   semantic entries — so an `update` only sends the uncached files to the LLM.
7. **Flush.** At process exit [`_flush_stat_index`](../catalog/graphify/cache.md#_flush_stat_index)
   writes the accumulated index to the file from
   [`_stat_index_file`](../catalog/graphify/cache.md#_stat_index_file), keyed on
   [`_stat_index_root`](../catalog/graphify/cache.md#_stat_index_root._stat_index_root).

## Key data structures
- **The stat index** — an in-memory dict
  [`_stat_index`](../catalog/graphify/cache.md#_stat_index._stat_index) mapping resolved paths
  to `{size, mtime_ns, hash}`, persisted per-root; its dirty flag is
  [`_stat_index_dirty`](../catalog/graphify/cache.md#_stat_index_dirty._stat_index_dirty). This
  is the fastpath's whole state.
- **Cache entry** — a JSON dict with `nodes`/`edges`(/`hyperedges`), stored at
  `{hash}.json`, with `source_file` fields relativized on disk (via
  [`_relativize_source_files_in`](../catalog/graphify/cache.md#_relativize_source_files_in)) and
  re-absolutized on load.
- **`_EXTRACTOR_VERSION`** — the string
  ([`_EXTRACTOR_VERSION`](../catalog/graphify/cache.md#_EXTRACTOR_VERSION)) that namespaces the
  AST cache; bumping it is how graphify invalidates every stale AST entry at once.

## Dynamics (design intent)
Extraction is driven by [`extract`](../catalog/graphify/extract.md#extract), which checks the
cache first — the worker [`_extract_single_file`](../catalog/graphify/extract.md#_extract_single_file)
runs in a subprocess and short-circuits on
[`load_cached`](../catalog/graphify/cache.md#load_cached) before parsing, then
[`save_cached`](../catalog/graphify/cache.md#save_cached)s the fresh result; the sequential
fallback [`_extract_sequential`](../catalog/graphify/extract.md#_extract_sequential) does the
same for small batches. The atomic temp-file write in
[`save_cached`](../catalog/graphify/cache.md#save_cached) is what lets parallel workers write
concurrently without corrupting entries; pruning of the semantic cache touches only
`cache/semantic/*.json`, never AST or in-flight temp files
(`test_semantic_prune_ignores_ast_and_tmp`).

## Edge cases
- **Non-files.** [`save_cached`](../catalog/graphify/cache.md#save_cached) no-ops on a path that
  isn't a regular file — subagent-produced semantic fragments occasionally carry a directory
  in `source_file`, and skipping them keeps one bad entry from aborting the batch.
- **Legacy entries.** [`load_cached`](../catalog/graphify/cache.md#load_cached) deliberately does
  not consult pre-versioning flat `cache/` or unversioned `cache/ast/` layouts
  (`test_legacy_unversioned_ast_entries_not_served`), but tolerates old absolute `source_file`
  fields by passing them through.
- **Windows lock on replace.** [`save_cached`](../catalog/graphify/cache.md#save_cached) falls
  back to copy-then-delete when `os.replace` hits a transient `PermissionError`.
- **Non-`.md` files** are always hashed in full — the frontmatter stripping only applies to
  `.md` (`test_non_md_file_hashed_fully`).

## Open questions
- The precise `prune_semantic_cache` logic exercised by the `test_semantic_prune_*` tests is
  not in this packet's subgraph; only the entry points it builds on
  ([`save_cached`](../catalog/graphify/cache.md#save_cached),
  [`cache_dir`](../catalog/graphify/cache.md#cache_dir),
  [`file_hash`](../catalog/graphify/cache.md#file_hash)) are cited here.

## See also
- graphify-watch — the incremental rebuild path that leans on this cache.
- graphify-__main__ — how `extract`/`update` reach the cache.
