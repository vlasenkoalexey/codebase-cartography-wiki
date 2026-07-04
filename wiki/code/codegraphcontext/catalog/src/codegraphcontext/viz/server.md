---
title: 'Module: src/codegraphcontext/viz/server.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/viz/server.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.viz.server`/
symbols:
  get_graph: get_graph().
  spa_fallback: spa_fallback().
  set_db_manager: set_db_manager().
  get_graph.get_eid: get_graph().get_eid().
  run_server: run_server().
  db_manager.db_manager: db_manager.db_manager.
  _safe_static_file: _safe_static_file().
  _ALLOWED_ORIGIN_REGEX: _ALLOWED_ORIGIN_REGEX.
  app: app.
  get_file: get_file().
  _static_root: _static_root().
  _safe_read_text_file: _safe_read_text_file().
  _static_dir._static_dir: _static_dir._static_dir.
  is_path_under_static: is_path_under_static().
---
# Module: [`src/codegraphcontext/viz/server.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py)

## Functions
- `_safe_read_text_file(path: str)` — [`L45`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L45)
- `_safe_static_file(relative_path: str)` — [`L28`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L28) — Resolve *relative_path* under the static root; reject traversal.
- `_static_root()` — [`L22`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L22)
- `get_eid(element)` — [`L82`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L82)
- `get_file(path: str)` — [`L309`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L309)
- `get_graph(repo_path: Optional[str] = None, cypher_query: Optional[str] = None)` — [`L78`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L78)
- `is_path_under_static(path: Path, root: Path)` — [`L37`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L37)
- `run_server(host: str = "127.0.0.1", port: int = 8000, static_dir: Optional[str] = None)` — [`L339`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L339)
- `set_db_manager(manager: DatabaseManager)` — [`L71`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L71)
- `spa_fallback(request: Request, full_path: str)` — [`L319`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L319)

## Module values
- `_ALLOWED_ORIGIN_REGEX` — [`L56`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L56)
- `_static_dir` — [`L69`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L69)
- `app` — [`L19`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L19)
- `db_manager` — [`L67`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/viz/server.py#L67)

