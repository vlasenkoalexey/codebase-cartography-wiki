---
title: 'Module: wikify/lint.py'
type: catalog
provenance: extracted
module: wikify/lint.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `wikify.lint`/
symbols:
  lint_page: lint_page().
  lint_doc_concepts: lint_doc_concepts().
  lint_silo: lint_silo().
  LintError: LintError#
  lint_page.flush_item: lint_page().flush_item().
  LintReport.errors: LintReport#errors.
  LintReport.ok: LintReport#ok().
  LintError.__str__: LintError#__str__().
  page_citations: page_citations().
  LintError.rule: LintError#rule.
  LintReport: LintReport#
  _resolve_citation: _resolve_citation().
  _LINK: _LINK.
  _is_symbol_link: _is_symbol_link().
  _LIST_ITEM: _LIST_ITEM.
  LintError.line: LintError#line.
  _CITED_SECTIONS: _CITED_SECTIONS.
  LintError.page: LintError#page.
  LintError.message: LintError#message.
  _frontmatter_dict: _frontmatter_dict().
  _is_evidence_link: _is_evidence_link().
---
# Module: [`wikify/lint.py`](../../../../../raw/code/wikify-repo/wikify/lint.py)

## Classes
### `LintError`
- def: [`wikify/lint.py:36`](../../../../../raw/code/wikify-repo/wikify/lint.py#L36) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- signature: `class LintError:`
- members:
  - `line` — [`L38`](../../../../../raw/code/wikify-repo/wikify/lint.py#L38)
  - `message` — [`L40`](../../../../../raw/code/wikify-repo/wikify/lint.py#L40)
  - `page` — [`L37`](../../../../../raw/code/wikify-repo/wikify/lint.py#L37)
  - `rule` — [`L39`](../../../../../raw/code/wikify-repo/wikify/lint.py#L39)
- protocol/private: `__str__`[`L42`](../../../../../raw/code/wikify-repo/wikify/lint.py#L42)
- used by: [`lint_page`](lint.md#lint_page), [`fix_page`](fix.md#fix_page), [`lint_doc_concepts`](lint.md#lint_doc_concepts), [`lint_silo`](lint.md#lint_silo), [`lint_docs`](docs.md#lint_docs), [`flush_item`](lint.md#lint_page.flush_item), [`errors`](lint.md#LintReport.errors)  (7 test-only)

### `LintReport`
- def: [`wikify/lint.py:47`](../../../../../raw/code/wikify-repo/wikify/lint.py#L47) — documented in [wikify-docs](../../concepts/wikify-docs.md)
- signature: `class LintReport:`
- members:
  - `ok(self)` — [`L51`](../../../../../raw/code/wikify-repo/wikify/lint.py#L51) — documented in [wikify-cli](../../concepts/wikify-cli.md)
  - `errors` — [`L48`](../../../../../raw/code/wikify-repo/wikify/lint.py#L48) — documented in [wikify-cli](../../concepts/wikify-cli.md)
- uses (calls/refs, reference-scoped): [`LintError`](lint.md#LintError)
- used by: [`finalize`](cli.md#finalize), [`_finalize_docs`](cli.md#_finalize_docs), [`lint_cmd`](cli.md#lint_cmd), [`lint_doc_concepts`](lint.md#lint_doc_concepts), [`lint_silo`](lint.md#lint_silo), [`lint_docs`](docs.md#lint_docs)  (5 test-only)

## Functions
- `_frontmatter_dict(page_path: Path)` — [`L55`](../../../../../raw/code/wikify-repo/wikify/lint.py#L55) — documented in [wikify-lint](../../concepts/wikify-lint.md)
- `_is_evidence_link(target: str)` — [`L92`](../../../../../raw/code/wikify-repo/wikify/lint.py#L92) — documented in [wikify-lint](../../concepts/wikify-lint.md)
- `_is_symbol_link(target: str)` — [`L71`](../../../../../raw/code/wikify-repo/wikify/lint.py#L71) — A symbol citation is a catalog link carrying an anchor. — documented in [wikify-lint](../../concepts/wikify-lint.md)
- `_resolve_citation(page_path: Path, target: str)` — [`L77`](../../../../../raw/code/wikify-repo/wikify/lint.py#L77) — Resolve a ``../catalog/<module>.md#anchor`` citation → moniker (or None). — documented in [wikify-lint](../../concepts/wikify-lint.md)
- `flush_item(item_lines: list[str], start: int)` — [`L111`](../../../../../raw/code/wikify-repo/wikify/lint.py#L111) — documented in [wikify-lint](../../concepts/wikify-lint.md)
- `lint_doc_concepts(wiki_slug_dir: str | Path, graph: SymbolGraph)` — [`L200`](../../../../../raw/code/wikify-repo/wikify/lint.py#L200) — Light lint for doc-derived concept pages (`doc-concepts/`): every catalog — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `lint_page(page_path: Path, graph: SymbolGraph, subgraph: set[str])` — [`L96`](../../../../../raw/code/wikify-repo/wikify/lint.py#L96) — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `lint_silo(wiki_slug_dir: str | Path, graph: SymbolGraph, cache_dir: str | Path, slug: str)` — [`L225`](../../../../../raw/code/wikify-repo/wikify/lint.py#L225) — Lint every concept page in a silo (citations resolve into module catalogs). — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `page_citations(page_path: Path)` — [`L187`](../../../../../raw/code/wikify-repo/wikify/lint.py#L187) — Resolve the monikers a concept page cites (via catalog anchor resolution).

## Module values
- `_CITED_SECTIONS` — [`L32`](../../../../../raw/code/wikify-repo/wikify/lint.py#L32) — documented in [wikify-lint](../../concepts/wikify-lint.md)
- `_LINK` — [`L30`](../../../../../raw/code/wikify-repo/wikify/lint.py#L30) — documented in [wikify-lint](../../concepts/wikify-lint.md)
- `_LIST_ITEM` — [`L31`](../../../../../raw/code/wikify-repo/wikify/lint.py#L31) — documented in [wikify-lint](../../concepts/wikify-lint.md)

