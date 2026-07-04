---
title: 'Module: tests/unit/test_typescript_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_typescript_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_typescript_method_resolution`/
symbols:
  _index: _index().
  _ctx: _ctx().
  _resolution_for: _resolution_for().
  test_local_no_receiver_resolves_same_file: test_local_no_receiver_resolves_same_file().
  test_local_this_receiver_resolves_class_method: test_local_this_receiver_resolves_class_method().
  test_global_object_receiver_classifies_builtin: test_global_object_receiver_classifies_builtin().
  test_json_receiver_classifies_builtin: test_json_receiver_classifies_builtin().
  test_bare_generic_method_stays_unknown: test_bare_generic_method_stays_unknown().
  test_project_shadows_builtin_global_name: test_project_shadows_builtin_global_name().
  test_no_cross_language_bind_for_global_object_owner: test_no_cross_language_bind_for_global_object_owner().
  test_this_method_ambiguous_across_classes_stays_unknown: test_this_method_ambiguous_across_classes_stays_unknown().
  test_this_method_unambiguous_resolves_local: test_this_method_unambiguous_resolves_local().
  test_this_method_never_falls_through_to_top_level_function: test_this_method_never_falls_through_to_top_level_function().
  test_variable_shadow_suppresses_builtin: test_variable_shadow_suppresses_builtin().
  test_import_shadow_suppresses_builtin: test_import_shadow_suppresses_builtin().
  test_shadow_local_is_file_scoped: test_shadow_local_is_file_scoped().
  test_integration_import_shadow_suppresses_builtin: test_integration_import_shadow_suppresses_builtin().
  test_integration_import_shadow_no_project_symbol_suppresses_builtin: test_integration_import_shadow_no_project_symbol_suppresses_builtin().
  test_integration_default_import_shadow_suppresses_builtin: test_integration_default_import_shadow_suppresses_builtin().
  test_integration_variable_shadow_suppresses_builtin: test_integration_variable_shadow_suppresses_builtin().
  test_integration_unshadowed_global_still_builtin: test_integration_unshadowed_global_still_builtin().
  test_integration_local_call_resolves: test_integration_local_call_resolves().
  test_integration_console_log_classifies_builtin: test_integration_console_log_classifies_builtin().
  test_integration_bare_method_stays_unknown: test_integration_bare_method_stays_unknown().
  test_shadow_locals_from_cache_are_module_scope_only: test_shadow_locals_from_cache_are_module_scope_only().
  test_function_local_shadow_no_longer_suppresses_builtin: test_function_local_shadow_no_longer_suppresses_builtin().
  test_build_context_none_when_no_typescript_file: test_build_context_none_when_no_typescript_file().
  test_build_context_present_for_tsx: test_build_context_present_for_tsx().
  test_integration_no_cross_language_mis_wire: test_integration_no_cross_language_mis_wire().
---
# Module: [`tests/unit/test_typescript_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py)

## Functions
- `_ctx(*, file_symbols: dict[str, list[tuple[str, str, int]]] | None = None, file_languages: dict[str, str] | None = None, global_name_table: dict[str, list[tuple[str, int]]] | None = None, file_class_methods: dict[str, dict[str, dict[str, int]]] | None = None, shadow_locals: dict[str, set[str]] | None = None)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L69)
- `_index(tmp_path: Path, files: dict[str, str])` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L39)
- `_resolution_for(db_path: str, callee_name: str)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L52)
- `test_bare_generic_method_stays_unknown()` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L146) — ``s.substring(2)`` — ``substring`` is a domain-collidable bare method name
- `test_build_context_none_when_no_typescript_file()` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L87) — Zero cost for non-TS projects: gated on ``file_languages``.
- `test_build_context_present_for_tsx()` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L99) — A ``.tsx`` file (tagged ``typescript``) builds a context.
- `test_function_local_shadow_no_longer_suppresses_builtin(tmp_path: Path)` — [`L485`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L485) — FULL INDEX PATH (#626 precision gain): ``function f() { const Math = 1 }``
- `test_global_object_receiver_classifies_builtin()` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L130)
- `test_import_shadow_suppresses_builtin()` — [`L247`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L247) — ``import { Map } from './map'; Map.of(...)`` — ``Map`` is shadowed by an
- `test_integration_bare_method_stays_unknown(tmp_path: Path)` — [`L401`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L401)
- `test_integration_console_log_classifies_builtin(tmp_path: Path)` — [`L390`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L390)
- `test_integration_default_import_shadow_suppresses_builtin(tmp_path: Path)` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L315) — FULL INDEX PATH (Codex P2 #4): a default import ``import Promise from
- `test_integration_import_shadow_no_project_symbol_suppresses_builtin(tmp_path: Path)` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L288) — FULL INDEX PATH (Codex P2 #4): ``import { Map } from 'immutable'`` with NO
- `test_integration_import_shadow_suppresses_builtin(tmp_path: Path)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L264) — FULL INDEX PATH (Codex P2 #3): ``import { Map } from './map'`` shadows the
- `test_integration_local_call_resolves(tmp_path: Path)` — [`L373`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L373)
- `test_integration_no_cross_language_mis_wire(tmp_path: Path)` — [`L419`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L419) — MANDATORY no-cross-language-mis-wire test.
- `test_integration_unshadowed_global_still_builtin(tmp_path: Path)` — [`L358`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L358) — Guard: an UN-shadowed ``Math.max()`` must still classify ``builtin`` — the
- `test_integration_variable_shadow_suppresses_builtin(tmp_path: Path)` — [`L337`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L337) — FULL INDEX PATH: ``const Promise = require('bluebird')`` shadows the
- `test_json_receiver_classifies_builtin()` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L138)
- `test_local_no_receiver_resolves_same_file()` — [`L111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L111)
- `test_local_this_receiver_resolves_class_method()` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L119)
- `test_no_cross_language_bind_for_global_object_owner()` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L169) — THE MOAT: a Python file owning a symbol named ``console`` must NOT
- `test_project_shadows_builtin_global_name()` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L156) — If the project defines a TS symbol named ``Math`` (a distinctive global),
- `test_shadow_local_is_file_scoped()` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L255) — A shadow in ``other.ts`` must NOT suppress the builtin in ``a.ts``.
- `test_shadow_locals_from_cache_are_module_scope_only(tmp_path: Path)` — [`L463`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L463) — SET-CONSTRUCTION pin through the real cache (#626): module-level
- `test_this_method_ambiguous_across_classes_stays_unknown()` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L188) — ``class A { foo(){} } class B { bar(){ this.foo(); } foo(){} }``.
- `test_this_method_never_falls_through_to_top_level_function()` — [`L220`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L220) — ``this.helper()`` must NOT bind to a top-level ``function helper`` — a
- `test_this_method_unambiguous_resolves_local()` — [`L207`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L207) — When exactly one class in the file defines the method, ``this.foo()``
- `test_variable_shadow_suppresses_builtin()` — [`L237`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_typescript_method_resolution.py#L237) — ``const Promise = require('bluebird'); Promise.all(...)`` — ``Promise`` is

