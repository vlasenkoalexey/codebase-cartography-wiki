---
title: 'Module: tests/core_engine/test_language_lens.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_language_lens.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_language_lens`/
symbols:
  isolated_detector: isolated_detector().
  test_language_lens_god_mode_reload_sweep: test_language_lens_god_mode_reload_sweep().
  test_identity_conflict_trap: test_identity_conflict_trap().
  test_tier_0_absolute_consensus: test_tier_0_absolute_consensus().
  test_ecosystem_consensus_collision: test_ecosystem_consensus_collision().
  test_tier_3_lexical_scan: test_tier_3_lexical_scan().
  test_tier_4_heuristic_discovery: test_tier_4_heuristic_discovery().
  test_hybrid_language_detection: test_hybrid_language_detection().
  test_prose_and_metadata_anchors: test_prose_and_metadata_anchors().
  test_focusing_error_hardware_failure: test_focusing_error_hardware_failure().
  test_safe_wrapper_stripping: test_safe_wrapper_stripping().
  test_local_ecosystem_consensus_and_toxic_pruning: test_local_ecosystem_consensus_and_toxic_pruning().
  test_legacy_focus_gateway: test_legacy_focus_gateway().
  test_hybrid_string_ignorance: test_hybrid_string_ignorance().
  test_tier_4_macro_and_handicaps: test_tier_4_macro_and_handicaps().
  test_empty_file_survival: test_empty_file_survival().
  test_regex_hallucination_clamp: test_regex_hallucination_clamp().
  test_corrupted_intent_vector_survival: test_corrupted_intent_vector_survival().
---
# Module: [`tests/core_engine/test_language_lens.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py)

## Functions
- `isolated_detector()` — [`L41`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L41) — Creates a fully isolated LanguageDetector that does NOT rely on your live — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
- `test_corrupted_intent_vector_survival(isolated_detector)` — [`L419`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L419) — Proves the engine gracefully ignores malformed Bayesian priors passed down
- `test_ecosystem_consensus_collision(isolated_detector)` — [`L155`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L155) — Proves the engine uses surrounding repo mass to resolve contested extensions.
- `test_empty_file_survival(isolated_detector, tmp_path)` — [`L378`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L378) — Proves the engine handles 0-byte files by safely defaulting to the
- `test_focusing_error_hardware_failure(mock_open, isolated_detector)` — [`L246`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L246) — Proves the engine safely raises a FocusingError if the OS locks the file.
- `test_hybrid_language_detection(isolated_detector)` — [`L212`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L212) — Proves the Handshake Registry can identify injected scripts.
- `test_hybrid_string_ignorance(isolated_detector)` — [`L327`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L327) — Proves the balanced end finder does not trip on triggers inside strings.
- `test_identity_conflict_trap(isolated_detector)` — [`L122`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L122) — Proves the engine catches files lying about their identity.
- `test_language_lens_god_mode_reload_sweep()` — [`L13`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L13) — Restored from your original file: Forces the Python interpreter to completely
- `test_legacy_focus_gateway(isolated_detector)` — [`L314`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L314) — Proves the legacy wrapper yields 'plaintext' for low-signal files.
- `test_local_ecosystem_consensus_and_toxic_pruning(mock_iterdir, isolated_detector)` — [`L283`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L283) — Proves the engine calculates local folder mass and applies toxic constraints.
- `test_prose_and_metadata_anchors(isolated_detector)` — [`L232`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L232) — Proves specific filenames bypass standard code physics.
- `test_regex_hallucination_clamp(isolated_detector)` — [`L397`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L397) — Proves the anti-hallucination shield works. The engine is tuned to prefer
- `test_safe_wrapper_stripping(isolated_detector)` — [`L261`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L261) — Proves the engine strips .template / .bak wrappers to find the true extension.
- `test_tier_0_absolute_consensus(isolated_detector)` — [`L141`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L141) — Proves absolute certainty when Extension and Shebang agree.
- `test_tier_3_lexical_scan(isolated_detector)` — [`L175`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L175) — Proves the fallback syntax verification works when ecosystem consensus is missing.
- `test_tier_4_heuristic_discovery(isolated_detector)` — [`L193`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L193) — Proves the engine can blindly identify a file with no extension.
- `test_tier_4_macro_and_handicaps(mock_time, isolated_detector)` — [`L344`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_lens.py#L344) — Proves C-family macros provide a density boost, and ABAP gets handicapped.

