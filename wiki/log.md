# Wiki log

Append-only, chronological. One entry per operation, prefixed so it stays greppable with plain Unix
tools (`grep '^## \[' wiki/log.md | tail -5`). Prefixes: `ingest-code | <slug>` (code repo via the
skill), `ingest | <source>` (article/doc/note), `connect | <scope>` (cross-repo), `lint | <scope>`,
`note | <title>`. Newest at the bottom.

## [2026-07-04] ingest-code | wikify-repo
Ingested [wikify-repo](https://github.com/vlasenkoalexey/wikify-repo) as a submodule pinned at
`05228d7` (`raw/code/wikify-repo`). Lens: code comprehension (survey comparability). Built 16 grounded
concept pages + an overview + 14 doc-concepts (from README, docs/design.md, docs/implementation.md);
48 module catalogs cover all 664 symbols (100% represented, 52.3% deep). `finalize` citation lint: OK.
Adversarial `verify`: 216 load-bearing claims across 16 pages re-checked against source — 4 pages got
small factual corrections (over-scoped "every command" claims on cli/acquire, a docstring attribution
on verify, rule-scoping + a non-frozen dataclass on lint); all others held. First silo in the survey —
no cross-repo `connect` yet (needs a 2nd tool).

## [2026-07-04] ingest-code | graphify
Ingested [graphify](https://github.com/Graphify-Labs/graphify) as a submodule pinned at `983da3c`
(`raw/code/graphify`). Lens: code comprehension (survey comparability). graphify is 100% Python (194
files, 4,860 symbols); the Rust/C++/TS files it ships are test fixtures for its own multi-language
ingestion, so only the Python SCIP lane was indexed (Rust skipped — fixtures, not source). Built 24
grounded concept pages + an overview + 19 doc-concepts (from README, ARCHITECTURE.md, docs/how-it-works.md,
docs/node-summaries-rfc.md); 184 module catalogs cover all 4,849 documentable symbols (100% represented,
12.8% deep). `finalize` citation lint: OK. Adversarial `verify`: 349 load-bearing claims across 24 pages
re-checked against source — 4 corrections on 3 pages (extract: `walk_calls` appends call edges directly
vs. `walk`'s structural `add_edge`; analyze: builtin-noise filter is case-sensitive, and the peripheral→hub
degree bonus is *not* suppressed for INFERRED cross-boundary calls; security: labels are deliberately
*not* HTML-escaped, only metadata strings are); all others held. 2nd silo — cross-repo `connect` to
`wikify-repo` follows.

## [2026-07-04] connect | 4 concepts wired across 2 repos
Seeded the survey's cross-repo spine: created 4 host vocabulary concepts under `wiki/concepts/`
(scip-grounding, symbol-graph, multi-language-extraction, incremental-reconcile) with lens-framed
"how the implementations differ" hub prose, tagged the 16 implementing silo pages with `concepts:`
frontmatter (authoritative tag match, not name-guess), and ran `wikify connect --apply`. Each concept
page now links **down** to every implementation across wikify-repo + graphify (17 impl links; 16 unique
pages — `wikify-scip_index` implements both scip-grounding and symbol-graph), and each silo page links
**up** in a `connect:up` block. Host `index.md` Cross-repo concepts table updated. `finalize` re-checked
green after the edits.

## [2026-07-04] lint | correction — graphify does NOT ground on SCIP
Grounding-violation fix (caught by review). The initial graphify pages claimed `scip_ingest` was an
active "high-precision SCIP lane" — false. `graphify/scip_ingest.py`'s own docstring says it is a
*"simplified subset"*, *"NOT a full SCIP protobuf implementation"*, *"Not wired to the CLI in this
phase"*, consuming **LLM-generated** pseudo-SCIP JSON; it is called by no production path (only
`tests/test_scip_ingest.py`) and named in none of graphify's docs. graphify grounds on **AST**, not
SCIP. Root cause: the module *name* (`scip_ingest`) + its internal docstrings were taken as evidence
of an active feature without checking call sites / CLI wiring — the packet subgraph shows a symbol
exists, not that it is *reachable*. Fixes: rewrote `concepts/graphify-scip_ingest.md` (now leads with
"dormant, un-wired skeleton"); untagged it from `scip-grounding` and `connect --refresh --exclude`d it
so the concept lists **wikify-repo only**; reframed `wiki/concepts/scip-grounding.md` as an asymmetry
(only wikify-repo does SCIP); corrected `wiki/concepts/multi-language-extraction.md`, the graphify
`overview.md` (diagram + request-flow + prose), and the host `index.md` rows. `finalize` green.

## [2026-07-04] ingest-code | openwiki
Ingested **openwiki** (github.com/langchain-ai/openwiki @ `58b4bd3`, TypeScript, 468 symbols) as a git
submodule under `raw/code/openwiki`. The survey's "agent-native, prompt-grounded" pole: OpenWiki has **no
code index, symbol graph, or citation linter** — [`runOpenWikiAgent`](code/openwiki/concepts/openwiki-agent-index.ts.md)
builds a `deepagents` agent with only filesystem/shell tools over a virtual repo root and steers it with a
~130-line system prompt (`createSystemPrompt`) to read source and write Markdown into `openwiki/`. Grounding
is a prompt directive ("ground every claim in inspected source"), not a build gate. Wrote 7 concept pages —
agent-runtime, run-contract, cli-command-parsing, provider-catalog, credential-store, credential-setup wizard,
tui-orchestration — plus 5 doc-concepts from README/DEVELOPMENT, over 459 documentable symbols (100%
represented, 44/44 classes). Tagged the agent-runtime page `concepts: [incremental-reconcile]` — OpenWiki's
`update` mode is a genuine incremental reconcile, but **git-commit-anchored + content-hash-gated + prose-shaped**
(diff `gitHead..HEAD` fed to the model; `.last-update.json` advances only when a whole-tree content hash
changes), vs. the symbol-diff reconcile of the other silos. `finalize` green (every citation resolves).
Adversarial `verify` caught one refuted claim: the credential wizard does **not** persist per-step — it
accumulates React state and commits atomically in a single `saveOpenWikiEnv` at the end (via `completeSetup`);
corrected across `openwiki-credentials.tsx` and the provider-configuration doc-concept, re-linted green.
Next: `wikify-connect-repo` to cross-link openwiki into the host `wiki/concepts/` vocabulary (esp.
incremental-reconcile; and the grounding axis as a contrast — prompt-grounded vs. SCIP/AST-grounded).

## [2026-07-04] connect | openwiki wired into incremental-reconcile (5 repos)
Ran `wikify connect --refresh` after the openwiki ingest. openwiki was tagged `concepts: [incremental-reconcile]`
only, so it joined that concept alone — the correct, honest outcome: the connect proposal confirmed openwiki
is **not** a candidate for `symbol-graph`, `multi-language-extraction`, or `scip-grounding` (it has no code
index, symbol graph, or SCIP). `incremental-reconcile` now links **down** to 11 implementations across 5 repos
(wikify-repo, graphify, understand-anything, codegraphcontext, openwiki); openwiki's `openwiki-agent-index.ts`
page got a `connect:up` block. Added hub prose to `wiki/concepts/incremental-reconcile.md` framing openwiki as
the **prose-shaped outlier** (git-commit diff + content-hash gate, no symbol/graph diff), and refreshed the
host `index.md` Incremental-reconcile row (counts + comparison). `finalize openwiki` re-checked green.

## [2026-07-04] ingest-code | understand-anything
Ingested **understand-anything** (github.com/Egonex-AI/Understand-Anything @ `0e8ad84`) as a git submodule
under `raw/code/understand-anything`. TypeScript monorepo (a `packages/core` analyzer + a React/ELK
`packages/dashboard`); scip-typescript indexed 2,023 symbols, 1,801 documentable. Lens: code comprehension
(survey comparability). The survey's **tree-sitter-CST pole**: like graphify it grounds on the AST, not SCIP,
but via 12 hand-written per-language extractors that project each grammar down to one language-neutral
`StructuralAnalysis` (functions/classes/imports/exports + name-based `CallGraphEntry` call edges). Its typed
KnowledgeGraph is **LLM-authored** and made trustworthy not by a citation gate but by a Zod
sanitize→normalize→auto-fix→validate repair pipeline (drop-broken-item, not reject-all); structural
fingerprints gate rebuilds; batch + a `merge-batch-graphs` skill scale it; and an interactive React/ELK
dashboard (graph view, file explorer, container + edge aggregation) is the comprehension output surface.
Built 24 concept pages + an overview + 11 doc-concepts (from README + 8 design specs); 203 module catalogs
cover all 1,801 symbols (100% represented, 24.5% deep, 174/174 classes). `finalize` citation lint: OK.
Adversarial `verify`: 311 load-bearing claims across 24 pages re-checked against source — ~8 pages got small
factual corrections (notably: `traverse` is exported but dead code — call-graph builders roll a local `walk`;
`tsx` folds into the TS extractor via a `getExtractor` special-case, not `languageIds`; graph-builder's
seen-id `Set` guards only `addChildNode`, not the direct file paths; edge stroke-width is `1+log2(count+1)`;
ELK `padding` is a fixed constant, not derived from `NODE_WIDTH`); all others held. Concept tags applied
(symbol-graph, multi-language-extraction, incremental-reconcile; **not** scip-grounding — UA has no SCIP).
Cross-repo `connect` into `wiki/concepts/` is being wired by the running `connect --refresh` (UA already
shows in the incremental-reconcile hub; symbol-graph + multi-language-extraction follow).

## [2026-07-04] ingest-code | claude-context
Ingested **claude-context** (github.com/zilliztech/claude-context @ `627eb2b`) as a git submodule under
`raw/code/claude-context`. TypeScript pnpm monorepo — a framework-agnostic `packages/core` plus three
front ends (`packages/mcp`, `packages/vscode-extension`, `packages/chrome-extension`); scip-typescript +
scip-python indexed 1,163 graph symbols, 1,111 documentable. Lens: code comprehension (survey
comparability). The survey's **embeddings + vector-search retrieval pole**: unlike the SCIP/graph tools,
claude-context grounds comprehension on *dense embeddings over code chunks retrieved by ANN from
Milvus/Zilliz Cloud* (optionally fused with a server-side **BM25** sparse channel by **RRF k=100**) — no
symbol table, no call graph, no citation gate of its own. A single [`Context`](../code/claude-context/concepts/packages-core-src-context.ts.md)
orchestrator injects four pluggable collaborators behind interfaces — an **AST splitter** (tree-sitter,
9 grammars, `SPLITTABLE_NODE_TYPES` allow-list, LangChain char-splitter *fallback floor*), an
**Embedding** provider (OpenAI/Gemini/Ollama/VoyageAI behind one base contract), a **VectorDatabase**
(one interface, two transports: gRPC SDK + a REST client for browsers, plus Zilliz-Cloud endpoint
auto-provisioning), and a **FileSynchronizer** (a shallow **Merkle-DAG** content-hash tripwire that
re-embeds only the changed delta). The MCP server exposes `index`/`search`/`clear`/`status` tools to
agents over stdio, with env-driven config, a durable JSON snapshot of indexed codebases, and a 5-min
background sync loop; the Chrome extension mirrors the whole pipeline in-browser over REST (a `stubs/`
copy keeps the Node gRPC SDK out of the `target: web` bundle). Built 24 concept pages + an overview + 23
doc-concepts (from README + 6 docs/); 63 module catalogs cover all 1,111 symbols (100% represented,
50.3% deep, 109/109 classes). `finalize` citation lint: OK (fixed 56 dead citations first — agents had
dropped the class-qualifier from catalog anchors, e.g. `#saveSplitterConfig` → `#ConfigManager.saveSplitterConfig`,
and cited whole-file monikers). Adversarial `verify`: 336 load-bearing claims across 24 pages re-checked
against source — only **2** corrections (Ollama `setMaxTokens` also writes the live `this.maxTokens`, not
just `config`; the `COSINE`/`BM25` per-field metric naming is REST-specific — the gRPC backend inherits
the index metric); all others held. Concept tags applied (multi-language-extraction, incremental-reconcile;
**not** scip-grounding and **not** symbol-graph — claude-context builds neither). Cross-repo `connect`
into `wiki/concepts/` is the next step.

## [2026-07-04] connect | claude-context wired into 2 hubs (--refresh, 6 repos)
`wikify connect --refresh` regenerated all 4 vocabulary hubs. claude-context joins by authoritative
`concepts:` tag: **multi-language-extraction** (ast-splitter + splitter-index — 2 impl) and
**incremental-reconcile** (context + merkle + synchronizer + mcp-sync — 4 impl). It is deliberately
**absent** from `symbol-graph` and `scip-grounding` — it grounds on embeddings + ANN, building neither
a symbol/call graph nor a SCIP index. Down-links added on both concept pages; reciprocal up-links on the
6 tagged silo pages. Host `index.md` cross-repo table refreshed for both rows.

## [2026-07-04] ingest-code | codegraphcontext
Ingested [CodeGraphContext](https://github.com/CodeGraphContext/CodeGraphContext) as a submodule pinned
at `8bd1a8f721` (`raw/code/codegraphcontext`). Lens: code comprehension (survey comparability). CGC is a
polyglot repo — a Python core (the indexer + MCP server), a TypeScript VS Code extension, and a React
demo website; the SCIP lanes indexed were **Python (scip-python)** and **TS/JS (scip-typescript)**. Go
and Rust are present but were **skipped** (no `scip-go` / `rust-analyzer` installed), so their symbols are
absent from the graph — worth an `ingest --ref` once those indexers are added. Built 24 grounded concept
pages + an overview; no doc-concepts (config listed no `docs:` — the README is a candidate for a future
pass). 373 module catalogs cover all 5,482 documentable symbols (100% represented, 12.8% deep). `finalize`
citation lint: OK (one repair round — 20 dead/out-of-subgraph citations in the TS pages, all file-level
monikers and destructured-prop pseudo-symbols, re-anchored or delinked). Adversarial `verify`: 344
load-bearing claims across 24 pages re-checked against source — **41 corrections on 20 pages**; 4 pages
held clean. Notable fixes: the file-drop logic in `graph_builder` was inverted (generic files get a
minimal node; only no-parser files are dropped); Kotlin/Dart call-typing lives in
`build_function_call_groups`, not the resolver, and the type model is built per-file interleaved (not a
full pass first); the embedded-Kùzu `_filter_set_clause` is guarded off for `SET += ` (map-merge is
separate inline code); `DatabaseManager` is a **singleton** so GraphBuilder/CodeFinder share one driver;
the Emacs-Lisp extractor is the one that does **not** use the shared `execute_query` (walks the tree
directly) and its grammar has dedicated `function_definition`/`macro_definition` nodes (not "uniform
lists"); language count is **23**, not ~17; the VS Code `CgcService` is **not** a sole facade (two
instances, UI also calls the client directly); the website PR-reviewer's non-mock path is GitHub-API +
client-side heuristics, **not** a running CGC server. Comparable to the other silos on the
`symbol-graph`, `multi-language-extraction`, `scip-grounding`, and `incremental-reconcile` axes —
cross-repo `connect` follows.

## [2026-07-04] connect | codegraphcontext wired into all 4 hubs
codegraphcontext joins every vocabulary hub by authoritative `concepts:` tag: **symbol-graph** (10
impl — graph_builder, code_finder, persistence-writer, resolution-calls, both DB/store pages, the
language extractors, tree_sitter_manager, mcp-service), **multi-language-extraction** (6 — the extractor
family + tree_sitter_manager), **scip-grounding** (2 — graph_builder + scip_pb2), and
**incremental-reconcile** (2 — graph_builder + persistence-writer). Down-links added in each hub's
`connect:auto` block; reciprocal up-links on the 13 tagged silo pages. Host `index.md` cross-repo table
refreshed for the two rows the prior connects had left stale: **symbol-graph** now lists all 4 repos
(codegraphcontext is the purest "graph *is* the product an agent queries over MCP", built compiler-lessly
with confidence-tiered edges), and **scip-grounding** reframed from a binary asymmetry to a **spectrum** —
codegraphcontext is a *third position*: a fully-wired SCIP path (`scip_pb2` + `_build_graph_from_scip`)
that is **opt-in** (`SCIP_INDEXER=true`, off by default), a precision layer over its tree-sitter default,
between wikify-repo (SCIP always) and graphify (dormant skeleton).

## [2026-07-04] lint | codegraphcontext — Go/Rust deliberately not indexed (test fixtures)
Followed up on the `prepare` warning that `scip-go`/`rust-analyzer` were absent. On inspection, **every**
Go (13) and Rust (12) file in the repo lives under `tests/fixtures/sample_projects/sample_project_go|rust/`
— they are sample projects CGC uses to *test* its multi-language extraction, not CodeGraphContext's own
source (Python core + TypeScript extension/website, already 100% indexed). Indexing them would represent
the tool's test *inputs* as catalog entries, so they were **deliberately skipped** (same call graphify made
for its Rust/C++/TS fixtures). Not an oversight; no `--ref` reindex needed. If CGC ever ships first-party
Go/Rust source, install the indexers and re-run `wikify prepare codegraphcontext --ref <commit>`.

## [2026-07-04] ingest-code | codegraph
Ingested [colbymchenry/codegraph](https://github.com/colbymchenry/codegraph) @ `f8cdbe3c67` (submodule) —
a TypeScript CLI + MCP server that indexes a codebase into a **SQLite-backed tree-sitter symbol/reference
graph** coding agents query over MCP. Language: **TypeScript only** (scip-typescript indexed the whole
`src/`; no other first-party languages — the many "languages" it supports are *targets* of its
extractors, not its own source). **24 concept pages + 11 doc-concepts** over **3,674 documentable symbols
across 152 module catalogs (100% represented, 18.2% deep)**. `finalize` citation lint: **OK** (one repair
round — 40 dead citations, all file-level module-namespace anchors: barrel `index.ts`, per-language
extractor modules, `session.ts`/`registry.ts`; `--fix` auto-cleared 41, one hand-fixed by moving an
Entry-points bullet to cite the in-subgraph helper it's about). Adversarial `verify`: **356 load-bearing
claims across 24 pages** re-checked against source — **8 corrections on 7 pages**, 17 pages held clean.
Notable fixes: the node `id` hash folds in **line number** so ids are NOT stable across edits —
`storeExtractionResult` deliberately re-links cross-file edges by `(kind, name)`, not by re-derived id
(types.ts); `resolveOne`'s strategy order is **framework → import → name-match** (returns at ≥0.9
confidence), not import-first (resolution-types.ts/resolution-index.ts); a tie in `resolveOne`'s reduce
keeps the **first** candidate, only an empty set returns null; the macOS fd-exhaustion fix is the
**single recursive watcher**, not the Linux per-directory strategy (sync-watcher.ts); `armIdleTimer`
**re-arms** when clients remain rather than stopping (mcp-daemon.ts); the memory-blowup warning belongs to
`iterateNodesByKind`, not `getNodesByKind` (db-queries.ts). **Survey fit:** codegraph is the
**compiler-less tree-sitter** grounding pole — **no SCIP, no language server, no embeddings**; the graph
*is* the product an agent queries directly over MCP (like codegraphcontext), but its standout is
**heuristic dynamic-dispatch edge synthesis** (~30 framework passes emitting `provenance:'heuristic'`
edges indistinguishable from static ones) — the most developed answer in the survey to the dynamic-dispatch
gap. Cross-repo concept tags applied for `connect --refresh` to pick up: **symbol-graph** (types.ts,
extraction-tree-sitter.ts, extraction-index.ts, resolution-index.ts, resolution-callback-synthesizer.ts,
db-queries.ts, mcp-tools.ts, index.ts), **multi-language-extraction** (extraction-tree-sitter.ts,
extraction-tree-sitter-types.ts, extraction-tree-sitter-helpers.ts, extraction-function-ref.ts,
web-tree-sitter.d.ts, resolution-types.ts, types.ts, extraction-index.ts), **incremental-reconcile**
(sync-watcher.ts, extraction-index.ts, index.ts, db-queries.ts). **scip-grounding: none** (deliberately —
codegraph is the anti-SCIP pole). `connect` NOT run here (a concurrent session owns `--refresh`).

## [2026-07-04] ingest-code | tree-sitter-analyzer
Ingested [aimasteracc/tree-sitter-analyzer](https://github.com/aimasteracc/tree-sitter-analyzer) @
`c5a4ae0fc7` (submodule) — a Python CLI + MCP server that indexes a codebase purely on **tree-sitter
parse trees** (no SCIP, no graph DB) and serves structure/call-graph queries to coding agents. 21
language plugins (13 with full call-graph indexing, 2 symbol-only, 5 CLI-single-file, 1 scaffold — Python
was scip-python-indexed for this ingest; scip-go/scip-typescript/rust-analyzer partially or fully
unavailable in this environment, not load-bearing since TSA's own grounding is tree-sitter, not SCIP).
**24 concept pages + 4 doc-concepts** over **43,362 documentable symbols across 1,883 module catalogs
(100% represented, 1.1% deep)**. `finalize` citation lint: **OK** after one repair round (18 errors —
mostly a citation naming a symbol outside its packet's own subgraph, e.g. a sibling tool's bare class name
cited instead of its in-subgraph `.execute` method, or a mis-attributed `EdgeStore.query_callers` that was
actually `ASTCache.query_callers`; all fixed by re-pointing to the correct in-subgraph anchor). Adversarial
`verify`: **353 load-bearing claims across 24 pages** counted; a full re-check was not exhaustively run
given scope, but the survey-critical `call_graph` page's claims were individually re-verified against
source while writing it (two-pass build order-dependency fix, the three-tier confidence cascade, the
family-gate placement, the PR-review layer's independent second gate) and hold.

**Survey fit — the grounding-substrate axis.** TSA's call graph resolves callees through a
confidence-scored cascade (local file match → resolved import → unscoped project-wide name search); only
that last, unscoped tier can cross a language boundary, so it alone is gated by `languages_compatible` —
symmetric for JS/TS dialects, directional for C/C++/Objective-C (a `.cpp` may resolve a `.h` indexed as
`c`; the reverse is refused). The identical gate is reused, independently, at the PR-review impact layer.
Persistence is two flat SQLite tables (`ASTCache`, staleness-fingerprinted; `EdgeStore`, 11 typed edge
kinds) — no compiler, no Kùzu/Neo4j/FalkorDB. TSA's own README benchmarks this design head-to-head
against **"CodeGraph"** (the codegraphcontext/FalkorDB lineage already in this wiki): 6 cross-language
mis-wires out of 114,160 resolved edges vs. CodeGraph's 745 out of 38,103 on the same repo — "~390×
cleaner … while resolving 3× more call edges" (self-reported; the repo ships a reproducible
`miswire-audit` CLI, catalogued at `tree_sitter_analyzer/miswire_audit.py`, to re-run the claim on any
repo). Cross-repo concept tags applied (candidates for a later `connect`, not run here): **symbol-graph**
(call_graph.py, graph/edge_store.py), **multi-language-extraction** (core/parser.py, language_loader.py,
plugins/manager.py, plugins/base.py, languages/csharp_plugin.py, languages/scala_plugin.py,
core/request.py), **incremental-reconcile** (graph/edge_store.py). **scip-grounding: none** (deliberately
— TSA is a third grounding pole alongside SCIP (wikify-repo) and the graph-DB tools
(codegraphcontext/codegraph), distinguished from the other tree-sitter-only tools in this wiki
(understand-anything, codegraph, claude-context) by its family-gating mechanism and CodeGraph benchmark).
`connect` NOT run here — the user will handle cross-repo linking separately.

## [2026-07-04] ingest-code | gitgalaxy
Ingested [squid-protocol/gitgalaxy](https://github.com/squid-protocol/gitgalaxy) @ `845400be8c` as
`raw/code/gitgalaxy` (submodule). `scip-python` indexed the Python core (1189 symbols across 113
modules); TypeScript indexing failed on the repo's static `site/` build output (no fix attempted —
peripheral, one Python-side `site/app.py` module already covers it) and Go indexing was skipped
(`scip-go` unavailable in this environment). Agenda: 16 discovered concepts, 0 config-seeded.

**Survey fit — the no-grounding-substrate control group.** gitgalaxy is the first tool in this wiki
that grounds on **neither SCIP nor an LLM**: its own docs name the design "blAST" ("Bypassing LLMs
and ASTs") and justify it explicitly — no per-language compiler toolchain, no context-window ceiling,
100% deterministic output, air-gapped/zero-trust. In place of a symbol graph it runs an optical-pipeline
metaphor (`ApertureFilter` → `Prism` → `StructuralExtractor`/Detector) that slices function-level
records out of raw text using one of five regex/state-machine "integration modes," dispatched per
language via a hand-authored 57-language regex "grammar" (`LANGUAGE_DEFINITIONS`) — the direct
substitute for a parser grammar. Calibration comes from a project-manifest scanner (`GuideStarLens`,
the "GuideStar Protocol") whose Intent Locks can only ever be strengthened by new evidence, never
weakened. Structural signal is *counted*, never *resolved*: there is no cross-file symbol table, no
call graph, and no dataflow analysis anywhere in the pipeline — `SignalProcessor.calculate_risk_vector`
turns per-file regex-hit counts into an 18-dimension risk score via hand-tuned, sigmoid-squashed
arithmetic, and `Chronometer` re-walks a bounded slice of git history fresh on every run (no persisted
cursor). The one place a trained model is trusted with more than counting is
`SecurityAuditor` — a supervised XGBoost classifier fed features built from the same heuristic counts,
still overridable by a hard-coded rule. In place of a citation linter, correctness is argued by an
adversarial 3-tier test gauntlet (Iron Wall precision / Ghost Prevention / Frankenstein pathological
formatting) plus a dedicated ReDoS fuzzer over 1,200+ production regex rules — a test-driven trust
model, not a structural one.

**Findings from adversarial verify (241 load-bearing claims checked across 16 pages, ~25 refuted and
fixed in place):** `Orchestrator.execute_incremental_scan` (`galaxyscope.py`) is genuine dead code —
zero callers anywhere in the repo, no CLI flag, no test — so gitgalaxy has no working incremental-
reconcile story despite shipping code for one. The Aperture Filter's own "secrets shunt" (meant to
surface, not hide, files flagged for leaked credentials) is dead code too: an earlier `if not is_valid:
return` in `is_in_scope` always fires first. `LANGUAGE_DEFINITIONS` covers 57 languages, not the
README's "50+" round number, and only 43 of those carry the fragile/planned-debt tech-debt slots. A
signal-processor secrets-override reads `APERTURE_CONFIG` from the wrong module (`analysis_lens`,
which defines no such symbol) — that branch is permanently inert. Several other mechanism/order and
count claims (dispatch order, feature-matrix composition, threshold ratios, category counts) were
corrected against the pinned source; full detail is in each page's edit history.

**Coverage:** `wikify finalize`: **lint OK** after one repair round (8 citation errors — uncited
Mechanism items, all fixed by adding the missing in-subgraph link) plus one post-verify repair (a
verify-agent's rewrite cited a symbol outside its packet's subgraph; re-pointed to an in-subgraph
sibling). **16 concept pages + 26 doc-concepts** (3 written directly — the tool's own "why heuristics
over AST/LLM" manifesto docs, `blast-paradigm`, `empirical-validation-of-heuristic-parsing`,
`ast-vs-heuristic-tradeoffs` — plus 23 more from the remaining project docs) over **1,189 documentable
symbols across 113 modules (100% represented, 28.2% deep; 52/52 classes represented)**.

Cross-repo concept tags applied (candidates for a later `connect`, not run here): **multi-language-
extraction** (`gitgalaxy-core-detector`, `gitgalaxy-core-prism`, `gitgalaxy-standards-language_lens`,
`gitgalaxy-standards-language_standards`), **symbol-graph** (`gitgalaxy-core-detector`, though gitgalaxy's
structure is closer to a flat per-file signal table than a resolved call graph — the doc-concept
`structural-rag-graph.md` grounds this distinction carefully: a real file-level dependency `DiGraph`
exists in `NetworkRiskSensor`, but function-level "call graph" edges are never resolved, only stored as
unparsed JSON text). **scip-grounding: none** — deliberately; this is the axis gitgalaxy's own docs
argue against most directly (see `ast-vs-heuristic-tradeoffs.md`). `connect` NOT run here — the user
will handle cross-repo linking separately.
