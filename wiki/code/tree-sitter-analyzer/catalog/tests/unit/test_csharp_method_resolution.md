---
title: 'Module: tests/unit/test_csharp_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_csharp_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_csharp_method_resolution`/
symbols:
  _build_ctx: _build_ctx().
  _index_and_build: _index_and_build().
  TestRegistrationAndDispatch.test_resolve_callee_dispatches_to_csharp: TestRegistrationAndDispatch#test_resolve_callee_dispatches_to_csharp().
  TestRegistrationAndDispatch.test_resolve_callee_moat_through_public_api: TestRegistrationAndDispatch#test_resolve_callee_moat_through_public_api().
  TestRealIndexIntegration.test_csharp_context_is_built_from_real_index: TestRealIndexIntegration#test_csharp_context_is_built_from_real_index().
  TestRealIndexIntegration.test_moat_holds_on_real_index: TestRealIndexIntegration#test_moat_holds_on_real_index().
  TestRealIndexIntegration.test_system_qualifier_resolves_on_real_index: TestRealIndexIntegration#test_system_qualifier_resolves_on_real_index().
  TestRealIndexIntegration.test_local_method_resolves_on_real_index: TestRealIndexIntegration#test_local_method_resolves_on_real_index().
  TestLocalAndProject.test_empty_method_tiers: TestLocalAndProject#test_empty_method_tiers().
  TestBuildCSharpContext.test_builds_when_csharp_present: TestBuildCSharpContext#test_builds_when_csharp_present().
  TestBuildCSharpContext.test_does_not_call_class_methods_thunk: TestBuildCSharpContext#test_does_not_call_class_methods_thunk().
  TestSystemQualifier.test_fully_qualified_system_console_is_stdlib: TestSystemQualifier#test_fully_qualified_system_console_is_stdlib().
  TestSystemQualifier.test_nested_system_namespace_is_stdlib: TestSystemQualifier#test_nested_system_namespace_is_stdlib().
  TestBclStaticTypeTier.test_bare_console_writeline_is_stdlib: TestBclStaticTypeTier#test_bare_console_writeline_is_stdlib().
  TestBclStaticTypeTier.test_bare_string_format_is_stdlib: TestBclStaticTypeTier#test_bare_string_format_is_stdlib().
  TestBclStaticTypeTier.test_bare_math_max_is_stdlib: TestBclStaticTypeTier#test_bare_math_max_is_stdlib().
  TestBclStaticTypeTier.test_project_owned_static_type_shadows_bcl: TestBclStaticTypeTier#test_project_owned_static_type_shadows_bcl().
  TestBclStaticTypeTier.test_foreign_language_console_does_not_shadow_bcl: TestBclStaticTypeTier#test_foreign_language_console_does_not_shadow_bcl().
  TestBclStaticTypeTier.test_non_bcl_static_type_is_unknown: TestBclStaticTypeTier#test_non_bcl_static_type_is_unknown().
  TestLocalAndProject.test_local_bare_method: TestLocalAndProject#test_local_bare_method().
  TestLocalAndProject.test_this_qualified_member_is_local: TestLocalAndProject#test_this_qualified_member_is_local().
  TestLocalAndProject.test_single_global_project: TestLocalAndProject#test_single_global_project().
  TestLocalAndProject.test_instance_receiver_is_unknown: TestLocalAndProject#test_instance_receiver_is_unknown().
  TestLocalAndProject.test_truly_unknown_name: TestLocalAndProject#test_truly_unknown_name().
  TestSelfReceiver.test_this_call_does_not_bind_cross_file_global: TestSelfReceiver#test_this_call_does_not_bind_cross_file_global().
  TestSelfReceiver.test_base_call_binds_same_file_member: TestSelfReceiver#test_base_call_binds_same_file_member().
  TestSelfReceiver.test_ambiguous_self_member_stays_unknown: TestSelfReceiver#test_ambiguous_self_member_stays_unknown().
  TestNoCrossLanguageMisWire.test_ambiguous_name_resolves_to_csharp_def_not_python: TestNoCrossLanguageMisWire#test_ambiguous_name_resolves_to_csharp_def_not_python().
  TestNoCrossLanguageMisWire.test_python_only_symbol_is_never_bound: TestNoCrossLanguageMisWire#test_python_only_symbol_is_never_bound().
  TestNoCrossLanguageMisWire.test_ambiguous_global_foreign_plus_self_stays_csharp: TestNoCrossLanguageMisWire#test_ambiguous_global_foreign_plus_self_stays_csharp().
  TestRegistrationAndDispatch.test_csharp_is_registered: TestRegistrationAndDispatch#test_csharp_is_registered().
  _REAL_CS: _REAL_CS.
  TestBuildCSharpContext.test_returns_none_when_no_csharp_file: TestBuildCSharpContext#test_returns_none_when_no_csharp_file().
  TestSystemQualifier.test_is_system_qualifier_helper: TestSystemQualifier#test_is_system_qualifier_helper().
  TestBuildCSharpContext.thunk: TestBuildCSharpContext#thunk().
  _REAL_PY: _REAL_PY.
  TestBuildCSharpContext: TestBuildCSharpContext#
  TestSystemQualifier: TestSystemQualifier#
  TestBclStaticTypeTier: TestBclStaticTypeTier#
  TestLocalAndProject: TestLocalAndProject#
  TestSelfReceiver: TestSelfReceiver#
  TestNoCrossLanguageMisWire: TestNoCrossLanguageMisWire#
  TestRegistrationAndDispatch: TestRegistrationAndDispatch#
  TestRealIndexIntegration: TestRealIndexIntegration#
---
# Module: [`tests/unit/test_csharp_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py)

## Classes
### `TestBclStaticTypeTier`
- def: [`tests/unit/test_csharp_method_resolution.py:167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L167)
- signature: `class TestBclStaticTypeTier:`
- members:
  - `test_bare_console_writeline_is_stdlib(self)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L168)
  - `test_bare_math_max_is_stdlib(self)` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L182)
  - `test_bare_string_format_is_stdlib(self)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L175)
  - `test_foreign_language_console_does_not_shadow_bcl(self)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L210) — A same-named symbol in a NON-C# file must NOT shadow the BCL claim —
  - `test_non_bcl_static_type_is_unknown(self)` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L233)
  - `test_project_owned_static_type_shadows_bcl(self)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L187) — If the project itself defines a class named ``Console`` (a same-
- uses (calls/refs, reference-scoped): [`resolve_csharp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#resolve_csharp_callee), [`build_csharp_context`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#build_csharp_context)  (1 test-only)

### `TestBuildCSharpContext`
- def: [`tests/unit/test_csharp_method_resolution.py:88`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L88)
- signature: `class TestBuildCSharpContext:`
- members:
  - `test_builds_when_csharp_present(self)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L99)
  - `test_does_not_call_class_methods_thunk(self)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L109)
  - `test_returns_none_when_no_csharp_file(self)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L89)
  - `thunk()` — [`L112`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L112)
- uses (calls/refs, reference-scoped): [`build_csharp_context`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#build_csharp_context), [`CSharpResolverContext`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#CSharpResolverContext)

### `TestLocalAndProject`
- def: [`tests/unit/test_csharp_method_resolution.py:246`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L246)
- signature: `class TestLocalAndProject:`
- members:
  - `test_empty_method_tiers(self)` — [`L288`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L288)
  - `test_instance_receiver_is_unknown(self)` — [`L273`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L273)
  - `test_local_bare_method(self)` — [`L247`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L247)
  - `test_single_global_project(self)` — [`L263`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L263)
  - `test_this_qualified_member_is_local(self)` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L254)
  - `test_truly_unknown_name(self)` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L281)
- uses (calls/refs, reference-scoped): [`resolve_csharp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#resolve_csharp_callee), [`BCL_STATIC_TYPES_CSHARP`](../../tree_sitter_analyzer/synapse_resolver/languages/_csharp_constants.md#BCL_STATIC_TYPES_CSHARP.BCL_STATIC_TYPES_CSHARP), [`EXTERNAL_METHODS_CSHARP`](../../tree_sitter_analyzer/synapse_resolver/languages/_csharp_constants.md#EXTERNAL_METHODS_CSHARP.EXTERNAL_METHODS_CSHARP), [`STDLIB_METHODS_CSHARP`](../../tree_sitter_analyzer/synapse_resolver/languages/_csharp_constants.md#STDLIB_METHODS_CSHARP.STDLIB_METHODS_CSHARP)  (1 test-only)

### `TestNoCrossLanguageMisWire`
- def: [`tests/unit/test_csharp_method_resolution.py:370`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L370)
- signature: `class TestNoCrossLanguageMisWire:`
- members:
  - `test_ambiguous_global_foreign_plus_self_stays_csharp(self)` — [`L399`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L399) — ``Run`` has (Greeter.cs, util.py); called from a 3rd C# file.
  - `test_ambiguous_name_resolves_to_csharp_def_not_python(self)` — [`L371`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L371) — ``Run`` exists in BOTH a .cs and a .py file.
  - `test_python_only_symbol_is_never_bound(self)` — [`L384`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L384) — ``OnlyPython`` exists ONLY in a Python file.
- uses (calls/refs, reference-scoped): [`resolve_csharp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#resolve_csharp_callee)  (1 test-only)

### `TestRealIndexIntegration`
- def: [`tests/unit/test_csharp_method_resolution.py:519`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L519)
- signature: `class TestRealIndexIntegration:`
- members:
  - `test_csharp_context_is_built_from_real_index(self, tmp_path)` — [`L520`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L520)
  - `test_local_method_resolves_on_real_index(self, tmp_path)` — [`L539`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L539) — The C# walker DOES record methods, so an unqualified same-file call
  - `test_moat_holds_on_real_index(self, tmp_path)` — [`L552`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L552) — A C# caller's ``Helper`` call must never bind to the same-named
  - `test_system_qualifier_resolves_on_real_index(self, tmp_path)` — [`L529`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L529)
- uses (calls/refs, reference-scoped): [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`resolve_csharp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#resolve_csharp_callee), [`CSharpResolverContext`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#CSharpResolverContext), [`file_languages`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#CSharpResolverContext.file_languages)  (3 test-only)

### `TestRegistrationAndDispatch`
- def: [`tests/unit/test_csharp_method_resolution.py:419`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L419)
- signature: `class TestRegistrationAndDispatch:`
- members:
  - `test_csharp_is_registered(self)` — [`L420`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L420)
  - `test_resolve_callee_dispatches_to_csharp(self)` — [`L425`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L425)
  - `test_resolve_callee_moat_through_public_api(self)` — [`L456`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L456)
- uses (calls/refs, reference-scoped): [`ResolverContext`](../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext), [`resolve_callee`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#resolve_callee), [`resolution`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.resolution), [`get_language_resolver`](../../tree_sitter_analyzer/synapse_resolver/_registry.md#get_language_resolver), [`resolved_file`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.resolved_file), [`language`](../../tree_sitter_analyzer/synapse_resolver/_registry.md#LanguageResolver.language)  (1 test-only)

### `TestSelfReceiver`
- def: [`tests/unit/test_csharp_method_resolution.py:302`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L302)
- doc: An explicit `this.` / `base.` receiver asserts the target is a
- signature: `class TestSelfReceiver:`
- members:
  - `test_ambiguous_self_member_stays_unknown(self)` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L327) — When >1 class in the file defines the member name, a ``this.`` call
  - `test_base_call_binds_same_file_member(self)` — [`L319`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L319)
  - `test_this_call_does_not_bind_cross_file_global(self)` — [`L308`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L308)
- uses (calls/refs, reference-scoped): [`resolve_csharp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#resolve_csharp_callee), [`build_csharp_context`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#build_csharp_context)  (1 test-only)

### `TestSystemQualifier`
- def: [`tests/unit/test_csharp_method_resolution.py:131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L131)
- signature: `class TestSystemQualifier:`
- members:
  - `test_fully_qualified_system_console_is_stdlib(self)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L132)
  - `test_is_system_qualifier_helper(self)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L149)
  - `test_nested_system_namespace_is_stdlib(self)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L139)
- uses (calls/refs, reference-scoped): [`resolve_csharp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/csharp.md#resolve_csharp_callee), [`is_system_qualifier`](../../tree_sitter_analyzer/synapse_resolver/languages/_csharp_constants.md#is_system_qualifier)  (1 test-only)

## Functions
- `_build_ctx()` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L35) — Greeter.cs + Helper.cs + a same-named Python symbol elsewhere.
- `_index_and_build(tmp_path, files: dict[str, str])` — [`L483`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L483) — Write ``files`` into ``tmp_path``, index them, return (cache, cs_ctx).

## Module values
- `_REAL_CS` — [`L500`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L500)
- `_REAL_PY` — [`L516`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_csharp_method_resolution.py#L516)

