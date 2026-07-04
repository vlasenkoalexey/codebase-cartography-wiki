---
title: 'Module: src/codegraphcontext/tools/indexing/pre_scan.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/indexing/pre_scan.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.indexing.pre_scan`/
symbols:
  _register_prescans: _register_prescans().
  pre_scan_for_imports: pre_scan_for_imports().
  _register_prescans.make_js: _register_prescans().make_js().
  _get_registry: _get_registry().
  _register_prescans.make_py: _register_prescans().make_py().
  _PRESCAN_REGISTRY._PRESCAN_REGISTRY: _PRESCAN_REGISTRY._PRESCAN_REGISTRY.
  _PreScanFn: _PreScanFn.
  _register_prescans.make_py.scan: _register_prescans().make_py().scan().
  _register_prescans.make_js.scan: _register_prescans().make_js().scan().
---
# Module: [`src/codegraphcontext/tools/indexing/pre_scan.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pre_scan.py)

## Functions
- `_get_registry()` — [`L91`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pre_scan.py#L91)
- `_register_prescans()` — [`L11`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pre_scan.py#L11) — documented in [codegraphcontext-tools-graph_builder](../../../../../concepts/codegraphcontext-tools-graph_builder.md)
- `make_js(ext: str)` — [`L42`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pre_scan.py#L42)
- `make_py(ext: str)` — [`L36`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pre_scan.py#L36)
- `pre_scan_for_imports(files: List[Path], parsers_keys: Any, get_parser: Callable[[str], Any])` — [`L98`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pre_scan.py#L98) — Dispatch pre-scan by file extension; *parsers_keys* is the set of supported extensions (e.g. graph_builder.parsers.keys()).
- `scan(files: List[Path], gp: Callable[[str], Any])` — [`L37`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pre_scan.py#L37)
- `scan(files: List[Path], gp: Callable[[str], Any])` — [`L43`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pre_scan.py#L43)

## Module values
- `_PRESCAN_REGISTRY` — [`L88`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pre_scan.py#L88)
- `_PreScanFn` — [`L8`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pre_scan.py#L8)

