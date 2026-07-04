---
title: Language standards — the regex grammar substituting for a parser
type: concept
provenance: mixed
concept: gitgalaxy-standards-language_standards
concepts: [multi-language-extraction]
updated: 2026-07-04
status: fresh
---
# Language standards — the regex grammar substituting for a parser

## Overview
This module is the actual "grammar" GitGalaxy uses instead of a parser: 57 hand-authored
per-language dictionaries under [`LANGUAGE_DEFINITIONS`](../catalog/gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS),
each mapping ~50-90 fixed, named "signal" slots (`branch`, `args`, `func_start`,
`class_start`, `safety`, `io`, `api`, `state_mutation`, …) to a compiled regex, plus shared
cross-language infrastructure ([`LENS_CONFIG`](../catalog/gitgalaxy/standards/language_standards.md#LENS_CONFIG))
used by every language's classification, and multilingual technical-debt patterns wired
into most (43 of 57) language definitions — the pure markup/data/IR entries (`json`,
`xml`, `markdown`, `csv`, and similar) skip them. Because there is no
compiler to check this "grammar" against, correctness here is an empirical property proven
by an extensive positive/negative/pathological test matrix and a dedicated ReDoS fuzzer,
not a formal one derived from parsing theory.

## Diagram
```mermaid
flowchart TD
    LD["LANGUAGE_DEFINITIONS (57 languages)"] --> C["\"c\": {extensions, shebangs,\nlexical_family, rules{...}}"]
    C --> FUNC["rules.func_start (ReDoS-hardened)"]
    LD -->|"rules.planned_debt ="| PD[GLOBAL_PLANNED_DEBT]
    LD -->|"rules.fragile_debt ="| FD[GLOBAL_FRAGILE_DEBT]
    LC[LENS_CONFIG] --> HR[HANDSHAKE_REGISTRY]
    LC --> DQ[DISQUALIFIERS]
    LC --> CF[COLLISION_FREQUENCIES]
    LC --> PA[PROSE_ANCHORS]
    LC --> TH[thresholds]
    HR -->|"compiled independently by"| DETECTOR["LanguageDetector.HANDSHAKE_REGISTRY"]
    HR -->|"compiled independently by"| PRISM["Prism.EMBEDDED_TRIGGERS + EMBEDDED_LOOKAHEAD_LIMIT"]
    LD --> M1["vault_sentinel.main"]
    LD --> M2["binary_anomaly_detector.main / run_xray_audit"]
    LD --> M3["sbom_generator.main"]
    LD --> M4["galaxyscope.main"]
```

## Design rationale (why it's built this way)
**Explicitly framed as rules, not a grammar.** The module's own header docstring says it
plainly: "This file contains the compiled regular expressions, mechanical delimiters, and
language-specific rules used to physically slice, parse, and identify source code across
the repository." There is no notion of a production rule that must fully derive a valid
program, or a parse that fails cleanly on invalid input — only a fixed vocabulary of named
regex signals that each language populates (or leaves `None`, e.g. Python's `macros` slot,
since Python has no C-style preprocessor).

**Adversarial engineering against ReDoS is a recurring, hand-repeated idiom.** The C
`func_start` rule carries an inline
comment block titled "THE REDOS IRON WALL," and its `args` rule documents a specific
mitigation ("the 1-Level Nesting Trick," replacing a naive `[^)]*` with
`(?:[^)(]+|\([^)]*\))*`) for function-pointer parameters. The same defensive pattern recurs
per-language: [`test_c_knr_ambiguity_trap`](../catalog/tests/core_engine/test_language_standards_strict.md#test_c_knr_ambiguity_trap)
proves "the C/C++ function spawner does not spiral into a 32,768-permutation death loop"
on legacy K&R-style declarations; [`test_csharp_iron_wall_redos`](../catalog/tests/core_engine/test_language_standards_strict.md#test_csharp_iron_wall_redos)
proves the C# equivalent "survives pathologically massive nested return types... without
triggering overlapping whitespace ReDoS"; [`test_cpp_macro_multiline_spiral`](../catalog/tests/core_engine/test_language_standards_strict.md#test_cpp_macro_multiline_spiral)
proves the C++ function spawner skips a thousand macro lines rather than scanning across
them; and [`test_c_pointer_ambiguity_overlap`](../catalog/tests/core_engine/test_language_standards_strict.md#test_c_pointer_ambiguity_overlap)
proves the pointer-depth alternation stays O(1) on 200 repeated `*` characters. None of this
is proven once at the regex-engine level — it is proven per-rule, per-language, by feeding
each pattern a specific pathological string.

**A grammar rule with no AST becomes a literal character count.** COBOL's fixed-column
format (column 7 is the "indicator area" for a comment) has no parser to consult, so the
rule is a regex that counts characters directly: `_line_anchor` is `^.{6}[*/dD]`.
[`test_cobol_ghost_satellite_prevention`](../catalog/tests/core_engine/test_language_standards_strict.md#test_cobol_ghost_satellite_prevention)
proves this column-awareness matters in practice — an indented SQL column reference or a
`01`-level data definition must *not* be hallucinated as an executable paragraph, which a
naive keyword-only regex would risk.

**One shared multilingual regex, not one per programming language.** [`GLOBAL_PLANNED_DEBT`](../catalog/gitgalaxy/standards/language_standards.md#GLOBAL_PLANNED_DEBT)
and [`GLOBAL_FRAGILE_DEBT`](../catalog/gitgalaxy/standards/language_standards.md#GLOBAL_FRAGILE_DEBT)
are each assigned directly into 43 of the 57 languages' `planned_debt`/`fragile_debt` rule
slots — the 14 pure markup/data/IR entries (`json`, `xml`, `markdown`, `csv`, `pbtxt`,
`mlir`, `proto`, `hlo`, `td`, `plaintext`, `glsl`, `nix`, `blp`, `batch`) have no `rules`
entry for either slot, since debt-comment tracking doesn't apply to formats with no
inline-comment convention of their own.
Their source constants ([`_SPACED_PLANNED`](../catalog/gitgalaxy/standards/language_standards.md#_SPACED_PLANNED)/[`_SPACED_FRAGILE`](../catalog/gitgalaxy/standards/language_standards.md#_SPACED_FRAGILE)
for Latin-script keywords across English, Spanish, Portuguese, French, German, Russian,
Italian, Polish, Dutch, and Indonesian; [`_DENSE_PLANNED`](../catalog/gitgalaxy/standards/language_standards.md#_DENSE_PLANNED)/[`_DENSE_FRAGILE`](../catalog/gitgalaxy/standards/language_standards.md#_DENSE_FRAGILE)
for Mandarin, Japanese, Korean, Hindi, and Arabic) show the "grammar" here generalizes
across *human* languages of code comments, not just programming-language syntax — something
a compiler-grade AST parser, which only needs to understand its one target language's
grammar, has no equivalent obligation to do.

**Operator collisions get their own regression tests, not just their own rules.** [`test_thermodynamic_operator_collisions`](../catalog/tests/core_engine/test_language_standards_strict.md#test_thermodynamic_operator_collisions)
"proves that common language operators (`<<`, `|`, `&`, `!`) do not trigger false positives
in the wrong metric categories" — C++'s bitwise-ops regex must not fire on `std::cout <<`,
Rust's must not fire on a closure's `|a|`, and TypeScript's `test` metric must not fire on
`regex.test(...)`. Every one of these is a case where the same character sequence is
meaningful in one grammar slot and noise in another, resolvable only by hand-tuning the
regex, never by a shared abstract syntax.

## Entry points
- [`LANGUAGE_DEFINITIONS`](../catalog/gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS) —
  the table itself; every consumer across this survey's GitGalaxy pages (the language lens,
  the structural extractor, Prism) receives it via constructor injection rather than
  importing it independently.
- [`main`](../catalog/gitgalaxy/tools/supply_chain_security/vault_sentinel.md#main),
  [`main`](../catalog/gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.md#main),
  [`main`](../catalog/gitgalaxy/tools/compliance/sbom_generator.md#main), and
  [`main`](../catalog/gitgalaxy/galaxyscope.md#main) — four independently runnable CLIs, each
  constructing its own filter/detector from this same table; it is a shared foundation for
  the whole toolset, not private to the full pipeline.
- [`run_xray_audit`](../catalog/gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.md#run_xray_audit) —
  a programmatic (non-CLI) entry point built on the same table, for GalaxyScope's own Phase
  10 ecosystem audits.

## Mechanism (step-by-step)
1. **Shared physics constants assemble first.** [`LENS_CONFIG`](../catalog/gitgalaxy/standards/language_standards.md#LENS_CONFIG)
   collects the cross-language tuning tables consumed by the language lens:
   [`COLLISION_FREQUENCIES`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.COLLISION_FREQUENCIES)
   (extensions needing disambiguation), [`PROSE_ANCHORS`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.PROSE_ANCHORS),
   [`DISQUALIFIERS`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.DISQUALIFIERS)
   (per-lexical-family negative regexes), [`HANDSHAKE_REGISTRY`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.HANDSHAKE_REGISTRY)
   (embedded-language triggers), and [`thresholds`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.thresholds)
   (the confidence-tier knobs documented on the language-lens page).
2. **The multilingual debt regexes compile once and fan out to most languages.** [`GLOBAL_PLANNED_DEBT`](../catalog/gitgalaxy/standards/language_standards.md#GLOBAL_PLANNED_DEBT)
   and [`GLOBAL_FRAGILE_DEBT`](../catalog/gitgalaxy/standards/language_standards.md#GLOBAL_FRAGILE_DEBT)
   are built once from [`_SPACED_PLANNED`](../catalog/gitgalaxy/standards/language_standards.md#_SPACED_PLANNED)/[`_DENSE_PLANNED`](../catalog/gitgalaxy/standards/language_standards.md#_DENSE_PLANNED)
   and [`_SPACED_FRAGILE`](../catalog/gitgalaxy/standards/language_standards.md#_SPACED_FRAGILE)/[`_DENSE_FRAGILE`](../catalog/gitgalaxy/standards/language_standards.md#_DENSE_FRAGILE),
   then assigned by reference into 43 of the 57 languages' `rules["planned_debt"]`/`rules["fragile_debt"]`
   slots (the 14 markup/data/IR-only entries opt out entirely) — a single edit updates the
   debt-marker vocabulary everywhere those slots are wired.
3. **Each language is a self-contained, versioned spec.** Every entry in [`LANGUAGE_DEFINITIONS`](../catalog/gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS)
   (Python, JavaScript, TypeScript, Java, C#, Go, Rust, C++, C, PHP, PowerShell, Shell, Ruby,
   Swift, Kotlin, SQL, HTML, CSS, Fortran, Assembly, Lua, Perl, Haskell, COBOL, and 30+ more,
   through niche entries like `mlir`, `hlo`, and `agc_assembly`) carries its own extensions,
   exact-match filenames, sibling discriminators, shebangs, `lexical_family`, and its own
   `_meta` block (`target_version`, `last_updated`, `blueprint_version`, `status`) —
   independently maintainable, unlike productions in a single unified grammar.
4. **The `rules` dict is the actual signal vocabulary.** Across the 43 languages that carry
   a full behavioral rule set, the same named slots recur (`branch`, `args`, `func_start`,
   `class_start`, `safety`, `safety_bypasses`, `high_risk_execution`, `io`, `api`,
   `state_mutation`, `dead_code`, `doc`, `test`, `concurrency`, `reflection_metaprogramming`,
   `import`, and the two slots this file itself supplies content for — `planned_debt` (always
   [`GLOBAL_PLANNED_DEBT`](../catalog/gitgalaxy/standards/language_standards.md#GLOBAL_PLANNED_DEBT))
   and `fragile_debt` (always [`GLOBAL_FRAGILE_DEBT`](../catalog/gitgalaxy/standards/language_standards.md#GLOBAL_FRAGILE_DEBT)))
   — so that the fixed-position signal vector documented on the analysis-lens page means the
   same thing whether it came from a Python file or a COBOL one — this positional
   consistency is what lets one downstream risk model score every *code* language uniformly.
   (The remaining 14 entries are markup/data/IR formats — `json`, `xml`, `markdown`, `csv`,
   and similar — with no `branch`/`func_start`/etc. slots at all, since there's no control
   flow or functions to detect.)
5. **Two engines compile the same handshake table for two different jobs.** The
   [`HANDSHAKE_REGISTRY`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.HANDSHAKE_REGISTRY)
   entries in [`LENS_CONFIG`](../catalog/gitgalaxy/standards/language_standards.md#LENS_CONFIG)
   get compiled independently into the language lens's own registry for embedded-language
   *classification* (`lang_mix`), and separately into [`EMBEDDED_TRIGGERS`](../catalog/gitgalaxy/core/prism.md#Prism.EMBEDDED_TRIGGERS)
   (bounded by [`EMBEDDED_LOOKAHEAD_LIMIT`](../catalog/gitgalaxy/core/prism.md#Prism.EMBEDDED_LOOKAHEAD_LIMIT),
   which mirrors [`HANDSHAKE_LOOKAHEAD_LIMIT`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.HANDSHAKE_LOOKAHEAD_LIMIT))
   for stream *splitting* — one source table, two independently compiled runtime copies.
6. **Correctness is fuzzed, not proven.** [`test_production_regex_redos_immunity`](../catalog/tests/security_auditing/test_redos_poison.md#TestProductionRegexSecurity.test_production_regex_redos_immunity)
   extracts every compiled regex out of [`LANGUAGE_DEFINITIONS`](../catalog/gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS)
   and fuzzes each one with adversarial input across an 8-worker multiprocessing pool with a
   stall-based kill switch, while [`test_global_regex_syntax_integrity`](../catalog/tests/core_engine/test_language_standards_strict.md#test_global_regex_syntax_integrity)
   is a much simpler sanity pass proving every rule in every language still compiles at all.
   Alongside these, three-way positive/negative/pathological suites — [`test_positive_function_extraction`](../catalog/tests/extraction/test_function_extraction_strict.md#TestFunctionExtraction.test_positive_function_extraction)/[`test_negative_function_extraction`](../catalog/tests/extraction/test_function_extraction_strict.md#TestFunctionExtraction.test_negative_function_extraction)/[`test_pathological_function_extraction`](../catalog/tests/extraction/test_function_extraction_strict.md#TestFunctionExtraction.test_pathological_function_extraction),
   and their `args`/`class`/`dependency` counterparts ([`test_positive_args_extraction`](../catalog/tests/extraction/test_args_extraction_strict.md#TestArgsExtraction.test_positive_args_extraction)/[`test_negative_args_extraction`](../catalog/tests/extraction/test_args_extraction_strict.md#TestArgsExtraction.test_negative_args_extraction)/[`test_pathological_args_extraction`](../catalog/tests/extraction/test_args_extraction_strict.md#TestArgsExtraction.test_pathological_args_extraction),
   [`test_positive_class_extraction`](../catalog/tests/extraction/test_class_extraction_strict.md#TestClassExtraction.test_positive_class_extraction)/[`test_negative_class_extraction`](../catalog/tests/extraction/test_class_extraction_strict.md#TestClassExtraction.test_negative_class_extraction)/[`test_pathological_class_extraction`](../catalog/tests/extraction/test_class_extraction_strict.md#TestClassExtraction.test_pathological_class_extraction),
   [`test_positive_dependency_extraction`](../catalog/tests/extraction/test_dependency_extraction_strict.md#TestDependencyExtraction.test_positive_dependency_extraction)/[`test_negative_dependency_extraction`](../catalog/tests/extraction/test_dependency_extraction_strict.md#TestDependencyExtraction.test_negative_dependency_extraction)/[`test_pathological_dependency_extraction`](../catalog/tests/extraction/test_dependency_extraction_strict.md#TestDependencyExtraction.test_pathological_dependency_extraction) —
   run parametrized across every language ID, each asserting either a real construct is
   caught, a structural lookalike is rejected ("GHOST … HALLUCINATED" assertions), or a
   deliberately mangled input still extracts cleanly.

## Key data structures
- [`LANGUAGE_DEFINITIONS`](../catalog/gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS) —
  57 top-level language entries (verified directly against the source file); each is
  `extensions`/`exact_matches`/`discriminators`/`internal_discriminator`/`shebangs`/`lexical_family`/`rules`.
- [`LENS_CONFIG`](../catalog/gitgalaxy/standards/language_standards.md#LENS_CONFIG) — the
  cross-language constants consumed by the classifier documented on the language-lens page.
- [`GLOBAL_PLANNED_DEBT`](../catalog/gitgalaxy/standards/language_standards.md#GLOBAL_PLANNED_DEBT)/[`GLOBAL_FRAGILE_DEBT`](../catalog/gitgalaxy/standards/language_standards.md#GLOBAL_FRAGILE_DEBT) —
  the shared multilingual TODO/FIXME regexes, built from the four private
  [`_SPACED_PLANNED`](../catalog/gitgalaxy/standards/language_standards.md#_SPACED_PLANNED)/[`_DENSE_PLANNED`](../catalog/gitgalaxy/standards/language_standards.md#_DENSE_PLANNED)/[`_SPACED_FRAGILE`](../catalog/gitgalaxy/standards/language_standards.md#_SPACED_FRAGILE)/[`_DENSE_FRAGILE`](../catalog/gitgalaxy/standards/language_standards.md#_DENSE_FRAGILE)
  string constants.
- [`HANDSHAKE_REGISTRY`](../catalog/gitgalaxy/standards/language_lens.md#LanguageDetector.HANDSHAKE_REGISTRY) /
  [`EMBEDDED_TRIGGERS`](../catalog/gitgalaxy/core/prism.md#Prism.EMBEDDED_TRIGGERS) — the two
  independently compiled copies of the same source list of embedded-language triggers, each
  bounded by its own lookahead-limit constant ([`HANDSHAKE_LOOKAHEAD_LIMIT`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.HANDSHAKE_LOOKAHEAD_LIMIT),
  [`EMBEDDED_LOOKAHEAD_LIMIT`](../catalog/gitgalaxy/core/prism.md#Prism.EMBEDDED_LOOKAHEAD_LIMIT)).

## Dynamics (design intent)
[`test_production_regex_redos_immunity`](../catalog/tests/security_auditing/test_redos_poison.md#TestProductionRegexSecurity.test_production_regex_redos_immunity)'s
docstring states its goal directly: "Extracts every single regex from the production
standards and blasts them with ReDoS payloads. Uses an 8-core isolated multiprocessing pool
to reduce overhead from 80 seconds down to ~0.5 seconds" — the linear-time claim this
survey's lens highlights ("gives up AST precision... gets in exchange linear-time") is
enforced here by a runtime fuzz-and-timeout harness over every one of the 1,200+ compiled
regexes, not by any static guarantee from the regex engine itself.

## Edge cases
- **A grammar rule that is purely positional.** COBOL's `_line_anchor` regex encodes "column
  7 is the comment indicator" as a literal 6-character skip; [`test_cobol_ghost_satellite_prevention`](../catalog/tests/core_engine/test_language_standards_strict.md#test_cobol_ghost_satellite_prevention)
  proves this prevents SQL/data-division lines from being hallucinated as executable
  paragraphs.
- **Shared operators, different meaning per language.** [`test_thermodynamic_operator_collisions`](../catalog/tests/core_engine/test_language_standards_strict.md#test_thermodynamic_operator_collisions)
  proves C++'s bitwise regex ignores `std::cout <<`, Rust's ignores closure pipes, and
  TypeScript's `test` metric ignores `regex.test(...)` calls — each a hand-tuned exception,
  not a shared parse rule.
- **Pathological but syntactically real code must still extract.** The `pathological` half
  of every extraction test triplet (e.g. [`test_pathological_class_extraction`](../catalog/tests/extraction/test_class_extraction_strict.md#TestClassExtraction.test_pathological_class_extraction))
  proves the regexes survive "Frankenstein" formatting — vertical newlines, decorator
  stacking, inheritance chains — without either crashing or silently missing the construct.

## Open questions
- Given [`LANGUAGE_DEFINITIONS`](../catalog/gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS)'s
  real size (over 10,000 lines, 57 languages), this page grounds its claims in the shared
  infrastructure plus the C and COBOL entries read directly; the individual rule sets for
  the other 50+ languages are not catalogued symbol-by-symbol here.
- [`HANDSHAKE_LOOKAHEAD_LIMIT`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.HANDSHAKE_LOOKAHEAD_LIMIT)
  and [`EMBEDDED_LOOKAHEAD_LIMIT`](../catalog/gitgalaxy/core/prism.md#Prism.EMBEDDED_LOOKAHEAD_LIMIT)
  both default to the same 50,000-character value sourced from [`LENS_CONFIG`](../catalog/gitgalaxy/standards/language_standards.md#LENS_CONFIG)'s
  `THRESHOLDS`, but are three separately-named constants on three different classes rather
  than one shared reference; whether that duplication is deliberate (so each engine can be
  re-tuned independently later) is not evident from the source read for this page.

## See also
- [GalaxyScope language lens](gitgalaxy-standards-language_lens.md) — the classifier that
  dispatches into this table's per-language rules.
- [GalaxyScope analysis lens](gitgalaxy-standards-analysis_lens.md) — the schemas and
  thresholds that give the `rules` dict's named slots (like `planned_debt`) their downstream
  risk meaning.
- [GalaxyScope orchestrator](gitgalaxy-galaxyscope.md) — where `LANGUAGE_DEFINITIONS` is
  loaded once and threaded through every worker process.
