---
title: 'Module: gitgalaxy/tools/cobol_to_java/cobol_to_java_build_forge.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/cobol_to_java/cobol_to_java_build_forge.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.cobol_to_java.cobol_to_java_build_forge`/generate_
symbols:
  generate_pom_xml: pom_xml().
  generate_application_yml: application_yml().
  generate_main_class: main_class().
---
# Module: [`gitgalaxy/tools/cobol_to_java/cobol_to_java_build_forge.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_build_forge.py)

## Functions
- `generate_application_yml(artifact_id: str)` — [`L109`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_build_forge.py#L109) — Scaffolds the application.yml with standard Postgres and JPA configurations.
- `generate_main_class(package_name: str, class_name: str)` — [`L143`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_build_forge.py#L143) — Scaffolds the Spring Boot Application entry point.
- `generate_pom_xml(group_id: str, artifact_id: str)` — [`L19`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_java/cobol_to_java_build_forge.py#L19) — Scaffolds a production-ready Maven pom.xml for the microservice.

