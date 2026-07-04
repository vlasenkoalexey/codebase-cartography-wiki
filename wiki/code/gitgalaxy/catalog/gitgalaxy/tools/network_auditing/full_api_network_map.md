---
title: 'Module: gitgalaxy/tools/network_auditing/full_api_network_map.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/network_auditing/full_api_network_map.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.network_auditing.full_api_network_map`/
symbols:
  main: main().
  run_api_audit: run_api_audit().
  parse_official_swagger: parse_official_swagger().
  map_physical_codebase: map_physical_codebase().
  auto_discover_swagger: auto_discover_swagger().
  FRAMEWORK_SIGNATURES: FRAMEWORK_SIGNATURES.
---
# Module: [`gitgalaxy/tools/network_auditing/full_api_network_map.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/network_auditing/full_api_network_map.py)

## Functions
- `auto_discover_swagger(target_dir: Path)` — [`L90`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/network_auditing/full_api_network_map.py#L90) — Scans for OpenAPI/Swagger specifications via filename and internal structural signatures.
- `main()` — [`L194`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/network_auditing/full_api_network_map.py#L194) — documented in [gitgalaxy-licensing](../../../../concepts/gitgalaxy-licensing.md)
- `map_physical_codebase(target_dir: Path)` — [`L159`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/network_auditing/full_api_network_map.py#L159) — Analyzes the source code to extract every executable API endpoint.
- `parse_official_swagger(swagger_path: Path)` — [`L133`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/network_auditing/full_api_network_map.py#L133) — Parses the official security documentation to extract a baseline of approved APIs.
- `run_api_audit(source_path: Path)` — [`L335`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/network_auditing/full_api_network_map.py#L335) — Programmatic entry point for GalaxyScope. — documented in [gitgalaxy-galaxyscope](../../../../concepts/gitgalaxy-galaxyscope.md)

## Module values
- `FRAMEWORK_SIGNATURES` — [`L32`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/network_auditing/full_api_network_map.py#L32)

