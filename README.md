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

This repo is built on top of the
[wikify-repo-demo](https://github.com/vlasenkoalexey/wikify-repo-demo) template — it provides the
wiki scaffolding (the three-layer `raw/` → `wiki/` layout, the `wikify-ingest-repo` /
`wikify-connect-repo` skills, and the `index.md` / `log.md` conventions); this repo instantiates it as
a survey of code-comprehension tools.

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

## How the surveyed tools compare

Nine code-comprehension tools have been ingested. The table below compares them on axes similar to a
grounded-tool comparison — **Specialization, Output, what the Code structure is grounded on,
Faithfulness (how it keeps claims true), Coverage, Inputs, Retrieval, Updates, and Locality**. Every
cell is drawn from that tool's own ingested silo (`wiki/code/<slug>/overview.md`) and the cross-repo
concept pages ([`wiki/concepts/`](wiki/concepts)), i.e. from the tools' real source at the pinned
commits — **these are my own conclusions from the wiki, not any tool's self-description.** Rows are
ordered by grounding substrate, from compiler-grade down to none. (Wide table — scroll right.)

| Tool | Specialization | Output | Grounded on | Faithfulness | Coverage | Inputs | Retrieval | Updates | Locality |
|---|---|---|---|---|---|---|---|---|---|
| [**wikify-repo**](https://github.com/vlasenkoalexey/wikify-repo) | Grounded internals wiki | Markdown wiki (concepts + symbol catalogs) | **SCIP** index + AST fallback | **Hard citation-lint build gate** + adversarial verify | Whole-repo (set-difference catalog floor) | Code (+ prose docs) | Read Markdown / grep → catalog anchor | Symbol-diff vs a commit **pin** (idempotent) | Local; agent owns the Markdown |
| [**codegraphcontext**](https://github.com/CodeGraphContext/CodeGraphContext) | Code graph agents query | Property graph (Neo4j-shape / embedded Kùzu) | Tree-sitter (23 langs) + *optional* SCIP | Confidence-tiered call resolution | Whole-repo graph | Code | **Cypher** (`CodeFinder`) over MCP | Re-index via graph builder | Local (embedded Kùzu) |
| [**codegraph**](https://github.com/colbymchenry/codegraph) | Code graph agents query | SQLite symbol graph | Tree-sitter (~39 langs); no SCIP/LSP | Confidence tiers + **provenance-tagged heuristic edges** | Whole-repo graph | Code | Deterministic **SQL** (FTS5→LIKE→fuzzy) over MCP | **Filesystem watcher** + daemon | Local-first (SQLite) |
| [**tree-sitter-analyzer**](https://github.com/aimasteracc/tree-sitter-analyzer) | Code intel / PR-impact | SQLite (AST cache + edge store), UML | Tree-sitter (21 langs), **family-gated** calls | Confidence **verdict envelopes** + cross-lang mis-wire gate | Whole-repo (largest: ~43k symbols) | Code | MCP/CLI facade (8 tools) | AST cache (SQLite) | Local (SQLite) |
| [**understand-anything**](https://github.com/Egonex-AI/Understand-Anything) | Code → interactive graph | Typed KnowledgeGraph + React/ELK dashboard | Tree-sitter CST (12 langs), name-based calls | **LLM-authored** graph, Zod sanitize/repair pipeline | Whole-repo (batch + merge) | Code (+ optional non-code) | Interactive **dashboard** (graph + file explorer) | Structural **fingerprint** gate | Local; LLM-authored artifact |
| [**graphify**](https://github.com/Graphify-Labs/graphify) | Any-input knowledge graph | Persistent NetworkX knowledge graph | AST extractors + **LLM** semantic pass (no SCIP) | Conservative edge recovery + god-node guard (no hard gate) | Whole-repo; communities + god-nodes | **Any** (code, prose, media) | Graph query / path / explain (MCP) | **Continuous** — cache + watcher + git hooks | Local; the graph *is* the product |
| [**claude-context**](https://github.com/zilliztech/claude-context) | Semantic code search | Vector index (embeddings) | Tree-sitter chunks → **dense embeddings** | Retrieval-only — returns real chunks, nothing synthesized to gate | Whole-repo chunk index | Code | **ANN vector** search (+ BM25 via RRF), MCP/IDE/browser | **Merkle-DAG** tripwire | **Cloud** vector DB (Milvus/Zilliz) |
| [**gitgalaxy**](https://github.com/squid-protocol/gitgalaxy) | Risk / security metrics | ~300 risk metrics (+ 1 XGBoost classifier) | **Regex "grammar"** (57 langs) — no AST, no LLM | Structure *counted*, not *resolved*; ReDoS/hallucination test gauntlets | Whole-repo (counts, no symbol table) | Code | Metrics report / scores | Full scan (incremental path is dead code) | Local |
| [**openwiki**](https://github.com/langchain-ai/openwiki) | Agent-written docs | Markdown docs | **None** — LLM reads source directly (prompt) | **Prompt directive only** — no build gate | Whatever the agent visits (unbounded) | Code | Read Markdown | **git-diff + whole-tree content-hash**, prose-shaped | Local CLI; 5-provider model routing |

### What I take from it

- **Grounding is a spectrum, and it is a precision↔breadth trade.** Exactly one tool (wikify-repo)
  pays for a compiler-grade **SCIP** index; the tree-sitter cluster (codegraphcontext, codegraph,
  tree-sitter-analyzer, understand-anything, and claude-context for chunking) trades that precision
  for language breadth from grammars; gitgalaxy pushes to the far end with regex *counts* and no AST;
  openwiki has no structural substrate at all. More languages, less certainty about any single edge.
- **Faithfulness is where the tools differ most — and only one has a hard gate.** wikify-repo *fails
  the build* if a claim doesn't resolve to a real symbol. Everyone else keeps trust a softer way:
  confidence tiers (codegraph, codegraphcontext, tree-sitter-analyzer), schema repair of an
  LLM-authored graph (understand-anything), conservative edge recovery (graphify), returning only real
  retrieved text (claude-context), adversarial test gauntlets (gitgalaxy), or a prompt instruction
  (openwiki). This axis, not language count, is the real dividing line.
- **Only wikify-repo pairs a hard gate with infrastructure-free retrieval.** Its grounding is baked
  into static Markdown + symbol catalogs, so an agent answers by just reading files and grepping — no
  MCP server, graph DB, or vector store to stand up. openwiki is the *only other* tool whose output
  you simply read, but it has no hard gate (prompt-only); every remaining tool trades tool-free
  reading for a runtime query surface (MCP + SQL/Cypher/graph ops, ANN over a vector DB, or a
  dashboard). So the *combination* — a rejecting grounding gate **and** a result you can consume with
  nothing but filesystem access — lands on wikify-repo alone. Two caveats keep this honest: the gate
  proves each **citation resolves to a real symbol**, not that the surrounding prose is semantically
  true (that is the separate, non-gating adversarial `verify` pass); and *tool-free* describes
  **retrieval**, not **production** — building the wiki still needs the SCIP indexers, the payoff being
  that the finished artifact then needs none.
- **Three output families.** Prose for a reader (wikify-repo, openwiki); a queryable graph/index for
  an agent (codegraphcontext, codegraph, tree-sitter-analyzer, graphify, understand-anything); and
  non-structural signal — embeddings for recall (claude-context) or risk numbers (gitgalaxy).
- **The dynamic-dispatch gap is mostly unaddressed — two tools take it seriously.** codegraph
  synthesizes `provenance:'heuristic'` edges with ~30 framework-specific passes, and
  tree-sitter-analyzer defends cross-language call wiring with a family gate (its README benchmarks
  ~390× fewer mis-wires). wikify-repo recovers some via class-hierarchy "virtual" edges; the rest
  largely report only what a static parse can see.
- **Retrieval follows the consumer.** Agent-first tools expose MCP query surfaces (SQL/Cypher/graph
  ops); semantic recall means vector search; a human reader gets Markdown or an interactive dashboard.
- **Locality/authorship.** All are local-first except claude-context, which leans on a cloud vector
  DB — the one privacy/ownership outlier. Orthogonally, the *artifact's author* splits deterministic
  builds (wikify-repo, codegraph, tree-sitter-analyzer, gitgalaxy) from LLM-authored ones
  (understand-anything, graphify's semantic pass, openwiki end-to-end) — which is exactly why the
  LLM-authored tools invest in repair/guard steps the deterministic ones don't need.

*Caveat: each verdict is read from the tool's pinned commit in this wiki; tools evolve. Drill into a
row's `overview.md` (linked from [`wiki/index.md`](wiki/index.md)) for the grounded detail behind any
cell.*

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
