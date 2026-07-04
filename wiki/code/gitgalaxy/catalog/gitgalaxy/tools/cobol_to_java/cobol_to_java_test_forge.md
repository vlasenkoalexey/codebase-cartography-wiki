---
title: 'Module: gitgalaxy/tools/cobol_to_java/cobol_to_java_test_forge.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/cobol_to_java/cobol_to_java_test_forge.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.cobol_to_java.cobol_to_java_test_forge`/
symbols:
  main: main().
  generate_context_test: generate_context_test().
  generate_controller_test: generate_controller_test().
---
# Module: [`gitgalaxy/tools/cobol_to_java/cobol_to_java_test_forge.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_test_forge.py)

## Functions
- `generate_context_test(package_name: str, class_name: str)` — [`L23`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_test_forge.py#L23) — Generates a @SpringBootTest to ensure the entire dependency injection context loads.
- `generate_controller_test(package_name: str, class_name: str, endpoint_path: str)` — [`L47`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_test_forge.py#L47) — Generates a @WebMvcTest to verify REST API mappings without booting the full server.
- `main()` — [`L84`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_test_forge.py#L84)

