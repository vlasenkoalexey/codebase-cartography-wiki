---
title: 'Module: tests/unit/test_c_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_c_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_c_method_resolution`/
symbols:
  _index_and_build: _index_and_build().
  _build_ctx: _build_ctx().
  TestRegistrationAndDispatch.test_resolve_callee_dispatches_to_c: TestRegistrationAndDispatch#test_resolve_callee_dispatches_to_c().
  TestRegistrationAndDispatch.test_resolve_callee_moat_through_public_api: TestRegistrationAndDispatch#test_resolve_callee_moat_through_public_api().
  TestRealIndexIntegration.test_c_context_is_built_from_real_index: TestRealIndexIntegration#test_c_context_is_built_from_real_index().
  TestRealIndexIntegration.test_moat_holds_on_real_index: TestRealIndexIntegration#test_moat_holds_on_real_index().
  TestRealIndexIntegration.test_foreign_malloc_does_not_shadow_libc_on_real_index: TestRealIndexIntegration#test_foreign_malloc_does_not_shadow_libc_on_real_index().
  TestRealIndexIntegration.test_libc_tier_resolves_on_real_index: TestRealIndexIntegration#test_libc_tier_resolves_on_real_index().
  TestRealIndexIntegration.test_project_defined_malloc_is_not_stdlib_on_real_index: TestRealIndexIntegration#test_project_defined_malloc_is_not_stdlib_on_real_index().
  TestRealIndexIntegration.test_local_free_function_resolves_on_real_index: TestRealIndexIntegration#test_local_free_function_resolves_on_real_index().
  TestBuildCContext.test_builds_when_c_present: TestBuildCContext#test_builds_when_c_present().
  TestLibcTier.test_malloc_is_stdlib: TestLibcTier#test_malloc_is_stdlib().
  TestLibcTier.test_printf_is_stdlib: TestLibcTier#test_printf_is_stdlib().
  TestLibcTier.test_memcpy_is_stdlib: TestLibcTier#test_memcpy_is_stdlib().
  TestLibcTier.test_project_shadows_libc_name: TestLibcTier#test_project_shadows_libc_name().
  TestLibcTier.test_project_shadows_libc_from_other_file: TestLibcTier#test_project_shadows_libc_from_other_file().
  TestLocalAndProject.test_local_free_function: TestLocalAndProject#test_local_free_function().
  TestLocalAndProject.test_single_global_project: TestLocalAndProject#test_single_global_project().
  TestLocalAndProject.test_struct_field_receiver_is_unknown: TestLocalAndProject#test_struct_field_receiver_is_unknown().
  TestLocalAndProject.test_dot_receiver_is_unknown: TestLocalAndProject#test_dot_receiver_is_unknown().
  TestLocalAndProject.test_truly_unknown_name: TestLocalAndProject#test_truly_unknown_name().
  TestNoCrossLanguageMisWire.test_ambiguous_name_resolves_to_c_def_not_python: TestNoCrossLanguageMisWire#test_ambiguous_name_resolves_to_c_def_not_python().
  TestNoCrossLanguageMisWire.test_python_only_symbol_is_never_bound: TestNoCrossLanguageMisWire#test_python_only_symbol_is_never_bound().
  TestNoCrossLanguageMisWire.test_ambiguous_global_foreign_plus_self_stays_c: TestNoCrossLanguageMisWire#test_ambiguous_global_foreign_plus_self_stays_c().
  TestNoCrossLanguageMisWire.test_c_caller_never_binds_cpp_definition: TestNoCrossLanguageMisWire#test_c_caller_never_binds_cpp_definition().
  TestCHeaderCompat.test_c_resolves_c_header_symbol: TestCHeaderCompat#test_c_resolves_c_header_symbol().
  TestRegistrationAndDispatch.test_c_is_registered: TestRegistrationAndDispatch#test_c_is_registered().
  _REAL_C: _REAL_C.
  TestBuildCContext.test_returns_none_when_no_c_file: TestBuildCContext#test_returns_none_when_no_c_file().
  TestBuildCContext.test_cpp_only_project_does_not_build_c_context: TestBuildCContext#test_cpp_only_project_does_not_build_c_context().
  TestLibcTier.test_is_libc_function_helper: TestLibcTier#test_is_libc_function_helper().
  TestLibcTier.test_libc_set_is_nonempty_and_lowercase: TestLibcTier#test_libc_set_is_nonempty_and_lowercase().
  _REAL_PY: _REAL_PY.
  _REAL_C_CUSTOM_MALLOC: _REAL_C_CUSTOM_MALLOC.
  _REAL_PY_MALLOC: _REAL_PY_MALLOC.
  TestBuildCContext: TestBuildCContext#
  TestLibcTier: TestLibcTier#
  TestLocalAndProject: TestLocalAndProject#
  TestNoCrossLanguageMisWire: TestNoCrossLanguageMisWire#
  TestCHeaderCompat: TestCHeaderCompat#
  TestRegistrationAndDispatch: TestRegistrationAndDispatch#
  TestRealIndexIntegration: TestRealIndexIntegration#
---
# Module: [`tests/unit/test_c_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py)

## Classes
### `TestBuildCContext`
- def: [`tests/unit/test_c_method_resolution.py:84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L84)
- signature: `class TestBuildCContext:`
- members:
  - `test_builds_when_c_present(self)` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L95)
  - `test_cpp_only_project_does_not_build_c_context(self)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L105)
  - `test_returns_none_when_no_c_file(self)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L85)
- uses (calls/refs, reference-scoped): [`build_c_context`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#build_c_context), [`CResolverContext`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#CResolverContext)

### `TestCHeaderCompat`
- def: [`tests/unit/test_c_method_resolution.py:328`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L328)
- signature: `class TestCHeaderCompat:`
- members:
  - `test_c_resolves_c_header_symbol(self)` — [`L329`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L329) — A C caller MAY resolve a symbol declared in a C-tagged header.
- uses (calls/refs, reference-scoped): [`resolve_c_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#resolve_c_callee), [`build_c_context`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#build_c_context)

### `TestLibcTier`
- def: [`tests/unit/test_c_method_resolution.py:123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L123)
- signature: `class TestLibcTier:`
- members:
  - `test_is_libc_function_helper(self)` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L179)
  - `test_libc_set_is_nonempty_and_lowercase(self)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L195)
  - `test_malloc_is_stdlib(self)` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L124)
  - `test_memcpy_is_stdlib(self)` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L134)
  - `test_printf_is_stdlib(self)` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L129)
  - `test_project_shadows_libc_from_other_file(self)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L159) — A project ``malloc`` in ANOTHER C file shadows the libc tier too.
  - `test_project_shadows_libc_name(self)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L139) — If the project defines a function whose name collides with a libc
- uses (calls/refs, reference-scoped): [`resolve_c_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#resolve_c_callee), [`build_c_context`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#build_c_context), [`is_libc_function`](../../tree_sitter_analyzer/synapse_resolver/languages/_c_constants.md#is_libc_function), [`LIBC_FUNCTIONS_C`](../../tree_sitter_analyzer/synapse_resolver/languages/_c_constants.md#LIBC_FUNCTIONS_C.LIBC_FUNCTIONS_C)  (1 test-only)

### `TestLocalAndProject`
- def: [`tests/unit/test_c_method_resolution.py:207`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L207)
- signature: `class TestLocalAndProject:`
- members:
  - `test_dot_receiver_is_unknown(self)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L234)
  - `test_local_free_function(self)` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L208)
  - `test_single_global_project(self)` — [`L215`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L215)
  - `test_struct_field_receiver_is_unknown(self)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L225)
  - `test_truly_unknown_name(self)` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L241)
- uses (calls/refs, reference-scoped): [`resolve_c_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#resolve_c_callee)  (1 test-only)

### `TestNoCrossLanguageMisWire`
- def: [`tests/unit/test_c_method_resolution.py:254`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L254)
- signature: `class TestNoCrossLanguageMisWire:`
- members:
  - `test_ambiguous_global_foreign_plus_self_stays_c(self)` — [`L283`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L283) — A name with one C and one Python global, called from a 3rd C file.
  - `test_ambiguous_name_resolves_to_c_def_not_python(self)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L255) — ``parse`` exists in BOTH a .c and a .py file.
  - `test_c_caller_never_binds_cpp_definition(self)` — [`L297`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L297) — DIRECTIONAL MOAT: a C caller must NEVER bind a C++ definition.
  - `test_python_only_symbol_is_never_bound(self)` — [`L268`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L268) — ``only_python`` exists ONLY in a Python file.
- uses (calls/refs, reference-scoped): [`resolve_c_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#resolve_c_callee), [`build_c_context`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#build_c_context)  (1 test-only)

### `TestRealIndexIntegration`
- def: [`tests/unit/test_c_method_resolution.py:469`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L469)
- signature: `class TestRealIndexIntegration:`
- members:
  - `test_c_context_is_built_from_real_index(self, tmp_path)` — [`L470`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L470) — A parsed ``.c`` file yields a non-None C resolver context.
  - `test_foreign_malloc_does_not_shadow_libc_on_real_index(self, tmp_path)` — [`L522`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L522) — THE MOAT under the custom-libc fix: a Python ``malloc`` must NOT count
  - `test_libc_tier_resolves_on_real_index(self, tmp_path)` — [`L479`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L479) — ``malloc`` -> ``stdlib`` end-to-end (maps-independent tier).
  - `test_local_free_function_resolves_on_real_index(self, tmp_path)` — [`L534`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L534) — An unqualified call to a same-file C free function (``helper``) must
  - `test_moat_holds_on_real_index(self, tmp_path)` — [`L491`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L491) — THE MOAT on a REAL index: a C caller's ``helper`` call must never
  - `test_project_defined_malloc_is_not_stdlib_on_real_index(self, tmp_path)` — [`L501`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L501) — Codex P2 (PR #353): a C project that DEFINES its own ``malloc`` must
- uses (calls/refs, reference-scoped): [`resolve_c_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#resolve_c_callee), [`CResolverContext`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#CResolverContext), [`file_languages`](../../tree_sitter_analyzer/synapse_resolver/languages/c.md#CResolverContext.file_languages)  (5 test-only)

### `TestRegistrationAndDispatch`
- def: [`tests/unit/test_c_method_resolution.py:359`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L359)
- signature: `class TestRegistrationAndDispatch:`
- members:
  - `test_c_is_registered(self)` — [`L360`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L360)
  - `test_resolve_callee_dispatches_to_c(self)` — [`L365`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L365)
  - `test_resolve_callee_moat_through_public_api(self)` — [`L391`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L391)
- uses (calls/refs, reference-scoped): [`ResolverContext`](../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext), [`resolve_callee`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#resolve_callee), [`resolution`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.resolution), [`get_language_resolver`](../../tree_sitter_analyzer/synapse_resolver/_registry.md#get_language_resolver), [`resolved_file`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.resolved_file), [`language`](../../tree_sitter_analyzer/synapse_resolver/_registry.md#LanguageResolver.language)  (1 test-only)

## Functions
- `_build_ctx()` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L38) — service.c + helper.c, with a same-named Python symbol elsewhere.
- `_index_and_build(tmp_path, files: dict[str, str])` — [`L424`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L424) — Write ``files`` into ``tmp_path``, index them, return (root, c_ctx).

## Module values
- `_REAL_C` — [`L439`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L439)
- `_REAL_C_CUSTOM_MALLOC` — [`L456`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L456)
- `_REAL_PY` — [`L450`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L450)
- `_REAL_PY_MALLOC` — [`L466`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_c_method_resolution.py#L466)

