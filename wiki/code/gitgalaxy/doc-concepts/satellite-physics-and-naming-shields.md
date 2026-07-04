---
title: Satellite physics and naming shields — the per-function math and label extraction
type: doc-concept
provenance: doc
source: docs/wiki/02-08-the-detector.md
updated: 2026-07-04
status: fresh
---
# Satellite physics and naming shields — the per-function math and label extraction

## Definition
Once the Detector's Master Dispatcher cleaves a block of logic from a file, the doc calls it a
"Satellite" and describes three physical quantities computed for it, feeding the 3D
visualization: **Control Flow Ratio** (branch density vs. linear execution, clamped 0-1),
**Logic Angle** (maps that ratio onto a display angle — steep 90° for linear functions, wide
22.5° for complex ones — via `Angle = 22.5 + (1.0 - cf_ratio) * 67.5`), and **Magnitude** (a
composite mass, given in the doc as a simplified `(branches+1)*(args+1)+(0.05*loc)`). Separately,
it describes a "gauntlet of Naming Shields" that extract a clean function name from raw
regex-captured text: a C++ Operator Shield (`operator<<`), a C++ Test Macro Shield
(`BOOST_AUTO_TEST_CASE(MyTest)` → `MyTest`), a C++ Scope Shield (protecting `::` from a
truncating single-colon guillotine), Objective-C bracketed message-syntax extraction, and a
Makefile Variable Shield protecting `$(VAR)` declarations from parenthesis-splitting logic.

## In gitgalaxy (grounded)
The physics formulas and the naming shields are both real, computed inside
[`StructuralExtractor._calculate_block_metrics`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._calculate_block_metrics)
and [`StructuralExtractor._extract_name`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._extract_name)
respectively — but reading the pinned source directly shows the doc's magnitude formula is a
simplification of a more defensive real one:
- **The real magnitude formula dampens arguments and doubles for recursion.** The actual code
  applies a square-root dampener to the argument count "to prevent combinatorial magnitude
  explosions," and doubles the whole magnitude for recursive functions ("Recursive functions
  are dangerous and mathematically dense"), before adding the `0.05 * effective_loc` term the
  doc's simplified formula does show. The doc's public-facing equation names the right inputs
  (branches, args, loc) but omits the dampening and recursion-doubling refinements present in
  the pinned source.
  > [!inferred] This gap (doc gives a clean illustrative formula; the code has extra guard
  > terms) mirrors this survey's broader observation about gitgalaxy's docs elsewhere — see
  > [empirical-validation-of-heuristic-parsing](empirical-validation-of-heuristic-parsing.md) —
  > that the public narrative simplifies mechanics the pinned source implements more
  > defensively.
- **Control Flow Ratio and Angle match exactly.** The pinned source computes
  `angle = 22.5 + (1.0 - control_flow_ratio) * 67.5`, letter-for-letter the doc's stated
  equation, inside the same method.
- **Naming shields are real, including the Makefile one.** [`_extract_name`](../catalog/gitgalaxy/core/detector.md#StructuralExtractor._extract_name)
  carries an inline comment reading "Variable Interpolation Preservation (Makefiles): Do not
  split variable names by parenthesis" and its allowed-character set explicitly includes `$`
  and `%` "plus Makefiles" — confirming the Makefile Variable Shield the doc names, which is
  not mentioned on the existing [The Detector](../concepts/gitgalaxy-core-detector.md) concept
  page's naming-shield list (C++ operator/test-macro/scope shields, Objective-C).

## Why it matters / when it applies
The Angle/Magnitude math exists purely to drive the Cartographer's 3D display (see
[the-cartographer-spatial-positioning](the-cartographer-spatial-positioning.md)) — a linear,
low-complexity function should visually read as a steep, simple satellite, while a deeply
branching one should read as a wide, sprawling one. That the doc's formula is a simplification
of the real one is a minor but genuine finding for this survey's "empirical validation" theme:
even gitgalaxy's own internal documentation trades some precision for readability when
describing its own heuristics, the same tension the tool applies to source code itself.

## Connections
- Code concepts: [The Detector](../concepts/gitgalaxy-core-detector.md) — owns
  `_calculate_block_metrics` and `_extract_name`.
- Module catalogs: [detector](../catalog/gitgalaxy/core/detector.md).
- Related doc-concepts: [active-matter-vs-ghost-mass](active-matter-vs-ghost-mass.md),
  [the-cartographer-spatial-positioning](the-cartographer-spatial-positioning.md),
  [empirical-validation-of-heuristic-parsing](empirical-validation-of-heuristic-parsing.md).

## Source
Extracted from `docs/wiki/02-08-the-detector.md` ("Satellite Physics & Naming Shields"
section); the near-duplicate `docs/wiki/02-07-the-prism.md` carries a shorter earlier draft
of the same section without the exact formulas (see
[atomic-literal-shield](atomic-literal-shield.md)'s Source note). Both kept in place.
