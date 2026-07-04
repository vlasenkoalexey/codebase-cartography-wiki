---
title: 'Module: src/codegraphcontext/cli/config_manager.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/cli/config_manager.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.cli.config_manager`/
symbols:
  resolve_context: resolve_context().
  load_context_config: load_context_config().
  console: console.
  get_config_value: get_config_value().
  save_context_config: save_context_config().
  create_context: create_context().
  load_config: load_config().
  CONFIG_FILE: CONFIG_FILE.
  CONFIG_DIR: CONFIG_DIR.
  discover_child_contexts._scan: discover_child_contexts()._scan().
  save_config: save_config().
  show_config: show_config().
  ResolvedContext.database: ResolvedContext#database.
  set_config_value: set_config_value().
  register_repo_in_context: register_repo_in_context().
  CONTEXT_CONFIG_FILE: CONTEXT_CONFIG_FILE.
  ensure_first_run_bootstrap: ensure_first_run_bootstrap().
  ContextConfig.contexts: ContextConfig#contexts.
  set_context_mode: set_context_mode().
  DEFAULT_CONFIG: DEFAULT_CONFIG.
  ensure_config_dir: ensure_config_dir().
  reset_config: reset_config().
  delete_context: delete_context().
  set_default_context: set_default_context().
  ResolvedContext.cgcignore_path: ResolvedContext#cgcignore_path.
  _default_global_db_path: _default_global_db_path().
  validate_config_value: validate_config_value().
  ensure_config_file: ensure_config_file().
  ResolvedContext.mode: ResolvedContext#mode.
  _save_workspace_mappings: _save_workspace_mappings().
  ResolvedContext.db_path: ResolvedContext#db_path.
  is_db_deletion_allowed: is_db_deletion_allowed().
  discover_child_contexts: discover_child_contexts().
  ContextConfig.mode: ContextConfig#mode.
  DATABASE_CREDENTIAL_KEYS: DATABASE_CREDENTIAL_KEYS.
  ResolvedContext: ResolvedContext#
  ResolvedContext.context_name: ResolvedContext#context_name.
  _migrate_legacy_config_yaml: _migrate_legacy_config_yaml().
  list_contexts: list_contexts().
  ContextConfig.default_context: ContextConfig#default_context.
  normalize_config_path: normalize_config_path().
  should_apply_project_dotenv: should_apply_project_dotenv().
  save_workspace_mapping: save_workspace_mapping().
  _load_workspace_mappings: _load_workspace_mappings().
  ensure_global_cgcignore: ensure_global_cgcignore().
  find_local_env: find_local_env().
  ContextInfo.database: ContextInfo#database.
  ContextInfo.db_path: ContextInfo#db_path.
  ContextInfo.repos: ContextInfo#repos.
  _FIRST_RUN_MARKER: _FIRST_RUN_MARKER.
  _LEGACY_CONTEXT_CONFIG_FILE: _LEGACY_CONTEXT_CONFIG_FILE.
  _default_db_path: _default_db_path().
  ContextInfo: ContextInfo#
  ContextInfo.cgcignore_path: ContextInfo#cgcignore_path.
  ResolvedContext.is_local: ResolvedContext#is_local.
  remove_workspace_mapping: remove_workspace_mapping().
  ContextConfig: ContextConfig#
  _LEGACY_FALKORDB_PATH: _LEGACY_FALKORDB_PATH.
  get_workspace_mapping: get_workspace_mapping().
  SUPPORTED_DATABASES.SUPPORTED_DATABASES: SUPPORTED_DATABASES.SUPPORTED_DATABASES.
  ContextInfo.name: ContextInfo#name.
  DATABASE_CLI_HELP: DATABASE_CLI_HELP.
  _print_welcome_banner: _print_welcome_banner().
  find_local_cgc_dir: find_local_cgc_dir().
  _atomic_write_text: _atomic_write_text().
  CONFIG_VALIDATORS: CONFIG_VALIDATORS.
  ContextNotFoundError: ContextNotFoundError#
  DiscoveredContext: DiscoveredContext#
  list_workspace_mappings: list_workspace_mappings().
  CONFIG_DESCRIPTIONS: CONFIG_DESCRIPTIONS.
  codegraphcontext_dotenv_at_cwd: codegraphcontext_dotenv_at_cwd().
  VALID_MODES: VALID_MODES.
  ContextConfig.version: ContextConfig#version.
  DEFAULT_CGCIGNORE_PATTERNS: DEFAULT_CGCIGNORE_PATTERNS.
  DiscoveredContext.path: DiscoveredContext#path.
  DiscoveredContext.cgc_path: DiscoveredContext#cgc_path.
  DiscoveredContext.repo_name: DiscoveredContext#repo_name.
  DiscoveredContext.database: DiscoveredContext#database.
  DiscoveredContext.db_path: DiscoveredContext#db_path.
  DiscoveredContext.cgcignore_path: DiscoveredContext#cgcignore_path.
  DB_PATH_ENV_KEYS: DB_PATH_ENV_KEYS.
---
# Module: [`src/codegraphcontext/cli/config_manager.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py)

## Classes
### `ContextConfig`
- def: [`src/codegraphcontext/cli/config_manager.py:709`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L709)
- members:
  - `contexts` — [`L714`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L714) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `default_context` — [`L713`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L713) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `mode` — [`L712`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L712) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `version` — [`L711`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L711)
- uses (calls/refs, reference-scoped): [`ContextInfo`](config_manager.md#ContextInfo)
- used by: [`resolve_context`](config_manager.md#resolve_context), [`load_context_config`](config_manager.md#load_context_config), [`save_context_config`](config_manager.md#save_context_config), [`create_context`](config_manager.md#create_context), [`context_list`](main.md#context_list), [`register_repo_in_context`](config_manager.md#register_repo_in_context), [`set_context_mode`](config_manager.md#set_context_mode), [`delete_context`](config_manager.md#delete_context), [`set_default_context`](config_manager.md#set_default_context), [`list_contexts`](config_manager.md#list_contexts), [`should_apply_project_dotenv`](config_manager.md#should_apply_project_dotenv)

### `ContextInfo`
- def: [`src/codegraphcontext/cli/config_manager.py:699`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L699)
- doc: Metadata for a single named context.
- signature: `class ContextInfo:`
- members:
  - `cgcignore_path` — [`L705`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L705)
  - `database` — [`L702`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L702) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `db_path` — [`L703`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L703) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `name` — [`L701`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L701)
  - `repos` — [`L704`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L704) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- used by: [`resolve_context`](config_manager.md#resolve_context), [`load_context_config`](config_manager.md#load_context_config), [`save_context_config`](config_manager.md#save_context_config), [`create_context`](config_manager.md#create_context), [`context_list`](main.md#context_list), [`register_repo_in_context`](config_manager.md#register_repo_in_context), [`contexts`](config_manager.md#ContextConfig.contexts), [`list_contexts`](config_manager.md#list_contexts)

### `ContextNotFoundError`  ·  implements/extends ValueError
- def: [`src/codegraphcontext/cli/config_manager.py:855`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L855)
- doc: Raised when --context names an unregistered workspace.
- signature: `class ContextNotFoundError(ValueError):`
- used by: [`_initialize_services`](cli_helpers.md#_initialize_services), [`resolve_context`](config_manager.md#resolve_context)

### `DiscoveredContext`
- def: [`src/codegraphcontext/cli/config_manager.py:1103`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1103)
- doc: A .codegraphcontext folder found in a child directory.
- signature: `class DiscoveredContext:`
- members:
  - `cgc_path` — [`L1106`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1106)
  - `cgcignore_path` — [`L1110`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1110)
  - `database` — [`L1108`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1108)
  - `db_path` — [`L1109`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1109)
  - `path` — [`L1105`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1105)
  - `repo_name` — [`L1107`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1107)
- used by: [`_scan`](config_manager.md#discover_child_contexts._scan), [`discover_child_contexts`](config_manager.md#discover_child_contexts)

### `ResolvedContext`
- def: [`src/codegraphcontext/cli/config_manager.py:830`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L830) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- doc: Result of resolve_context() — everything needed to instantiate the DB.
- signature: `class ResolvedContext:`
- members:
  - `cgcignore_path` — [`L836`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L836) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `context_name` — [`L833`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L833) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `database` — [`L834`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L834) — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
  - `db_path` — [`L835`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L835) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
  - `is_local` — [`L837`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L837)
  - `mode` — [`L832`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L832) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- used by: [`_initialize_services`](cli_helpers.md#_initialize_services), [`switch_context_tool`](../server.md#MCPServer.switch_context_tool), [`_load_credentials`](main.md#_load_credentials), [`resolve_context`](config_manager.md#resolve_context), [`db_manager`](../server.md#MCPServer.db_manager), [`watch_helper`](cli_helpers.md#watch_helper), [`index_helper`](cli_helpers.md#index_helper), [`get_status`](../api/router.md#get_status), [`reindex_helper`](cli_helpers.md#reindex_helper), [`add_package_helper`](cli_helpers.md#add_package_helper), [`_kuzu_fallback_path`](cli_helpers.md#_kuzu_fallback_path), [`resolved_context`](../server.md#MCPServer.resolved_context), [`do_index`](cli_helpers.md#watch_helper.do_index)

## Functions
- `_atomic_write_text(path: Path, content: str, *, secure: bool = False)` — [`L19`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L19) — Write *content* to *path* atomically (temp file + replace).
- `_default_db_path(context_name: str, database: str)` — [`L717`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L717) — Return the canonical DB path for a named context. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `_default_global_db_path(database: str)` — [`L725`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L725) — Return the canonical DB path for the global context. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `_load_workspace_mappings()` — [`L1167`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1167) — Load the ``workspace_mappings`` section from config.yaml.
- `_migrate_legacy_config_yaml()` — [`L746`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L746) — Rename cgc_config.yaml -> config.yaml if the old name exists and the new one does not. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `_print_welcome_banner()` — [`L585`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L585) — Print a one-time welcome message explaining the context system.
- `_save_workspace_mappings(mappings: Dict[str, Dict[str, str]])` — [`L1179`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1179) — Write *mappings* back into the ``workspace_mappings`` key of config.yaml, — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `_scan(directory: Path, depth: int)` — [`L1127`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1127)
- `codegraphcontext_dotenv_at_cwd(cwd: Optional[Path] = None)` — [`L354`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L354) — Return ``<cwd>/.codegraphcontext/.env`` if that file exists, else None.
- `create_context(name: str, database: str = "falkordb", db_path: Optional[str] = None)` — [`L997`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L997) — Create a new named context. Returns True on success. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `delete_context(name: str)` — [`L1028`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1028) — Delete a named context from the registry. Returns True on success. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `discover_child_contexts(start: Optional[Path] = None, max_depth: int = 1)` — [`L1113`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1113) — Walk child directories of *start* up to *max_depth* levels looking for
- `ensure_config_dir(path: Optional[Path] = None)` — [`L228`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L228) — Ensure that the configuration directory exists. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `ensure_config_file()` — [`L620`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L620) — Create default .env config file on first run if it does not exist. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)
- `ensure_first_run_bootstrap(show_welcome: bool = False)` — [`L600`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L600) — Run one-time setup for brand-new installs. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `ensure_global_cgcignore()` — [`L238`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L238) — Create ``~/.codegraphcontext/global/.cgcignore`` with sensible defaults
- `find_local_cgc_dir(start: Optional[Path] = None)` — [`L840`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L840) — Check *start* (default: cwd) for a ``.codegraphcontext/`` directory that
- `find_local_env()` — [`L324`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L324) — Find a local .env file by searching current directory and parents.
- `get_config_value(key: str)` — [`L527`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L527) — Get a specific configuration value. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `get_workspace_mapping(cwd: Path)` — [`L1200`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1200) — Look up a saved workspace mapping for *cwd*.
- `is_db_deletion_allowed()` — [`L533`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L533) — True when destructive delete/clear operations are permitted. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `list_contexts()` — [`L1092`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1092) — Return all named contexts. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `list_workspace_mappings()` — [`L1241`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1241) — Return all saved workspace mappings.
- `load_config()` — [`L250`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L250) — Load configuration with priority support. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `load_context_config()` — [`L754`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L754) — Load ~/.codegraphcontext/config.yaml. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `normalize_config_path(value: str, *, absolute: bool = False, base_dir: Optional[Path] = None)` — [`L213`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L213) — Normalize config path values.
- `register_repo_in_context(context_name: str, repo_path: str, auto_create: bool = False)` — [`L1043`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1043) — Add a repo path to a named context (idempotent). — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `remove_workspace_mapping(cwd: Path)` — [`L1230`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1230) — Delete a saved workspace mapping. Returns True if one was removed.
- `reset_config()` — [`L565`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L565) — Reset configuration to defaults (preserves database credentials). — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `resolve_context(cli_context: Optional[str] = None, cwd: Optional[Path] = None)` — [`L859`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L859) — Determine which context / DB to use. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `save_config(config: Dict[str, str], preserve_db_credentials: bool = True)` — [`L366`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L366) — Save configuration to file. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `save_context_config(cfg: ContextConfig)` — [`L796`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L796) — Persist ContextConfig to ~/.codegraphcontext/config.yaml. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `save_workspace_mapping(cwd: Path, context_path: Path)` — [`L1209`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1209) — Persist an association from *cwd* to a ``.codegraphcontext`` directory.
- `set_config_value(key: str, value: str)` — [`L538`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L538) — Set a configuration value. Returns True if successful. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `set_context_mode(mode: str)` — [`L1068`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1068) — Set the global CGC mode. Returns True on success. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `set_default_context(name: str)` — [`L1080`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L1080) — Set the default named context used when no --context flag is given. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `should_apply_project_dotenv()` — [`L300`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L300) — True when cwd-local ``.codegraphcontext/.env`` should merge with global config.
- `show_config()` — [`L635`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L635) — Display current configuration in a nice table. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `validate_config_value(key: str, value: str)` — [`L427`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L427) — Validate a configuration value. — documented in [codegraphcontext-cli-main](../../../../concepts/codegraphcontext-cli-main.md)

## Module values
- `CONFIG_DESCRIPTIONS` — [`L91`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L91)
- `CONFIG_DIR` — [`L32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L32) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `CONFIG_FILE` — [`L33`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L33) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `CONFIG_VALIDATORS` — [`L157`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L157)
- `CONTEXT_CONFIG_FILE` — [`L691`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L691) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `DATABASE_CLI_HELP` — [`L178`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L178)
- `DATABASE_CREDENTIAL_KEYS` — [`L41`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L41) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `DB_PATH_ENV_KEYS` — [`L36`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L36)
- `DEFAULT_CGCIGNORE_PATTERNS` — [`L184`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L184)
- `DEFAULT_CONFIG` — [`L49`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L49) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `SUPPORTED_DATABASES` — [`L177`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L177)
- `VALID_MODES` — [`L695`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L695)
- `_FIRST_RUN_MARKER` — [`L582`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L582)
- `_LEGACY_CONTEXT_CONFIG_FILE` — [`L692`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L692)
- `_LEGACY_FALKORDB_PATH` — [`L722`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L722)
- `console` — [`L16`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/config_manager.py#L16) — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)

