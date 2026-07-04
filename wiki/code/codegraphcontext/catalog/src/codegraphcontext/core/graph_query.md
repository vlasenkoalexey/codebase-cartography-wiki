---
title: 'Module: src/codegraphcontext/core/graph_query.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/core/graph_query.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.core.graph_query`/GraphQueryInterface#
symbols:
  GraphQueryInterface: ''
  GraphQueryInterface.get_driver: get_driver().
  GraphQueryInterface.close_driver: close_driver().
  GraphQueryInterface.is_connected: is_connected().
  GraphQueryInterface.get_backend_type: get_backend_type().
  GraphQueryInterface.validate_config: validate_config().
  GraphQueryInterface.test_connection: test_connection().
  GraphQueryInterface.name: name.
---
# Module: [`src/codegraphcontext/core/graph_query.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/graph_query.py)

## Classes
### `GraphQueryInterface`  ·  implements/extends ABC
- def: [`src/codegraphcontext/core/graph_query.py:16`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/graph_query.py#L16)
- doc: Minimal contract shared by all CGC graph database managers.
- signature: `class GraphQueryInterface(ABC):`
- members:
  - `close_driver(self)` — [`L26`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/graph_query.py#L26) — Release connections and embedded database resources. — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `get_backend_type(self)` — [`L34`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/graph_query.py#L34) — Stable backend identifier (e.g. ``neo4j``, ``kuzudb``, ``falkordb``).
  - `get_driver(self)` — [`L22`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/graph_query.py#L22) — Return a driver wrapper exposing ``session()`` compatible with Neo4j. — documented in [codegraphcontext-core-database_embedded_kuzu](../../../../concepts/codegraphcontext-core-database_embedded_kuzu.md)
  - `is_connected(self)` — [`L30`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/graph_query.py#L30) — True when the backend is reachable and can execute a trivial query.
  - `test_connection(cls, *args, **kwargs)` — [`L44`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/graph_query.py#L44) — Check whether the backend driver is installed and usable.
  - `validate_config(cls, *args, **kwargs)` — [`L39`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/graph_query.py#L39) — Validate backend-specific configuration before connecting.
  - `name` — [`L19`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/core/graph_query.py#L19)
- uses (calls/refs, reference-scoped): [`get_driver`](database_embedded_kuzu.md#EmbeddedGraphManager.get_driver), [`close_driver`](database_embedded_kuzu.md#EmbeddedGraphManager.close_driver), [`EmbeddedGraphManager`](database_embedded_kuzu.md#EmbeddedGraphManager), [`test_connection`](database_embedded_kuzu.md#EmbeddedGraphManager.test_connection), [`get_backend_type`](database_embedded_kuzu.md#EmbeddedGraphManager.get_backend_type), [`is_connected`](database_embedded_kuzu.md#EmbeddedGraphManager.is_connected), [`validate_config`](database_embedded_kuzu.md#EmbeddedGraphManager.validate_config)
- used by: [`EmbeddedGraphManager`](database_embedded_kuzu.md#EmbeddedGraphManager), [`_initialized`](database_embedded_kuzu.md#EmbeddedGraphManager._initialized)

