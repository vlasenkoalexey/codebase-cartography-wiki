---
title: The Detector — StructuralExtractor and the five AST-free "integration modes"
type: concept
provenance: mixed
concept: gitgalaxy-core-detector
concepts: [multi-language-extraction, symbol-graph]
updated: 2026-07-04
status: fresh
---
# The Detector — StructuralExtractor and the five AST-free "integration modes"

## Overview
[`StructuralExtractor`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor) is the piece of
GitGalaxy that turns a language-tagged, already-split code/comment text stream into a list of
function-level records (`FunctionNode`) and file-level signal counts — without ever building a parse
tree. Its one idea: every language's block-scoping convention falls into a small number of families
(braces, indentation, keywords, bare labels, statement terminators), so rather than writing a universal
parser, [`splice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.splice) hands each segment
to [`_function_slice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._function_slice), a
dispatcher that routes it to one of five purpose-built regex/state-machine "integration modes" —
[`_slice_by_labels`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_labels),
[`_slice_by_braces`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_braces),
[`_slice_by_indentation`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_indentation),
[`_slice_by_keywords`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_keywords), and
[`_slice_by_terminator`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_terminator).
Every mode ultimately funnels into the same metrics engine,
[`_calculate_block_metrics`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._calculate_block_metrics),
so a downstream consumer sees one uniform [`FunctionNode`](../catalog/gitgalaxy/core/detector.md#FunctionNode)
regardless of which mode produced it. This is the module the survey's "no grounding substrate" framing is
really about: no compiler, no LLM — five different ways of counting how a stream of text nests, chosen by
looking up the language, not by understanding it.

## Diagram
```mermaid
flowchart TD
    S["splice()"] --> FS["_function_slice — Master Dispatcher"]
    FS -->|"get_mode == mode_d"| SBK["_slice_by_keywords (Mode D)"]
    FS -->|"get_mode == mode_e"| SBT["_slice_by_terminator (Mode E)"]
    FS -->|"lang in asm/cobol/fortran, or column_sensitive family"| SBL["_slice_by_labels (Mode A)"]
    FS -->|"single_line_only/multi_style_dash family, or python/yaml"| SBI["_slice_by_indentation (Mode C)"]
    FS -->|"default"| SBB["_slice_by_braces (Mode B)"]
    SBK -->|"config lookup"| GC["get_config"]
    SBT -->|"config lookup"| GC
    SBK --> ALS["_apply_literal_shield"]
    SBK --> ESN["_extract_semantic_name"]
    SBL --> CBM["_calculate_block_metrics"]
    SBB --> CBM
    SBI --> CBM
    SBK --> CBM
    SBT --> CBM
    CBM --> EN["_extract_name"]
    CBM --> FN["FunctionNode"]
```

## Design rationale (why it's built this way)
[`StructuralExtractor`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor)'s own docstring states
the trade directly: "AST parsers often fail when encountering non-standard syntax, legacy dialects, or
partially-broken codebases," so the class "utilizes Fluid State Counters and O(1) lexical masking to
achieve high-fidelity node extraction at ~100,000 LOC/sec … without requiring fully-compilable source
code." Five modes exist, not one, because the underlying assumption a slicer must make about "where does
a block end" is fundamentally different per language family: C-family and Lisp nest with a single
balanced-delimiter pair (Mode B), Python/YAML nest by whitespace column (Mode C), Ruby/Shell/Lua/Elixir
nest by paired keywords with no delimiter at all (Mode D), SQL/Erlang/Prolog have no nesting, only flat
statements ended by a terminator token (Mode E), and legacy Assembly/COBOL have no scope construct
whatsoever — only labels and a return instruction (Mode A). Trying to cover all five with one regex would
require the regex to encode a different grammar for each, which is exactly the AST it is trying to avoid.

Routing itself is two-tiered by design: [`_function_slice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._function_slice)
first asks a per-language configuration lookup (resolved through
[`get_config`](../catalog/gitgalaxy/core/detector.md#ScopeParsingRegistry.get_config)) whether the
language is explicitly registered for Mode D or Mode E; only if it is not does it fall back to a generic
`lexical_family` tag (assembly/cobol/fortran or a `column_sensitive` family → Mode A;
`single_line_only`/`multi_style_dash` family or `python`/`yaml` → Mode C; everything else → Mode B, the
default). Concretely, this means adding a new keyword-scoped or terminator-scoped language is a
declarative registry entry (an `openers`/`closers` or `terminator`/`igniter` regex list), not new slicing
code — while every other language gets a reasonable default from a family tag with zero code change.
> [!inferred]
> This two-tier design (explicit override, generic family fallback) mirrors the same "precision path,
> guaranteed floor" shape the survey's [multi-language-extraction](../../../concepts/multi-language-extraction.md)
> axis compares across tools, except here both the "precision" and the "floor" are still regex — there is
> no AST fallback anywhere in this pipeline.

Mode B's brace-balance scanner is the one that invests the most defensive engineering, because it is also
the one most exposed to false positives: a stray brace inside a string, a comment, or a `#else {` inside a
dead preprocessor branch will desynchronize a naive depth counter. [`_slice_by_braces`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_braces)
shields string/char/backtick literals and both comment styles with one combined regex before scanning,
and — strictly for C-family languages — runs a small line-by-line state machine that tracks
`#if`/`#elif`/`#else`/`#endif` nesting and blanks out dead branches and multi-line `#define` macros
(backslash continuations) so their raw braces never reach the balance counter.
[`test_detector_mode_b_multiline_macros`](../catalog/tests/core_engine/test_detector.md#test_detector_mode_b_multiline_macros)
and [`test_detector_c_macro_dead_branch_shield`](../catalog/tests/core_engine/test_detector.md#test_detector_c_macro_dead_branch_shield)
pin exactly this behavior.

Mode D's "Ruby/Elixir Inline Modifier Guard" is the sharpest example of how much language-specific
nuance a keyword-based (rather than delimiter-based) scanner needs: `if`, `unless`, `while`, and `until`
are block openers in Ruby *unless* they appear as a trailing statement modifier (`return true if x`), in
which case they open nothing. [`_slice_by_keywords`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_keywords)
resolves this by checking whether the line's safe (literal/comment-shielded) text actually *starts* with
the keyword; if it does not, every modifier match on that line is subtracted back out of the opener count
so it can never falsely deepen the scope stack —
[`test_detector_mode_d_ruby_inline_modifier`](../catalog/tests/core_engine/test_detector.md#test_detector_mode_d_ruby_inline_modifier)
exists specifically to pin this.

Several metrics are explicit, acknowledged approximations rather than ground truth, which matters for the
survey's framing of what this control group gives up: [`_calculate_block_metrics`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._calculate_block_metrics)'s
own docstring calls its Big-O estimate "a 95% accurate proxy" for cyclomatic nesting depth, computed from
indentation rather than from a real AST; recursion is detected by counting whether a function's own name
occurs more than once inside its own body (no argument-binding or call-graph check); and
[`_classify_function`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.splice) (invoked from
`_calculate_block_metrics`, itself reached from every mode underneath `splice`; the classifier itself is
not in this packet's subgraph — see Open questions) falls back
to naming-convention substring matches (`get`/`fetch` → `io`, `set`/`save` → `mutation`, …) whenever no
explicit `@type:`/`@gal_type:` annotation is present, as
[`test_detector_function_classification`](../catalog/tests/core_engine/test_detector.md#test_detector_function_classification)
and [`test_detector_explicit_type_override`](../catalog/tests/core_engine/test_detector.md#test_detector_explicit_type_override)
demonstrate.

## Entry points
- [`splice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.splice) — the single per-file
  entry point. It receives the already-separated `code_stream`/`comment_stream` (produced upstream by the
  Prism), a confidence score, and — when available — the file's `raw_content`, which it snapshots into
  [`raw_content_lines`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.raw_content_lines) for
  later docstring harvesting. Everything else on this page executes underneath a single `splice` call.
- [`_init_worker`](../catalog/gitgalaxy/galaxyscope.md#_init_worker) — how a `StructuralExtractor`
  instance comes to exist at all. Because "Python's Global Interpreter Lock (GIL) prevents true
  multi-threading for CPU-bound tasks," GitGalaxy spawns separate OS worker processes and this
  boot-loader instantiates one extractor per active language *inside* the child's own memory — explicitly
  to avoid having to pickle compiled regex objects across the multiprocessing IPC boundary. `splice` is
  therefore always called on a warm, per-language, per-process singleton, never freshly constructed per
  file.

## Mechanism (step-by-step)
1. **Confidence and format gate.** [`splice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.splice)
   first applies an "Ecosystem Gravity Override": if the primary language is `c`, `cpp`, or `objective-c`,
   confidence is forced to `1.0` regardless of what was passed in, because pure-macro C/C++ headers often
   contain no braces/loops/branches and would otherwise fall below the `0.42` confidence floor and be
   silently dropped. Any file that still lands below `0.42`, or whose language is `plaintext`,
   `markdown`, `json`, `yaml`, or `csv`, returns an empty, zeroed-out result immediately — a deliberate
   bypass rather than an attempt to force a parse.
2. **ReDoS neutralization.** Still inside `splice`, every line longer than 1500 characters (hex arrays,
   `.depend` files, minified blobs) is blanked to a single safe character while its exact length and
   leading indentation are preserved, so line count and column geometry survive but the regex engine
   never has to backtrack across a pathological line.
   [`test_detector_anti_redos_line_limiter`](../catalog/tests/core_engine/test_detector.md#test_detector_anti_redos_line_limiter)
   pins this.
3. **Segment partition and signal pass.** `splice` then partitions the shielded stream into per-language
   segments (so an embedded `<script>` or `asm!()` block is scanned under its own rules) and runs the
   regex signal pass that produces, per segment, a spatial map of exactly where every rule fired.
   [`test_detector_embedded_language_partitioning`](../catalog/tests/core_engine/test_detector.md#test_detector_embedded_language_partitioning)
   confirms the engine "dynamically swaps languages mid-file" when it hits one of these handshakes. The
   partitioner and signal-counting pass are internal to `splice` and are not separately named symbols in
   this packet (see Open questions).
4. **Master dispatch.** [`_function_slice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._function_slice)
   walks each `(lang_id, code, offset)` segment together with its spatial map, asks
   [`get_config`](../catalog/gitgalaxy/core/detector.md#ScopeParsingRegistry.get_config) whether the
   language is registered for Mode D or Mode E, and otherwise falls back to a `lexical_family`-driven
   choice among Modes A/B/C, described in Design rationale above.
5. **Mode A — labels.** [`_slice_by_labels`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_labels)
   greedily takes everything from one label match to the next (or end of file) and then trims the block
   backward to the *last* recognized return-family instruction found inside that window — because
   Assembly/COBOL have no block delimiter, only a linear sequence of labeled instructions.
   [`test_detector_mode_a_labels`](../catalog/tests/core_engine/test_detector.md#test_detector_mode_a_labels)
   pins the greedy-then-trim behavior.
6. **Mode B — braces.** [`_slice_by_braces`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_braces)
   swaps to `()` for `lisp` and otherwise balances `{}`, after shielding literals/comments and (for C-family
   languages only) blanking dead preprocessor branches and multi-line macros so their raw braces cannot
   desynchronize the balance count — see Design rationale for why this mode carries the most shielding.
   [`test_detector_mode_b_lisp_family`](../catalog/tests/core_engine/test_detector.md#test_detector_mode_b_lisp_family)
   confirms the opener/closer swap.
7. **Mode C — indentation.** [`_slice_by_indentation`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_indentation)
   shields strings/comments with an index-preserving mask (every masked character becomes a space or stays
   a newline, so offsets still line up 1:1 with the original text), records the base indent of the
   `def`/`class` line, and scans forward until a non-blank line's indentation drops back to or below that
   base — Python's own grammar makes indentation load-bearing, so this heuristic gets a free, exact scope
   boundary for exactly the one family where it is guaranteed to work.
   [`test_detector_mode_c_indentation`](../catalog/tests/core_engine/test_detector.md#test_detector_mode_c_indentation)
   pins the drop-back-to-base-indent termination.
8. **Mode D — keyword handshake stack.** [`_slice_by_keywords`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_keywords)
   applies [`_apply_literal_shield`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._apply_literal_shield)
   (which additionally handles heredocs and Ruby `%` literals), then walks the file line by line
   maintaining a `stack_depth` counter that increments on opener keywords and decrements on closer
   keywords (both resolved via [`get_config`](../catalog/gitgalaxy/core/detector.md#ScopeParsingRegistry.get_config)),
   naming each captured block with [`_extract_semantic_name`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._extract_semantic_name).
   Top-level lines that never open a scope are swept into a `global_dust` bucket and, if non-empty, emitted
   as one final satellite so module-level logic is never silently dropped —
   [`test_detector_global_dust_and_unterminated`](../catalog/tests/core_engine/test_detector.md#test_detector_global_dust_and_unterminated)
   pins this.
9. **Mode E — terminator cleaving.** [`_slice_by_terminator`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_terminator)
   tracks no nesting at all: it watches for an `igniter` pattern (e.g. `SELECT`/`CREATE` for SQL) to open a
   new "orbit," accumulates lines, and closes the instant a `terminator` token (`;` for SQL, `.` for
   Erlang/Prolog) appears — the simplest mode, because declarative/logic languages have no nested block
   scope at all, only flat statements. Its language configuration also comes from
   [`get_config`](../catalog/gitgalaxy/core/detector.md#ScopeParsingRegistry.get_config).
10. **Uniform metrics.** Every mode's captured block is handed to
    [`_calculate_block_metrics`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._calculate_block_metrics),
    which binary-searches (`bisect`) into the segment's precomputed spatial map to count branch/linear
    hits inside the block's exact character range — an O(log N) range query rather than a second regex
    pass — then derives Big-O depth from indentation, recursion from name-occurrence count, and a magnitude
    score, producing one
    [`FunctionNode`](../catalog/gitgalaxy/core/detector.md#FunctionNode). The block's name itself is
    resolved earlier, by each mode's own caller code, and passed in as a plain parameter: Modes A/B/C
    (labels/braces/indentation) resolve it via [`_extract_name`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._extract_name)'s
    gauntlet of per-language "naming shields" (Objective-C message syntax, C++ operator overloads, C++
    test-macro unwrapping, `::`-preserving truncation) before `_calculate_block_metrics` is ever called,
    while Mode D names its blocks via `_extract_semantic_name` and Mode E derives a name inline from its
    igniter match — `_calculate_block_metrics` itself never calls a name extractor.
    [`test_detector_cpp_objc_name_extraction`](../catalog/tests/core_engine/test_detector.md#test_detector_cpp_objc_name_extraction)
    and [`test_detector_big_o_and_recursion`](../catalog/tests/core_engine/test_detector.md#test_detector_big_o_and_recursion)
    pin these.
11. **Class linkage and orphan detection.** Back in `splice`, a class-declaration regex bounds each class
    from one declaration to the next (or EOF), and every `FunctionNode` whose `start_line` falls inside a
    class's span is linked to it — from which LCOM (lack-of-cohesion) and state-entanglement scores are
    derived purely from argument/mutation counts, no type information required. A separate word-frequency
    pass over the whole file then flags functions whose name occurs nowhere else as orphaned, and
    duplicate-named functions as duplicates. [`test_detector_class_extraction_and_lcom`](../catalog/tests/core_engine/test_detector.md#test_detector_class_extraction_and_lcom)
    and [`test_detector_classification_and_wiring`](../catalog/tests/core_engine/test_detector.md#test_detector_classification_and_wiring)
    pin this.
12. **Auto-heal and token mass.** If a `StructuralExtractor` is constructed for a language absent from its
    injected [`languages`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.languages) registry,
    it re-imports [`LANGUAGE_DEFINITIONS`](../catalog/gitgalaxy/standards/language_standards.md#LANGUAGE_DEFINITIONS)
    directly and re-derives its rules rather than failing —
    [`test_detector_auto_heal_bootloader`](../catalog/tests/core_engine/test_detector.md#test_detector_auto_heal_bootloader)
    pins this. `splice` finally computes [`get_token_mass`](../catalog/gitgalaxy/core/detector.md#get_token_mass)
    over the raw content; if `tiktoken` is not installed this returns `None` rather than `0`, explicitly
    "to prevent dataset poisoning" — [`test_detector_missing_tiktoken_fallback`](../catalog/tests/core_engine/test_detector.md#test_detector_missing_tiktoken_fallback)
    pins the `None`-not-`0` distinction.

## Key data structures
- [`FunctionNode`](../catalog/gitgalaxy/core/detector.md#FunctionNode) — the one output shape every mode
  produces. It carries duplicate-keyed fields on purpose (`branch_count`/`branch`, `args`/`args_count`,
  `structural_weight`/`mag`/`impact`) — a dual-key compatibility shim so older and newer pipeline stages
  can read whichever name they expect — alongside `calls_out_to` (a capped, deduplicated list of
  bare-name invocations found in the block), `hit_vector` (per-rule hit counts local to this function),
  and `token_mass`.
- [`languages`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.languages) /
  [`primary_lang_id`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.primary_lang_id) — the
  per-instance language registry and the language this specific extractor was constructed for; every mode
  method receives `rules`/`lang_id` derived from these rather than re-resolving them per call.
- [`raw_content_lines`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.raw_content_lines) — a
  snapshot of the unshielded original file, refreshed on every `splice` call, that docstring/comment
  harvesting reads by exact line index rather than re-splitting the file per function.
- [`HANDSHAKE_LOOKAHEAD_LIMIT`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.HANDSHAKE_LOOKAHEAD_LIMIT)
  — the 50,000-character cap on how far an embedded-language handshake (e.g. `<script>…</script>`) is
  allowed to search for its closing token, bounding worst-case scan cost on a pathological or unterminated
  embed.

> [!inferred]
> The repo's own `core/README.md` describes a downstream module, `network_risk_sensor.py` (not in this
> packet), that wires files together into a dependency graph using each file's raw imports and the
> `calls_out_to` this page's `FunctionNode` records produce. If that description is accurate, this
> module's per-file class/function linkage and `calls_out_to` lists are the raw node/edge material a
> cross-file call graph is later built from — which is why `symbol-graph` is tagged on this page even
> though the graph itself is assembled elsewhere.

## Dynamics (design intent)
There is no concurrency inside `StructuralExtractor` itself — every mode is a single sequential pass over
its segment. The concurrency story lives one layer up, in
[`_init_worker`](../catalog/gitgalaxy/galaxyscope.md#_init_worker): because the GIL rules out real
multi-threading for this CPU-bound work, GitGalaxy runs one OS process per worker and warms a
`StructuralExtractor` per active language *inside that process's own memory*, specifically so compiled
regex objects never have to cross a multiprocessing pickle boundary. `splice` is consequently always
invoked against a long-lived, per-process, per-language instance — the `MAX_SATELLITES` (250) and
`MAX_DEPTH` (50) clamps that appear across every mode exist because a single pathological file must not be
allowed to balloon the memory or recursion-equivalent cost of that shared worker.

## Edge cases
- Files below the `0.42` confidence floor, or tagged `plaintext`/`markdown`/`json`/`yaml`/`csv`, never
  reach any integration mode at all — they return a fully empty payload from
  [`splice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.splice)'s early bypass.
- A regex rule that raises during the signal pass or the comment pass is caught, logged, and zeroed rather
  than aborting the file — [`test_detector_regex_execution_catch_block`](../catalog/tests/core_engine/test_detector.md#test_detector_regex_execution_catch_block)
  and [`test_detector_defensive_catch_blocks`](../catalog/tests/core_engine/test_detector.md#test_detector_defensive_catch_blocks)
  both pin "the engine survives a catastrophic regex execution failure" without dropping the rest of the
  file's functions.
- Mode D's trailing, still-open block at end-of-file is emitted as `<name>_[Truncated]`, and Mode E's
  unterminated trailing statement is emitted as `<name>_[Unterminated]` — both are kept rather than
  silently discarded.
- A rule whose hit count exceeds the segment's own character length is treated as a runaway match and
  zeroed defensively rather than trusted, inside the (out-of-subgraph) signal-counting pass — see
  `test_detector_empty_pattern_continuations` for the adjacent "empty/malformed pattern is skipped safely"
  guarantee.
- [`get_token_mass`](../catalog/gitgalaxy/core/detector.md#get_token_mass) returns `None`, not `0`, when
  `tiktoken` is missing, so downstream cost math can distinguish "unmeasured" from "measured as free."

## Open questions
- [`_function_slice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._function_slice) resolves
  its per-language mode/opener/closer/terminator/igniter configuration through
  [`get_config`](../catalog/gitgalaxy/core/detector.md#ScopeParsingRegistry.get_config), but the
  containing registry class, its `DEFINITIONS` matrix, and its `_ALIASES` map are not themselves separate
  entries in this packet's subgraph, so their exact per-language regex lists are described from reading
  `detector.py` directly rather than cited here.
- The segment partitioner, the whole-segment signal-counting pass, the comment-stream analyzer, the
  metadata/docstring decoder, the security-signal spatial-correlation pass, and this file's own copy of
  the balanced-bracket scanner are all called from `splice`/`_calculate_block_metrics` per source, but
  none are separate symbols in this packet's subgraph — their behavior above is described from source and
  from the tests that exercise them (e.g. `test_detector_advanced_appsec_sensors`,
  `test_detector_ghost_tether_and_metadata`), not linked directly.
- Whether `calls_out_to` and the class/inheritance linkage this page's `splice` builds are actually
  consumed by `network_risk_sensor.py` to build a cross-file graph is inferred from the repo's own
  `core/README.md`; that module is out of this packet's scope so the claim cannot be cited to a symbol
  here.

## See also
- [The Prism](gitgalaxy-core-prism.md) — produces the `code_stream`/`comment_stream` pair this page's
  `splice` consumes.
- [The Aperture Filter](gitgalaxy-core-aperture.md) — decides which files ever reach the Detector.
- [The GuideStar Protocol](gitgalaxy-core-guidestar_lens.md) — the upstream intent signal that can push a
  file's confidence past the Detector's `0.42` floor.
