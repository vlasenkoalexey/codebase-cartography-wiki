---
title: 'Module: wikify/cli.py'
type: catalog
provenance: extracted
module: wikify/cli.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `wikify.cli`/
symbols:
  prepare: prepare().
  finalize: finalize().
  _finalize_docs: _finalize_docs().
  plan: plan().
  _prepare_docs: _prepare_docs().
  Paths.wiki_slug: Paths#wiki_slug.
  lint_cmd: lint_cmd().
  coverage: coverage().
  _load: _load().
  verify: verify().
  _derive_agenda: _derive_agenda().
  app: app.
  Paths.cache: Paths#cache.
  _graph: _graph().
  Paths.slug: Paths#slug.
  Paths.state: Paths#state.
  _scip_indexes: _scip_indexes().
  Paths.wiki_base: Paths#wiki_base.
  connect: connect().
  _source: _source().
  Paths: Paths#
  Paths.scip: Paths#scip.
  Paths.wiki_subdir: Paths#wiki_subdir.
  _today: _today().
  Paths.wiki: Paths#wiki.
  Paths.scip_cpp: Paths#scip_cpp.
  Paths.raw: Paths#raw.
  Paths.set_wiki_subdir: Paths#set_wiki_subdir().
  Paths.config: Paths#config.
  _find_docs: _find_docs().
  _scip_clang_bin: _scip_clang_bin().
  _expand_shards: _expand_shards().
  Paths.__init__: Paths#__init__().
  Paths.root: Paths#root.
---
# Module: [`wikify/cli.py`](../../../../../raw/code/wikify-repo/wikify/cli.py)

## Classes
### `Paths`
- def: [`wikify/cli.py:46`](../../../../../raw/code/wikify-repo/wikify/cli.py#L46)
- signature: `class Paths:`
- members:
  - `set_wiki_subdir(self, subdir: str | None)` — [`L59`](../../../../../raw/code/wikify-repo/wikify/cli.py#L59) — Place this repo's wiki at ``wiki/<subdir>/<slug>`` (subdir="" → ``wiki/<slug>``).
  - `cache` — [`L50`](../../../../../raw/code/wikify-repo/wikify/cli.py#L50) — documented in [wikify-cli](../../concepts/wikify-cli.md)
  - `config` — [`L52`](../../../../../raw/code/wikify-repo/wikify/cli.py#L52)
  - `raw` — [`L51`](../../../../../raw/code/wikify-repo/wikify/cli.py#L51)
  - `root` — [`L48`](../../../../../raw/code/wikify-repo/wikify/cli.py#L48)
  - `scip` — [`L53`](../../../../../raw/code/wikify-repo/wikify/cli.py#L53)
  - `scip_cpp` — [`L54`](../../../../../raw/code/wikify-repo/wikify/cli.py#L54)
  - `slug` — [`L49`](../../../../../raw/code/wikify-repo/wikify/cli.py#L49) — documented in [wikify-cli](../../concepts/wikify-cli.md)
  - `state` — [`L55`](../../../../../raw/code/wikify-repo/wikify/cli.py#L55)
  - `wiki` — [`L56`](../../../../../raw/code/wikify-repo/wikify/cli.py#L56)
  - `wiki_base` — [`L62`](../../../../../raw/code/wikify-repo/wikify/cli.py#L62)
  - `wiki_slug` — [`L63`](../../../../../raw/code/wikify-repo/wikify/cli.py#L63) — documented in [wikify-cli](../../concepts/wikify-cli.md)
  - `wiki_subdir` — [`L61`](../../../../../raw/code/wikify-repo/wikify/cli.py#L61)
- protocol/private: `__init__`[`L47`](../../../../../raw/code/wikify-repo/wikify/cli.py#L47)
- uses (calls/refs, reference-scoped): [`state_path`](state.md#state_path)
- used by: [`prepare`](cli.md#prepare), [`finalize`](cli.md#finalize), [`_finalize_docs`](cli.md#_finalize_docs), [`plan`](cli.md#plan), [`_prepare_docs`](cli.md#_prepare_docs), [`coverage`](cli.md#coverage), [`lint_cmd`](cli.md#lint_cmd), [`_load`](cli.md#_load), [`verify`](cli.md#verify), [`_graph`](cli.md#_graph), [`_scip_indexes`](cli.md#_scip_indexes)  (1 test-only)

## Functions
- `_derive_agenda(graph, cfg: RepoConfig)` — [`L142`](../../../../../raw/code/wikify-repo/wikify/cli.py#L142) — The DERIVED agenda (decision 8): discovery ranks modules by centrality and — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `_expand_shards(repo_dir: Path, patterns: list[str])` — [`L116`](../../../../../raw/code/wikify-repo/wikify/cli.py#L116) — Expand ``index_shards`` globs to sorted, de-duped repo-relative paths.
- `_finalize_docs(p: Paths, cfg: RepoConfig, repo: str | None)` — [`L180`](../../../../../raw/code/wikify-repo/wikify/cli.py#L180) — Docs-mode finalize: gate `src:` citations against the doc map + coverage floor + — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `_find_docs(repo_dir: Path, patterns: list[str])` — [`L97`](../../../../../raw/code/wikify-repo/wikify/cli.py#L97) — Repo-relative project-doc paths matched by ``cfg.docs`` globs (sorted, deduped).
- `_graph(p: Paths)` — [`L136`](../../../../../raw/code/wikify-repo/wikify/cli.py#L136) — Build the graph, merging every language's SCIP index present in the cache. — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `_load(root: Path, slug: str)` — [`L79`](../../../../../raw/code/wikify-repo/wikify/cli.py#L79) — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `_prepare_docs(p: Paths, cfg: RepoConfig, acq)` — [`L158`](../../../../../raw/code/wikify-repo/wikify/cli.py#L158) — Docs-mode prepare: no SCIP — enumerate docs, build the anchor map, emit one packet — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `_scip_clang_bin()` — [`L70`](../../../../../raw/code/wikify-repo/wikify/cli.py#L70) — The vendored scip-clang if present (glibc-compatible build), else PATH.
- `_scip_indexes(p: Paths)` — [`L129`](../../../../../raw/code/wikify-repo/wikify/cli.py#L129) — Every ``.scip`` for this slug — ``<slug>.scip`` (python) + ``<slug>.<lang>.scip`` (cpp,
- `_source(cfg: RepoConfig, repo: str | None)` — [`L89`](../../../../../raw/code/wikify-repo/wikify/cli.py#L89)
- `_today()` — [`L66`](../../../../../raw/code/wikify-repo/wikify/cli.py#L66)
- `connect(apply: str = typer.Option("", help="Comma-separated concept keys to connect (wire inline)."), refresh: bool = typer.Option(False, help="Re-apply all already-connected concepts."), exclude: str = typer.Option("", help="Comma-separated 'repo/rel-path' matches to drop."), root: Path = typer.Option(Path("."), help="Project root."), vocab: str = typer.Option("concepts", help="Wiki subdir holding the concept vocabulary."))` — [`L467`](../../../../../raw/code/wikify-repo/wikify/cli.py#L467) — Stage 7 — connect ingested silos on the concept axis, inline (no model, no side-table). — documented in [wikify-connect](../../concepts/wikify-connect.md)
- `coverage(slug: str, root: Path = typer.Option(Path("."), help="Project root."), emit: bool = typer.Option(False, help="Write/refresh catalog pages."))` — [`L420`](../../../../../raw/code/wikify-repo/wikify/cli.py#L420) — Report whole-repo coverage (set-difference over the SCIP symbol table). — documented in [wikify-coverage](../../concepts/wikify-coverage.md)
- `finalize(slug: str, repo: str = typer.Option(None, help="Source path or git URL (overrides config)."), root: Path = typer.Option(Path("."), help="Project root."), fix: bool = typer.Option(False, help="Auto-repair deterministically-fixable lint errors first."))` — [`L328`](../../../../../raw/code/wikify-repo/wikify/cli.py#L328) — Stage 6: lint the agent-written pages, assemble the index, update state. — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `lint_cmd(slug: str, root: Path = typer.Option(Path("."), help="Project root."), fix: bool = typer.Option(False, help="Auto-repair deterministically-fixable errors in place."))` — [`L398`](../../../../../raw/code/wikify-repo/wikify/cli.py#L398) — Re-run the citation linter alone (Stage 6 gate); ``--fix`` auto-repairs first. — documented in [wikify-lint](../../concepts/wikify-lint.md)
- `plan(slug: str, ref: str = typer.Option(None, help="Pinned commit/tag."), repo: str = typer.Option(None, help="Source path or git URL."), root: Path = typer.Option(Path("."), help="Project root."))` — [`L500`](../../../../../raw/code/wikify-repo/wikify/cli.py#L500) — Dry-run: print the reconcile delta against the DERIVED agenda, emit nothing. — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `prepare(slug: str, ref: str = typer.Option(None, help="Pinned commit/tag to ingest."), repo: str = typer.Option(None, help="Source path or git URL (overrides config)."), root: Path = typer.Option(Path("."), help="Project root."), reindex: bool = typer.Option(True, help="(Re)run scip-python."))` — [`L218`](../../../../../raw/code/wikify-repo/wikify/cli.py#L218) — Stages 0-4: acquire, index, build graph, emit packets, print the plan. — documented in [wikify-acquire](../../concepts/wikify-acquire.md)
- `verify(slug: str, page: str = typer.Option(None, help="Dump claims for one concept (stem or filename)."), root: Path = typer.Option(Path("."), help="Project root."))` — [`L442`](../../../../../raw/code/wikify-repo/wikify/cli.py#L442) — List the load-bearing claims to adversarially verify (worklist for the — documented in [wikify-verify](../../concepts/wikify-verify.md)

## Module values
- `app` — [`L40`](../../../../../raw/code/wikify-repo/wikify/cli.py#L40) — documented in [wikify-cli](../../concepts/wikify-cli.md)

