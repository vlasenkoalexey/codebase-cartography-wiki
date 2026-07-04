---
title: 'Module: scripts/format_change_management.py'
type: catalog
provenance: extracted
module: scripts/format_change_management.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.format_change_management`/
symbols:
  main: main().
  FormatChangeManager.db: FormatChangeManager#db.
  FormatChangeManager.approve_change_request: FormatChangeManager#approve_change_request().
  FormatChangeManager.implement_change: FormatChangeManager#implement_change().
  FormatChangeManager.rollback_change: FormatChangeManager#rollback_change().
  FormatChangeManager.generate_change_report: FormatChangeManager#generate_change_report().
  FormatChangeManager.create_change_request: FormatChangeManager#create_change_request().
  FormatChangeManager.logger: FormatChangeManager#logger.
  FormatChangeDatabase.db_path: FormatChangeDatabase#db_path.
  FormatChangeDatabase.update_change_request_status: FormatChangeDatabase#update_change_request_status().
  project_root: project_root.
  FormatChangeDatabase.get_change_request: FormatChangeDatabase#get_change_request().
  FormatChangeDatabase.get_format_versions: FormatChangeDatabase#get_format_versions().
  FormatChangeDatabase.create_format_version: FormatChangeDatabase#create_format_version().
  FormatChangeDatabase.get_pending_requests: FormatChangeDatabase#get_pending_requests().
  FormatChangeDatabase.init_database: FormatChangeDatabase#init_database().
  FormatChangeDatabase.create_change_request: FormatChangeDatabase#create_change_request().
  FormatChangeDatabase.add_approval: FormatChangeDatabase#add_approval().
  FormatChangeManager._backup_current_format: FormatChangeManager#_backup_current_format().
  FormatChangeManager._restore_from_backup: FormatChangeManager#_restore_from_backup().
  FormatChangeDatabase.__init__: FormatChangeDatabase#__init__().
  FormatChangeDatabase.get_active_version: FormatChangeDatabase#get_active_version().
  FormatChangeManager.golden_master_manager: FormatChangeManager#golden_master_manager.
  FormatChangeManager.change_types: FormatChangeManager#change_types.
  FormatChangeManager.approval_requirements: FormatChangeManager#approval_requirements.
  FormatChangeDatabase: FormatChangeDatabase#
  FormatChangeManager: FormatChangeManager#
  FormatChangeManager._setup_logging: FormatChangeManager#_setup_logging().
  FormatChangeManager._assess_change_impact: FormatChangeManager#_assess_change_impact().
  FormatChangeManager._check_approval_requirements: FormatChangeManager#_check_approval_requirements().
  FormatChangeManager.__init__: FormatChangeManager#__init__().
---
# Module: [`scripts/format_change_management.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py)

## Classes
### `FormatChangeDatabase`
- def: [`scripts/format_change_management.py:27`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L27)
- doc: Database for tracking format changes
- signature: `class FormatChangeDatabase:`
- members:
  - `add_approval(self, change_request_id: int, approver: str, status: str, comments: str = "")` — [`L150`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L150) — Add approval to change request
  - `create_change_request(self, requester: str, format_type: str, change_type: str, description: str, justification: str, impact_assessment: str = "")` — [`L113`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L113) — Create a new format change request
  - `create_format_version(self, format_type: str, version: str, change_request_id: int, specification_hash: str, golden_master_hash: str = "")` — [`L204`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L204) — Create new format version
  - `get_active_version(self, format_type: str)` — [`L311`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L311) — Get active format version
  - `get_change_request(self, request_id: int)` — [`L269`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L269) — Get specific change request
  - `get_format_versions(self, format_type: str)` — [`L291`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L291) — Get format version history
  - `get_pending_requests(self)` — [`L250`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L250) — Get pending change requests
  - `init_database(self)` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L34) — Initialize change management database
  - `update_change_request_status(self, change_request_id: int, status: str, reviewer: str = "", comments: str = "")` — [`L175`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L175) — Update change request status
  - `db_path` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L31)
- protocol/private: `__init__`[`L30`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L30)
- used by: [`main`](format_change_management.md#main), [`approve_change_request`](format_change_management.md#FormatChangeManager.approve_change_request), [`db`](format_change_management.md#FormatChangeManager.db), [`implement_change`](format_change_management.md#FormatChangeManager.implement_change), [`rollback_change`](format_change_management.md#FormatChangeManager.rollback_change), [`generate_change_report`](format_change_management.md#FormatChangeManager.generate_change_report), [`create_change_request`](format_change_management.md#FormatChangeManager.create_change_request)

### `FormatChangeManager`
- def: [`scripts/format_change_management.py:335`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L335)
- doc: Format change management system
- signature: `class FormatChangeManager:`
- members:
  - `_assess_change_impact(self, format_type: str, change_type: str, description: str)` — [`L411`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L411) — Assess impact of proposed change
  - `_backup_current_format(self, format_type: str, new_version: str)` — [`L528`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L528) — Backup current format specification
  - `_check_approval_requirements(self, request_id: int, required_approvers: list[str])` — [`L474`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L474) — Check if approval requirements are met
  - `_restore_from_backup(self, format_type: str, version: str)` — [`L595`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L595) — Restore format from backup
  - `_setup_logging(self)` — [`L361`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L361) — Setup logging for change management
  - `approve_change_request(self, request_id: int, approver: str, status: str, comments: str = "")` — [`L442`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L442) — Approve or reject change request
  - `create_change_request(self, requester: str, format_type: str, change_type: str, description: str, justification: str, impact_assessment: str = "")` — [`L375`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L375) — Create new format change request
  - `generate_change_report(self, output_file: str = "format_change_report.json")` — [`L623`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L623) — Generate comprehensive change management report
  - `implement_change(self, request_id: int, implementer: str)` — [`L482`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L482) — Implement approved format change
  - `rollback_change(self, request_id: int, rollback_reason: str)` — [`L552`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L552) — Rollback implemented format change
  - `approval_requirements` — [`L353`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L353)
  - `change_types` — [`L344`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L344)
  - `db` — [`L339`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L339)
  - `golden_master_manager` — [`L340`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L340)
  - `logger` — [`L341`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L341)
- protocol/private: `__init__`[`L338`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L338)
- uses (calls/refs, reference-scoped): [`update_change_request_status`](format_change_management.md#FormatChangeDatabase.update_change_request_status), [`get_change_request`](format_change_management.md#FormatChangeDatabase.get_change_request), [`get_format_versions`](format_change_management.md#FormatChangeDatabase.get_format_versions), [`create_format_version`](format_change_management.md#FormatChangeDatabase.create_format_version), [`get_pending_requests`](format_change_management.md#FormatChangeDatabase.get_pending_requests), [`add_approval`](format_change_management.md#FormatChangeDatabase.add_approval), [`create_change_request`](format_change_management.md#FormatChangeDatabase.create_change_request), [`FormatChangeDatabase`](format_change_management.md#FormatChangeDatabase)  (1 test-only)
- used by: [`main`](format_change_management.md#main)

## Functions
- `main()` — [`L655`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L655) — Main change management function

## Module values
- `project_root` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/scripts/format_change_management.py#L21)

