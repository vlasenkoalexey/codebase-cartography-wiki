---
title: 'Module: gitgalaxy/tools/cobol_to_java/cobol_to_java_spring_forge.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/cobol_to_java/cobol_to_java_spring_forge.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.cobol_to_java.cobol_to_java_spring_forge`/
symbols:
  generate_java_entity: generate_java_entity().
  main: main().
  parse_pic_clause: parse_pic_clause().
  parse_pic_clause.count_nines: parse_pic_clause().count_nines().
  map_type_to_java: map_type_to_java().
---
# Module: [`gitgalaxy/tools/cobol_to_java/cobol_to_java_spring_forge.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_spring_forge.py)

## Functions
- `count_nines(part)` — [`L74`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_spring_forge.py#L74)
- `generate_java_entity(schema_json: dict, package_name: str)` — [`L96`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_spring_forge.py#L96) — Generates a JPA Entity enforcing exact COBOL memory constraints & overlaps.
- `main()` — [`L225`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_spring_forge.py#L225)
- `map_type_to_java(json_type: str, description: str)` — [`L26`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_spring_forge.py#L26) — Maps JSON schema types to Java classes.
- `parse_pic_clause(description: str)` — [`L35`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_spring_forge.py#L35) — Analyzes COBOL PIC, OCCURS, and REDEFINES clauses in the description

