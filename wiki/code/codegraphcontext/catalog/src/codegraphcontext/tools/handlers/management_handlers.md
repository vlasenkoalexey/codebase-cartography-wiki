---
title: 'Module: src/codegraphcontext/tools/handlers/management_handlers.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/handlers/management_handlers.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.handlers.management_handlers`/
symbols:
  load_bundle: load_bundle().
  check_job_status: check_job_status().
  list_jobs: list_jobs().
  search_registry_bundles: search_registry_bundles().
  delete_repository: delete_repository().
  get_repository_stats: get_repository_stats().
  list_indexed_repositories: list_indexed_repositories().
  load_bundle._ensure_allowed_bundle_path: load_bundle()._ensure_allowed_bundle_path().
---
# Module: [`src/codegraphcontext/tools/handlers/management_handlers.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/management_handlers.py)

## Functions
- `_ensure_allowed_bundle_path(candidate: Path)` — [`L159`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/management_handlers.py#L159)
- `check_job_status(job_manager: JobManager, **args)` — [`L56`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/management_handlers.py#L56) — Tool to check job status — documented in [codegraphcontext-core-jobs](../../../../../concepts/codegraphcontext-core-jobs.md)
- `delete_repository(graph_builder: GraphBuilder, **args)` — [`L24`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/management_handlers.py#L24) — Tool to delete a repository from the graph.
- `get_repository_stats(code_finder: CodeFinder, **args)` — [`L325`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/management_handlers.py#L325) — Tool to get statistics about indexed repositories.
- `list_indexed_repositories(code_finder: CodeFinder, **args)` — [`L11`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/management_handlers.py#L11) — Tool to list indexed repositories.
- `list_jobs(job_manager: JobManager)` — [`L108`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/management_handlers.py#L108) — Tool to list all jobs
- `load_bundle(code_finder: CodeFinder, **args)` — [`L131`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/management_handlers.py#L131) — Tool to load a .cgc bundle into the database. — documented in [codegraphcontext-server](../../../../../concepts/codegraphcontext-server.md)
- `search_registry_bundles(code_finder: CodeFinder, **args)` — [`L246`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/management_handlers.py#L246) — Tool to search for bundles in the registry.

