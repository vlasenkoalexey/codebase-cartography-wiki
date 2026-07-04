---
title: 'Module: src/codegraphcontext/tools/indexing/pipeline.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/indexing/pipeline.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.indexing.pipeline`/run_tree_sitter_index_async().
symbols:
  run_tree_sitter_index_async: ''
  run_tree_sitter_index_async.process_file: process_file().
---
# Module: [`src/codegraphcontext/tools/indexing/pipeline.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pipeline.py)

## Functions
- `process_file(file: Path)` — [`L69`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pipeline.py#L69) — documented in [codegraphcontext-core-jobs](../../../../../concepts/codegraphcontext-core-jobs.md)
- `run_tree_sitter_index_async(path: Path, is_dependency: bool, job_id: Optional[str], cgcignore_path: Optional[str], writer: GraphWriter, job_manager: JobManager, parsers: Dict[str, str], get_parser: Callable[[str], Any], parse_file: Callable[[Path, Path, bool], Dict[str, Any]], add_minimal_file_node: Callable[[Path, Path, bool], None], call_resolution_diagnostics: Optional[List[Dict[str, Any]]] = None)` — [`L32`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/indexing/pipeline.py#L32) — Parse all discovered files, write symbols, then inheritance + CALLS. — documented in [codegraphcontext-cli-cli_helpers](../../../../../concepts/codegraphcontext-cli-cli_helpers.md)

