---
title: 'Module: src/codegraphcontext/cli/setup_wizard.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/cli/setup_wizard.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.cli.setup_wizard`/
symbols:
  console: console.
  setup_docker: setup_docker().
  _configure_ide: _configure_ide().
  _save_neo4j_credentials: _save_neo4j_credentials().
  setup_existing_db: setup_existing_db().
  setup_hosted_db: setup_hosted_db().
  setup_local_db: setup_local_db().
  configure_mcp_client: configure_mcp_client().
  run_command: run_command().
  run_neo4j_setup_wizard: run_neo4j_setup_wizard().
  _generate_mcp_json: _generate_mcp_json().
  setup_local_binary: setup_local_binary().
  convert_mcp_json_to_yaml: convert_mcp_json_to_yaml().
  _configure_goose: _configure_goose().
  _check_write_access: _check_write_access().
  _print_opencode_mcp_instructions: _print_opencode_mcp_instructions().
  DEFAULT_NEO4J_URI: DEFAULT_NEO4J_URI.
  DEFAULT_NEO4J_USERNAME: DEFAULT_NEO4J_USERNAME.
  find_latest_neo4j_creds_file: find_latest_neo4j_creds_file().
  find_jetbrains_mcp_config: find_jetbrains_mcp_config().
  DEFAULT_NEO4J_BOLT_PORT: DEFAULT_NEO4J_BOLT_PORT.
  DEFAULT_NEO4J_HTTP_PORT: DEFAULT_NEO4J_HTTP_PORT.
  get_project_root: get_project_root().
---
# Module: [`src/codegraphcontext/cli/setup_wizard.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py)

## Functions
- `_check_write_access(path: Path)` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L18)
- `_configure_goose(mcp_config)` — [`L193`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L193) — Configures Goose CLI with the MCP server.
- `_configure_ide(mcp_config)` — [`L312`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L312) — Asks user for their IDE and configures it automatically.
- `_generate_mcp_json(creds)` — [`L65`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L65) — Generates and prints the MCP JSON configuration.
- `_print_opencode_mcp_instructions(mcp_config: dict)` — [`L180`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L180) — OpenCode manages MCP in its own UI; we only print the stdio snippet + doc link.
- `_save_neo4j_credentials(creds)` — [`L32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L32) — Save Neo4j credentials to .env file (database setup only).
- `configure_mcp_client()` — [`L563`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L563) — Configure MCP client (IDE/CLI) integration.
- `convert_mcp_json_to_yaml()` — [`L158`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L158)
- `find_jetbrains_mcp_config()` — [`L140`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L140)
- `find_latest_neo4j_creds_file()` — [`L682`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L682) — Finds the latest Neo4j credentials file in the Downloads folder.
- `get_project_root()` — [`L497`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L497) — Always return the directory where the user runs `cgc` (CWD).
- `run_command(command, console, shell=False, check=True, input_text=None)` — [`L501`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L501) — Runs a command, captures its output, and handles execution.
- `run_neo4j_setup_wizard()` — [`L536`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L536) — Guides the user through setting up Neo4j database for CodeGraphContext.
- `setup_docker()` — [`L955`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L955) — Creates Docker files and runs docker-compose for Neo4j.
- `setup_existing_db()` — [`L696`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L696) — Guides user to configure an existing Neo4j instance.
- `setup_hosted_db()` — [`L814`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L814) — Guides user to configure a remote Neo4j instance.
- `setup_local_binary()` — [`L1116`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L1116) — Automates the installation and configuration of Neo4j on Ubuntu/Debian.
- `setup_local_db()` — [`L932`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L932) — Guides user to set up a local Neo4j instance.

## Module values
- `DEFAULT_NEO4J_BOLT_PORT` — [`L29`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L29)
- `DEFAULT_NEO4J_HTTP_PORT` — [`L30`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L30)
- `DEFAULT_NEO4J_URI` — [`L27`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L27)
- `DEFAULT_NEO4J_USERNAME` — [`L28`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L28)
- `console` — [`L16`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_wizard.py#L16)

