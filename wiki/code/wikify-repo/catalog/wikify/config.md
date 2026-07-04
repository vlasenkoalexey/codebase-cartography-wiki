---
title: 'Module: wikify/config.py'
type: catalog
provenance: extracted
module: wikify/config.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `wikify.config`/
symbols:
  load_config: load_config().
  _parse_concept: _parse_concept().
  RepoConfig.concepts: RepoConfig#concepts.
  Concept.slug: Concept#slug.
  RepoConfig: RepoConfig#
  Concept: Concept#
  Concept.seeds: Concept#seeds.
  RepoConfig.ref: RepoConfig#ref.
  RepoConfig.acquire: RepoConfig#acquire.
  _as_list: _as_list().
  _parse_seeds: _parse_seeds().
  _parse_concepts: _parse_concepts().
  validate_config: validate_config().
  Concept.auto: Concept#auto.
  RepoConfig.languages: RepoConfig#languages.
  RepoConfig.source_type: RepoConfig#source_type.
  RepoConfig.bazel_targets: RepoConfig#bazel_targets.
  RepoConfig.wiki_subdir: RepoConfig#wiki_subdir.
  RepoConfig.doc_globs: RepoConfig#doc_globs.
  RepoConfig.synthesis_focus: RepoConfig#synthesis_focus.
  RepoConfig.tests: RepoConfig#tests.
  RepoConfig.docs: RepoConfig#docs.
  _SEEDS_RE: _SEEDS_RE.
  RepoConfig.slug: RepoConfig#slug.
  RepoConfig.build: RepoConfig#build.
  RepoConfig.coverage_collapse: RepoConfig#coverage_collapse.
  RepoConfig.coverage_exclude: RepoConfig#coverage_exclude.
  RepoConfig.compile_commands: RepoConfig#compile_commands.
  RepoConfig.index_shards: RepoConfig#index_shards.
  _ALLOWED_KEYS: _ALLOWED_KEYS.
  _DASH: _DASH.
  _HTML_COMMENT_RE: _HTML_COMMENT_RE.
  _BACKTICK_TOKEN_RE: _BACKTICK_TOKEN_RE.
  Concept.note: Concept#note.
  RepoConfig.repo: RepoConfig#repo.
  RepoConfig.source_url: RepoConfig#source_url.
  _CONCEPT_RE: _CONCEPT_RE.
  _AUTO_RE: _AUTO_RE.
  _split_frontmatter: _split_frontmatter().
---
# Module: [`wikify/config.py`](../../../../../raw/code/wikify-repo/wikify/config.py)

## Classes
### `Concept`
- def: [`wikify/config.py:51`](../../../../../raw/code/wikify-repo/wikify/config.py#L51) — documented in [wikify-config](../../concepts/wikify-config.md)
- doc: One architectural concept from the `## Concepts` list.
- signature: `class Concept:`
- members:
  - `auto` — [`L61`](../../../../../raw/code/wikify-repo/wikify/config.py#L61) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `note` — [`L62`](../../../../../raw/code/wikify-repo/wikify/config.py#L62) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `seeds` — [`L60`](../../../../../raw/code/wikify-repo/wikify/config.py#L60) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `slug` — [`L59`](../../../../../raw/code/wikify-repo/wikify/config.py#L59) — documented in [wikify-diff](../../concepts/wikify-diff.md)
- used by: [`prepare`](cli.md#prepare), [`build_packet`](packet.md#build_packet), [`compute_plan`](diff.md#compute_plan), [`_parse_concept`](config.md#_parse_concept), [`_derive_agenda`](cli.md#_derive_agenda), [`concepts`](config.md#RepoConfig.concepts), [`_parse_concepts`](config.md#_parse_concepts)  (8 test-only)

### `RepoConfig`
- def: [`wikify/config.py:66`](../../../../../raw/code/wikify-repo/wikify/config.py#L66) — documented in [wikify-cli](../../concepts/wikify-cli.md)
- doc: Parsed `config/<slug>.md` — an authored ingest input, not a product.
- signature: `class RepoConfig:`
- members:
  - `acquire` — [`L79`](../../../../../raw/code/wikify-repo/wikify/config.py#L79) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `bazel_targets` — [`L108`](../../../../../raw/code/wikify-repo/wikify/config.py#L108) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `build` — [`L71`](../../../../../raw/code/wikify-repo/wikify/config.py#L71) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `compile_commands` — [`L103`](../../../../../raw/code/wikify-repo/wikify/config.py#L103) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `concepts` — [`L121`](../../../../../raw/code/wikify-repo/wikify/config.py#L121) — documented in [wikify-cli](../../concepts/wikify-cli.md)
  - `coverage_collapse` — [`L96`](../../../../../raw/code/wikify-repo/wikify/config.py#L96) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `coverage_exclude` — [`L97`](../../../../../raw/code/wikify-repo/wikify/config.py#L97) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `doc_globs` — [`L90`](../../../../../raw/code/wikify-repo/wikify/config.py#L90) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `docs` — [`L120`](../../../../../raw/code/wikify-repo/wikify/config.py#L120) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `index_shards` — [`L118`](../../../../../raw/code/wikify-repo/wikify/config.py#L118) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `languages` — [`L70`](../../../../../raw/code/wikify-repo/wikify/config.py#L70) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `ref` — [`L72`](../../../../../raw/code/wikify-repo/wikify/config.py#L72) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `repo` — [`L73`](../../../../../raw/code/wikify-repo/wikify/config.py#L73) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `slug` — [`L69`](../../../../../raw/code/wikify-repo/wikify/config.py#L69) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `source_type` — [`L87`](../../../../../raw/code/wikify-repo/wikify/config.py#L87) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `source_url` — [`L113`](../../../../../raw/code/wikify-repo/wikify/config.py#L113) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `synthesis_focus` — [`L102`](../../../../../raw/code/wikify-repo/wikify/config.py#L102) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `tests` — [`L119`](../../../../../raw/code/wikify-repo/wikify/config.py#L119) — documented in [wikify-config](../../concepts/wikify-config.md)
  - `wiki_subdir` — [`L83`](../../../../../raw/code/wikify-repo/wikify/config.py#L83) — documented in [wikify-config](../../concepts/wikify-config.md)
- uses (calls/refs, reference-scoped): [`Concept`](config.md#Concept)
- used by: [`prepare`](cli.md#prepare), [`finalize`](cli.md#finalize), [`load_config`](config.md#load_config), [`_finalize_docs`](cli.md#_finalize_docs), [`plan`](cli.md#plan), [`compute_plan`](diff.md#compute_plan), [`_prepare_docs`](cli.md#_prepare_docs), [`_load`](cli.md#_load), [`_derive_agenda`](cli.md#_derive_agenda), [`_source`](cli.md#_source), [`validate_config`](config.md#validate_config)  (13 test-only)

## Functions
- `_as_list(value: object)` — [`L135`](../../../../../raw/code/wikify-repo/wikify/config.py#L135) — Coerce an absent/scalar/list frontmatter value to a list of str. — documented in [wikify-config](../../concepts/wikify-config.md)
- `_parse_concept(line: str)` — [`L159`](../../../../../raw/code/wikify-repo/wikify/config.py#L159) — Parse one ``- ...`` concept list item into a ``Concept``. — documented in [wikify-config](../../concepts/wikify-config.md)
- `_parse_concepts(body: str)` — [`L192`](../../../../../raw/code/wikify-repo/wikify/config.py#L192) — Extract concepts from the ``## Concepts`` section of the body. — documented in [wikify-config](../../concepts/wikify-config.md)
- `_parse_seeds(payload: str)` — [`L144`](../../../../../raw/code/wikify-repo/wikify/config.py#L144) — Parse a ``seeds:`` payload → ``(seeds, auto, note)``. — documented in [wikify-config](../../concepts/wikify-config.md)
- `_split_frontmatter(text: str)` — [`L124`](../../../../../raw/code/wikify-repo/wikify/config.py#L124) — Return ``(frontmatter_yaml, body)`` from leading ``---`` fences.
- `load_config(path: str | Path)` — [`L219`](../../../../../raw/code/wikify-repo/wikify/config.py#L219) — Parse and validate ``config/<slug>.md`` into a ``RepoConfig``. — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `validate_config(cfg: RepoConfig)` — [`L213`](../../../../../raw/code/wikify-repo/wikify/config.py#L213) — Raise ``ValueError`` if the parsed config violates the schema. — documented in [wikify-config](../../concepts/wikify-config.md)

## Module values
- `_ALLOWED_KEYS` — [`L24`](../../../../../raw/code/wikify-repo/wikify/config.py#L24) — documented in [wikify-config](../../concepts/wikify-config.md)
- `_AUTO_RE` — [`L47`](../../../../../raw/code/wikify-repo/wikify/config.py#L47)
- `_BACKTICK_TOKEN_RE` — [`L46`](../../../../../raw/code/wikify-repo/wikify/config.py#L46)
- `_CONCEPT_RE` — [`L33`](../../../../../raw/code/wikify-repo/wikify/config.py#L33)
- `_DASH` — [`L30`](../../../../../raw/code/wikify-repo/wikify/config.py#L30)
- `_HTML_COMMENT_RE` — [`L45`](../../../../../raw/code/wikify-repo/wikify/config.py#L45)
- `_SEEDS_RE` — [`L40`](../../../../../raw/code/wikify-repo/wikify/config.py#L40)

