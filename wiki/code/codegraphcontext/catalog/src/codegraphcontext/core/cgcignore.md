---
title: 'Module: src/codegraphcontext/core/cgcignore.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/cgcignore.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.cgcignore`/
symbols:
  build_ignore_spec: build_ignore_spec().
  CGCIgnoreMatcher.match_file: CGCIgnoreMatcher#match_file().
  CGCIgnoreMatcher._compile_patterns: CGCIgnoreMatcher#_compile_patterns().
  find_cgcignore: find_cgcignore().
  CGCIgnoreMatcher.rules: CGCIgnoreMatcher#rules.
  parse_cgcignore_lines: parse_cgcignore_lines().
  read_cgcignore_patterns: read_cgcignore_patterns().
  _resolve_explicit_path: _resolve_explicit_path().
  CGCIgnoreMatcher: CGCIgnoreMatcher#
  ensure_default_cgcignore: ensure_default_cgcignore().
  CGCIgnoreMatcher.root_dir: CGCIgnoreMatcher#root_dir.
  CGCIgnoreMatcher._translate_segment: CGCIgnoreMatcher#_translate_segment().
  CGCIgnoreMatcher.__init__: CGCIgnoreMatcher#__init__().
---
# Module: [`src/codegraphcontext/core/cgcignore.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py)

## Classes
### `CGCIgnoreMatcher`
- def: [`src/codegraphcontext/core/cgcignore.py:89`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L89)
- signature: `class CGCIgnoreMatcher:`
- members:
  - `_translate_segment(self, seg: str)` — [`L94`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L94) — Translates a single gitwildmatch segment into regex, completely avoiding fnmatch.
  - `match_file(self, file_path)` — [`L183`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L183) — Returns True if the file should be ignored.
  - `root_dir` — [`L91`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L91)
  - `rules` — [`L92`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L92)
- protocol/private: `__init__`[`L90`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L90), `_compile_patterns`[`L134`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L134)
- uses (calls/refs, reference-scoped): [`warning_logger`](../utils/debug_log.md#warning_logger)
- used by: [`discover_files_to_index`](../tools/indexing/discovery.md#discover_files_to_index), [`build_ignore_spec`](cgcignore.md#build_ignore_spec), [`should_skip_file`](../tools/indexing/scip_pipeline.md#run_scip_index_async.should_skip_file)

## Functions
- `_resolve_explicit_path(ignore_root: Path, explicit_path: Optional[str])` — [`L8`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L8) — Resolve an explicit .cgcignore path relative to *ignore_root*.
- `build_ignore_spec(ignore_root: Path, default_patterns: list[str], explicit_path: Optional[str] = None)` — [`L211`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L211) — Build CGCIgnoreMatcher using merged default + user .cgcignore patterns.
- `ensure_default_cgcignore(path: Path, default_patterns: list[str])` — [`L67`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L67) — Create a .cgcignore file with default patterns when it does not exist.
- `find_cgcignore(ignore_root: Path, explicit_path: Optional[str] = None)` — [`L32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L32) — Find a repository-local .cgcignore, with explicit path fallback.
- `parse_cgcignore_lines(lines: Iterable[str])` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L18) — Return valid ignore patterns from raw .cgcignore lines.
- `read_cgcignore_patterns(path: Path, default_patterns: list[str])` — [`L77`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/cgcignore.py#L77) — Read .cgcignore patterns and merge them with defaults.

