---
title: Local-first tree-sitter grounding
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Local-first tree-sitter grounding

## Definition
CodeGraph is a **pre-built knowledge graph of every symbol, call edge, and dependency** in a codebase, and it is built **100% locally** — no data leaves the machine, no API keys, no external services, SQLite only. Crucially the graph is **deterministic**: symbols and edges are derived from the tree-sitter AST, *not* LLM-summarized. This is what makes it trustworthy grounding for an agent — the returned source is the real source at a real line, across **20+ languages** (TypeScript, Python, Go, Rust, Java, C/C++, CUDA, Swift, Kotlin, Ruby, and many more), each supported automatically from the file extension with zero per-language config.

## In codegraph (grounded)
The README's three-stage pipeline — **Extraction → Storage → Resolution** — maps directly onto the code:

1. **Extraction.** tree-sitter parses source into ASTs; language-specific queries extract nodes and edges. The core walker is [`TreeSitterExtractor.extract`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.extract) / [`extractFromSource`](../catalog/src/extraction/tree-sitter.ts.md#extractFromSource) in **`src/extraction/tree-sitter.ts`**, emitting nodes via [`TreeSitterExtractor.createNode`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.createNode) and call edges via [`TreeSitterExtractor.extractCall`](../catalog/src/extraction/tree-sitter.ts.md#TreeSitterExtractor.extractCall). The crawl over a whole project is driven by [`ExtractionOrchestrator.indexAll`](../catalog/src/extraction/index.ts.md#ExtractionOrchestrator.indexAll) / [`indexFile`](../catalog/src/extraction/index.ts.md#ExtractionOrchestrator.indexFile) in **`src/extraction/index.ts`**.
2. **Zero-config file selection.** The README's "your code, not third-party noise" promise is the ignore machinery in the orchestrator — [`buildDefaultIgnore`](../catalog/src/extraction/index.ts.md#buildDefaultIgnore) / [`DEFAULT_IGNORE_PATTERNS`](../catalog/src/extraction/index.ts.md#DEFAULT_IGNORE_PATTERNS) skip `node_modules`, `dist`, `.venv`, etc.; [`MAX_FILE_SIZE`](../catalog/src/extraction/index.ts.md#MAX_FILE_SIZE) drops files over 1 MB (minified bundles, vendored blobs).
3. **The node/edge vocabulary.** Every extractor and resolver emits the exact strings in **`src/types.ts`**: the [`NodeKind`](../catalog/src/types.ts.md#NodeKind) union (`class`, `function`, `method`, `route`, `component`, …) and the [`EdgeKind`](../catalog/src/types.ts.md#EdgeKind) union (`calls`, `imports`, `extends`, `implements`, `references`, …), carried on [`Node`](../catalog/src/types.ts.md#Node) and [`Edge`](../catalog/src/types.ts.md#Edge) records tagged with a [`Language`](../catalog/src/types.ts.md#Language).
4. **Resolution.** After extraction, references are resolved (calls→definitions, imports→sources, inheritance, framework routes) via [`CodeGraph.resolveReferences`](../catalog/src/index.ts.md#CodeGraph.resolveReferences).

Storage itself is a local SQLite DB (`.codegraph/codegraph.db`) with FTS5 full-text search — the graph the extraction fills in.

## Why it matters / when it applies
Because extraction is deterministic and local, the agent can **trust results without re-verifying** — the README explicitly tells it not to re-grep. It also means the tool works offline on private code with no keys. The breadth of languages (and content-based detection for CUDA in `.h`/`.hpp`, MSL-as-C++ for Metal, etc.) is what lets a single tool answer questions on any repo the agent opens. Where static parsing *can't* reach — runtime dynamic dispatch, reflection, DI containers — the README is honest that those are a genuine static-analysis frontier, bridged only by explicit synthesizers.

## Connections
- Code concepts: [extraction-tree-sitter.ts](../concepts/extraction-tree-sitter.ts.md) — the AST walker in depth; [extraction-index.ts](../concepts/extraction-index.ts.md) — the orchestrator, ignore rules, and sync; [extraction-tree-sitter-types.ts](../concepts/extraction-tree-sitter-types.ts.md) and [extraction-tree-sitter-helpers.ts](../concepts/extraction-tree-sitter-helpers.ts.md) — the extractor contract and shared helpers; [extraction-parse-pool.ts](../concepts/extraction-parse-pool.ts.md) — off-main-thread parsing; [types.ts](../concepts/types.ts.md) — the NodeKind/EdgeKind vocabulary; [resolution-index.ts](../concepts/resolution-index.ts.md) and [resolution-callback-synthesizer.ts](../concepts/resolution-callback-synthesizer.ts.md) — reference resolution and dynamic-dispatch bridging.
- Module catalogs: [extraction/tree-sitter.ts](../catalog/src/extraction/tree-sitter.ts.md), [extraction/index.ts](../catalog/src/extraction/index.ts.md), [types.ts](../catalog/src/types.ts.md).
- Related doc-concepts: [mcp-tool-surface](mcp-tool-surface.md) — what reads this graph; [init-and-autosync](init-and-autosync.md) — when extraction runs.

## Source
Extracted from `README.md` (kept in place) — the "Key Features", "How It Works", "Configuration", and "Supported Languages" sections.
