---
title: 'Module: tests/unit/test_cpp_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_cpp_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_cpp_method_resolution`/
symbols:
  _build_ctx: _build_ctx().
  _index_and_build: _index_and_build().
  TestRegistrationAndDispatch.test_resolve_callee_dispatches_to_cpp: TestRegistrationAndDispatch#test_resolve_callee_dispatches_to_cpp().
  TestRegistrationAndDispatch.test_resolve_callee_moat_through_public_api: TestRegistrationAndDispatch#test_resolve_callee_moat_through_public_api().
  TestRealIndexIntegration.test_cpp_context_is_built_from_real_index: TestRealIndexIntegration#test_cpp_context_is_built_from_real_index().
  TestRealIndexIntegration.test_moat_holds_on_real_index: TestRealIndexIntegration#test_moat_holds_on_real_index().
  TestRealIndexIntegration.test_this_member_call_never_mis_binds_on_real_index: TestRealIndexIntegration#test_this_member_call_never_mis_binds_on_real_index().
  _build_multiclass_ctx: _build_multiclass_ctx().
  TestRealIndexIntegration.test_stdlib_qualifier_resolves_on_real_index: TestRealIndexIntegration#test_stdlib_qualifier_resolves_on_real_index().
  TestRealIndexIntegration.test_local_free_function_resolves_on_real_index: TestRealIndexIntegration#test_local_free_function_resolves_on_real_index().
  TestBuildCppContext.test_builds_when_cpp_present: TestBuildCppContext#test_builds_when_cpp_present().
  TestBuildCppContext.test_does_not_call_class_methods_thunk: TestBuildCppContext#test_does_not_call_class_methods_thunk().
  TestStdlibQualifier.test_std_sort_is_stdlib: TestStdlibQualifier#test_std_sort_is_stdlib().
  TestStdlibQualifier.test_std_make_unique_is_stdlib: TestStdlibQualifier#test_std_make_unique_is_stdlib().
  TestStdlibQualifier.test_nested_std_namespace_is_stdlib: TestStdlibQualifier#test_nested_std_namespace_is_stdlib().
  TestLocalAndProject.test_local_free_function: TestLocalAndProject#test_local_free_function().
  TestLocalAndProject.test_this_qualified_member_is_local: TestLocalAndProject#test_this_qualified_member_is_local().
  TestLocalAndProject.test_implicit_this_member_is_local: TestLocalAndProject#test_implicit_this_member_is_local().
  TestLocalAndProject.test_single_global_project: TestLocalAndProject#test_single_global_project().
  TestLocalAndProject.test_instance_receiver_is_unknown: TestLocalAndProject#test_instance_receiver_is_unknown().
  TestLocalAndProject.test_non_stdlib_qualified_is_unknown: TestLocalAndProject#test_non_stdlib_qualified_is_unknown().
  TestLocalAndProject.test_truly_unknown_name: TestLocalAndProject#test_truly_unknown_name().
  TestExplicitSelfReceiver.test_this_call_does_not_bind_same_file_free_function: TestExplicitSelfReceiver#test_this_call_does_not_bind_same_file_free_function().
  TestExplicitSelfReceiver.test_this_call_does_not_bind_same_file_class: TestExplicitSelfReceiver#test_this_call_does_not_bind_same_file_class().
  TestExplicitSelfReceiver.test_this_call_does_not_bind_cross_file_global: TestExplicitSelfReceiver#test_this_call_does_not_bind_cross_file_global().
  TestExplicitSelfReceiver.test_self_receiver_variants_do_not_bind_free_function: TestExplicitSelfReceiver#test_self_receiver_variants_do_not_bind_free_function().
  TestExplicitSelfReceiver.test_unqualified_free_function_still_binds_local: TestExplicitSelfReceiver#test_unqualified_free_function_still_binds_local().
  TestMultiClassOwnerScoping.test_self_call_to_ambiguous_member_stays_unknown: TestMultiClassOwnerScoping#test_self_call_to_ambiguous_member_stays_unknown().
  TestMultiClassOwnerScoping.test_implicit_this_call_to_ambiguous_member_stays_unknown: TestMultiClassOwnerScoping#test_implicit_this_call_to_ambiguous_member_stays_unknown().
  TestMultiClassOwnerScoping.test_self_call_to_single_owner_member_still_binds: TestMultiClassOwnerScoping#test_self_call_to_single_owner_member_still_binds().
  TestMultiClassOwnerScoping.test_unqualified_free_function_unaffected_by_method_ambiguity: TestMultiClassOwnerScoping#test_unqualified_free_function_unaffected_by_method_ambiguity().
  TestNoCrossLanguageMisWire.test_ambiguous_name_resolves_to_cpp_def_not_python: TestNoCrossLanguageMisWire#test_ambiguous_name_resolves_to_cpp_def_not_python().
  TestNoCrossLanguageMisWire.test_python_only_symbol_is_never_bound: TestNoCrossLanguageMisWire#test_python_only_symbol_is_never_bound().
  TestNoCrossLanguageMisWire.test_ambiguous_global_only_foreign_plus_self_stays_cpp: TestNoCrossLanguageMisWire#test_ambiguous_global_only_foreign_plus_self_stays_cpp().
  TestCHeaderCompat.test_cpp_resolves_c_header_symbol: TestCHeaderCompat#test_cpp_resolves_c_header_symbol().
  TestRegistrationAndDispatch.test_cpp_is_registered: TestRegistrationAndDispatch#test_cpp_is_registered().
  _REAL_CPP: _REAL_CPP.
  TestBuildCppContext.test_returns_none_when_no_cpp_file: TestBuildCppContext#test_returns_none_when_no_cpp_file().
  TestStdlibQualifier.test_is_stdlib_qualifier_helper: TestStdlibQualifier#test_is_stdlib_qualifier_helper().
  _REAL_PY: _REAL_PY.
  TestBuildCppContext.thunk: TestBuildCppContext#thunk().
  TestBuildCppContext: TestBuildCppContext#
  TestStdlibQualifier: TestStdlibQualifier#
  TestLocalAndProject: TestLocalAndProject#
  TestExplicitSelfReceiver: TestExplicitSelfReceiver#
  TestMultiClassOwnerScoping: TestMultiClassOwnerScoping#
  TestNoCrossLanguageMisWire: TestNoCrossLanguageMisWire#
  TestCHeaderCompat: TestCHeaderCompat#
  TestRegistrationAndDispatch: TestRegistrationAndDispatch#
  TestRealIndexIntegration: TestRealIndexIntegration#
---
# Module: [`tests/unit/test_cpp_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py)

## Classes
### `TestBuildCppContext`
- def: [`tests/unit/test_cpp_method_resolution.py:83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L83)
- signature: `class TestBuildCppContext:`
- members:
  - `test_builds_when_cpp_present(self)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L94)
  - `test_does_not_call_class_methods_thunk(self)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L104)
  - `test_returns_none_when_no_cpp_file(self)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L84)
  - `thunk()` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L107)
- uses (calls/refs, reference-scoped): [`build_cpp_context`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#build_cpp_context), [`CppResolverContext`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#CppResolverContext)

### `TestCHeaderCompat`
- def: [`tests/unit/test_cpp_method_resolution.py:439`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L439)
- signature: `class TestCHeaderCompat:`
- members:
  - `test_cpp_resolves_c_header_symbol(self)` — [`L440`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L440) — A C++ caller MAY resolve a symbol defined in a C-tagged header.
- uses (calls/refs, reference-scoped): [`resolve_cpp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#resolve_cpp_callee), [`build_cpp_context`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#build_cpp_context)

### `TestExplicitSelfReceiver`
- def: [`tests/unit/test_cpp_method_resolution.py:231`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L231)
- doc: An explicit `this->` / `self` receiver asserts the target is a
- signature: `class TestExplicitSelfReceiver:`
- members:
  - `test_self_receiver_variants_do_not_bind_free_function(self)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L271)
  - `test_this_call_does_not_bind_cross_file_global(self)` — [`L259`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L259)
  - `test_this_call_does_not_bind_same_file_class(self)` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L250)
  - `test_this_call_does_not_bind_same_file_free_function(self)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L240)
  - `test_unqualified_free_function_still_binds_local(self)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L282)
- uses (calls/refs, reference-scoped): [`resolve_cpp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#resolve_cpp_callee)  (1 test-only)

### `TestLocalAndProject`
- def: [`tests/unit/test_cpp_method_resolution.py:163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L163)
- signature: `class TestLocalAndProject:`
- members:
  - `test_implicit_this_member_is_local(self)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L185) — An unqualified call may also resolve to a same-file member.
  - `test_instance_receiver_is_unknown(self)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L203)
  - `test_local_free_function(self)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L164)
  - `test_non_stdlib_qualified_is_unknown(self)` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L211)
  - `test_single_global_project(self)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L193)
  - `test_this_qualified_member_is_local(self)` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L171) — An explicit ``this->`` call MAY bind to a same-file MEMBER.
  - `test_truly_unknown_name(self)` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L218)
- uses (calls/refs, reference-scoped): [`resolve_cpp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#resolve_cpp_callee)  (1 test-only)

### `TestMultiClassOwnerScoping`
- def: [`tests/unit/test_cpp_method_resolution.py:344`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L344)
- signature: `class TestMultiClassOwnerScoping:`
- members:
  - `test_implicit_this_call_to_ambiguous_member_stays_unknown(self)` — [`L357`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L357)
  - `test_self_call_to_ambiguous_member_stays_unknown(self)` — [`L345`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L345)
  - `test_self_call_to_single_owner_member_still_binds(self)` — [`L365`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L365)
  - `test_unqualified_free_function_unaffected_by_method_ambiguity(self)` — [`L374`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L374)
- uses (calls/refs, reference-scoped): [`resolve_cpp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#resolve_cpp_callee)  (1 test-only)

### `TestNoCrossLanguageMisWire`
- def: [`tests/unit/test_cpp_method_resolution.py:388`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L388)
- signature: `class TestNoCrossLanguageMisWire:`
- members:
  - `test_ambiguous_global_only_foreign_plus_self_stays_cpp(self)` — [`L419`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L419) — A name with one C++ and one Python global, called from a 3rd C++ file.
  - `test_ambiguous_name_resolves_to_cpp_def_not_python(self)` — [`L389`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L389) — ``parse`` exists in BOTH a .cpp and a .py file.
  - `test_python_only_symbol_is_never_bound(self)` — [`L404`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L404) — ``only_python`` exists ONLY in a Python file.
- uses (calls/refs, reference-scoped): [`resolve_cpp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#resolve_cpp_callee)  (1 test-only)

### `TestRealIndexIntegration`
- def: [`tests/unit/test_cpp_method_resolution.py:570`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L570)
- signature: `class TestRealIndexIntegration:`
- members:
  - `test_cpp_context_is_built_from_real_index(self, tmp_path)` — [`L571`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L571) — A parsed ``.cpp`` file yields a non-None C++ resolver context.
  - `test_local_free_function_resolves_on_real_index(self, tmp_path)` — [`L639`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L639) — When the extractor populates C++ symbols, an unqualified call to a
  - `test_moat_holds_on_real_index(self, tmp_path)` — [`L592`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L592) — THE MOAT on a REAL index: a C++ caller's ``helper`` call must never
  - `test_stdlib_qualifier_resolves_on_real_index(self, tmp_path)` — [`L581`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L581) — ``std::sort`` -> ``stdlib`` end-to-end (maps-independent tier).
  - `test_this_member_call_never_mis_binds_on_real_index(self, tmp_path)` — [`L607`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L607) — ``this->helper`` on a real index resolves to a C++ member or stays
- uses (calls/refs, reference-scoped): [`resolve_cpp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#resolve_cpp_callee), [`CppResolverContext`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#CppResolverContext), [`file_languages`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#CppResolverContext.file_languages)  (3 test-only)

### `TestRegistrationAndDispatch`
- def: [`tests/unit/test_cpp_method_resolution.py:466`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L466)
- signature: `class TestRegistrationAndDispatch:`
- members:
  - `test_cpp_is_registered(self)` — [`L467`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L467)
  - `test_resolve_callee_dispatches_to_cpp(self)` — [`L472`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L472)
  - `test_resolve_callee_moat_through_public_api(self)` — [`L500`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L500)
- uses (calls/refs, reference-scoped): [`ResolverContext`](../../tree_sitter_analyzer/synapse_resolver/_context.md#ResolverContext), [`resolve_callee`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#resolve_callee), [`resolution`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.resolution), [`get_language_resolver`](../../tree_sitter_analyzer/synapse_resolver/_registry.md#get_language_resolver), [`resolved_file`](../../tree_sitter_analyzer/synapse_resolver/__init__.md#ResolvedCallee.resolved_file), [`language`](../../tree_sitter_analyzer/synapse_resolver/_registry.md#LanguageResolver.language)  (1 test-only)

### `TestStdlibQualifier`
- def: [`tests/unit/test_cpp_method_resolution.py:126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L126)
- signature: `class TestStdlibQualifier:`
- members:
  - `test_is_stdlib_qualifier_helper(self)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L146)
  - `test_nested_std_namespace_is_stdlib(self)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L139)
  - `test_std_make_unique_is_stdlib(self)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L132)
  - `test_std_sort_is_stdlib(self)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L127)
- uses (calls/refs, reference-scoped): [`resolve_cpp_callee`](../../tree_sitter_analyzer/synapse_resolver/languages/cpp.md#resolve_cpp_callee), [`is_stdlib_qualifier`](../../tree_sitter_analyzer/synapse_resolver/languages/_cpp_constants.md#is_stdlib_qualifier)  (1 test-only)

## Functions
- `_build_ctx()` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L32) — service.cpp + helper.cpp, with a same-named Python symbol elsewhere.
- `_build_multiclass_ctx()` — [`L304`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L304) — One .cpp file with TWO classes that each define ``dispatch``.
- `_index_and_build(tmp_path, files: dict[str, str])` — [`L540`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L540) — Write ``files`` into ``tmp_path``, index them, return (root, cpp_ctx).

## Module values
- `_REAL_CPP` — [`L555`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L555)
- `_REAL_PY` — [`L567`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_cpp_method_resolution.py#L567)

