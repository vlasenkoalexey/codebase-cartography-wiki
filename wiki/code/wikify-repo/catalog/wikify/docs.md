---
title: 'Module: wikify/docs.py'
type: catalog
provenance: extracted
module: wikify/docs.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `wikify.docs`/
symbols:
  docs_coverage: docs_coverage().
  build_doc_map: build_doc_map().
  lint_docs: lint_docs().
  DocInfo: DocInfo#
  _markdown_anchors: _markdown_anchors().
  DocInfo.relpath: DocInfo#relpath.
  doc_packet_text: doc_packet_text().
  _HeadingHTMLParser.handle_endtag: _HeadingHTMLParser#handle_endtag().
  DocsCoverage.render: DocsCoverage#render().
  DocInfo.anchors: DocInfo#anchors.
  write_doc_packets: write_doc_packets().
  assemble_docs_index: assemble_docs_index().
  _html_anchors: _html_anchors().
  enumerate_docs: enumerate_docs().
  _HeadingHTMLParser.handle_starttag: _HeadingHTMLParser#handle_starttag().
  _ADAPTERS: _ADAPTERS.
  DocsCoverage.uncovered: DocsCoverage#uncovered.
  slugify: slugify().
  DocInfo.page_slug: DocInfo#page_slug().
  _HeadingHTMLParser.handle_data: _HeadingHTMLParser#handle_data().
  DocsCoverage.total: DocsCoverage#total.
  page_source_cites: page_source_cites().
  _HeadingHTMLParser.anchors: _HeadingHTMLParser#anchors.
  _HeadingHTMLParser._h: _HeadingHTMLParser#_h.
  DocsCoverage.covered: DocsCoverage#covered.
  _HeadingHTMLParser._buf: _HeadingHTMLParser#_buf.
  DocsCoverage: DocsCoverage#
  assemble_docs_index._list: assemble_docs_index()._list().
  _SLUG_STRIP: _SLUG_STRIP.
  _ATX: _ATX.
  _SETEXT: _SETEXT.
  _HeadingHTMLParser: _HeadingHTMLParser#
  DEFAULT_DOC_GLOBS: DEFAULT_DOC_GLOBS.
  _SKIP: _SKIP.
  DocInfo.lines: DocInfo#lines.
  _SRC_CITE: _SRC_CITE.
  _outbound_links: _outbound_links().
  _HeadingHTMLParser.__init__: _HeadingHTMLParser#__init__().
---
# Module: [`wikify/docs.py`](../../../../../raw/code/wikify-repo/wikify/docs.py)

## Classes
### `DocInfo`
- def: [`wikify/docs.py:121`](../../../../../raw/code/wikify-repo/wikify/docs.py#L121) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- signature: `class DocInfo:`
- members:
  - `page_slug(self)` — [`L127`](../../../../../raw/code/wikify-repo/wikify/docs.py#L127) — Filename-safe slug for this doc's ``sources/<page_slug>.md`` landing page. — documented in [wikify-docs](../../concepts/wikify-docs.md)
  - `anchors` — [`L123`](../../../../../raw/code/wikify-repo/wikify/docs.py#L123) — documented in [wikify-docs](../../concepts/wikify-docs.md)
  - `lines` — [`L124`](../../../../../raw/code/wikify-repo/wikify/docs.py#L124) — documented in [wikify-docs](../../concepts/wikify-docs.md)
  - `relpath` — [`L122`](../../../../../raw/code/wikify-repo/wikify/docs.py#L122)
- used by: [`_finalize_docs`](cli.md#_finalize_docs), [`_prepare_docs`](cli.md#_prepare_docs), [`docs_coverage`](docs.md#docs_coverage), [`build_doc_map`](docs.md#build_doc_map), [`lint_docs`](docs.md#lint_docs), [`doc_packet_text`](docs.md#doc_packet_text), [`write_doc_packets`](docs.md#write_doc_packets)  (3 test-only)

### `DocsCoverage`
- def: [`wikify/docs.py:203`](../../../../../raw/code/wikify-repo/wikify/docs.py#L203) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- signature: `class DocsCoverage:`
- members:
  - `render(self)` — [`L208`](../../../../../raw/code/wikify-repo/wikify/docs.py#L208)
  - `covered` — [`L205`](../../../../../raw/code/wikify-repo/wikify/docs.py#L205) — documented in [wikify-docs](../../concepts/wikify-docs.md)
  - `total` — [`L204`](../../../../../raw/code/wikify-repo/wikify/docs.py#L204) — documented in [wikify-docs](../../concepts/wikify-docs.md)
  - `uncovered` — [`L206`](../../../../../raw/code/wikify-repo/wikify/docs.py#L206) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- used by: [`_finalize_docs`](cli.md#_finalize_docs), [`docs_coverage`](docs.md#docs_coverage), [`assemble_docs_index`](docs.md#assemble_docs_index)  (1 test-only)

### `_HeadingHTMLParser`  ·  implements/extends HTMLParser
- def: [`wikify/docs.py:66`](../../../../../raw/code/wikify-repo/wikify/docs.py#L66)
- signature: `class _HeadingHTMLParser(HTMLParser):`
- members:
  - `handle_data(self, data: str)` — [`L82`](../../../../../raw/code/wikify-repo/wikify/docs.py#L82)
  - `handle_endtag(self, tag: str)` — [`L86`](../../../../../raw/code/wikify-repo/wikify/docs.py#L86)
  - `handle_starttag(self, tag: str, attrs: list[tuple[str, str | None]])` — [`L73`](../../../../../raw/code/wikify-repo/wikify/docs.py#L73)
  - `anchors` — [`L69`](../../../../../raw/code/wikify-repo/wikify/docs.py#L69)
- protocol/private: `__init__`[`L67`](../../../../../raw/code/wikify-repo/wikify/docs.py#L67), `_buf`[`L71`](../../../../../raw/code/wikify-repo/wikify/docs.py#L71), `_h`[`L70`](../../../../../raw/code/wikify-repo/wikify/docs.py#L70)
- uses (calls/refs, reference-scoped): [`slugify`](docs.md#slugify)
- used by: [`_html_anchors`](docs.md#_html_anchors)

## Functions
- `_html_anchors(text: str)` — [`L94`](../../../../../raw/code/wikify-repo/wikify/docs.py#L94) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- `_list(sub: str)` — [`L328`](../../../../../raw/code/wikify-repo/wikify/docs.py#L328)
- `_markdown_anchors(text: str)` — [`L46`](../../../../../raw/code/wikify-repo/wikify/docs.py#L46) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- `_outbound_links(text: str, docs: set[str], self_rel: str)` — [`L244`](../../../../../raw/code/wikify-repo/wikify/docs.py#L244) — Repo-relative docs this doc links to (markdown links resolved against its dir).
- `assemble_docs_index(wiki_slug_dir: str | Path, slug: str, commit: str, date: str, cov: DocsCoverage)` — [`L323`](../../../../../raw/code/wikify-repo/wikify/docs.py#L323)
- `build_doc_map(repo_dir: Path, docs: list[str])` — [`L146`](../../../../../raw/code/wikify-repo/wikify/docs.py#L146) — Parse each doc's anchors via its format adapter → the resolvable-anchor table. — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `doc_packet_text(repo_dir: Path, slug: str, commit: str, info: DocInfo, doc_map: dict[str, DocInfo], date: str, max_lines: int = 500)` — [`L263`](../../../../../raw/code/wikify-repo/wikify/docs.py#L263) — The packet for one doc: provenance, ready-to-paste ``src:`` citations, the doc text — documented in [wikify-docs](../../concepts/wikify-docs.md)
- `docs_coverage(doc_map: dict[str, DocInfo], wiki_slug_dir: str | Path)` — [`L218`](../../../../../raw/code/wikify-repo/wikify/docs.py#L218) — A doc is *represented* if it has a ``sources/<page_slug>.md`` page or is cited anywhere. — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `enumerate_docs(repo_dir: Path, globs: list[str] | None)` — [`L132`](../../../../../raw/code/wikify-repo/wikify/docs.py#L132) — Repo-relative doc paths matched by ``globs`` (sorted, deduped, vendor-skipped).
- `lint_docs(wiki_slug_dir: str | Path, doc_map: dict[str, DocInfo])` — [`L175`](../../../../../raw/code/wikify-repo/wikify/docs.py#L175) — Gate: every ``src:`` citation must resolve to a real doc + (if given) a real anchor. — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `page_source_cites(page_path: Path)` — [`L166`](../../../../../raw/code/wikify-repo/wikify/docs.py#L166) — (doc, anchor|None, line) for every ``src:`` citation on the page. — documented in [wikify-docs](../../concepts/wikify-docs.md)
- `slugify(text: str)` — [`L36`](../../../../../raw/code/wikify-repo/wikify/docs.py#L36) — A GitHub-flavoured heading anchor: lowercase, punctuation dropped, spaces→hyphens. — documented in [wikify-docs](../../concepts/wikify-docs.md)
- `write_doc_packets(cache_dir: Path, slug: str, repo_dir: Path, doc_map: dict[str, DocInfo], commit: str, date: str)` — [`L307`](../../../../../raw/code/wikify-repo/wikify/docs.py#L307) — documented in [wikify-docs](../../concepts/wikify-docs.md)

## Module values
- `DEFAULT_DOC_GLOBS` — [`L111`](../../../../../raw/code/wikify-repo/wikify/docs.py#L111)
- `_ADAPTERS` — [`L104`](../../../../../raw/code/wikify-repo/wikify/docs.py#L104) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- `_ATX` — [`L42`](../../../../../raw/code/wikify-repo/wikify/docs.py#L42) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- `_SETEXT` — [`L43`](../../../../../raw/code/wikify-repo/wikify/docs.py#L43) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- `_SKIP` — [`L113`](../../../../../raw/code/wikify-repo/wikify/docs.py#L113)
- `_SLUG_STRIP` — [`L33`](../../../../../raw/code/wikify-repo/wikify/docs.py#L33) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- `_SRC_CITE` — [`L163`](../../../../../raw/code/wikify-repo/wikify/docs.py#L163) — documented in [wikify-docs](../../concepts/wikify-docs.md)

