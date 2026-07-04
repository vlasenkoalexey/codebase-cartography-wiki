---
title: 'Module: gitgalaxy/tools/cobol_to_cobol/cobol_compiler_forge.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/cobol_to_cobol/cobol_compiler_forge.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.cobol_to_cobol.cobol_compiler_forge`/
symbols:
  main: main().
  flatten_copybooks: flatten_copybooks().
  generate_build_jcl: generate_build_jcl().
  MAX_RECURSION_DEPTH: MAX_RECURSION_DEPTH.
  detect_cobol_dialect: detect_cobol_dialect().
  extract_intent: extract_intent().
---
# Module: [`gitgalaxy/tools/cobol_to_cobol/cobol_compiler_forge.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_compiler_forge.py)

## Functions
- `detect_cobol_dialect(content: str)` — [`L25`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_compiler_forge.py#L25) — Scans for post-1974 structural signatures to determine the compiler era.
- `extract_intent(source_text: str)` — [`L86`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_compiler_forge.py#L86) — Extracts the program identity and file assignment boundaries.
- `flatten_copybooks(source_text: str, base_dir: Path, current_depth: int = 0)` — [`L36`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_compiler_forge.py#L36) — Recursively inlines COPY statements to create a self-contained execution payload.
- `generate_build_jcl(source_text: str, prog_name: str, files: set, dialect: str)` — [`L102`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_compiler_forge.py#L102) — Generates the JCL deployment configuration mapping program files to physical data sets.
- `main()` — [`L167`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_compiler_forge.py#L167)

## Module values
- `MAX_RECURSION_DEPTH` — [`L22`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_compiler_forge.py#L22)

