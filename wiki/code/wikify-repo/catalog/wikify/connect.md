---
title: 'Module: wikify/connect.py'
type: catalog
provenance: extracted
module: wikify/connect.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `wikify.connect`/
symbols:
  apply_connections: apply_connections().
  build_index: build_index().
  discover_silos: discover_silos().
  _down_block: _down_block().
  compute_report: compute_report().
  _page_matches_key: _page_matches_key().
  _token_matches: _token_matches().
  _up_block: _up_block().
  Match.repo: Match#repo.
  _tokens: _tokens().
  connected_keys: connected_keys().
  Match: Match#
  SiloPage: SiloPage#
  SiloPage.repo: SiloPage#repo.
  SiloPage.path: SiloPage#path.
  _DOWN_BEGIN: _DOWN_BEGIN.
  SiloPage.rel_from_wiki: SiloPage#rel_from_wiki.
  Match.rel_from_wiki: Match#rel_from_wiki.
  Match.confidence: Match#confidence.
  load_vocabulary: load_vocabulary().
  _insert_after_frontmatter_h1: _insert_after_frontmatter_h1().
  _UP_BEGIN: _UP_BEGIN.
  _DOWN_END: _DOWN_END.
  _UP_END: _UP_END.
  SiloPage.title: SiloPage#title.
  SiloPage.tags: SiloPage#tags.
  SiloPage.tokens: SiloPage#tokens.
  _frontmatter_span: _frontmatter_span().
  _replace_block: _replace_block().
  _relpath: _relpath().
  _STOP: _STOP.
  _MIN_PREFIX: _MIN_PREFIX.
  Match.path: Match#path.
  Match.title: Match#title.
---
# Module: [`wikify/connect.py`](../../../../../raw/code/wikify-repo/wikify/connect.py)

## Classes
### `Match`
- def: [`wikify/connect.py:80`](../../../../../raw/code/wikify-repo/wikify/connect.py#L80) — documented in [wikify-connect](../../concepts/wikify-connect.md)
- signature: `class Match:`
- members:
  - `confidence` — [`L85`](../../../../../raw/code/wikify-repo/wikify/connect.py#L85) — documented in [wikify-connect](../../concepts/wikify-connect.md)
  - `path` — [`L82`](../../../../../raw/code/wikify-repo/wikify/connect.py#L82) — documented in [wikify-connect](../../concepts/wikify-connect.md)
  - `rel_from_wiki` — [`L83`](../../../../../raw/code/wikify-repo/wikify/connect.py#L83) — documented in [wikify-connect](../../concepts/wikify-connect.md)
  - `repo` — [`L81`](../../../../../raw/code/wikify-repo/wikify/connect.py#L81) — documented in [wikify-connect](../../concepts/wikify-connect.md)
  - `title` — [`L84`](../../../../../raw/code/wikify-repo/wikify/connect.py#L84) — documented in [wikify-connect](../../concepts/wikify-connect.md)
- used by: [`apply_connections`](connect.md#apply_connections), [`build_index`](connect.md#build_index), [`_down_block`](connect.md#_down_block), [`compute_report`](connect.md#compute_report)  (2 test-only)

### `SiloPage`
- def: [`wikify/connect.py:68`](../../../../../raw/code/wikify-repo/wikify/connect.py#L68) — documented in [wikify-connect](../../concepts/wikify-connect.md)
- doc: One silo concept page — the grounding target a vocabulary key resolves to.
- signature: `class SiloPage:`
- members:
  - `path` — [`L72`](../../../../../raw/code/wikify-repo/wikify/connect.py#L72) — documented in [wikify-connect](../../concepts/wikify-connect.md)
  - `rel_from_wiki` — [`L73`](../../../../../raw/code/wikify-repo/wikify/connect.py#L73) — documented in [wikify-connect](../../concepts/wikify-connect.md)
  - `repo` — [`L71`](../../../../../raw/code/wikify-repo/wikify/connect.py#L71) — documented in [wikify-connect](../../concepts/wikify-connect.md)
  - `tags` — [`L75`](../../../../../raw/code/wikify-repo/wikify/connect.py#L75) — documented in [wikify-connect](../../concepts/wikify-connect.md)
  - `title` — [`L74`](../../../../../raw/code/wikify-repo/wikify/connect.py#L74) — documented in [wikify-connect](../../concepts/wikify-connect.md)
  - `tokens` — [`L76`](../../../../../raw/code/wikify-repo/wikify/connect.py#L76) — documented in [wikify-connect](../../concepts/wikify-connect.md)
- used by: [`apply_connections`](connect.md#apply_connections), [`build_index`](connect.md#build_index), [`discover_silos`](connect.md#discover_silos), [`compute_report`](connect.md#compute_report), [`_page_matches_key`](connect.md#_page_matches_key)  (2 test-only)

## Functions
- `_down_block(key: str, hits: list[Match], concept_rel: str)` — [`L206`](../../../../../raw/code/wikify-repo/wikify/connect.py#L206) — The ``## In this wiki's repos`` block for a concept page: links down to each — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_frontmatter_span(text: str)` — [`L88`](../../../../../raw/code/wikify-repo/wikify/connect.py#L88) — Return (frontmatter dict, body_start_index). body_start is the char offset just
- `_insert_after_frontmatter_h1(text: str, block: str)` — [`L231`](../../../../../raw/code/wikify-repo/wikify/connect.py#L231) — Insert ``block`` right after the frontmatter and the first ``# H1`` heading (so an — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_page_matches_key(page: SiloPage, key: str)` — [`L151`](../../../../../raw/code/wikify-repo/wikify/connect.py#L151) — Correspondence confidence of ``page`` to vocabulary ``key`` or None. ``"tag"`` if an — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_relpath(from_wiki_rel: str, to_wiki_rel: str)` — [`L201`](../../../../../raw/code/wikify-repo/wikify/connect.py#L201) — A markdown link from the page at ``wiki/<from_wiki_rel>`` to ``wiki/<to_wiki_rel>``.
- `_replace_block(text: str, begin: str, end: str, block: str | None)` — [`L183`](../../../../../raw/code/wikify-repo/wikify/connect.py#L183) — Replace the ``begin…end`` delimited block with ``block`` (None → remove it). If the — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_token_matches(key_tok: str, page_toks: set[str])` — [`L52`](../../../../../raw/code/wikify-repo/wikify/connect.py#L52) — A key token is present in a page's tokens: exact, or prefix-share ≥ _MIN_PREFIX — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_tokens(text: str)` — [`L47`](../../../../../raw/code/wikify-repo/wikify/connect.py#L47) — Lowercase alphanumeric tokens, split on any non-alnum, stopwords dropped. — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_up_block(page_rel: str, keys: list[str], vocab_subdir: str)` — [`L223`](../../../../../raw/code/wikify-repo/wikify/connect.py#L223) — The one-line up-link block for a silo page: the cross-repo concept(s) it's part of. — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `apply_connections(wiki_dir: str | Path, keys: list[str], vocab_subdir: str = "concepts", exclude: set[str] | None = None)` — [`L258`](../../../../../raw/code/wikify-repo/wikify/connect.py#L258) — Wire the chosen ``keys`` inline and bidirectionally, idempotently. For each key: — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `build_index(silos: list[SiloPage], vocab: list[str])` — [`L163`](../../../../../raw/code/wikify-repo/wikify/connect.py#L163) — Invert (vocabulary × silo pages) → ``concept key → [Match]`` (tag before name, then — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `compute_report(wiki_dir: str | Path, vocab_subdir: str = "concepts")` — [`L321`](../../../../../raw/code/wikify-repo/wikify/connect.py#L321) — A one-screen proposal for ``wikify connect`` stdout: which concepts *could* be — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `connected_keys(wiki_dir: str | Path, vocab_subdir: str = "concepts")` — [`L244`](../../../../../raw/code/wikify-repo/wikify/connect.py#L244) — Vocabulary keys already connected — their concept page carries a down-block. This is — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `discover_silos(wiki_dir: str | Path, vocab_subdir: str = "concepts")` — [`L117`](../../../../../raw/code/wikify-repo/wikify/connect.py#L117) — Every silo concept page in the wiki. A **silo** is any directory holding an — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `load_vocabulary(wiki_dir: str | Path, vocab_subdir: str = "concepts")` — [`L105`](../../../../../raw/code/wikify-repo/wikify/connect.py#L105) — The host wiki's controlled concept vocabulary — stems of ``wiki/<vocab_subdir>/*.md`` — documented in [wikify-connect](../../concepts/wikify-connect.md)

## Module values
- `_DOWN_BEGIN` — [`L41`](../../../../../raw/code/wikify-repo/wikify/connect.py#L41) — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_DOWN_END` — [`L42`](../../../../../raw/code/wikify-repo/wikify/connect.py#L42) — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_MIN_PREFIX` — [`L37`](../../../../../raw/code/wikify-repo/wikify/connect.py#L37) — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_STOP` — [`L33`](../../../../../raw/code/wikify-repo/wikify/connect.py#L33) — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_UP_BEGIN` — [`L43`](../../../../../raw/code/wikify-repo/wikify/connect.py#L43) — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `_UP_END` — [`L44`](../../../../../raw/code/wikify-repo/wikify/connect.py#L44) — documented in [wikify-connect](../../concepts/wikify-connect.md)

