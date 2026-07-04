---
slug: gitgalaxy
repo: https://github.com/squid-protocol/gitgalaxy
acquire: submodule
docs:
  - README.md
  - docs/gitgalaxy_architecture_brief.md
  - docs/wiki/01-01-project-overview.md
  - docs/wiki/01-03-the-blast-paradigm.md
  - docs/wiki/01-06-the-structural-rag-graph.md
  - docs/wiki/02-01-pipeline-overview.md
  - docs/wiki/02-02-optical-orchestration.md
  - docs/wiki/02-03-aperture-filter.md
  - docs/wiki/02-04-guidestar-protocol.md
  - docs/wiki/02-05-language-lens.md
  - docs/wiki/02-07-the-prism.md
  - docs/wiki/02-08-the-detector.md
  - docs/wiki/02-09-signal-processing.md
  - docs/wiki/03-08-claim-8-empirical-validation-of-ast-free-parsing.md
  - docs/wiki/03-10-claim-10-ast-vs-heuristic-parsing.md
synthesis_focus: >-
  Code comprehension — how GitGalaxy's "blAST" engine maps a codebase WITHOUT an AST
  and WITHOUT an LLM: its regex/heuristic structural-signature sequencing, the
  optical-pipeline metaphor (aperture filter, language lens, prism, detector) that
  turns raw source text into a 3D knowledge graph, and how it grounds architectural
  risk metrics in those heuristics instead of a parser or a model. This is the
  survey's "no grounding substrate" control group — emphasize what it deliberately
  gives up (AST precision, semantic understanding) and what it gets in exchange
  (linear-time, zero-dependency, air-gapped, 50+ language polyglot scanning) so it is
  directly comparable to the SCIP-grounded tools (wikify-repo), embedding tools
  (claude-context), and graph-DB tools (codegraphcontext, graphify) already in the
  survey.
---

## Concepts
<!-- Auto-seeded from code centrality. Add seed concepts here to go deeper into a subsystem. -->
