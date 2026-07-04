---
title: 'Module: gitgalaxy/tools/cobol_to_cobol/cobol_agent_task_forge.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/cobol_to_cobol/cobol_agent_task_forge.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.cobol_to_cobol.cobol_agent_task_forge`/
symbols:
  forge_agent_jobs: forge_agent_jobs().
  generate_agent_ticket: generate_agent_ticket().
---
# Module: [`gitgalaxy/tools/cobol_to_cobol/cobol_agent_task_forge.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_agent_task_forge.py)

## Functions
- `forge_agent_jobs(staging_dir: Path, source_dir: Path, architectural_anomalies: list)` — [`L54`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_agent_task_forge.py#L54) — Parses global architectural anomalies and generates individual JSON task tickets per file. — documented in [gitgalaxy-cobol_refractor_controller](../../../../concepts/gitgalaxy-cobol_refractor_controller.md)
- `generate_agent_ticket(file_name: str, source_file: Path, anomalies: list, ir_state: dict)` — [`L22`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_agent_task_forge.py#L22) — Generates a structured JSON task ticket for an autonomous agent.

