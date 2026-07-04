# Agentic code mapping tools methodology analysis

**A survey of code-comprehension tools — written as the thing it studies.** This repo ingests the
tools people use to *map, analyze, and understand codebases* (wikify-repo, graphify,
understand-anything, …) and turns each tool's own source into a grounded markdown wiki. Then it
compares them on the concept axis — and because every page is grounded, **every claim in the
comparison cites the tool's actual implementation**, not a README or a blog post.

The method is itself one of the tools under survey: the [Karpathy LLM-wiki
pattern](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f), driven here by
[wikify-repo](https://github.com/vlasenkoalexey/wikify-repo). So the repo is doubly self-referential:
a code-comprehension tool is used to comprehend code-comprehension tools.

## What's in it

Two source types feed **one wiki** (one `index.md`, one `log.md`):

- **Code repos — the tools under survey.** Each tool's source is ingested by the
  **`wikify-ingest-repo`** skill into a grounded, lint-clean wiki: a mechanism page per subsystem
  (prose + Mermaid + citations to real SCIP symbols), a symbol catalog, and pages derived from the
  tool's own docs. One silo per tool under `wiki/code/<slug>/`.
- **Cross-repo concept pages — where the survey lives.** Once two or more tools are ingested, the
  **`wikify-connect-repo`** skill cross-links the same concept (e.g. *symbol graph*, *grounding /
  citation gate*, *chunking*, *query routing*) across tools: the concept page in `wiki/concepts/`
  links **down** to each tool's implementation, and each implementation links back **up**. This is
  the "compare their internal approaches" layer — grounded, not hand-waved.
- **Articles / docs / notes — the surrounding literature.** Papers and posts about code comprehension,
  ingested the classic Karpathy way (read → summarize → cross-link) into `wiki/topics/` and
  `wiki/sources/`.

See [`SCHEMA.md`](SCHEMA.md) for the full workflow (ingest / connect / query / lint).

## Repo layout

```
SCHEMA.md              single source of truth — the three layers, ingest/connect/query/lint, retrieval rules.
raw/                   immutable inputs — never modified.
  code/<slug>/           ingested tools as git SUBMODULES, pinned by gitlink (acquire: submodule).
  sources/               ingested articles / docs / notes — committed source of truth.
wiki/                  LLM-owned markdown — the product.
  index.md               read-first catalog: tools, cross-repo concepts, topics, sources, notes.
  log.md                 append-only event log (## [date] <op> | <name>).
  code/<slug>/           one wiki per surveyed tool:
      overview.md            high-level map — main concepts + system diagrams.
      concepts/              grounded mechanism pages (prose + Mermaid + citations).
      catalog/               per-module symbol catalogs — signatures, docstrings, source links, uses-by.
      doc-concepts/          pages derived from the tool's own docs.
  concepts/              cross-tool vocabulary — each concept links down to every tool's implementation.
  sources/               one summary page per ingested article.
  topics/                synthesized prose pages — entities, concepts, comparisons.
  notes/                 cross-cutting answers filed back from queries.
```

Tool sources under `raw/code/` are **git submodules** (pinned by gitlink). After cloning:
```bash
git submodule update --init
```

## Add a tool to the survey

In **Claude Code, Codex, or Antigravity**, just say:
> ingest https://github.com/owner/some-code-comprehension-tool

The skill pins + indexes the repo, writes the grounded pages, lints them, assembles
`wiki/code/<slug>/`, and updates `index.md` + `log.md`. Re-running is idempotent; `ingest --ref
<commit>` updates to a newer commit and rebuilds only what changed. From the **second** tool on, it
connects shared concepts into the cross-repo `wiki/concepts/` pages — that's where the comparison
accumulates.

Install the tooling once — see [wikify-repo](https://github.com/vlasenkoalexey/wikify-repo)
(`pip install -e .` → `setup-vendor.sh` → `install-skill.sh /path/to/this-repo`).

## Browse it (no install)

Open [`wiki/index.md`](wiki/index.md) and follow links, or `grep -ri "<term>" wiki/`. Everything is
plain markdown — no embeddings, no database. An agent answers cheaply by reading `index.md`, grepping
to the right page, and citing the catalog anchor.

## Why a wiki and not just grep over the source?

The wiki sits *between* raw repos and your questions: the cross-references are already there, the
dynamic-dispatch seams a call-graph walk misses are covered by deterministic catalogs, and every
mechanism page is grounded in real SCIP symbols. For a *comparison* this matters twice over — the
claim "tool A grounds claims in a symbol graph, tool B in embeddings" is anchored to the exact code
that does it, so the survey stays honest as the tools evolve. The tedious bookkeeping is done once and
kept current, so answers are fast, grounded, and consistent.

> Note on citation anchors: a citation like `catalog/<module>.md#Graph.build` resolves against the
> catalog's frontmatter `symbols:` map (that's what the linter gates), not against a rendered
> heading — so clicking one on github.com opens the right catalog *file* but won't auto-scroll.
> Grep the anchor name inside the file, or read the wiki locally.
