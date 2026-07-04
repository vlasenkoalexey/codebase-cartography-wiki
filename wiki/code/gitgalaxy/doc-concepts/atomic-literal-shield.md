---
title: The Atomic Literal Shield — masking strings before they can desync the scope stack
type: doc-concept
provenance: doc
source: docs/wiki/02-08-the-detector.md
updated: 2026-07-04
status: fresh
---
# The Atomic Literal Shield — masking strings before they can desync the scope stack

## Definition
Strings are the natural enemy of a regex-based structural parser: a stray `{` or unmatched
`"` sitting inside a string literal can permanently desynchronize a brace/quote-balance
counter, "shattering the parsed logic." The doc names the Detector's defense the "Atomic
Literal Shield" — a pre-processing pass that masks disruptive text *without* altering the
file's physical line counts or character indexing, so the parsed structure still maps 1:1 onto
the original source. It calls out four specific hazards it handles: multi-character "Advanced
Atomic Quotes" (C++ raw string literals, Python triple quotes) processed *before* single
quotes so they aren't prematurely split; "Heredoc Isolation" for scripting languages via a
line-by-line state machine; Ruby's bracketed `%` string literal family, gated strictly to
Ruby; and a diagnostic timer that logs a warning if shielding a single file takes over 0.5
seconds (a ReDoS-performance tripwire).

## In gitgalaxy (grounded)
Every claim in the doc matches the pinned source of
[`StructuralExtractor._apply_literal_shield`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._apply_literal_shield),
read directly rather than only cited generically:
- The method's regex explicitly orders a C++ raw-string alternative
  (`` R"([a-zA-Z0-9_]*)\(.*?\)\1" ``) before the standard double/single-quote alternatives in
  one combined pattern, with an inline comment: "Handles Python (`\"\"\"`), C++ (`R"(...)"`),
  and standard strings" — confirming the "surgical ordering" the doc describes is a real
  property of one compiled pattern, not two separate passes that could disagree.
- Heredoc isolation is a genuine line-by-line state machine: it tracks an
  `active_heredoc_delimiter` across lines via a compiled opener pattern
  (`` <<[-~]?\s*['"]?\\?([a-zA-Z_][a-zA-Z0-9_]*)['"]? ``) and closes only when a line's
  stripped text exactly matches that delimiter.
- The Ruby `%` literal shield is gated behind a language check and masks four bracket families
  (`%{...}`, `%[...]`, `%(...)`, `%|...|`) via `re.DOTALL` substitutions that preserve
  newlines — exactly the "strictly gated to Ruby" claim.
- The 0.5-second diagnostic is a real, timed instrumentation block: the method records
  `time.time()` checkpoints around the quote pass, the heredoc pass, and the percent-literal
  pass, and — if the total exceeds `0.5` — logs a `[DIAGNOSTIC-SHIELD]` warning breaking down
  which of the three sub-passes was slow, not just a generic "this was slow" message.

## Why it matters / when it applies
This is the Detector's counterpart to a problem the Prism solves independently for comment
stripping via its own [`LITERAL_MASK_PATTERN`](../catalog/gitgalaxy/core/prism.md#Prism.LITERAL_MASK_PATTERN) —
two separately-implemented literal shields exist because the two stages mask literals for
different purposes (the Prism protects comment delimiters from string contents; the Detector
protects brace/scope balance from string contents) and neither reuses the other's regex. The
per-stage timing diagnostic is the doc's own admission that this defense has a real
performance cost worth watching, not a free abstraction — consistent with this survey's
broader observation that gitgalaxy's regex-only design requires continuous, hand-authored
ReDoS defenses at every stage rather than a single grammar-level guarantee.

## Connections
- Code concepts: [The Detector](../concepts/gitgalaxy-core-detector.md) — owns
  `_apply_literal_shield`, invoked from Mode D's
  [`_slice_by_keywords`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._slice_by_keywords);
  [The Prism](../concepts/gitgalaxy-core-prism.md) — the parallel, independently-implemented
  literal-masking discipline for comment stripping.
- Module catalogs: [detector](../catalog/gitgalaxy/core/detector.md), [prism](../catalog/gitgalaxy/core/prism.md).
- Related doc-concepts: [active-matter-vs-ghost-mass](active-matter-vs-ghost-mass.md),
  [satellite-physics-and-naming-shields](satellite-physics-and-naming-shields.md).

## Source
Extracted from `docs/wiki/02-08-the-detector.md` ("The Atomic Literal Shield" section). Note:
at the pinned commit, `docs/wiki/02-07-the-prism.md` — despite its filename — contains an
earlier, near-duplicate draft of this same section (compare the two files directly; they
differ only in wording and the presence of "v6.3.0 Protocol" framing added in 02-08). It does
not document `gitgalaxy/core/prism.py`'s actual behavior, which is covered separately by the
[The Prism](../concepts/gitgalaxy-core-prism.md) code concept page. Both doc files are kept in
place; this page and its siblings on this topic draw from 02-08 as the fuller version.
