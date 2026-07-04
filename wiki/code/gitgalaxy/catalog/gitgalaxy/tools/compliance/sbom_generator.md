---
title: 'Module: gitgalaxy/tools/compliance/sbom_generator.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/compliance/sbom_generator.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.compliance.sbom_generator`/
symbols:
  main: main().
  UniversalManifestSlicer.locate_physical_package: UniversalManifestSlicer#locate_physical_package().
  UniversalManifestSlicer.slice_manifest: UniversalManifestSlicer#slice_manifest().
  UniversalManifestSlicer: UniversalManifestSlicer#
---
# Module: [`gitgalaxy/tools/compliance/sbom_generator.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/compliance/sbom_generator.py)

## Classes
### `UniversalManifestSlicer`
- def: [`gitgalaxy/tools/compliance/sbom_generator.py:25`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/compliance/sbom_generator.py#L25)
- doc: Uses regex and standard parsing to slice dependencies from any ecosystem.
- signature: `class UniversalManifestSlicer:`
- members:
  - `locate_physical_package(target_path: Path, pkg_name: str, ecosystem: str)` — [`L128`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/compliance/sbom_generator.py#L128) — Hunts for the physical location of a package within the project bounds.
  - `slice_manifest(manifest_path: Path)` — [`L29`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/compliance/sbom_generator.py#L29)
- used by: [`main`](sbom_generator.md#main)  (2 test-only)

## Functions
- `main()` — [`L179`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/compliance/sbom_generator.py#L179) — documented in [gitgalaxy-licensing](../../../../concepts/gitgalaxy-licensing.md)

