---
title: 'Module: gitgalaxy/tools/cobol_to_cobol/cobol_lexical_patcher.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/cobol_to_cobol/cobol_lexical_patcher.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.cobol_to_cobol.cobol_lexical_patcher`/
symbols:
  patch_lexical_traps: patch_lexical_traps().
  detect_cobol_dialect: detect_cobol_dialect().
---
# Module: [`gitgalaxy/tools/cobol_to_cobol/cobol_lexical_patcher.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_lexical_patcher.py)

## Functions
- `detect_cobol_dialect(content: str)` — [`L20`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_lexical_patcher.py#L20) — Scans for post-1974 structural signatures to determine the compiler era. — documented in [gitgalaxy-cobol_refractor_controller](../../../../concepts/gitgalaxy-cobol_refractor_controller.md)
- `patch_lexical_traps(filepath: Path)` — [`L35`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_lexical_patcher.py#L35) — Scans the file for NEXT SENTENCE. If found, rewrites it safely based on the — documented in [gitgalaxy-cobol_refractor_controller](../../../../concepts/gitgalaxy-cobol_refractor_controller.md)

