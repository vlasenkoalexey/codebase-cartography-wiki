---
title: 'Module: gitgalaxy/tools/cobol_to_cobol/cobol_graveyard_finder.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/cobol_to_cobol/cobol_graveyard_finder.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.cobol_to_cobol.cobol_graveyard_finder`/
symbols:
  main: main().
  x_ray_dead_code: x_ray_dead_code().
  resolve_copybooks: resolve_copybooks().
  resolve_copybooks.replacer: resolve_copybooks().replacer().
---
# Module: [`gitgalaxy/tools/cobol_to_cobol/cobol_graveyard_finder.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_graveyard_finder.py)

## Functions
- `main()` — [`L165`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_graveyard_finder.py#L165)
- `replacer(match)` — [`L42`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_graveyard_finder.py#L42)
- `resolve_copybooks(content: str, source_path: Path)` — [`L22`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_graveyard_finder.py#L22) — Recursively hunts for COBOL 'COPY' statements and injects the contents of the — documented in [gitgalaxy-cobol_refractor_controller](../../../../concepts/gitgalaxy-cobol_refractor_controller.md)
- `x_ray_dead_code(filepath: Path)` — [`L85`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_graveyard_finder.py#L85) — Parses a fully-expanded COBOL file to find mathematically unreachable logic and memory. — documented in [gitgalaxy-cobol_refractor_controller](../../../../concepts/gitgalaxy-cobol_refractor_controller.md)

