---
title: 'Module: wikify/coverage.py'
type: catalog
provenance: extracted
module: wikify/coverage.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `wikify.coverage`/
symbols:
  render_catalog: render_catalog().
  compute_report: compute_report().
  CoverageReport.render: CoverageReport#render().
  emit_catalogs: emit_catalogs().
  documentable_symbols: documentable_symbols().
  render_catalog._link_targets: render_catalog()._link_targets().
  covered_monikers: covered_monikers().
  qualified_name: qualified_name().
  class_symbols: class_symbols().
  _rel_names: _rel_names().
  render_catalog._detail: render_catalog()._detail().
  symbol_anchor_map: symbol_anchor_map().
  class_connections: class_connections().
  CoverageReport.represented: CoverageReport#represented().
  _clean_sig: _clean_sig().
  by_module: by_module().
  CoverageReport.total: CoverageReport#total.
  catalog_ref: catalog_ref().
  _params: _params().
  CoverageReport.pct_deep: CoverageReport#pct_deep().
  CoverageReport.pct_represented: CoverageReport#pct_represented().
  catalog_rel_path: catalog_rel_path().
  _owner_class: _owner_class().
  CoverageReport.covered: CoverageReport#covered.
  _glob_any: _glob_any().
  render_catalog._loc_line: render_catalog()._loc_line().
  CoverageReport.catalog_only: CoverageReport#catalog_only.
  CoverageReport.uncovered_examples: CoverageReport#uncovered_examples.
  _rel_catalog_link: _rel_catalog_link().
  _is_noise_path: _is_noise_path().
  render_catalog._loc: render_catalog()._loc().
  CoverageReport.classes_total: CoverageReport#classes_total.
  CoverageReport.classes_represented: CoverageReport#classes_represented.
  _src_link: _src_link().
  CoverageReport: CoverageReport#
  CoverageReport.modules: CoverageReport#modules.
  render_catalog._cov_tag: render_catalog()._cov_tag().
  DOCUMENTABLE_SUFFIXES: DOCUMENTABLE_SUFFIXES.
  _CATALOG_LINK: _CATALOG_LINK.
  _ANCHOR_UNSAFE: _ANCHOR_UNSAFE.
  _NOISE_SEGMENTS: _NOISE_SEGMENTS.
  _compress_anchor_map: _compress_anchor_map().
---
# Module: [`wikify/coverage.py`](../../../../../raw/code/wikify-repo/wikify/coverage.py)

## Classes
### `CoverageReport`
- def: [`wikify/coverage.py:119`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L119)
- signature: `class CoverageReport:`
- members:
  - `pct_deep(self)` — [`L133`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L133)
  - `pct_represented(self)` — [`L137`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L137)
  - `render(self)` — [`L140`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L140) — documented in [wikify-cli](../../concepts/wikify-cli.md)
  - `represented(self)` — [`L129`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L129) — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
  - `catalog_only` — [`L122`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L122) — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
  - `classes_represented` — [`L125`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L125)
  - `classes_total` — [`L124`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L124)
  - `covered` — [`L121`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L121) — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
  - `modules` — [`L123`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L123)
  - `total` — [`L120`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L120)
  - `uncovered_examples` — [`L126`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L126) — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- used by: [`finalize`](cli.md#finalize), [`compute_report`](coverage.md#compute_report), [`coverage`](cli.md#coverage)  (1 test-only)

## Functions
- `_clean_sig(sym: Symbol)` — [`L244`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L244) — The real `def …`/`class …` line — decorator lines stripped, collapsed to one
- `_compress_anchor_map(anchor_map: dict[str, str])` — [`L330`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L330) — Factor the common moniker prefix out of an anchor→moniker map.
- `_cov_tag(moniker: str)` — [`L372`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L372)
- `_detail(sym, moniker: str)` — [`L390`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L390) — One symbol's detail bullet: `name(params)` — Lnnn — docstring summary. — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- `_glob_any(path: str, patterns)` — [`L512`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L512) — True if ``path`` matches any glob in ``patterns`` (``*`` spans ``/``, so — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- `_is_noise_path(def_path: str | None)` — [`L318`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L318)
- `_link_targets(targets: list[str], cap: int = 40)` — [`L429`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L429) — Render in-repo edge targets, ranked by importance, linked to their catalog. — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- `_loc(sym)` — [`L377`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L377) — `def: file:line`, linked to the pinned source when ``source_base`` is set.
- `_loc_line(sym)` — [`L384`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L384) — Compact source link `Lnnn` (the file is the catalog's module).
- `_owner_class(moniker: str)` — [`L232`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L232) — Name of the enclosing class for a method/term, or None if module-level.
- `_params(sym: Symbol)` — [`L255`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L255) — The parameter tuple from a callable's signature, e.g. ``(self, modules=None)``.
- `_rel_catalog_link(from_module: str, to_module: str)` — [`L272`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L272) — Relative link from one module's catalog page to another's.
- `_rel_names(sym: Symbol)` — [`L301`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L301) — documented in [wikify-monikers](../../concepts/wikify-monikers.md)
- `_src_link(source_base: str | None, path: str, line: int | None = None)` — [`L323`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L323) — Permalink into the pinned source (``<base>/<path>#L<line>``), or None.
- `by_module(symbols: dict[str, Symbol])` — [`L107`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L107) — Group documentable monikers by their definition file (the module). — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- `catalog_ref(module_path: str, moniker: str)` — [`L216`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L216) — Citation target a concept page uses (``concepts/`` → ``../catalog/…#anchor``).
- `catalog_rel_path(module_path: str)` — [`L189`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L189) — Map a module file path to its catalog page path (mirrors the source tree). — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- `class_connections(graph: SymbolGraph, class_moniker: str, member_monikers: list[str])` — [`L280`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L280) — Roll member edges up to the class → (uses, used_by) target monikers. — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- `class_symbols(graph: SymbolGraph)` — [`L71`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L71) — In-repo class definitions only (suffix == Type).
- `compute_report(graph: SymbolGraph, wiki_slug_dir: str | Path, catalogued: set[str] | None = None)` — [`L152`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L152) — Classify every documentable symbol as covered / catalog-only / unrepresented. — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `covered_monikers(graph: SymbolGraph, wiki_slug_dir: str | Path)` — [`L83`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L83) — Map each concept-cited moniker → the concept page slug that cites it. — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- `documentable_symbols(graph: SymbolGraph)` — [`L62`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L62) — Every in-repo symbol worth representing in the wiki (has a def + is citable). — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `emit_catalogs(graph: SymbolGraph, wiki_slug_dir: str | Path, repo_dir: str | Path | None = None, source_url: str | None = None, collapse: list[str] | None = None, exclude: list[str] | None = None)` — [`L518`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L518) — Write one catalog page per in-repo module. Returns (catalogued monikers, paths). — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `qualified_name(moniker: str)` — [`L200`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L200) — Anchor for a symbol within its module catalog: descriptor names after the — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- `render_catalog(graph: SymbolGraph, module_path: str, monikers: list[str], covered: dict[str, str], source_base: str | None = None, collapse: bool = False)` — [`L344`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L344) — Render one module's catalog page from the graph (no synthesis). — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- `symbol_anchor_map(graph: SymbolGraph, monikers: list[str])` — [`L221`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L221) — {anchor → moniker} for a module's symbols (the linter's resolution table). — documented in [wikify-coverage](../../concepts/wikify-coverage.md)

## Module values
- `DOCUMENTABLE_SUFFIXES` — [`L56`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L56)
- `_ANCHOR_UNSAFE` — [`L197`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L197)
- `_CATALOG_LINK` — [`L80`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L80)
- `_NOISE_SEGMENTS` — [`L314`](../../../../../raw/code/wikify-repo/wikify/coverage.py#L314)

