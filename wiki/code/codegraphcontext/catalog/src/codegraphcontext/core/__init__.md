---
title: 'Module: src/codegraphcontext/core/__init__.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/__init__.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core`/
symbols:
  get_database_manager: get_database_manager().
  is_falkordb_usable: is_falkordb_usable().
  _fallback_db_path_for: _fallback_db_path_for().
  mark_falkordb_unavailable: mark_falkordb_unavailable().
  _is_ladybugdb_available: _is_ladybugdb_available().
  _is_neo4j_configured: _is_neo4j_configured().
  _is_nornic_configured: _is_nornic_configured().
  _FALKORDB_DISABLED: _FALKORDB_DISABLED.
  _is_kuzudb_available: _is_kuzudb_available().
  _is_falkordb_available: _is_falkordb_available().
  __getattr__: __getattr__().
  _is_falkordb_remote_configured: _is_falkordb_remote_configured().
  _LAZY_IMPORTS: _LAZY_IMPORTS.
  __all__: __all__.
---
# Module: [`src/codegraphcontext/core/__init__.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py)

## Functions
- `__getattr__(name: str)` — [`L295`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L295)
- `_fallback_db_path_for(db_path: Optional[str], target_backend: str)` — [`L27`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L27) — Adjust a FalkorDB-specific db_path when falling back to a different backend.
- `_is_falkordb_available()` — [`L75`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L75) — Check if FalkorDB Lite is installed (Unix only).
- `_is_falkordb_remote_configured()` — [`L89`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L89) — Check if a remote FalkorDB host is configured.
- `_is_kuzudb_available()` — [`L61`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L61) — Check if KùzuDB is installed.
- `_is_ladybugdb_available()` — [`L68`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L68) — Check if LadybugDB is installed.
- `_is_neo4j_configured()` — [`L93`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L93) — Check if Neo4j is configured with credentials.
- `_is_nornic_configured()` — [`L101`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L101) — Check if Nornic is configured with credentials.
- `get_database_manager(db_path: Optional[str] = None)` — [`L109`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L109) — Factory function to get the appropriate database manager based on configuration. — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- `is_falkordb_usable()` — [`L57`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L57) — True when FalkorDB Lite is installed and has not failed this session.
- `mark_falkordb_unavailable()` — [`L51`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L51) — Remember that FalkorDB Lite cannot run in this process.

## Module values
- `_FALKORDB_DISABLED` — [`L24`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L24)
- `_LAZY_IMPORTS` — [`L286`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L286)
- `__all__` — [`L302`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/__init__.py#L302)

