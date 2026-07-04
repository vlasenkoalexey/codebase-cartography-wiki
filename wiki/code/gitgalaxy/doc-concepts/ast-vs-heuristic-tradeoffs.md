---
title: AST vs. heuristic tradeoffs — what gitgalaxy's own docs admit it cannot do
type: doc-concept
provenance: doc
source: docs/wiki/03-10-claim-10-ast-vs-heuristic-parsing.md
updated: 2026-07-04
status: fresh
---
# AST vs. heuristic tradeoffs — what gitgalaxy's own docs admit it cannot do

## Definition
Unlike the promotional framing elsewhere in the docs, this page is an unusually candid
three-way accounting: what ASTs and gitgalaxy's heuristics both achieve, what gitgalaxy can do
that an AST cannot, and — the section most relevant to this survey — **what an AST can do that
gitgalaxy explicitly cannot**: "Absolute Semantic Precision" (gitgalaxy "uses bounded lookaheads to
prevent 99% of hallucinations, but it is not infallible" vs. an AST's mathematical grammar
guarantee), "Deep Type Inference" (an AST resolves `var x`'s real type from an assignment three
files away; gitgalaxy "can only analyze the explicitly declared syntax within the immediate file
boundary"), "Variable-Level Data Flow" (an AST can taint-track one variable across fifty lines;
gitgalaxy "measures aggregate *State Flux* ... but cannot reliably trace a single variable's
lifecycle"), and "Macro Expansion" (a C preprocessor macro hides logic an AST expands and
gitgalaxy does not).

## In gitgalaxy (grounded)
Every limitation the doc names maps onto a real absence in the pinned source, not just a caveat:
- **No cross-file symbol resolution.** [`StructuralExtractor`](../concepts/gitgalaxy-core-detector.md)'s
  Subgraph shows every extractor method operating on one file's text/segments at a time; there is
  no moniker table, no cross-file reference index, and no import-resolution step anywhere in the
  pipeline comparable to a SCIP `graph` stage — confirming "cannot see a dependency three files
  away" is architectural, not an implementation gap.
- **Aggregate, not per-variable, mutation tracking.** [`SignalProcessor.calculate_risk_vector`](../concepts/gitgalaxy-metrics-signal_processor.md)
  produces file-level `RISK_SCHEMA` scores (counts and densities) — there is no per-symbol state
  object a "State Flux" score could be attributed back to, matching the doc's own admission that
  it "measures aggregate ... total mutations in a file."
- **No macro expansion.** The [Language standards](../concepts/gitgalaxy-standards-language_standards.md)
  regex tables match C/C++ syntax as written; there is no preprocessor pass anywhere in
  [`gitgalaxy/standards/language_standards.py`](../catalog/gitgalaxy/standards/language_standards.md),
  so a macro-hidden `int x = 5;` is invisible to the engine exactly as the doc states.
- **The one place a model is trusted with more than counting** is
  [`SecurityAuditor`](../concepts/gitgalaxy-security-security_auditor.md)'s XGBoost classifier —
  and even that is a supervised model over the same heuristic feature counts, not a semantic
  analysis, and is described elsewhere as still overridable by a hard-coded rule.

## Why it matters / when it applies
This is the single most important source document for this survey's specific interest in
gitgalaxy: it is gitgalaxy's *own* engineers stating, in writing, exactly the axis this wiki
compares tools on. The doc's own "Synthesis" section draws the line explicitly — use an AST
toolchain "when you need to safely automate variable renaming, enforce strict type-checking, or
trace exact data-flow paths for targeted vulnerability patching," and use gitgalaxy "when you need
to audit a 5-million-line polyglot enterprise repository in 40 seconds." That is a direct,
first-party admission that gitgalaxy is not attempting the grounding guarantee wikify-repo's SCIP
index or a real symbol/call graph provides (see the survey's [scip-grounding](../../../concepts/scip-grounding.md)
and [symbol-graph](../../../concepts/symbol-graph.md) cross-repo pages) — it is trading precision
for scale, coverage, and zero-toolchain polyglot reach, and says so plainly.

## Connections
- Code concepts: [The Detector](../concepts/gitgalaxy-core-detector.md), [Signal Processor](../concepts/gitgalaxy-metrics-signal_processor.md),
  [SecurityAuditor](../concepts/gitgalaxy-security-security_auditor.md) — the one module that adds a
  trained model on top of the heuristic counts.
- Module catalogs: [language_standards](../catalog/gitgalaxy/standards/language_standards.md),
  [signal_processor](../catalog/gitgalaxy/metrics/signal_processor.md).
- Related doc-concepts: [blast-paradigm](blast-paradigm.md), [empirical-validation-of-heuristic-parsing](empirical-validation-of-heuristic-parsing.md).

## Source
Extracted from `docs/wiki/03-10-claim-10-ast-vs-heuristic-parsing.md`, kept in place.
