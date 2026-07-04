---
slug: tree-sitter-analyzer
repo: https://github.com/aimasteracc/tree-sitter-analyzer
acquire: submodule
docs:
  - README.md
synthesis_focus: >-
  Code comprehension — how tree-sitter-analyzer grounds a codebase on tree-sitter
  (rather than SCIP or a graph DB): its multi-language (13-language) parsing
  pipeline, how it builds a call graph with family-gating (restricting edge
  resolution to type/language-compatible symbol families to avoid cross-language
  mis-wires), and how it exposes structure/query results to an agent (CLI/MCP).
  Emphasize what makes it comparable to the other surveyed tools for the
  cross-repo concept pages — specifically the grounding substrate axis: tree-sitter
  parse trees + family-gating vs. wikify-repo's SCIP symbol graph vs. the graph-DB
  approach in codegraphcontext/CodeGraph — and surface the README's claimed
  cross-language call-graph accuracy comparison against "CodeGraph"
  (codegraphcontext/FalkorDB lineage).
---

## Concepts
<!-- Auto-seeded from code centrality. Add seed concepts here to go deeper into a subsystem. -->
