---
slug: claude-context
repo: https://github.com/zilliztech/claude-context
acquire: submodule
docs:
  - README.md
  - docs/dive-deep/asynchronous-indexing-workflow.md
  - docs/dive-deep/file-inclusion-rules.md
  - docs/getting-started/quick-start.md
  - docs/getting-started/environment-variables.md
  - docs/getting-started/prerequisites.md
  - docs/troubleshooting/faq.md
synthesis_focus: >-
  Code comprehension — how claude-context makes an entire codebase semantically
  searchable for coding agents: its ingest/indexing pipeline, how it chunks and
  represents code (AST-aware splitting, embeddings, vector store), the semantic
  retrieval/search path, incremental sync (Merkle-tree change detection), and
  the MCP-server interface that exposes search to agents. Emphasize what makes it
  comparable to the other surveyed tools (wikify-repo, graphify,
  understand-anything) for the cross-repo concept pages — e.g. the grounding
  substrate (embeddings/vector search vs. SCIP symbol graph vs. knowledge graph),
  multi-language extraction, and incremental reconcile.
---

## Concepts
<!-- Auto-seeded from code centrality. Add seed concepts here to go deeper into a subsystem. -->
