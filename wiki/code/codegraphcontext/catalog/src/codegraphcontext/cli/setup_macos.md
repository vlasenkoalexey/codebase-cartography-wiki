---
title: 'Module: src/codegraphcontext/cli/setup_macos.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/cli/setup_macos.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.cli.setup_macos`/
symbols:
  setup_macos_binary: setup_macos_binary().
  _set_initial_password: _set_initial_password().
  _has_brew: _has_brew().
  _brew_install_neo4j: _brew_install_neo4j().
  _brew_start: _brew_start().
  _escape_cypher_password: _escape_cypher_password().
---
# Module: [`src/codegraphcontext/cli/setup_macos.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_macos.py)

## Functions
- `_brew_install_neo4j(run_command, console)` — [`L9`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_macos.py#L9)
- `_brew_start(service: str, run_command, console)` — [`L16`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_macos.py#L16)
- `_escape_cypher_password(password: str)` — [`L19`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_macos.py#L19)
- `_has_brew(run_command, console)` — [`L6`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_macos.py#L6)
- `_set_initial_password(new_pw: str, run_command, console)` — [`L23`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_macos.py#L23)
- `setup_macos_binary(console, prompt, run_command, _save_neo4j_credentials)` — [`L33`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/cli/setup_macos.py#L33) — Automates Neo4j install & config on macOS via Homebrew.

