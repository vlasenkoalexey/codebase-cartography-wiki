---
title: 'Module: gitgalaxy/standards/language_lens.py'
type: catalog
provenance: extracted
module: gitgalaxy/standards/language_lens.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.standards.language_lens`/
symbols:
  LanguageDetector.inspect: LanguageDetector#inspect().
  LanguageDetector.logger: LanguageDetector#logger.
  LanguageDetector.HANDSHAKE_REGISTRY: LanguageDetector#HANDSHAKE_REGISTRY.
  LanguageDetector.thresholds: LanguageDetector#thresholds.
  LanguageDetector._forge_result: LanguageDetector#_forge_result().
  LanguageDetector.languages: LanguageDetector#languages.
  LanguageDetector._tier_3_lexical_scan: LanguageDetector#_tier_3_lexical_scan().
  LanguageDetector._tier_4_heuristic_discovery: LanguageDetector#_tier_4_heuristic_discovery().
  LanguageDetector.anchor_map: LanguageDetector#anchor_map.
  LanguageDetector.DISQUALIFIERS: LanguageDetector#DISQUALIFIERS.
  LanguageDetector._calibrate_lookup_maps: LanguageDetector#_calibrate_lookup_maps().
  LanguageDetector.COLLISION_FREQUENCIES: LanguageDetector#COLLISION_FREQUENCIES.
  LanguageDetector.extension_map: LanguageDetector#extension_map.
  LanguageDetector._evaluate_ecosystem_gravity: LanguageDetector#_evaluate_ecosystem_gravity().
  LanguageDetector._tier_1_metadata_lock: LanguageDetector#_tier_1_metadata_lock().
  LanguageDetector._detect_hybrids: LanguageDetector#_detect_hybrids().
  LanguageDetector._tier_2_fingerprint_check: LanguageDetector#_tier_2_fingerprint_check().
  LanguageDetector.PROSE_ANCHORS: LanguageDetector#PROSE_ANCHORS.
  LanguageDetector: LanguageDetector#
  LanguageDetector._capture_raw_signal: LanguageDetector#_capture_raw_signal().
  LanguageDetector.focus: LanguageDetector#focus().
  DetectorResult: DetectorResult#
  LanguageDetector._find_balanced_end: LanguageDetector#_find_balanced_end().
  LanguageDetector.lexical_heuristics: LanguageDetector#lexical_heuristics.
  FocusingError: FocusingError#
  DetectorResult.lang_id: DetectorResult#lang_id.
  DetectorResult.intensity: DetectorResult#intensity.
  DetectorResult.family: DetectorResult#family.
  DetectorResult.lock_tier: DetectorResult#lock_tier.
  DetectorResult.source_proof: DetectorResult#source_proof.
  DetectorResult.candidates: DetectorResult#candidates.
  DetectorResult.path: DetectorResult#path.
  DetectorResult.lang_mix: DetectorResult#lang_mix.
  DetectorResult.loc: DetectorResult#loc.
  DetectorResult.size_bytes: DetectorResult#size_bytes.
  DetectorResult.anomaly_flags: DetectorResult#anomaly_flags.
  LanguageDetector.__init__: LanguageDetector#__init__().
---
# Module: [`gitgalaxy/standards/language_lens.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py)

## Classes
### `DetectorResult`  ·  implements/extends _TypedDict
- def: [`gitgalaxy/standards/language_lens.py:26`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L26) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
- doc: Structured classification metadata for the Pipeline Orchestrator.
- signature: `class DetectorResult(TypedDict):`
- members:
  - `anomaly_flags` — [`L39`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L39)
  - `candidates` — [`L34`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L34)
  - `family` — [`L31`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L31)
  - `intensity` — [`L30`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L30)
  - `lang_id` — [`L29`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L29)
  - `lang_mix` — [`L36`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L36)
  - `loc` — [`L37`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L37)
  - `lock_tier` — [`L32`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L32)
  - `path` — [`L35`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L35)
  - `size_bytes` — [`L38`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L38)
  - `source_proof` — [`L33`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L33)
- used by: [`inspect`](language_lens.md#LanguageDetector.inspect), [`_forge_result`](language_lens.md#LanguageDetector._forge_result)

### `FocusingError`  ·  implements/extends Exception
- def: [`gitgalaxy/standards/language_lens.py:42`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L42) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
- doc: Exception raised for I/O or execution failures during linguistic classification.
- signature: `class FocusingError(Exception):`
- used by: [`_capture_raw_signal`](language_lens.md#LanguageDetector._capture_raw_signal)

### `LanguageDetector`
- def: [`gitgalaxy/standards/language_lens.py:48`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L48)
- doc: Linguistic Classification Engine.
- signature: `class LanguageDetector:`
- members:
  - `_calibrate_lookup_maps(self)` — [`L110`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L110) — Builds O(1) dictionaries mapping extensions and exact filenames to languages. — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `_capture_raw_signal(self, file_path: Union[str, Path])` — [`L1018`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L1018) — DEFENSIVE GUARD: Restricts I/O memory allocation to 50KB. — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `_detect_hybrids(self, content: str, primary_id: str)` — [`L1061`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L1061) — Identifies secondary logic streams (like HTML inside PHP files) via syntax handshakes. — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `_evaluate_ecosystem_gravity(self, file_path: Union[str, Path], ext: str, global_tally: Dict[str, int])` — [`L551`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L551) — Resolves identical extension collisions (e.g., .h) by surveying the surrounding — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `_forge_result(self, lang_id: str, intensity: float, tier: int, proof: str, base: DetectorResult, content_sample: str = "")` — [`L989`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L989) — Packs metadata and metrics into the formal classification dictionary structure. — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `_tier_3_lexical_scan(self, content: str, ext: str, claimed_lang: str = "undeterminable", gravity_lang: Optional[str] = None)` — [`L699`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L699) — The Strict Boundary Scanner. — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `_tier_4_heuristic_discovery(self, content: str, coding_loc: int, ext: str = "", gravity_lang: Optional[str] = None)` — [`L788`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L788) — Heuristic Discovery for unknown or extensionless files. — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `focus(self, file_path: Union[str, Path], content_sample: str = "", **kwargs)` — [`L132`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L132) — Legacy Support Gateway for systems expecting the older Tuple return format. — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `inspect(self, file_path: Union[str, Path], content_sample: str = "", has_intent: bool = False, intent_lang: str = "", intent_vector: Optional[Dict[str, Any]] = None, ext_tally: Optional[Dict[str, int]] = None, **kwargs)` — [`L144`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L144) — Primary classification orchestrator combining metadata, context, and lexical analysis. — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `COLLISION_FREQUENCIES` — [`L86`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L86) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `DISQUALIFIERS` — [`L90`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L90) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `HANDSHAKE_REGISTRY` — [`L95`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L95) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `PROSE_ANCHORS` — [`L87`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L87) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `anchor_map` — [`L82`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L82) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `extension_map` — [`L81`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L81) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `languages` — [`L71`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L71) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `lexical_heuristics` — [`L72`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L72) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
  - `logger` — [`L75`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L75)
  - `thresholds` — [`L85`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L85) — documented in [gitgalaxy-standards-language_lens](../../../concepts/gitgalaxy-standards-language_lens.md)
- protocol/private: `__init__`[`L65`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L65), `_find_balanced_end`[`L1031`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L1031), `_tier_1_metadata_lock`[`L659`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L659), `_tier_2_fingerprint_check`[`L672`](../../../../../../raw/code/gitgalaxy/gitgalaxy/standards/language_lens.py#L672)
- uses (calls/refs, reference-scoped): [`LENS_CONFIG`](language_standards.md#LENS_CONFIG), [`DetectorResult`](language_lens.md#DetectorResult), [`EXACT_FILE_MATCH`](gitgalaxy_config.md#EXACT_FILE_MATCH), [`FocusingError`](language_lens.md#FocusingError)
- used by: [`main`](../tools/compliance/sbom_generator.md#main), [`_init_worker`](../galaxyscope.md#_init_worker)  (1 test-only)

