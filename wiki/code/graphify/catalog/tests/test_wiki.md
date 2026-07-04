---
title: 'Module: tests/test_wiki.py'
type: catalog
provenance: extracted
module: tests/test_wiki.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_wiki`/
symbols:
  _make_graph: _make_graph().
  LABELS: LABELS.
  COMMUNITIES: COMMUNITIES.
  test_wiki_links_resolve_to_real_files: test_wiki_links_resolve_to_real_files().
  test_to_wiki_writes_index: test_to_wiki_writes_index().
  test_to_wiki_returns_article_count: test_to_wiki_returns_article_count().
  test_wiki_emits_no_obsidian_wikilinks: test_wiki_emits_no_obsidian_wikilinks().
  test_wiki_links_to_nodes_without_articles_are_plain_text: test_wiki_links_to_nodes_without_articles_are_plain_text().
  test_to_wiki_god_node_article_created: test_to_wiki_god_node_article_created().
  test_index_lists_god_nodes: test_index_lists_god_nodes().
  test_community_article_shows_cohesion: test_community_article_shows_cohesion().
  test_god_node_article_has_connections: test_god_node_article_has_connections().
  test_god_node_article_links_community: test_god_node_article_links_community().
  test_to_wiki_community_articles_created: test_to_wiki_community_articles_created().
  test_index_links_all_communities: test_index_links_all_communities().
  test_community_article_has_cross_links: test_community_article_has_cross_links().
  test_community_article_has_audit_trail: test_community_article_has_audit_trail().
  test_to_wiki_skips_missing_god_node_ids: test_to_wiki_skips_missing_god_node_ids().
  test_to_wiki_no_labels_uses_fallback: test_to_wiki_no_labels_uses_fallback().
  test_article_navigation_footer: test_article_navigation_footer().
  test_wiki_link_display_keeps_label_but_target_is_filename: test_wiki_link_display_keeps_label_but_target_is_filename().
  GOD_NODES: GOD_NODES.
  _inline_links: _inline_links().
  test_to_wiki_drops_stale_community_nodes: test_to_wiki_drops_stale_community_nodes().
  test_to_wiki_all_stale_raises: test_to_wiki_all_stale_raises().
  test_to_wiki_stale_nodes_prints_warning: test_to_wiki_stale_nodes_prints_warning().
  COHESION: COHESION.
  test_wiki_special_characters_in_label_resolve: test_wiki_special_characters_in_label_resolve().
  test_wiki_links_use_collision_suffixed_slug: test_wiki_links_use_collision_suffixed_slug().
  test_community_article_truncation_notice: test_community_article_truncation_notice().
  test_cross_community_links_without_node_community_attrs: test_cross_community_links_without_node_community_attrs().
  test_god_node_article_community_without_node_attr: test_god_node_article_community_without_node_attr().
  test_community_article_handles_null_source_file: test_community_article_handles_null_source_file().
  test_to_wiki_case_only_distinct_labels_dont_overwrite: test_to_wiki_case_only_distinct_labels_dont_overwrite().
  test_to_wiki_god_node_label_case_collides_with_community: test_to_wiki_god_node_label_case_collides_with_community().
  test_wiki_link_with_bracketed_label_resolves: test_wiki_link_with_bracketed_label_resolves().
  _MD_LINK: _MD_LINK.
---
# Module: [`tests/test_wiki.py`](../../../../../raw/code/graphify/tests/test_wiki.py)

## Functions
- `_inline_links(text)` — [`L12`](../../../../../raw/code/graphify/tests/test_wiki.py#L12) — Yield (display, decoded_target) for each inline markdown link, skipping
- `_make_graph()` — [`L23`](../../../../../raw/code/graphify/tests/test_wiki.py#L23)
- `test_article_navigation_footer(tmp_path)` — [`L143`](../../../../../raw/code/graphify/tests/test_wiki.py#L143)
- `test_community_article_handles_null_source_file(tmp_path)` — [`L224`](../../../../../raw/code/graphify/tests/test_wiki.py#L224) — source_file=None on a node must not crash sorted() with TypeError (#1016).
- `test_community_article_has_audit_trail(tmp_path)` — [`L98`](../../../../../raw/code/graphify/tests/test_wiki.py#L98)
- `test_community_article_has_cross_links(tmp_path)` — [`L83`](../../../../../raw/code/graphify/tests/test_wiki.py#L83)
- `test_community_article_shows_cohesion(tmp_path)` — [`L91`](../../../../../raw/code/graphify/tests/test_wiki.py#L91)
- `test_community_article_truncation_notice(tmp_path)` — [`L150`](../../../../../raw/code/graphify/tests/test_wiki.py#L150) — Communities with more than 25 nodes show a truncation notice.
- `test_cross_community_links_without_node_community_attrs(tmp_path)` — [`L165`](../../../../../raw/code/graphify/tests/test_wiki.py#L165) — Cross-community links must work even when nodes have no 'community' attribute (#925).
- `test_god_node_article_community_without_node_attr(tmp_path)` — [`L178`](../../../../../raw/code/graphify/tests/test_wiki.py#L178) — God node article must show community name even when node has no 'community' attr (#925).
- `test_god_node_article_has_connections(tmp_path)` — [`L106`](../../../../../raw/code/graphify/tests/test_wiki.py#L106)
- `test_god_node_article_links_community(tmp_path)` — [`L117`](../../../../../raw/code/graphify/tests/test_wiki.py#L117)
- `test_index_links_all_communities(tmp_path)` — [`L67`](../../../../../raw/code/graphify/tests/test_wiki.py#L67)
- `test_index_lists_god_nodes(tmp_path)` — [`L75`](../../../../../raw/code/graphify/tests/test_wiki.py#L75)
- `test_to_wiki_all_stale_raises(tmp_path)` — [`L206`](../../../../../raw/code/graphify/tests/test_wiki.py#L206) — If every community node is stale, raise ValueError with a helpful message (#936).
- `test_to_wiki_case_only_distinct_labels_dont_overwrite(tmp_path)` — [`L237`](../../../../../raw/code/graphify/tests/test_wiki.py#L237) — Two community labels differing only by case must each get their own
- `test_to_wiki_community_articles_created(tmp_path)` — [`L54`](../../../../../raw/code/graphify/tests/test_wiki.py#L54)
- `test_to_wiki_drops_stale_community_nodes(tmp_path)` — [`L194`](../../../../../raw/code/graphify/tests/test_wiki.py#L194) — Stale node IDs in communities dict are silently dropped without crash (#936).
- `test_to_wiki_god_node_article_created(tmp_path)` — [`L61`](../../../../../raw/code/graphify/tests/test_wiki.py#L61)
- `test_to_wiki_god_node_label_case_collides_with_community(tmp_path)` — [`L257`](../../../../../raw/code/graphify/tests/test_wiki.py#L257) — Community and god-node articles share one slug-dedup set, so a god-node
- `test_to_wiki_no_labels_uses_fallback(tmp_path)` — [`L133`](../../../../../raw/code/graphify/tests/test_wiki.py#L133)
- `test_to_wiki_returns_article_count(tmp_path)` — [`L47`](../../../../../raw/code/graphify/tests/test_wiki.py#L47)
- `test_to_wiki_skips_missing_god_node_ids(tmp_path)` — [`L124`](../../../../../raw/code/graphify/tests/test_wiki.py#L124) — God node with bad ID should not crash.
- `test_to_wiki_stale_nodes_prints_warning(tmp_path, capsys)` — [`L214`](../../../../../raw/code/graphify/tests/test_wiki.py#L214) — Stale node IDs trigger a stderr warning showing the drop count (#936).
- `test_to_wiki_writes_index(tmp_path)` — [`L41`](../../../../../raw/code/graphify/tests/test_wiki.py#L41)
- `test_wiki_emits_no_obsidian_wikilinks(tmp_path)` — [`L279`](../../../../../raw/code/graphify/tests/test_wiki.py#L279) — No generated file may contain Obsidian [[...]] syntax. Those links resolve
- `test_wiki_link_display_keeps_label_but_target_is_filename(tmp_path)` — [`L305`](../../../../../raw/code/graphify/tests/test_wiki.py#L305) — The fix's whole point: a link's display text is the human label (with
- `test_wiki_link_with_bracketed_label_resolves(tmp_path)` — [`L338`](../../../../../raw/code/graphify/tests/test_wiki.py#L338) — A label containing `[` / `]` (e.g. a generic like `Array[T]`) still
- `test_wiki_links_resolve_to_real_files(tmp_path)` — [`L289`](../../../../../raw/code/graphify/tests/test_wiki.py#L289) — Every inline markdown link target across the whole wiki must point at a
- `test_wiki_links_to_nodes_without_articles_are_plain_text(tmp_path)` — [`L356`](../../../../../raw/code/graphify/tests/test_wiki.py#L356) — A god node links its neighbours, but only communities and god nodes get
- `test_wiki_links_use_collision_suffixed_slug(tmp_path)` — [`L376`](../../../../../raw/code/graphify/tests/test_wiki.py#L376) — When two labels collide on disk and the second article gets a numeric
- `test_wiki_special_characters_in_label_resolve(tmp_path)` — [`L316`](../../../../../raw/code/graphify/tests/test_wiki.py#L316) — Labels with spaces, &, #, and parentheses must still produce a link whose

## Module values
- `COHESION` — [`L37`](../../../../../raw/code/graphify/tests/test_wiki.py#L37)
- `COMMUNITIES` — [`L35`](../../../../../raw/code/graphify/tests/test_wiki.py#L35)
- `GOD_NODES` — [`L38`](../../../../../raw/code/graphify/tests/test_wiki.py#L38)
- `LABELS` — [`L36`](../../../../../raw/code/graphify/tests/test_wiki.py#L36)
- `_MD_LINK` — [`L9`](../../../../../raw/code/graphify/tests/test_wiki.py#L9)

