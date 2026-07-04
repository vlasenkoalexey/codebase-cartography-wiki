---
title: 'Module: src/codegraphcontext/core/jobs.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/jobs.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.jobs`/Job
symbols:
  JobManager.update_job: Manager#update_job().
  JobStatus: Status#
  JobManager.create_job: Manager#create_job().
  JobManager.find_active_job_by_path: Manager#find_active_job_by_path().
  JobInfo.estimated_time_remaining: Info#estimated_time_remaining().
  JobInfo.start_time: Info#start_time.
  JobManager: Manager#
  JobInfo.status: Info#status.
  JobInfo.end_time: Info#end_time.
  JobManager.get_job: Manager#get_job().
  JobManager.cleanup_old_jobs: Manager#cleanup_old_jobs().
  JobManager.jobs: Manager#jobs.
  JobManager.list_jobs: Manager#list_jobs().
  JobStatus.RUNNING: Status#RUNNING.
  JobManager.lock: Manager#lock.
  JobStatus.COMPLETED: Status#COMPLETED.
  JobInfo: Info#
  JobInfo.total_files: Info#total_files.
  JobInfo.processed_files: Info#processed_files.
  JobInfo.progress_percentage: Info#progress_percentage().
  JobStatus.FAILED: Status#FAILED.
  JobInfo.errors: Info#errors.
  JobInfo.path: Info#path.
  JobInfo.__post_init__: Info#__post_init__().
  JobStatus.PENDING: Status#PENDING.
  JobStatus.CANCELLED: Status#CANCELLED.
  JobInfo.job_id: Info#job_id.
  JobInfo.current_file: Info#current_file.
  JobInfo.status_message: Info#status_message.
  JobInfo.is_dependency: Info#is_dependency.
  JobInfo.estimated_duration: Info#estimated_duration.
  JobInfo.actual_duration: Info#actual_duration.
  JobInfo.result: Info#result.
  JobManager.__init__: Manager#__init__().
---
# Module: [`src/codegraphcontext/core/jobs.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py)

## Classes
### `JobInfo`
- def: [`src/codegraphcontext/core/jobs.py:24`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L24) — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
- doc: A data class to hold all information about a single background job.
- signature: `class JobInfo:`
- members:
  - `__post_init__(self)` — [`L44`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L44) — Ensures the errors list is initialized after the object is created.
  - `estimated_time_remaining(self)` — [`L57`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L57) — Calculates the estimated time remaining based on the average time per file. — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
  - `progress_percentage(self)` — [`L50`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L50) — Calculates the completion percentage of the job.
  - `actual_duration` — [`L38`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L38)
  - `current_file` — [`L35`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L35)
  - `end_time` — [`L32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L32)
  - `errors` — [`L39`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L39)
  - `estimated_duration` — [`L37`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L37)
  - `is_dependency` — [`L42`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L42) — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
  - `job_id` — [`L29`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L29) — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
  - `path` — [`L41`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L41) — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
  - `processed_files` — [`L34`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L34)
  - `result` — [`L40`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L40)
  - `start_time` — [`L31`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L31) — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
  - `status` — [`L30`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L30) — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
  - `status_message` — [`L36`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L36)
  - `total_files` — [`L33`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L33)
- uses (calls/refs, reference-scoped): [`JobStatus`](jobs.md#JobStatus), [`RUNNING`](jobs.md#JobStatus.RUNNING)
- used by: [`_run_index_with_progress`](../cli/cli_helpers.md#_run_index_with_progress), [`check_job_status`](../tools/handlers/management_handlers.md#check_job_status), [`create_job`](jobs.md#JobManager.create_job), [`check_job_status_tool`](../tools/system.md#SystemTools.check_job_status_tool), [`find_active_job_by_path`](jobs.md#JobManager.find_active_job_by_path), [`list_jobs`](../tools/handlers/management_handlers.md#list_jobs), [`list_jobs_tool`](../tools/system.md#SystemTools.list_jobs_tool), [`get_job`](jobs.md#JobManager.get_job), [`cleanup_old_jobs`](jobs.md#JobManager.cleanup_old_jobs), [`jobs`](jobs.md#JobManager.jobs), [`list_jobs`](jobs.md#JobManager.list_jobs)

### `JobManager`
- def: [`src/codegraphcontext/core/jobs.py:66`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L66) — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- doc: A thread-safe manager for creating, updating, and retrieving information
- signature: `class JobManager:`
- members:
  - `cleanup_old_jobs(self, max_age_hours: int = 24)` — [`L124`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L124) — Removes old jobs from memory to prevent memory leaks.
  - `create_job(self, path: str, is_dependency: bool = False)` — [`L75`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L75) — Creates a new job, assigns it a unique ID, and stores it. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
  - `find_active_job_by_path(self, path: str)` — [`L107`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L107) — Finds the most recent, currently active (pending or running) job for a given path. — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
  - `get_job(self, job_id: str)` — [`L97`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L97) — Retrieves the information for a single job.
  - `list_jobs(self)` — [`L102`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L102) — Returns a list of all jobs currently in the manager.
  - `update_job(self, job_id: str, **kwargs)` — [`L88`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L88) — Updates the information for a specific job in a thread-safe manner. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
  - `jobs` — [`L72`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L72) — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
  - `lock` — [`L73`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L73) — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
- protocol/private: `__init__`[`L71`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L71)
- uses (calls/refs, reference-scoped): [`JobStatus`](jobs.md#JobStatus), [`start_time`](jobs.md#JobInfo.start_time), [`status`](jobs.md#JobInfo.status), [`end_time`](jobs.md#JobInfo.end_time), [`RUNNING`](jobs.md#JobStatus.RUNNING), [`JobInfo`](jobs.md#JobInfo), [`path`](jobs.md#JobInfo.path), [`PENDING`](jobs.md#JobStatus.PENDING), [`is_dependency`](jobs.md#JobInfo.is_dependency), [`job_id`](jobs.md#JobInfo.job_id)
- used by: [`run_tree_sitter_index_async`](../tools/indexing/pipeline.md#run_tree_sitter_index_async), [`_initialize_services`](../cli/cli_helpers.md#_initialize_services), [`run_scip_index_async`](../tools/indexing/scip_pipeline.md#run_scip_index_async), [`build_graph_from_path_async`](../tools/graph_builder.md#GraphBuilder.build_graph_from_path_async), [`_run_index_with_progress`](../cli/cli_helpers.md#_run_index_with_progress), [`watch_helper`](../cli/cli_helpers.md#watch_helper), [`_run_loop`](../server.md#MCPServer._run_loop), [`check_job_status`](../tools/handlers/management_handlers.md#check_job_status), [`check_job_status_tool`](../tools/system.md#SystemTools.check_job_status_tool), [`list_jobs`](../tools/handlers/management_handlers.md#list_jobs), [`job_manager`](../server.md#MCPServer.job_manager), [`list_jobs_tool`](../tools/system.md#SystemTools.list_jobs_tool), [`process_file`](../tools/indexing/pipeline.md#run_tree_sitter_index_async.process_file), [`__init__`](../tools/graph_builder.md#GraphBuilder.__init__), [`__init__`](../tools/system.md#SystemTools.__init__)

### `JobStatus`  ·  implements/extends Enum
- def: [`src/codegraphcontext/core/jobs.py:15`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L15) — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- doc: Enumeration for the possible statuses of a background job.
- signature: `class JobStatus(Enum):`
- members:
  - `CANCELLED` — [`L21`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L21)
  - `COMPLETED` — [`L19`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L19)
  - `FAILED` — [`L20`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L20)
  - `PENDING` — [`L17`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L17) — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
  - `RUNNING` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/jobs.py#L18) — documented in [codegraphcontext-core-jobs](../../../../concepts/codegraphcontext-core-jobs.md)
- used by: [`run_tree_sitter_index_async`](../tools/indexing/pipeline.md#run_tree_sitter_index_async), [`run_scip_index_async`](../tools/indexing/scip_pipeline.md#run_scip_index_async), [`build_graph_from_path_async`](../tools/graph_builder.md#GraphBuilder.build_graph_from_path_async), [`_run_index_with_progress`](../cli/cli_helpers.md#_run_index_with_progress), [`check_job_status`](../tools/handlers/management_handlers.md#check_job_status), [`create_job`](jobs.md#JobManager.create_job), [`check_job_status_tool`](../tools/system.md#SystemTools.check_job_status_tool), [`find_active_job_by_path`](jobs.md#JobManager.find_active_job_by_path), [`estimated_time_remaining`](jobs.md#JobInfo.estimated_time_remaining), [`status`](jobs.md#JobInfo.status)

