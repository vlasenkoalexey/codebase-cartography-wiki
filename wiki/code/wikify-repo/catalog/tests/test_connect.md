---
title: 'Module: tests/test_connect.py'
type: catalog
provenance: extracted
module: tests/test_connect.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `tests.test_connect`/
symbols:
  test_name_match_across_repos: test_name_match_across_repos().
  test_explicit_tag_beats_name_and_ranks_first: test_explicit_tag_beats_name_and_ranks_first().
  test_curated_vocab_dir_is_not_a_silo: test_curated_vocab_dir_is_not_a_silo().
  test_apply_is_idempotent_and_reflects_connection_state: test_apply_is_idempotent_and_reflects_connection_state().
  _build: _build().
  _silo: _silo().
  test_apply_writes_inline_bidirectional_links: test_apply_writes_inline_bidirectional_links().
  _vocab: _vocab().
  test_prefix_token_matching: test_prefix_token_matching().
---
# Module: [`tests/test_connect.py`](../../../../../raw/code/wikify-repo/tests/test_connect.py)

## Functions
- `_build(wiki: Path)` — [`L31`](../../../../../raw/code/wikify-repo/tests/test_connect.py#L31)
- `_silo(wiki: Path, subdir: str, slug: str, pages: dict[str, str])` — [`L15`](../../../../../raw/code/wikify-repo/tests/test_connect.py#L15) — Create a silo: wiki/<subdir>/<slug>/{overview.md, concepts/*.md}.
- `_vocab(wiki: Path, keys: list[str])` — [`L24`](../../../../../raw/code/wikify-repo/tests/test_connect.py#L24)
- `test_apply_is_idempotent_and_reflects_connection_state(tmp_path)` — [`L126`](../../../../../raw/code/wikify-repo/tests/test_connect.py#L126)
- `test_apply_writes_inline_bidirectional_links(tmp_path)` — [`L100`](../../../../../raw/code/wikify-repo/tests/test_connect.py#L100)
- `test_curated_vocab_dir_is_not_a_silo(tmp_path)` — [`L91`](../../../../../raw/code/wikify-repo/tests/test_connect.py#L91)
- `test_explicit_tag_beats_name_and_ranks_first(tmp_path)` — [`L61`](../../../../../raw/code/wikify-repo/tests/test_connect.py#L61)
- `test_name_match_across_repos(tmp_path)` — [`L37`](../../../../../raw/code/wikify-repo/tests/test_connect.py#L37)
- `test_prefix_token_matching()` — [`L79`](../../../../../raw/code/wikify-repo/tests/test_connect.py#L79)

