---
title: 'Module: evaluation/servers/grep_server.py'
type: catalog
provenance: extracted
module: evaluation/servers/grep_server.py
status: fresh
symbol_base: scip-python python claude-context 0.0.0 `evaluation.servers.grep_server`/
symbols:
  search_text: search_text().
  mcp: mcp.
  is_git_repository: is_git_repository().
---
# Module: [`evaluation/servers/grep_server.py`](../../../../../../raw/code/claude-context/evaluation/servers/grep_server.py)

## Functions
- `is_git_repository(path: str)` — [`L20`](../../../../../../raw/code/claude-context/evaluation/servers/grep_server.py#L20) — Check if the given path is inside a git repository.
- `search_text(pattern: str, path: Optional[str] = None, include: Optional[str] = None)` — [`L36`](../../../../../../raw/code/claude-context/evaluation/servers/grep_server.py#L36) — Searches for a regular expression pattern within the content of files in a specified directory (or current working directory). Can filter files by a glob pattern. Returns the lines containing matches, along with their file paths and line numbers.

## Module values
- `mcp` — [`L17`](../../../../../../raw/code/claude-context/evaluation/servers/grep_server.py#L17)

