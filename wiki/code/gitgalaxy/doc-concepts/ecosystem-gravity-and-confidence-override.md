---
title: Ecosystem Gravity — from collision resolution to a trusted confidence override
type: doc-concept
provenance: doc
source: docs/wiki/02-05-language-lens.md
updated: 2026-07-04
status: fresh
---
# Ecosystem Gravity — from collision resolution to a trusted confidence override

## Definition
"Ecosystem Gravity" is a two-stage mechanism spanning two pipeline phases, described across
two docs. First, the Language Lens's Tier 1.5 lock resolves highly contested extensions
(`.h`, `.m`) by surveying the surrounding directory — and, if inconclusive, the whole
repository — for the dominant implementation language, computing three masses: **Base Mass**
(ordinary supporting extensions), **Discriminator Mass** (highly specific proof files like
`CMakeLists.txt`, weighted 2x), and **Toxic Mass** (disqualifying extensions that trigger
"Thermodynamic collapse," zeroing the score outright). A candidate must clear a 70% dominance
ratio globally (60% if the local folder alone is decisive) to win the lock. Second, the
Detector's own "Ecosystem Gravity Override" *trusts* that upstream lock: if the Lens
previously placed a file in the `c`/`cpp`/`objective-c` orbit, the Detector force-sets parsing
confidence to `1.0`, specifically so pure-macro C/C++ headers — which naturally contain no
braces, loops, or branches — don't fall below the Detector's own `0.42` structural-confidence
floor and vanish into "Dark Matter" unparsed.

## In gitgalaxy (grounded)
Both halves are real, and the numbers in the doc match the pinned source exactly:
- **Collision resolution.** [`_evaluate_ecosystem_gravity`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector._evaluate_ecosystem_gravity)
  computes `base_mass`, a `discrim_mass` scaled by exactly `2.0`, and a `toxic_mass` that zeroes
  the score to `0.0` ("Collapsed") if any disqualifying extension is present. The dominance
  threshold is read from [`thresholds`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.thresholds)
  (`ECOSYSTEM_DOMINANCE_MIN`, defaulting to `0.70`) for the global pass, with a hardcoded
  `0.60` floor for a Local-folder-only win — precisely the 70%/60% split the doc describes.
- **The Detector's override.** Inside [`splice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.splice),
  the very first lines read the file's [`primary_lang_id`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.primary_lang_id):
  "if `self.primary_lang_id in ["c", "cpp", "objective-c"]: confidence = 1.0" — executed
  *before* the `0.42`-floor bypass check that would otherwise relegate the file to an empty,
  unparsed result. The pinned source's own comment names this exactly: "THE ECOSYSTEM GRAVITY
  OVERRIDE ... This prevents pure-macro headers from falling below the 0.42 floor and
  vanishing into Unparsable Artifacts."

## Why it matters / when it applies
This is a concrete example of trust propagating *between* two independently-heuristic stages
rather than each stage re-deriving certainty from scratch: the Detector does not re-run its
own language confidence math for a `.h` file — it defers entirely to whatever the Lens already
decided at Tier 1.5, on the reasoning that ecosystem-level evidence (every sibling file in the
folder is C++) is *more* trustworthy for this narrow case than the Detector's own structural
signal (a macro-only header has no structure to find). It is also a place the two docs
describe the same design decision with slightly different emphasis — 02-05 frames it from the
Lens's collision-resolution side, 02-08 frames it from the Detector's confidence-floor side —
and reading both together is what makes the full data flow legible.

## Connections
- Code concepts: [Language lens](../concepts/gitgalaxy-standards-language_lens.md) — produces
  the ecosystem-gravity lock this override consumes; [The Detector](../concepts/gitgalaxy-core-detector.md) —
  where the override is spent, in `splice`'s "Confidence and format gate" mechanism step.
- Module catalogs: [language_lens](../catalog/gitgalaxy/standards/language_lens.md),
  [detector](../catalog/gitgalaxy/core/detector.md).
- Related doc-concepts: [language-lens-bayesian-trust-tiers](language-lens-bayesian-trust-tiers.md),
  [polyglot-handshake-detection](polyglot-handshake-detection.md).

## Source
Extracted from `docs/wiki/02-05-language-lens.md` and `docs/wiki/02-08-the-detector.md`
(the "Ecosystem Gravity Override" section), both kept in place. Note: at the pinned commit,
`docs/wiki/02-07-the-prism.md` contains an earlier, near-duplicate draft of the Detector
content found in `02-08-the-detector.md` — despite its filename, it documents the Detector,
not the Prism (`gitgalaxy/core/prism.py`). This doc-concept draws the Ecosystem Gravity
Override material from whichever of the two carries it; see
[atomic-literal-shield](atomic-literal-shield.md)'s Source section for the same note.
