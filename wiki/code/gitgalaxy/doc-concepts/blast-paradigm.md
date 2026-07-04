---
title: The blAST paradigm — heuristics as a deliberate substitute for ASTs and LLMs
type: doc-concept
provenance: doc
source: docs/wiki/01-03-the-blast-paradigm.md
updated: 2026-07-04
status: fresh
---
# The blAST paradigm — heuristics as a deliberate substitute for ASTs and LLMs

## Definition
"blAST" (**B**ypassing **L**LMs **a**nd **AST**s) is gitgalaxy's name for its own architectural
choice: treat source code as raw structural text and hunt it with bounded, deterministic regular
expressions, rather than compiling an Abstract Syntax Tree or handing chunks of it to a model. The
doc frames this explicitly as a *third path* between the two dominant industry approaches, chosen
because both existing approaches "collapse" at the scale gitgalaxy targets — a 5-million-line,
15-year-old polyglot enterprise monolith — for reasons the doc itemizes precisely: ASTs need "a
bespoke, perfectly maintained parser for every single language" and go blind on any file they
cannot fully parse; LLMs cannot hold a multi-million-line codebase in context, will "guess
(hallucinate)" an unseen dependency, produce a different answer on every run, and cannot be handed
proprietary source code at all under a zero-trust/air-gapped requirement.

## In gitgalaxy (grounded)
The doc's own comparison table names four measurable axes — speed, repeatability, behavior on
broken code, and language coverage — and every one of them is a real, load-bearing design
constraint on the code, not just marketing:
- **Speed / no toolchain.** There is no per-language compiler or interpreter anywhere in the
  pipeline; [`StructuralExtractor.splice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor.splice)
  dispatches every language to one of five regex/state-machine
  [`_function_slice`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._function_slice)
  modes, and [`get_token_mass`](../catalog/gitgalaxy/core/detector.md#get_token_mass) estimates size
  by counting tokens in text, never by invoking a parser or a model.
- **Repeatability.** Because every stage is a pure function of the file's bytes plus a fixed
  regex/config table (see [Language standards](../concepts/gitgalaxy-standards-language_standards.md)),
  re-running the pipeline on unchanged input reproduces the same `FunctionNode` records — there is
  no sampling temperature or model variance to reproduce.
- **Resilience to broken/incomplete code.** [`ApertureFilter`](../concepts/gitgalaxy-core-aperture.md)
  and the Detector never require a file to compile; a syntax error or missing import simply cannot
  break a regex match the way it aborts an AST build.
- **"The Physics of Code."** The doc's central metaphor — judging a file by "the *shape* of the
  text" (indentation depth, keyword density, Shannon entropy) rather than what a variable is named
  or does — is exactly what [`SignalProcessor.calculate_risk_vector`](../concepts/gitgalaxy-metrics-signal_processor.md)
  computes: risk scores derived from counted regex hits and entropy, never from resolved semantics.

## Why it matters / when it applies
This doc is the clearest first-person statement of the survey's own framing of gitgalaxy as the
**"no grounding substrate" control group**: it isn't that gitgalaxy failed to build a SCIP index or
wire up an LLM — it explicitly rejects both as unsuitable for its stated scale/privacy/determinism
goals, in a domain (architecture/risk *observability*, not compilation or refactoring) where
compiler-grade precision is not the deliverable. The tradeoff is made explicit elsewhere in the
tool's own docs — see [AST vs. heuristic tradeoffs](ast-vs-heuristic-tradeoffs.md) for the honest
accounting of what this choice gives up.

## Connections
- Code concepts: [The Detector](../concepts/gitgalaxy-core-detector.md) — the regex/state-machine
  engine this paradigm names; [Language standards](../concepts/gitgalaxy-standards-language_standards.md) —
  the per-language regex "grammar"; [Signal Processor](../concepts/gitgalaxy-metrics-signal_processor.md) —
  where counted structural signal becomes a risk score.
- Module catalogs: [detector](../catalog/gitgalaxy/core/detector.md), [language_standards](../catalog/gitgalaxy/standards/language_standards.md).
- Related doc-concepts: [empirical-validation-of-heuristic-parsing](empirical-validation-of-heuristic-parsing.md),
  [ast-vs-heuristic-tradeoffs](ast-vs-heuristic-tradeoffs.md), [structural-rag-graph](structural-rag-graph.md).

## Source
Extracted from `docs/wiki/01-03-the-blast-paradigm.md`, kept in place.
