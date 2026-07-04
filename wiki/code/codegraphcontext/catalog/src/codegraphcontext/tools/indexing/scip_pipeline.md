---
title: 'Module: src/codegraphcontext/tools/indexing/scip_pipeline.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/indexing/scip_pipeline.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.indexing.scip_pipeline`/
symbols:
  run_scip_index_async: run_scip_index_async().
  run_scip_index_async.should_skip_file: run_scip_index_async().should_skip_file().
  name_from_symbol: name_from_symbol().
---
# Module: [`src/codegraphcontext/tools/indexing/scip_pipeline.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/scip_pipeline.py)

## Functions
- `name_from_symbol(symbol: str)` — [`L24`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/scip_pipeline.py#L24)
- `run_scip_index_async(path: Path, is_dependency: bool, job_id: Optional[str], lang: str, writer: GraphWriter, job_manager: JobManager, parsers_keys: Any, get_parser: Callable[[str], Any], scip_indexer_mod: Any, cgcignore_path: Optional[str] = None)` — [`L34`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/scip_pipeline.py#L34) — Run SCIP CLI, write graph, supplement with Tree-sitter, write SCIP CALLS edges. — documented in [codegraphcontext-cli-cli_helpers](../../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `should_skip_file(file_path: Path)` — [`L73`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/scip_pipeline.py#L73)

