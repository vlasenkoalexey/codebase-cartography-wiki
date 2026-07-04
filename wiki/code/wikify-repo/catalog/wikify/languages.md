---
title: 'Module: wikify/languages.py'
type: catalog
provenance: extracted
module: wikify/languages.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `wikify.languages`/
symbols:
  LANGS.LANGS: LANGS.LANGS.
  detect_languages: detect_languages().
  ensure_indexer: ensure_indexer().
  scip_path: scip_path().
  _has_ext: _has_ext().
  Lang: Lang#
  Lang.bin: Lang#bin.
  Lang.label: Lang#label.
  Lang.install: Lang#install.
  Lang.scip_suffix: Lang#scip_suffix.
  Lang.run: Lang#run.
  AUTO_RUN.AUTO_RUN: AUTO_RUN.AUTO_RUN.
  Lang.exts: Lang#exts.
  Lang.markers: Lang#markers.
  _MIN_FILES: _MIN_FILES.
  _SKIP_DIRS: _SKIP_DIRS.
  _WALK_CAP: _WALK_CAP.
  Lang.key: Lang#key.
---
# Module: [`wikify/languages.py`](../../../../../raw/code/wikify-repo/wikify/languages.py)

## Classes
### `Lang`
- def: [`wikify/languages.py:27`](../../../../../raw/code/wikify-repo/wikify/languages.py#L27) — documented in [wikify-languages](../../concepts/wikify-languages.md)
- signature: `class Lang:`
- members:
  - `bin` — [`L32`](../../../../../raw/code/wikify-repo/wikify/languages.py#L32) — documented in [wikify-languages](../../concepts/wikify-languages.md)
  - `exts` — [`L30`](../../../../../raw/code/wikify-repo/wikify/languages.py#L30) — documented in [wikify-languages](../../concepts/wikify-languages.md)
  - `install` — [`L33`](../../../../../raw/code/wikify-repo/wikify/languages.py#L33) — documented in [wikify-languages](../../concepts/wikify-languages.md)
  - `key` — [`L28`](../../../../../raw/code/wikify-repo/wikify/languages.py#L28)
  - `label` — [`L29`](../../../../../raw/code/wikify-repo/wikify/languages.py#L29) — documented in [wikify-languages](../../concepts/wikify-languages.md)
  - `markers` — [`L31`](../../../../../raw/code/wikify-repo/wikify/languages.py#L31) — documented in [wikify-languages](../../concepts/wikify-languages.md)
  - `run` — [`L35`](../../../../../raw/code/wikify-repo/wikify/languages.py#L35)
  - `scip_suffix` — [`L34`](../../../../../raw/code/wikify-repo/wikify/languages.py#L34) — documented in [wikify-languages](../../concepts/wikify-languages.md)
- used by: [`prepare`](cli.md#prepare), [`LANGS`](languages.md#LANGS.LANGS), [`detect_languages`](languages.md#detect_languages), [`ensure_indexer`](languages.md#ensure_indexer), [`scip_path`](languages.md#scip_path)  (1 test-only)

## Functions
- `_has_ext(repo: Path, exts: tuple[str, ...])` — [`L72`](../../../../../raw/code/wikify-repo/wikify/languages.py#L72) — documented in [wikify-languages](../../concepts/wikify-languages.md)
- `detect_languages(repo_dir: str | Path)` — [`L88`](../../../../../raw/code/wikify-repo/wikify/languages.py#L88) — Languages present in the repo — a root marker file, or ≥ _MIN_FILES source files. — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `ensure_indexer(lang: Lang)` — [`L102`](../../../../../raw/code/wikify-repo/wikify/languages.py#L102) — True if ``lang.bin`` is available. Otherwise print install guidance and — only when — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `scip_path(cache_dir: str | Path, slug: str, key: str)` — [`L98`](../../../../../raw/code/wikify-repo/wikify/languages.py#L98) — documented in [wikify-languages](../../concepts/wikify-languages.md)

## Module values
- `AUTO_RUN` — [`L64`](../../../../../raw/code/wikify-repo/wikify/languages.py#L64)
- `LANGS` — [`L38`](../../../../../raw/code/wikify-repo/wikify/languages.py#L38) — documented in [wikify-languages](../../concepts/wikify-languages.md)
- `_MIN_FILES` — [`L66`](../../../../../raw/code/wikify-repo/wikify/languages.py#L66) — documented in [wikify-languages](../../concepts/wikify-languages.md)
- `_SKIP_DIRS` — [`L67`](../../../../../raw/code/wikify-repo/wikify/languages.py#L67) — documented in [wikify-languages](../../concepts/wikify-languages.md)
- `_WALK_CAP` — [`L69`](../../../../../raw/code/wikify-repo/wikify/languages.py#L69) — documented in [wikify-languages](../../concepts/wikify-languages.md)

