---
title: Empirical validation of heuristic parsing — the adversarial test gauntlets
type: doc-concept
provenance: doc
source: docs/wiki/03-08-claim-8-empirical-validation-of-ast-free-parsing.md
updated: 2026-07-04
status: fresh
---
# Empirical validation of heuristic parsing — the adversarial test gauntlets

## Definition
Because gitgalaxy's regex tables *are* its compiler — there is no independent parser to fall back
on or cross-check against — the doc argues that ordinary unit tests are insufficient proof that
"you cannot reliably parse code with regular expressions" is false in gitgalaxy's specific,
bounded sense. Instead it describes a **3-tier adversarial matrix** every structural rule across
30+ languages must survive: **the Iron Wall** (precision — must isolate exactly the target
identifier, nothing more), **Ghost Prevention** (must return nothing when fed a structural
lookalike — a variable assignment, an instantiation, a control-flow condition — that merely
resembles a definition), and **the Frankenstein Test** (must still extract correctly, in linear
time, from pathologically formatted real-world code).

## In gitgalaxy (grounded)
This is not aspirational — the described test suites exist in the pinned source and their
functions are real, indexed symbols:
- **Ghost Prevention** is exercised by the negative-extraction tests, e.g.
  [`test_negative_function_extraction`](../catalog/tests/extraction/test_function_extraction_strict.md#TestFunctionExtraction.test_negative_function_extraction),
  [`test_negative_class_extraction`](../catalog/tests/extraction/test_class_extraction_strict.md#TestClassExtraction.test_negative_class_extraction),
  [`test_negative_args_extraction`](../catalog/tests/extraction/test_args_extraction_strict.md#TestArgsExtraction.test_negative_args_extraction),
  and [`test_negative_dependency_extraction`](../catalog/tests/extraction/test_dependency_extraction_strict.md#TestDependencyExtraction.test_negative_dependency_extraction) —
  each asserts the corresponding extractor in
  [`StructuralExtractor`](../concepts/gitgalaxy-core-detector.md) returns nothing for a
  structural lookalike.
- **The Frankenstein Test / ReDoS Shield** is exercised by the language-standards gauntlet:
  [`test_csharp_iron_wall_redos`](../catalog/tests/core_engine/test_language_standards_strict.md#test_csharp_iron_wall_redos),
  [`test_c_knr_ambiguity_trap`](../catalog/tests/core_engine/test_language_standards_strict.md#test_c_knr_ambiguity_trap),
  [`test_cpp_macro_multiline_spiral`](../catalog/tests/core_engine/test_language_standards_strict.md#test_cpp_macro_multiline_spiral),
  [`test_cobol_ghost_satellite_prevention`](../catalog/tests/core_engine/test_language_standards_strict.md#test_cobol_ghost_satellite_prevention),
  and [`test_global_regex_syntax_integrity`](../catalog/tests/core_engine/test_language_standards_strict.md#test_global_regex_syntax_integrity),
  plus [`test_detector_anti_redos_line_limiter`](../catalog/tests/core_engine/test_detector.md#test_detector_anti_redos_line_limiter)
  at the Detector level.
- **Bounded lookaheads** — the doc's mechanism for avoiding catastrophic backtracking — are a real,
  named constant on the hot path, not just a claim:
  [`StructuralExtractor.HANDSHAKE_LOOKAHEAD_LIMIT`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.HANDSHAKE_LOOKAHEAD_LIMIT)
  (50,000 chars) caps how far a keyword-mode search scans forward, and
  [`Prism.EMBEDDED_LOOKAHEAD_LIMIT`](../catalog/gitgalaxy/core/prism.md#Prism.EMBEDDED_LOOKAHEAD_LIMIT)
  does the analogous job for embedded-language detection in the comment/code splitter.

## Why it matters / when it applies
This is the honest answer to "how do you trust a citation-free, compiler-free parser": gitgalaxy
substitutes a *test-driven* proof (thousands of adversarial fixtures per language, fuzzed for
ReDoS) for the *structural* proof a real grammar/compiler would give you. It is a genuinely
different trust model from the other tools in this survey — wikify-repo's citation linter proves
every wiki claim resolves to a real SCIP symbol; gitgalaxy's gauntlets instead prove its
*extractors* behave correctly against known-hard inputs, with no independent oracle checking that
the extracted `FunctionNode` list matches ground truth on arbitrary unseen code. A rule that passes
every gauntlet can still misfire on a pattern nobody thought to write a fixture for — the tradeoff
[ast-vs-heuristic-tradeoffs](ast-vs-heuristic-tradeoffs.md) names directly ("bounded lookaheads to
prevent 99% of hallucinations, but it is not infallible").

## Connections
- Code concepts: [The Detector](../concepts/gitgalaxy-core-detector.md) — the extractor these
  gauntlets validate; [The Prism](../concepts/gitgalaxy-core-prism.md) — shares the same
  lookahead-bounding discipline; [Language standards](../concepts/gitgalaxy-standards-language_standards.md) —
  "correctness here is an empirical property proven by an extensive test matrix... not a formal one
  derived from parsing theory," exactly the claim this doc makes explicit.
- Module catalogs: [detector](../catalog/gitgalaxy/core/detector.md), [prism](../catalog/gitgalaxy/core/prism.md),
  [test_language_standards_strict](../catalog/tests/core_engine/test_language_standards_strict.md).
- Related doc-concepts: [blast-paradigm](blast-paradigm.md), [ast-vs-heuristic-tradeoffs](ast-vs-heuristic-tradeoffs.md).

## Source
Extracted from `docs/wiki/03-08-claim-8-empirical-validation-of-ast-free-parsing.md`, kept in place.
