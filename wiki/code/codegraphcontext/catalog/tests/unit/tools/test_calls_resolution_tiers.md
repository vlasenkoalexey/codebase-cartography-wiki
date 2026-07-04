---
title: 'Module: tests/unit/tools/test_calls_resolution_tiers.py'
type: catalog
provenance: extracted
module: tests/unit/tools/test_calls_resolution_tiers.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.tools.test_calls_resolution_tiers`/
symbols:
  resolve: resolve().
  _call: _call().
  TestTier1SelfReceiver.test_this_receiver_resolves_to_caller: TestTier1SelfReceiver#test_this_receiver_resolves_to_caller().
  TestTier1SelfReceiver.test_super_receiver_resolves_to_caller: TestTier1SelfReceiver#test_super_receiver_resolves_to_caller().
  TestTier2LocalName.test_local_function_resolves_to_caller: TestTier2LocalName#test_local_function_resolves_to_caller().
  TestTier9SameFileFallback.test_unresolvable_obj_call_falls_back_to_caller: TestTier9SameFileFallback#test_unresolvable_obj_call_falls_back_to_caller().
  CALLER: CALLER.
  TestReturnShape.test_confidence_always_present: TestReturnShape#test_confidence_always_present().
  TestReturnShape.test_resolution_tier_always_present: TestReturnShape#test_resolution_tier_always_present().
  TestReturnShape.test_legacy_keys_still_present: TestReturnShape#test_legacy_keys_still_present().
  TestReturnShape.test_file_type_when_no_caller_context: TestReturnShape#test_file_type_when_no_caller_context().
  TestTier1SelfReceiver.test_this_receiver_tier_is_1: TestTier1SelfReceiver#test_this_receiver_tier_is_1().
  TestTier1SelfReceiver.test_this_receiver_confidence_is_1: TestTier1SelfReceiver#test_this_receiver_confidence_is_1().
  TestTier2LocalName.test_local_function_tier_is_2: TestTier2LocalName#test_local_function_tier_is_2().
  TestTier2LocalName.test_local_function_confidence: TestTier2LocalName#test_local_function_confidence().
  TestTier3InferredFQN.test_fqn_import_resolves_cross_file: TestTier3InferredFQN#test_fqn_import_resolves_cross_file().
  TestTier3InferredFQN.test_tier3_over_tier4_when_fqn_resolves: TestTier3InferredFQN#test_tier3_over_tier4_when_fqn_resolves().
  TestTier4InferredShortName.test_short_name_fallback_when_no_fqn_key: TestTier4InferredShortName#test_short_name_fallback_when_no_fqn_key().
  TestTier5UniqueShortName.test_unique_name_in_imports_map: TestTier5UniqueShortName#test_unique_name_in_imports_map().
  TestTier6QualifiedImport.test_fqn_direct_lookup_in_imports_map: TestTier6QualifiedImport#test_fqn_direct_lookup_in_imports_map().
  TestTier7PathSubstring.test_fqn_as_path_substring: TestTier7PathSubstring#test_fqn_as_path_substring().
  TestTier8AlphabeticalFirst.test_multiple_candidates_no_import_hint: TestTier8AlphabeticalFirst#test_multiple_candidates_no_import_hint().
  TestTier9SameFileFallback.test_skip_external_suppresses_tier9: TestTier9SameFileFallback#test_skip_external_suppresses_tier9().
  TestTier9SameFileFallback.test_skip_external_does_not_suppress_tier1: TestTier9SameFileFallback#test_skip_external_does_not_suppress_tier1().
  TestTier9SameFileFallback.test_skip_external_does_not_suppress_tier2: TestTier9SameFileFallback#test_skip_external_does_not_suppress_tier2().
  TestReturnShape: TestReturnShape#
  TestTier1SelfReceiver: TestTier1SelfReceiver#
  TestTier2LocalName: TestTier2LocalName#
  TestTier3InferredFQN: TestTier3InferredFQN#
  TestTier4InferredShortName: TestTier4InferredShortName#
  TestTier5UniqueShortName: TestTier5UniqueShortName#
  TestTier6QualifiedImport: TestTier6QualifiedImport#
  TestTier7PathSubstring: TestTier7PathSubstring#
  TestTier8AlphabeticalFirst: TestTier8AlphabeticalFirst#
  TestTier8AlphabeticalFirst.test_tier8_confidence_is_low: TestTier8AlphabeticalFirst#test_tier8_confidence_is_low().
  TestTier9SameFileFallback: TestTier9SameFileFallback#
  TestTier9SameFileFallback.test_tier9_confidence_is_very_low: TestTier9SameFileFallback#test_tier9_confidence_is_very_low().
  TestTierConfidenceOrdering: TestTierConfidenceOrdering#
  TestTierConfidenceOrdering.test_tier1_highest_confidence: TestTierConfidenceOrdering#test_tier1_highest_confidence().
  TestTierConfidenceOrdering.test_tier9_lowest_confidence: TestTierConfidenceOrdering#test_tier9_lowest_confidence().
  TestTierConfidenceOrdering.test_all_confidences_in_range: TestTierConfidenceOrdering#test_all_confidences_in_range().
---
# Module: [`tests/unit/tools/test_calls_resolution_tiers.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py)

## Classes
### `TestReturnShape`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:57`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L57)
- signature: `class TestReturnShape:`
- members:
  - `test_confidence_always_present(self)` — [`L59`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L59)
  - `test_file_type_when_no_caller_context(self)` — [`L77`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L77) — A call with context=None must return type='file' (backward compat).
  - `test_legacy_keys_still_present(self)` — [`L69`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L69) — Existing consumers must not break — all original keys must be returned.
  - `test_resolution_tier_always_present(self)` — [`L64`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L64)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTier1SelfReceiver`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:88`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L88)
- signature: `class TestTier1SelfReceiver:`
- members:
  - `test_super_receiver_resolves_to_caller(self)` — [`L102`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L102)
  - `test_this_receiver_confidence_is_1(self)` — [`L98`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L98)
  - `test_this_receiver_resolves_to_caller(self)` — [`L90`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L90)
  - `test_this_receiver_tier_is_1(self)` — [`L94`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L94)
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestTier2LocalName`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:112`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L112)
- signature: `class TestTier2LocalName:`
- members:
  - `test_local_function_confidence(self)` — [`L122`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L122)
  - `test_local_function_resolves_to_caller(self)` — [`L114`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L114)
  - `test_local_function_tier_is_2(self)` — [`L118`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L118)
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestTier3InferredFQN`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:131`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L131)
- signature: `class TestTier3InferredFQN:`
- members:
  - `test_fqn_import_resolves_cross_file(self)` — [`L133`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L133) — When local_imports has the FQN and imports_map[FQN] has exactly 1 path, use Tier 3.
  - `test_tier3_over_tier4_when_fqn_resolves(self)` — [`L150`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L150) — Tier 3 (FQN) must win over Tier 4 (short-name first-match).
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTier4InferredShortName`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:169`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L169)
- signature: `class TestTier4InferredShortName:`
- members:
  - `test_short_name_fallback_when_no_fqn_key(self)` — [`L171`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L171) — When no FQN key exists, fall back to short-name first-match (Tier 4).
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTier5UniqueShortName`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:187`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L187)
- signature: `class TestTier5UniqueShortName:`
- members:
  - `test_unique_name_in_imports_map(self)` — [`L189`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L189)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTier6QualifiedImport`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:202`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L202)
- signature: `class TestTier6QualifiedImport:`
- members:
  - `test_fqn_direct_lookup_in_imports_map(self)` — [`L204`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L204) — When local_imports[name]=FQN and imports_map[FQN] has 1 path → Tier 6.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTier7PathSubstring`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:225`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L225)
- signature: `class TestTier7PathSubstring:`
- members:
  - `test_fqn_as_path_substring(self)` — [`L227`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L227) — When FQN can't resolve directly but matches as a file-path substring → Tier 7.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTier8AlphabeticalFirst`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:249`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L249)
- signature: `class TestTier8AlphabeticalFirst:`
- members:
  - `test_multiple_candidates_no_import_hint(self)` — [`L251`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L251) — When multiple paths, no import hint, no obj type → Tier 8 first-match.
  - `test_tier8_confidence_is_low(self)` — [`L262`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L262) — Tier 8 is a last-resort guess — confidence must be below 0.5.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestTier9SameFileFallback`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:271`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L271)
- signature: `class TestTier9SameFileFallback:`
- members:
  - `test_skip_external_does_not_suppress_tier1(self)` — [`L292`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L292) — self.method() is not external — skip_external must not suppress it.
  - `test_skip_external_does_not_suppress_tier2(self)` — [`L298`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L298) — Local name resolution is not external — skip_external must not suppress it.
  - `test_skip_external_suppresses_tier9(self)` — [`L286`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L286) — When skip_external=True, unresolvable obj.method() calls must return None.
  - `test_tier9_confidence_is_very_low(self)` — [`L282`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L282) — Tier 9 is definitionally wrong for obj.method() — confidence must be < 0.2.
  - `test_unresolvable_obj_call_falls_back_to_caller(self)` — [`L273`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L273) — obj.method() with no type info and no imports_map match → same-file fallback.
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestTierConfidenceOrdering`
- def: [`tests/unit/tools/test_calls_resolution_tiers.py:308`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L308)
- signature: `class TestTierConfidenceOrdering:`
- members:
  - `test_all_confidences_in_range(self)` — [`L320`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L320) — All confidence values must be in [0.0, 1.0].
  - `test_tier1_highest_confidence(self)` — [`L310`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L310) — Tier 1 (certain) must have the highest confidence of all tiers.
  - `test_tier9_lowest_confidence(self)` — [`L315`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L315) — Tier 9 (same-file fallback) must have the lowest confidence.

## Functions
- `_call(called_name, full_name=None, inferred_obj_type=None, context=("caller_fn", None, 1))` — [`L28`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L28)
- `resolve(call_dict, local_names=None, local_imports=None, imports_map=None, skip_external=False)` — [`L42`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L42)

## Module values
- `CALLER` — [`L39`](../../../../../../../raw/code/codegraphcontext/tests/unit/tools/test_calls_resolution_tiers.py#L39)

