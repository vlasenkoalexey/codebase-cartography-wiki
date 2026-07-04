---
title: 'Module: tests/test_import_extension_resolution.py'
type: catalog
provenance: extracted
module: tests/test_import_extension_resolution.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_import_extension_resolution`/
symbols:
  _write: _write().
  _import_targets: _import_targets().
  test_bare_path_import_resolves_in_ts_file: test_bare_path_import_resolves_in_ts_file().
  test_directory_import_resolves_to_index_ts: test_directory_import_resolves_to_index_ts().
  test_dot_svelte_import_resolves_to_dot_svelte_ts: test_dot_svelte_import_resolves_to_dot_svelte_ts().
  test_explicit_ts_import_still_works: test_explicit_ts_import_still_works().
  test_explicit_svelte_import_still_works: test_explicit_svelte_import_still_works().
  test_alias_import_with_bare_path_resolves: test_alias_import_with_bare_path_resolves().
  test_type_only_import_with_bare_path_resolves: test_type_only_import_with_bare_path_resolves().
  test_alias_directory_import_resolves_to_index_ts: test_alias_directory_import_resolves_to_index_ts().
  test_end_to_end_multi_dot_import_resolves: test_end_to_end_multi_dot_import_resolves().
  test_resolve_chain_alias_and_extension_compose: test_resolve_chain_alias_and_extension_compose().
  test_external_module_unchanged: test_external_module_unchanged().
  test_ts_dynamic_import_bare_path_resolves: test_ts_dynamic_import_bare_path_resolves().
  test_ts_dynamic_import_alias_with_bare_path_resolves: test_ts_dynamic_import_alias_with_bare_path_resolves().
  test_dynamic_import_bare_path_resolves: test_dynamic_import_bare_path_resolves().
  test_resolve_returns_existing_path_unchanged: test_resolve_returns_existing_path_unchanged().
  test_resolve_bare_path_to_ts: test_resolve_bare_path_to_ts().
  test_resolve_bare_path_to_tsx: test_resolve_bare_path_to_tsx().
  test_resolve_bare_path_to_svelte: test_resolve_bare_path_to_svelte().
  test_resolve_prefers_ts_over_svelte_when_both_exist: test_resolve_prefers_ts_over_svelte_when_both_exist().
  test_resolve_file_wins_over_sibling_directory: test_resolve_file_wins_over_sibling_directory().
  test_resolve_directory_to_index_ts: test_resolve_directory_to_index_ts().
  test_resolve_directory_prefers_index_ts_over_index_js: test_resolve_directory_prefers_index_ts_over_index_js().
  test_resolve_svelte_to_svelte_ts_for_rune_files: test_resolve_svelte_to_svelte_ts_for_rune_files().
  test_resolve_svelte_to_svelte_js_for_javascript_rune_files: test_resolve_svelte_to_svelte_js_for_javascript_rune_files().
  test_resolve_svelte_prefers_svelte_ts_over_svelte_js: test_resolve_svelte_prefers_svelte_ts_over_svelte_js().
  test_resolve_real_svelte_file_wins_over_svelte_ts_sibling: test_resolve_real_svelte_file_wins_over_svelte_ts_sibling().
  test_resolve_js_to_ts_when_real_file_is_ts: test_resolve_js_to_ts_when_real_file_is_ts().
  test_resolve_jsx_to_tsx_when_real_file_is_tsx: test_resolve_jsx_to_tsx_when_real_file_is_tsx().
  test_resolve_real_js_stays_js_when_ts_does_not_exist: test_resolve_real_js_stays_js_when_ts_does_not_exist().
  test_named_imports_emit_symbol_edges_after_resolution: test_named_imports_emit_symbol_edges_after_resolution().
  test_resolve_does_not_match_partial_directory_name: test_resolve_does_not_match_partial_directory_name().
  test_resolve_directory_without_index_returns_unchanged: test_resolve_directory_without_index_returns_unchanged().
  test_resolve_handles_subpath_into_directory_with_index: test_resolve_handles_subpath_into_directory_with_index().
  test_resolve_does_not_treat_dotfile_as_extension: test_resolve_does_not_treat_dotfile_as_extension().
  test_resolve_multi_dot_helper_file: test_resolve_multi_dot_helper_file().
  test_resolve_multi_dot_with_explicit_extension_still_works: test_resolve_multi_dot_with_explicit_extension_still_works().
  test_resolve_ambient_d_ts_via_bare_path: test_resolve_ambient_d_ts_via_bare_path().
  test_resolve_returns_unchanged_when_nothing_matches: test_resolve_returns_unchanged_when_nothing_matches().
---
# Module: [`tests/test_import_extension_resolution.py`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py)

## Functions
- `_import_targets(result: dict)` — [`L27`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L27)
- `_write(path: Path, body: str)` — [`L21`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L21)
- `test_alias_directory_import_resolves_to_index_ts(tmp_path)` — [`L334`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L334) — `from '$lib/queue'` where queue/ is a directory under src/lib/.
- `test_alias_import_with_bare_path_resolves(tmp_path)` — [`L276`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L276) — `$lib/foo` (alias + bare path) — both layers must work together.
- `test_bare_path_import_resolves_in_ts_file(tmp_path)` — [`L181`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L181) — The #716 reproducer: TS file imports a sibling without an extension.
- `test_directory_import_resolves_to_index_ts(tmp_path)` — [`L195`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L195) — `from './queue'` must resolve to `./queue/index.ts`.
- `test_dot_svelte_import_resolves_to_dot_svelte_ts(tmp_path)` — [`L212`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L212) — Svelte 5 rune file: import written as .svelte, real file is .svelte.ts.
- `test_dynamic_import_bare_path_resolves(tmp_path)` — [`L510`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L510) — The regex pass for `import('...')` in .svelte files must also use
- `test_end_to_end_multi_dot_import_resolves(tmp_path)` — [`L424`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L424) — End-to-end sanity for the multi-dot pattern via the import handler.
- `test_explicit_svelte_import_still_works(tmp_path)` — [`L243`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L243) — Real .svelte file imports must still resolve when the .svelte file
- `test_explicit_ts_import_still_works(tmp_path)` — [`L229`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L229) — The most common case — import with explicit .ts extension — must
- `test_external_module_unchanged(tmp_path)` — [`L258`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L258) — Bare module specifiers (no leading dot, no alias match) must still
- `test_named_imports_emit_symbol_edges_after_resolution(tmp_path)` — [`L314`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L314) — `import { foo, bar } from './module'` should emit per-symbol `imports`
- `test_resolve_ambient_d_ts_via_bare_path(tmp_path)` — [`L416`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L416) — Ambient TS declaration files (foo.d.ts) — bare import `./foo.d`
- `test_resolve_bare_path_to_svelte(tmp_path)` — [`L52`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L52)
- `test_resolve_bare_path_to_ts(tmp_path)` — [`L40`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L40)
- `test_resolve_bare_path_to_tsx(tmp_path)` — [`L46`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L46)
- `test_resolve_chain_alias_and_extension_compose(tmp_path)` — [`L438`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L438) — Alias → bare path → .svelte.ts. Two layers of resolution must
- `test_resolve_directory_prefers_index_ts_over_index_js(tmp_path)` — [`L86`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L86)
- `test_resolve_directory_to_index_ts(tmp_path)` — [`L80`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L80)
- `test_resolve_directory_without_index_returns_unchanged(tmp_path)` — [`L366`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L366) — A directory with no index file should fall through to the
- `test_resolve_does_not_match_partial_directory_name(tmp_path)` — [`L352`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L352) — Regression guard: `from './foo'` where './foo' doesn't exist but
- `test_resolve_does_not_treat_dotfile_as_extension(tmp_path)` — [`L386`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L386) — Edge case: `.eslintrc` and similar dotfiles. Path('.eslintrc').suffix
- `test_resolve_file_wins_over_sibling_directory(tmp_path)` — [`L66`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L66) — Real-world repro: a project has both `auth.ts` (file) and `auth/`
- `test_resolve_handles_subpath_into_directory_with_index(tmp_path)` — [`L377`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L377) — `./foo/sub` where ./foo/sub/index.ts exists — nested subpath.
- `test_resolve_js_to_ts_when_real_file_is_ts(tmp_path)` — [`L151`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L151) — TS ESM convention: imports written as .js but the actual file is .ts.
- `test_resolve_jsx_to_tsx_when_real_file_is_tsx(tmp_path)` — [`L158`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L158)
- `test_resolve_multi_dot_helper_file(tmp_path)` — [`L396`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L396) — Common patterns: foo.shared.ts, foo.config.ts, foo.compile.ts,
- `test_resolve_multi_dot_with_explicit_extension_still_works(tmp_path)` — [`L410`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L410) — Sanity: `from './foo.shared.ts'` (explicit) still wins over implicit.
- `test_resolve_prefers_ts_over_svelte_when_both_exist(tmp_path)` — [`L58`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L58) — Vite resolver order: .ts wins over .svelte for ambiguous bare paths.
- `test_resolve_real_js_stays_js_when_ts_does_not_exist(tmp_path)` — [`L171`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L171) — If `.js` exists and `.ts` does not, keep the `.js` rewrite from
- `test_resolve_real_svelte_file_wins_over_svelte_ts_sibling(tmp_path)` — [`L140`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L140) — If `foo.svelte` IS a real markup file, importing `./foo.svelte`
- `test_resolve_returns_existing_path_unchanged(tmp_path)` — [`L35`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L35)
- `test_resolve_returns_unchanged_when_nothing_matches(tmp_path)` — [`L164`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L164) — External / truly missing paths fall back to the input — preserves
- `test_resolve_svelte_prefers_svelte_ts_over_svelte_js(tmp_path)` — [`L121`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L121) — When both `.svelte.ts` and `.svelte.js` exist (hybrid project mid-
- `test_resolve_svelte_to_svelte_js_for_javascript_rune_files(tmp_path)` — [`L106`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L106) — JS variant of the rune file pattern: a `.svelte.js` file (used in
- `test_resolve_svelte_to_svelte_ts_for_rune_files(tmp_path)` — [`L93`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L93) — Svelte 5: `from './foo.svelte'` may actually point at `foo.svelte.ts`
- `test_ts_dynamic_import_alias_with_bare_path_resolves(tmp_path)` — [`L485`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L485) — The other branch of the dynamic-import handler — alias resolution —
- `test_ts_dynamic_import_bare_path_resolves(tmp_path)` — [`L461`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L461) — Real-world repro: a TS file uses `await import('./foo')` (no extension)
- `test_type_only_import_with_bare_path_resolves(tmp_path)` — [`L298`](../../../../../raw/code/graphify/tests/test_import_extension_resolution.py#L298) — `import type { X } from './foo'` — type-only imports must go through

