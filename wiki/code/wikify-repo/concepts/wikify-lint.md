---
title: The citation linter — wikify's hallucination gate
type: concept
provenance: mixed
concept: wikify-lint
updated: 2026-07-04
status: fresh
---
# The citation linter — wikify's hallucination gate

## Overview
This is the mechanism that makes a wikify wiki *trustworthy* rather than merely
plausible. Every other stage produces prose; this stage decides whether that prose
is allowed to ship. The linter reads each agent-written concept page as plain text
and enforces three deterministic rules: (1) every symbol citation must resolve —
through the module catalog's frontmatter map — to a moniker that actually exists in
the repo's SCIP index; (2) inside the two load-bearing sections (`Entry points`,
`Mechanism`) every list item must carry a citation, so the reasoning is grounded and
not asserted; (3) no page may cite a symbol that lies outside the packet it was
synthesized from, which is how an *invented* symbol is caught. The key design idea is
that grounding is enforced by a **build gate written in Python**, not by asking a model
to police itself — the same reason a compiler, not a code reviewer, is what guarantees
your program parses. [`lint_page`](../catalog/wikify/lint.md#lint_page) is the per-page
checker; [`lint_silo`](../catalog/wikify/lint.md#lint_silo) runs it over a whole repo;
[`finalize`](../catalog/wikify/cli.md#finalize) is the CLI stage that refuses to
assemble the wiki if any error remains.

## Diagram
```mermaid
flowchart TD
    finalize["finalize (Stage 6 gate)"] --> lint_silo["lint_silo — every concept page"]
    lint_silo -->|per page| read_subgraph["read_subgraph — allowed symbols"]
    lint_silo --> lint_page["lint_page — scan lines"]
    read_subgraph --> lint_page
    lint_page -->|"link on line?"| is_sym["_is_symbol_link"]
    is_sym -->|"catalog anchor"| resolve["_resolve_citation → moniker"]
    resolve --> graph["SymbolGraph (SCIP index)"]
    graph -->|"rule 1 / rule 3 check"| err["LintError"]
    lint_page -->|"in Entry points / Mechanism"| flush["flush_item — rule 2"]
    flush --> err
    err --> report["LintReport.ok?"]
    report -->|"no"| exit["finalize raises Exit(1)"]
    report -->|"yes"| assemble["assemble index + state"]
```

## Design rationale (why it's built this way)
The module docstring states the intent bluntly: this is *"Stage 6 — the citation
linter … The hallucination floor. Hard, deterministic gate."* The word that matters is
**deterministic**. A grounding rule that lived inside the synthesis prompt would be
subject to the same failure mode it is meant to prevent — a model that hallucinates a
symbol is exactly the model you cannot trust to notice it hallucinated. So wikify
splits the pipeline along a hard Python/LLM seam: synthesis is the model's job, and
verification is pure code with zero model calls. [`lint_page`](../catalog/wikify/lint.md#lint_page)
is a line scanner over regex matches, not an NLP pass.

The second non-obvious decision is *how* the linter checks a claim without
understanding English. It cannot judge whether a sentence is true, so it does not try.
Instead it exploits structure: rule 2 is scoped to two named section headings
and to markdown list items. As the docstring puts it, the rules are *"Checkable
without NLP because rules 2–3 are scoped to named sections and list items."* The
constant [`_CITED_SECTIONS`](../catalog/wikify/lint.md#_CITED_SECTIONS) is literally
`("Entry points", "Mechanism")` — a prefix match on the heading text. This is the
whole trick: the synthesis contract *promises* that load-bearing claims live in those
sections as list items, and the linter *enforces* that each such item is anchored to a
real symbol. Comprehension is thereby made mechanically auditable.

Third, resolution is indirected through the catalog rather than checking a symbol
table directly, which keeps the wiki's own cross-links honest.
[`_resolve_citation`](../catalog/wikify/lint.md#_resolve_citation) does not look a
symbol up by name; it *follows the citation link the same way a reader would* — open
the catalog page it points at, read that page's `symbols` frontmatter map, and
reconstruct the moniker from `symbol_base` + suffix. A citation therefore passes only
if the link a human would click actually lands on the symbol's real home. This is the
axis on which wikify differs from name-based code-comprehension tools: it never trusts
a symbol *name* string; it demands the name resolve through the SCIP index (see the
[`wikify-monikers`](wikify-monikers.md) identity scheme).

> [!inferred]
> Compared with tools that build a name-keyed call graph and let a model narrate over
> it, the distinguishing property here is that a claim which cannot be tied to an
> indexed symbol is *rejected at build time* rather than surfaced with lower
> confidence. The gate is binary and offline; that is the comparison point the survey
> cares about.

## Entry points
- [`finalize`](../catalog/wikify/cli.md#finalize) is the primary entry: Stage 6 of an
  ingest. After it emits the module catalogs (the symbol homes citations resolve
  against), it runs the silo lint and — crucially — *refuses to proceed* if any error
  remains, echoing `LINT FAILED` and raising a non-zero exit. Nothing downstream (the
  index, the reconcile state) is written until the wiki is clean. This is what makes
  "grounded" a property of the artifact and not a hope.
- [`lint_cmd`](../catalog/wikify/cli.md#lint_cmd) is the standalone `wikify lint`
  command — the same Stage 6 gate re-run on demand against pages already on disk,
  useful in CI or after hand-edits. With `--fix` it auto-repairs first; without it, it
  is a pure check that exits non-zero on any residual error.
- [`lint_silo`](../catalog/wikify/lint.md#lint_silo) is the batch driver control
  reaches from either CLI command: it globs every `concepts/*.md` page, looks up each
  page's own allowed-symbol set, lints it, and collects the errors into one report.

## Mechanism (step-by-step)
1. **Per page, load the ground truth of what may be cited.**
   [`lint_silo`](../catalog/wikify/lint.md#lint_silo) derives a concept slug from each
   page's filename and calls [`read_subgraph`](../catalog/wikify/packet.md#read_subgraph)
   to load `<concept>.subgraph.txt` — the exact set of monikers the synthesis packet
   handed the agent. This set is the linter's definition of "in bounds"; anything cited
   outside it is, by construction, something the agent was never given and therefore
   likely invented.

2. **Scan the page line by line, tracking section and inferred-block state.**
   [`lint_page`](../catalog/wikify/lint.md#lint_page) walks the text once, updating a
   `section` variable on each `## ` heading and a flag for whether it is currently
   inside a `> [!inferred]` blockquote. This single pass is what lets a regex linter
   apply section-scoped rules without a parser — state is just two variables carried
   down the lines.

3. **Rule 1 + rule 3 — validate every citation on the line.** For each markdown link
   the [`_LINK`](../catalog/wikify/lint.md#_LINK) regex finds,
   [`_is_symbol_link`](../catalog/wikify/lint.md#_is_symbol_link) decides whether it is
   a symbol citation (a `catalog/…​.md#anchor` link). If so,
   [`_resolve_citation`](../catalog/wikify/lint.md#_resolve_citation) turns it into a
   moniker: a `None` result means the anchor is not in the target catalog (rule 1,
   "dead citation"); a moniker absent from the [`SymbolGraph`](../catalog/wikify/graph.md#SymbolGraph)
   means it resolved to something not in the SCIP index (rule 1); and a moniker present
   in the graph but absent from this page's subgraph is rule 3, "cited symbol outside
   packet subgraph." Note the ordering — resolvable-but-out-of-bounds is a *different*
   failure from unresolvable, and only the out-of-bounds check is gated on a non-empty
   subgraph.

4. **Rule 2 — group list items in cited sections and require each be grounded.** When
   the current section starts with one of [`_CITED_SECTIONS`](../catalog/wikify/lint.md#_CITED_SECTIONS)
   and the line is not inside an inferred block, the scanner uses
   [`_LIST_ITEM`](../catalog/wikify/lint.md#_LIST_ITEM) to detect item starts and
   accumulates continuation lines, so a multi-line bullet is judged as one unit. When
   an item ends, [`flush_item`](../catalog/wikify/lint.md#lint_page.flush_item) checks
   whether its body contains at least one symbol link *or* an evidence link
   ([`_is_evidence_link`](../catalog/wikify/lint.md#_is_evidence_link), i.e. a link into
   `tests/` or `sources/`); if neither, it records a rule-2 "uncited item" error. This
   is why every Entry-point bullet and Mechanism step in this very page carries a
   citation — the linter would reject them otherwise.

5. **Collect, judge, and gate.** Each violation is one
   [`LintError`](../catalog/wikify/lint.md#LintError) (page, line, rule number,
   message); the per-page lists roll up into a [`LintReport`](../catalog/wikify/lint.md#LintReport)
   whose [`errors`](../catalog/wikify/lint.md#LintReport.errors) list drives its `ok`
   property. Back in [`finalize`](../catalog/wikify/cli.md#finalize), a non-`ok` report
   prints every error and exits — the build stops here.

6. **Optionally auto-repair the deterministically fixable failures first.** With
   `--fix`, [`finalize`](../catalog/wikify/cli.md#finalize) instead calls
   [`fix_silo`](../catalog/wikify/fix.md#fix_silo), which runs
   [`fix_page`](../catalog/wikify/fix.md#fix_page) per page and then re-lints. The
   fixer mirrors the linter's validity test exactly: a rule-1 dead anchor is
   re-pointed to the packet's known-correct link, a rule-3 out-of-subgraph link is
   de-linked but its prose kept as inline code, and a rule-2 uncited item is repaired
   by linking a citable symbol it already names. What cannot be fixed mechanically is
   left as a residual error for a human — the gate never lowers the bar to pass itself.

## Key data structures
- [`LintError`](../catalog/wikify/lint.md#LintError) — a dataclass of
  `(page, line, rule, message)`. Carrying the *rule number* is what lets the fixer and
  the tests reason about *kinds* of failure (rule 1 vs 2 vs 3) rather than parsing
  messages.
- [`LintReport`](../catalog/wikify/lint.md#LintReport) — a wrapper over the
  [`errors`](../catalog/wikify/lint.md#LintReport.errors) list whose `ok` property is
  the single boolean the build gate branches on. Reports compose by concatenating
  error lists (the silo lint and the doc-concept lint are merged before the gate).
- The catalog **`symbols` frontmatter map** — not defined in this module but the
  resolution table [`_resolve_citation`](../catalog/wikify/lint.md#_resolve_citation)
  reads via [`_frontmatter_dict`](../catalog/wikify/lint.md#_frontmatter_dict). Anchors
  map to moniker *suffixes* factored under a shared `symbol_base`, so citations resolve
  against the catalog the agent actually links to.
- The **subgraph set** from [`read_subgraph`](../catalog/wikify/packet.md#read_subgraph)
  — the per-concept allow-list of monikers that defines rule 3's boundary.

## Dynamics (design intent)
The rule set is pinned by a focused test suite that exercises each rule in isolation,
which doubles as the executable spec. A clean page produces no errors
([`test_clean_page_passes`](../catalog/tests/test_lint.md#test_clean_page_passes)); a
citation whose anchor is missing from the catalog is rule 1
([`test_rule1_anchor_not_in_catalog`](../catalog/tests/test_lint.md#test_rule1_anchor_not_in_catalog)),
as is one that resolves to a moniker the SCIP index does not know
([`test_rule1_resolves_to_unknown_moniker`](../catalog/tests/test_lint.md#test_rule1_resolves_to_unknown_moniker));
an uncited Mechanism item is rule 2
([`test_rule2_uncited_mechanism_item`](../catalog/tests/test_lint.md#test_rule2_uncited_mechanism_item))
while the same prose inside an inferred block is deliberately exempt
([`test_rule2_inferred_block_is_exempt`](../catalog/tests/test_lint.md#test_rule2_inferred_block_is_exempt));
and citing a resolvable symbol that is not in the packet is rule 3
([`test_rule3_out_of_subgraph`](../catalog/tests/test_lint.md#test_rule3_out_of_subgraph)).
The fixer's honesty is likewise pinned: it links a named symbol when one is available
([`test_rule2_uncited_step_links_named_symbol`](../catalog/tests/test_fix.md#test_rule2_uncited_step_links_named_symbol))
but leaves the item for a human when no citable symbol is named
([`test_rule2_unfixable_when_no_citable_symbol_named`](../catalog/tests/test_fix.md#test_rule2_unfixable_when_no_citable_symbol_named)).

## Edge cases
- **Empty subgraph disables rule 3.** [`lint_page`](../catalog/wikify/lint.md#lint_page)
  only applies the out-of-subgraph check when a subgraph exists (`if subgraph and …`).
  A page with no packet — e.g. a hand-authored orphan — has its citations validated for
  resolution (rules 1–2) but is not bounded, and the fixer must not strip its valid
  links ([`test_empty_subgraph_page_is_left_untouched`](../catalog/tests/test_fix.md#test_empty_subgraph_page_is_left_untouched)).
- **Doc-concept pages get a lighter gate.**
  [`lint_doc_concepts`](../catalog/wikify/lint.md#lint_doc_concepts) applies only rule
  1: pages derived from a project's own docs "may state prose freely" and are bound to
  no packet, so the subgraph and uncited-item gates are switched off — they simply may
  not cite a symbol that does not exist
  ([`test_doc_concept_lint_ignores_subgraph_and_uncited`](../catalog/tests/test_doc_concepts.md#test_doc_concept_lint_ignores_subgraph_and_uncited)).
- **Evidence links satisfy rule 2 but are not subgraph-checked.** A link into `tests/`
  or `sources/` counts as grounding for [`flush_item`](../catalog/wikify/lint.md#lint_page.flush_item)
  yet is not a symbol citation, so rules 1/3 skip it — a claim can be grounded in a
  test rather than a symbol.
- **Docs-mode analog.** For prose ingests, [`lint_docs`](../catalog/wikify/docs.md#lint_docs)
  is the parallel gate: it swaps the grounding anchor from a SCIP symbol to a source
  document `#section`, but keeps the same "every citation must resolve" spirit.

## Open questions
- The fixer's rule-2 repair path (`_cite_item_mention`) and the packet cite-map it uses
  are referenced by [`fix_page`](../catalog/wikify/fix.md#fix_page)/[`fix_silo`](../catalog/wikify/fix.md#fix_silo)
  but are outside this packet's subgraph, so the exact heuristic for choosing *which*
  named symbol to link is not documented here.
- Rule 2's section detection is a prefix match on heading text via
  [`_CITED_SECTIONS`](../catalog/wikify/lint.md#_CITED_SECTIONS); how robust this is to
  heading variants (e.g. renamed or nested sections) is not settled by the source read.

## See also
- [`wikify-coverage`](wikify-coverage.md) — the other Stage 6 floor: enumeration over
  the symbol table so no module is silently dropped (lint checks what's *said*; coverage
  checks what's *represented*).
- [`wikify-verify`](wikify-verify.md) — the adversarial pass layered on top of the
  deterministic lint gate.
- [`wikify-monikers`](wikify-monikers.md) — the SCIP moniker identity the linter
  resolves every citation to.
- [`wikify-graph`](wikify-graph.md) — the `SymbolGraph` the linter checks resolved
  monikers against.
- [`wikify-docs`](wikify-docs.md) — docs-mode ingest, whose `lint_docs` is the prose
  analog of this gate.
