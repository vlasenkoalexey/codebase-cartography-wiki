---
title: 'Module: src/codegraphcontext/tools/system.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/system.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.system`/
symbols:
  SystemTools.check_job_status_tool: SystemTools#check_job_status_tool().
  SystemTools.list_jobs_tool: SystemTools#list_jobs_tool().
  SystemTools.__init__: SystemTools#__init__().
  SystemTools.execute_cypher_query_tool: SystemTools#execute_cypher_query_tool().
  SystemTools.find_dead_code_tool: SystemTools#find_dead_code_tool().
  SystemTools.db_manager: SystemTools#db_manager.
  SystemTools.job_manager: SystemTools#job_manager.
  logger: logger.
  SystemTools: SystemTools#
---
# Module: [`src/codegraphcontext/tools/system.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/system.py)

## Classes
### `SystemTools`
- def: [`src/codegraphcontext/tools/system.py:21`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/system.py#L21)
- doc: Handles system-level tools like job management and direct DB queries.
- signature: `class SystemTools:`
- members:
  - `check_job_status_tool(self, job_id: str)` — [`L28`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/system.py#L28) — Tool to check job status — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
  - `execute_cypher_query_tool(self, cypher_query: str)` — [`L84`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/system.py#L84) — Tool to execute a read-only Cypher query.
  - `find_dead_code_tool(self)` — [`L123`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/system.py#L123) — Finds potentially unused functions (dead code).
  - `list_jobs_tool(self)` — [`L68`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/system.py#L68) — Tool to list all jobs
  - `db_manager` — [`L25`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/system.py#L25)
  - `job_manager` — [`L26`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/system.py#L26)
- protocol/private: `__init__`[`L24`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/system.py#L24)
- uses (calls/refs, reference-scoped): [`get_driver`](../core/database.md#DatabaseManager.get_driver), [`DatabaseManager`](../core/database.md#DatabaseManager), [`JobStatus`](../core/jobs.md#JobStatus), [`estimated_time_remaining`](../core/jobs.md#JobInfo.estimated_time_remaining), [`JobManager`](../core/jobs.md#JobManager), [`start_time`](../core/jobs.md#JobInfo.start_time), [`status`](../core/jobs.md#JobInfo.status), [`end_time`](../core/jobs.md#JobInfo.end_time), [`get_job`](../core/jobs.md#JobManager.get_job), [`list_jobs`](../core/jobs.md#JobManager.list_jobs), [`RUNNING`](../core/jobs.md#JobStatus.RUNNING), [`COMPLETED`](../core/jobs.md#JobStatus.COMPLETED)

## Module values
- `logger` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/system.py#L18)

