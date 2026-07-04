---
title: 'Module: tests/e2e/conftest.py'
type: catalog
provenance: extracted
module: tests/e2e/conftest.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.e2e.conftest`/
symbols:
  initialized: initialized().
  MCPClient: MCPClient#
  MCPClient.call: MCPClient#call().
  MCPClient.initialize: MCPClient#initialize().
  MCPClient.stderr_text: MCPClient#stderr_text().
  MCPClient.list_tools: MCPClient#list_tools().
  _spawn_mcp: _spawn_mcp().
  MCPClient.proc: MCPClient#proc.
  MCPClient._send: MCPClient#_send().
  MCPClient._recv: MCPClient#_recv().
  MCPClient.__post_init__: MCPClient#__post_init__().
  mcp_server_factory: mcp_server_factory().
  REPO_ROOT: REPO_ROOT.
  MCPClient._next_id: MCPClient#_next_id.
  MCPClient.drain: MCPClient#drain().
  MCPClient.terminate: MCPClient#terminate().
  mcp_server_factory.make: mcp_server_factory().make().
  mcp_server: mcp_server().
  MCPClient._stderr_thread: MCPClient#_stderr_thread.
  MCPClient._initialized: MCPClient#_initialized.
  clone_repo_factory: clone_repo_factory().
  DEFAULT_CALL_TIMEOUT_SEC: DEFAULT_CALL_TIMEOUT_SEC.
  DEFAULT_HANDSHAKE_TIMEOUT_SEC: DEFAULT_HANDSHAKE_TIMEOUT_SEC.
  MCPClient._stderr_buf: MCPClient#_stderr_buf.
  MCPClient._stderr_lock: MCPClient#_stderr_lock.
  _frame: _frame().
  _read_line: _read_line().
  MCPClient.project_root: MCPClient#project_root.
  clone_repo_factory._clone: clone_repo_factory()._clone().
---
# Module: [`tests/e2e/conftest.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py)

## Classes
### `MCPClient`
- def: [`tests/e2e/conftest.py:133`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L133)
- doc: Test-side handle on a spawned TSA MCP server subprocess.
- signature: `class MCPClient:`
- members:
  - `_recv(self, timeout: float)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L180) — Read one JSON-RPC *response* (has an ``id``) from stdout.
  - `_send(self, payload: dict[str, Any])` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L172) — Serialise and frame a JSON-RPC payload to the server's stdin.
  - `call(self, tool_name: str, arguments: dict[str, Any] | None = None, *, timeout: float = DEFAULT_CALL_TIMEOUT_SEC)` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L267) — Invoke ``tools/call`` and return the full response dict.
  - `drain()` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L152)
  - `initialize(self, *, client_name: str = "tree-sitter-analyzer-e2e", client_version: str = "0.0.0", timeout: float = DEFAULT_HANDSHAKE_TIMEOUT_SEC)` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L202) — Send ``initialize`` and the ``notifications/initialized`` ack.
  - `list_tools(self, *, timeout: float = DEFAULT_CALL_TIMEOUT_SEC)` — [`L246`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L246) — Return the ``tools/list`` array (after a successful initialize).
  - `stderr_text(self)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L167) — Return everything the server has written to stderr so far.
  - `terminate(self, *, timeout: float = 5)` — [`L299`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L299) — Stop the server. Idempotent and best-effort.
  - `proc` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L136)
  - `project_root` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L137)
- protocol/private: `__post_init__`[`L144`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L144), `_initialized`[`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L142), `_next_id`[`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L141), `_stderr_buf`[`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L138), `_stderr_lock`[`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L139), `_stderr_thread`[`L140`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L140)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (33 test-only callers)

## Functions
- `_clone(url: str, name: str)` — [`L405`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L405)
- `_frame(payload: bytes)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L89) — Append a newline to ``payload`` for the MCP 1.x stdio transport.
- `_read_line(stream: Any, timeout: float)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L94) — Read one newline-terminated JSON line from ``stream``.
- `_spawn_mcp(project_root: str | Path, env: dict[str, str] | None = None, python: str | None = None)` — [`L321`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L321) — Launch the TSA MCP server for the given project root.
- `clone_repo_factory(tmp_path_factory: pytest.TempPathFactory)` — [`L383`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L383) — Session-scoped factory: shallow-clone a public git repo once per session.
- `initialized(client: MCPClient, *, timeout: float = DEFAULT_HANDSHAKE_TIMEOUT_SEC)` — [`L474`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L474) — Idempotently initialize ``client`` and return it.
- `make(project_root: str | Path, env: dict[str, str] | None = None, python: str | None = None)` — [`L355`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L355)
- `mcp_server(mcp_server_factory: Callable[..., MCPClient])` — [`L371`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L371) — Default MCP server pointed at the TSA checkout itself.
- `mcp_server_factory()` — [`L347`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L347) — Return a factory that lifecycle-manages MCPClient instances.

## Module values
- `DEFAULT_CALL_TIMEOUT_SEC` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L70)
- `DEFAULT_HANDSHAKE_TIMEOUT_SEC` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L75)
- `REPO_ROOT` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tests/e2e/conftest.py#L65)

